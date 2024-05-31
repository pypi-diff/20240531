# Comparing `tmp/rapidfuzz-3.9.1.tar.gz` & `tmp/rapidfuzz-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapidfuzz-3.9.1.tar", last modified: Sun May 19 20:11:26 2024, max compression
+gzip compressed data, was "rapidfuzz-3.9.2.tar", last modified: Tue May 28 23:02:54 2024, max compression
```

## Comparing `rapidfuzz-3.9.1.tar` & `rapidfuzz-3.9.2.tar`

### file list

```diff
@@ -1,288 +1,288 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.954500 rapidfuzz-3.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)    31645 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-19 20:11:26.954500 rapidfuzz-3.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10972 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.894500 rapidfuzz-3.9.1/_custom_build/
--rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/_custom_build/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.894500 rapidfuzz-3.9.1/cmake/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/cmake/CheckCPUArch.c.in
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/cmake/CheckCPUArch.cmake
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.894500 rapidfuzz-3.9.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.894500 rapidfuzz-3.9.1/docs/Contributing/
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Contributing/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/License.rst
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/References.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.894500 rapidfuzz-3.9.1/docs/Usage/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.898500 rapidfuzz-3.9.1/docs/Usage/distance/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/DamerauLevenshtein.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/Hamming.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/Indel.rst
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/Jaro.rst
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/JaroWinkler.rst
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/LCSseq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/Levenshtein.rst
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/OSA.rst
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/Postfix.rst
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/Prefix.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.898500 rapidfuzz-3.9.1/docs/Usage/distance/img/
--rw-r--r--   0 runner    (1001) docker     (127)    37487 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/img/damerau_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)    42028 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/img/indel_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34090 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/img/jaro.svg
--rw-r--r--   0 runner    (1001) docker     (127)    34913 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/img/jaro_winkler.svg
--rw-r--r--   0 runner    (1001) docker     (127)    37821 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/img/osa.svg
--rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/img/uniform_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/distance/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/fuzz.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.902500 rapidfuzz-3.9.1/docs/Usage/img/
--rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/WRatio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    42028 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/indel_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)    41626 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/partial_ratio_long_needle.svg
--rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/partial_ratio_short_needle.svg
--rw-r--r--   0 runner    (1001) docker     (127)    28491 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/partial_token_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24769 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/partial_token_set_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25404 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/partial_token_sort_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    24367 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    27273 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/token_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    25693 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/token_set_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/token_sort_ratio.svg
--rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/img/uniform_levenshtein.svg
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/process.rst
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/Usage/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/changelog_link.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.902500 rapidfuzz-3.9.1/docs/img/
--rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/img/RapidFuzz.svg
--rw-r--r--   0 runner    (1001) docker     (127)    56024 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/img/cdist.svg
--rw-r--r--   0 runner    (1001) docker     (127)    54183 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/img/scorer.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.890500 rapidfuzz-3.9.1/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.902500 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.902500 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.906500 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    23194 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17962 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.906500 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/
--rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    30315 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18309 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    20702 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    45010 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    27628 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    37942 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz_impl.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-19 20:10:59.000000 rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/rapidfuzz_all.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.910500 rapidfuzz-3.9.1/extern/taskflow/
--rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-05-19 20:11:00.000000 rapidfuzz-3.9.1/extern/taskflow/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-19 20:11:00.000000 rapidfuzz-3.9.1/extern/taskflow/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-19 20:11:00.000000 rapidfuzz-3.9.1/extern/taskflow/TaskflowConfig.cmake.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.910500 rapidfuzz-3.9.1/extern/taskflow/taskflow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.910500 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/critical.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16653 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/data_pipeline.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/find.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/for_each.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/launch.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    21985 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/partitioner.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    47366 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/pipeline.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/reduce.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18008 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/scan.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    21365 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/sort.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/transform.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.914500 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/async.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/async_task.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/declarations.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/environment.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/error.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    54781 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/executor-module-opt.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    69853 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/executor.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    45123 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/flow_builder.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/graph.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/notifier.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    26126 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/observer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/semaphore.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    18518 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/task.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/taskflow.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/topology.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/tsq.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/core/worker.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/taskflow.hpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.918500 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/iterator.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/macros.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/math.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    19899 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/object_pool.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/os.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    29321 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/serializer.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/singleton.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    31329 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/small_vector.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/stream.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/traits.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-19 20:11:01.000000 rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/uuid.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-19 20:11:23.000000 rapidfuzz-3.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 20:11:26.954500 rapidfuzz-3.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.890500 rapidfuzz-3.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.930500 rapidfuzz-3.9.1/src/rapidfuzz/
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.934500 rapidfuzz-3.9.1/src/rapidfuzz/FeatureDetector/
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/FeatureDetector/CpuInfo.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/FeatureDetector/CpuInfo.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.934500 rapidfuzz-3.9.1/src/rapidfuzz/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/__pyinstaller/hook-rapidfuzz.py
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/_common_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/_feature_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)   266395 2024-05-19 20:11:19.000000 rapidfuzz-3.9.1/src/rapidfuzz/_feature_detector_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/_feature_detector_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    25736 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/cpp_common.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    17473 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/cpp_common.pxd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.950500 rapidfuzz-3.9.1/src/rapidfuzz/distance/
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/DamerauLevenshtein.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/DamerauLevenshtein.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/DamerauLevenshtein_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Hamming.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Hamming.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9081 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Hamming_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Indel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Indel.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Indel_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Jaro.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Jaro.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/JaroWinkler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/JaroWinkler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/JaroWinkler_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Jaro_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/LCSseq.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/LCSseq.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/LCSseq_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Levenshtein.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Levenshtein_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/OSA.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/OSA.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/OSA_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Postfix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Postfix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Postfix_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Prefix.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/Prefix_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize.pyi
--rw-r--r--   0 runner    (1001) docker     (127)  1693935 2024-05-19 20:11:20.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize_cpp.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    29674 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    26320 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize_py.py
--rw-r--r--   0 runner    (1001) docker     (127)    49089 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics.hpp
--rw-r--r--   0 runner    (1001) docker     (127)  1506049 2024-05-19 20:11:21.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    62949 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  1514092 2024-05-19 20:11:22.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp_avx2.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp_avx2.pyx
--rw-r--r--   0 runner    (1001) docker     (127)  1514092 2024-05-19 20:11:23.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp_sse2.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp_sse2.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_py.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   678100 2024-05-19 20:11:15.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   680081 2024-05-19 20:11:16.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp_avx2.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp_avx2.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   680081 2024-05-19 20:11:16.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp_sse2.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp_sse2.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    25530 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/fuzz_py.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/process.py
--rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/process.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    23286 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/process_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/process_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)  2151605 2024-05-19 20:11:18.000000 rapidfuzz-3.9.1/src/rapidfuzz/process_cpp_impl.cxx
--rw-r--r--   0 runner    (1001) docker     (127)    79018 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/process_cpp_impl.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    26688 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/process_py.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/rapidfuzz.h
--rw-r--r--   0 runner    (1001) docker     (127)   293266 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/unicodetype_db.h
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils.hpp
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   502929 2024-05-19 20:11:19.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils_cpp.cxx
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils_cpp.hpp
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils_cpp.pyx
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/src/rapidfuzz/utils_py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.954500 rapidfuzz-3.9.1/src/rapidfuzz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-05-19 20:11:26.000000 rapidfuzz-3.9.1/src/rapidfuzz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-05-19 20:11:26.000000 rapidfuzz-3.9.1/src/rapidfuzz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 20:11:26.000000 rapidfuzz-3.9.1/src/rapidfuzz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-19 20:11:26.000000 rapidfuzz-3.9.1/src/rapidfuzz.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-19 20:11:26.000000 rapidfuzz-3.9.1/src/rapidfuzz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-19 20:11:26.000000 rapidfuzz-3.9.1/src/rapidfuzz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.950500 rapidfuzz-3.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15407 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 20:11:26.954500 rapidfuzz-3.9.1/tests/distance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_DamerauLevenshtein.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_Hamming.py
--rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_Indel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_Jaro.py
--rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_JaroWinkler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_LCSseq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_Levenshtein.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_OSA.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_Postfix.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_Prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/distance/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/test_cpp_fallback.py
--rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/test_fuzz.py
--rw-r--r--   0 runner    (1001) docker     (127)    14447 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/test_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (127)    26380 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/test_process.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/test_pure_python_fallback.py
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-19 20:10:57.000000 rapidfuzz-3.9.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.618162 rapidfuzz-3.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    31778 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-05-28 23:02:54.618162 rapidfuzz-3.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.558161 rapidfuzz-3.9.2/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (127)     2604 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/_custom_build/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.562161 rapidfuzz-3.9.2/cmake/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/cmake/CheckCPUArch.c.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/cmake/CheckCPUArch.cmake
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.562161 rapidfuzz-3.9.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.562161 rapidfuzz-3.9.2/docs/Contributing/
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Contributing/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/License.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/References.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.562161 rapidfuzz-3.9.2/docs/Usage/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.562161 rapidfuzz-3.9.2/docs/Usage/distance/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/DamerauLevenshtein.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/Hamming.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/Indel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/Jaro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/JaroWinkler.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/LCSseq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/Levenshtein.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/OSA.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/Postfix.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/Prefix.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.566161 rapidfuzz-3.9.2/docs/Usage/distance/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    37487 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/img/damerau_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    42028 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/img/indel_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34090 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/img/jaro.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    34913 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/img/jaro_winkler.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    37821 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/img/osa.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/img/uniform_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/distance/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/fuzz.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.566161 rapidfuzz-3.9.2/docs/Usage/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    25251 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/img/WRatio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    42028 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/img/indel_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    41626 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/img/partial_ratio_long_needle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    41360 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/img/partial_ratio_short_needle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    28491 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/img/partial_token_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24769 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/img/partial_token_set_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25404 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/img/partial_token_sort_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    24367 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/img/ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    27273 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/img/token_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    25693 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/img/token_set_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    26611 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/img/token_sort_ratio.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    32664 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/img/uniform_levenshtein.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/process.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/Usage/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/changelog_link.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.566161 rapidfuzz-3.9.2/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/img/RapidFuzz.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    56024 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/img/cdist.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    54183 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/img/scorer.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3160 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.558161 rapidfuzz-3.9.2/extern/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.570161 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.570161 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.570161 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    23194 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17962 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16290 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17443 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.574161 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/
+-rw-r--r--   0 runner    (1001) docker     (127)     6203 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6649 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6480 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7537 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8008 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30315 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18309 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    20702 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    45010 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9776 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    27628 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    37942 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/fuzz_impl.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/rapidfuzz_all.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.574161 rapidfuzz-3.9.2/extern/taskflow/
+-rw-r--r--   0 runner    (1001) docker     (127)    14371 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/taskflow/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/taskflow/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-28 23:02:28.000000 rapidfuzz-3.9.2/extern/taskflow/TaskflowConfig.cmake.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.578162 rapidfuzz-3.9.2/extern/taskflow/taskflow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.578162 rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/critical.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16653 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/data_pipeline.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    14616 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/find.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/for_each.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/launch.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21985 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/partitioner.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    47366 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/pipeline.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12080 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/reduce.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18008 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/scan.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    21365 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/sort.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/transform.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.582162 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/async.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5007 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/async_task.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/declarations.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/environment.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/error.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    54781 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/executor-module-opt.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    69853 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/executor.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    45123 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/flow_builder.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/graph.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/notifier.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    26126 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/observer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/semaphore.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18518 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/task.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    16679 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/taskflow.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/topology.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/tsq.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/core/worker.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/taskflow.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.582162 rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/iterator.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/macros.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/math.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    19899 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/object_pool.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/os.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    29321 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/serializer.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/singleton.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    31329 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/small_vector.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/stream.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/traits.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-05-28 23:02:29.000000 rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/uuid.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-28 23:02:51.000000 rapidfuzz-3.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:02:54.618162 rapidfuzz-3.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.558161 rapidfuzz-3.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.598162 rapidfuzz-3.9.2/src/rapidfuzz/
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.598162 rapidfuzz-3.9.2/src/rapidfuzz/FeatureDetector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/FeatureDetector/CpuInfo.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/FeatureDetector/CpuInfo.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.598162 rapidfuzz-3.9.2/src/rapidfuzz/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/__pyinstaller/hook-rapidfuzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/_common_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/_feature_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)   266395 2024-05-28 23:02:47.000000 rapidfuzz-3.9.2/src/rapidfuzz/_feature_detector_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/_feature_detector_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     4027 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25736 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/cpp_common.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    17473 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/cpp_common.pxd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.614162 rapidfuzz-3.9.2/src/rapidfuzz/distance/
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/DamerauLevenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/DamerauLevenshtein.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/DamerauLevenshtein_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Hamming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Hamming.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9081 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Hamming_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Indel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Indel.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10034 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Indel_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Jaro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Jaro.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/JaroWinkler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/JaroWinkler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6481 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/JaroWinkler_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Jaro_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/LCSseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/LCSseq.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11504 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/LCSseq_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Levenshtein.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    17103 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Levenshtein_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/OSA.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/OSA.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6251 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/OSA_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Postfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Postfix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5039 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Postfix_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Prefix.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5015 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/Prefix_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3989 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/_initialize.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)  1693935 2024-05-28 23:02:48.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/_initialize_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/_initialize_cpp.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    29674 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/_initialize_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    26320 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/_initialize_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49089 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/metrics.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)  1506049 2024-05-28 23:02:49.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/metrics_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    62949 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/metrics_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1514092 2024-05-28 23:02:50.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/metrics_cpp_avx2.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/metrics_cpp_avx2.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)  1514092 2024-05-28 23:02:51.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/metrics_cpp_sse2.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/metrics_cpp_sse2.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/distance/metrics_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/fuzz.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   678100 2024-05-28 23:02:43.000000 rapidfuzz-3.9.2/src/rapidfuzz/fuzz_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     9678 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/fuzz_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/fuzz_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   680081 2024-05-28 23:02:44.000000 rapidfuzz-3.9.2/src/rapidfuzz/fuzz_cpp_avx2.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/fuzz_cpp_avx2.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)   680081 2024-05-28 23:02:44.000000 rapidfuzz-3.9.2/src/rapidfuzz/fuzz_cpp_sse2.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/fuzz_cpp_sse2.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    25933 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/fuzz_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/process.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    23286 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/process_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/process_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)  2151605 2024-05-28 23:02:46.000000 rapidfuzz-3.9.2/src/rapidfuzz/process_cpp_impl.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)    79018 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/process_cpp_impl.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    26688 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/process_py.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/rapidfuzz.h
+-rw-r--r--   0 runner    (1001) docker     (127)   293266 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/unicodetype_db.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/utils.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   502929 2024-05-28 23:02:47.000000 rapidfuzz-3.9.2/src/rapidfuzz/utils_cpp.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/utils_cpp.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/utils_cpp.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/src/rapidfuzz/utils_py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.618162 rapidfuzz-3.9.2/src/rapidfuzz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12052 2024-05-28 23:02:54.000000 rapidfuzz-3.9.2/src/rapidfuzz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9502 2024-05-28 23:02:54.000000 rapidfuzz-3.9.2/src/rapidfuzz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:02:54.000000 rapidfuzz-3.9.2/src/rapidfuzz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-28 23:02:54.000000 rapidfuzz-3.9.2/src/rapidfuzz.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 23:02:54.000000 rapidfuzz-3.9.2/src/rapidfuzz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-28 23:02:54.000000 rapidfuzz-3.9.2/src/rapidfuzz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.618162 rapidfuzz-3.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15407 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:54.618162 rapidfuzz-3.9.2/tests/distance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/distance/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/distance/test_DamerauLevenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/distance/test_Hamming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/distance/test_Indel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/distance/test_Jaro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/distance/test_JaroWinkler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/distance/test_LCSseq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/distance/test_Levenshtein.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/distance/test_OSA.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/distance/test_Postfix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/distance/test_Prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/distance/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10165 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/distance/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/test_cpp_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12939 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/test_fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14447 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/test_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26380 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/test_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/test_pure_python_fallback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-28 23:02:26.000000 rapidfuzz-3.9.2/tests/test_utils.py
```

### Comparing `rapidfuzz-3.9.1/CHANGELOG.rst` & `rapidfuzz-3.9.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 ---------
 
+[3.9.2] - 2024-05-28
+^^^^^^^^^^^^^^^^^^^^
+Fixed
+~~~~~
+* fix supported versions of taskflow in cmake to be in the range v3.3 - v3.7
+
+
 [3.9.1] - 2024-05-19
 ^^^^^^^^^^^^^^^^^^^^
 Fixed
 ~~~~~
 * disable AVX2 on MacOS since it did lead to illegal instructions being generated
```

### Comparing `rapidfuzz-3.9.1/CMakeLists.txt` & `rapidfuzz-3.9.2/CMakeLists.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cmake_minimum_required(VERSION 3.12...3.24)
+cmake_minimum_required(VERSION 3.12...3.29)
 
 set(CMAKE_INTERPROCEDURAL_OPTIMIZATION TRUE)
 set(CMAKE_POSITION_INDEPENDENT_CODE ON)
 set(SKBUILD_LINK_LIBRARIES_KEYWORD PRIVATE)
 set(THREADS_PREFER_PTHREAD_FLAG ON)
 
 list(APPEND CMAKE_MODULE_PATH "${CMAKE_CURRENT_SOURCE_DIR}/cmake")
@@ -69,15 +69,27 @@
 include(CheckCPUArch)
 
 check_cpu_arch_x64(RAPIDFUZZ_ARCH_X64)
 check_cpu_arch_x86(RAPIDFUZZ_ARCH_X86)
 
 set(RF_BASE_DIR ${CMAKE_CURRENT_SOURCE_DIR}/src)
 
-find_package(Taskflow 3.3.0 QUIET)
+find_package(Taskflow 3.7.0 QUIET)
+if(NOT Taskflow_FOUND)
+  find_package(Taskflow 3.6.0 QUIET)
+endif()
+if(NOT Taskflow_FOUND)
+  find_package(Taskflow 3.5.0 QUIET)
+endif()
+if(NOT Taskflow_FOUND)
+  find_package(Taskflow 3.4.0 QUIET)
+endif()
+if(NOT Taskflow_FOUND)
+  find_package(Taskflow 3.3.0 QUIET)
+endif()
 if(Taskflow_FOUND)
   message(STATUS "Using system supplied version of Taskflow")
 else()
   message(STATUS "Using packaged version of Taskflow")
   set(TF_BUILD_CUDA
       OFF
       CACHE BOOL "Enables build of CUDA code")
```

### Comparing `rapidfuzz-3.9.1/LICENSE` & `rapidfuzz-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/MANIFEST.in` & `rapidfuzz-3.9.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/PKG-INFO` & `rapidfuzz-3.9.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidfuzz
-Version: 3.9.1
+Version: 3.9.2
 Summary: rapid fuzzy string matching
 Home-page: https://github.com/rapidfuzz/RapidFuzz
 Author: Max Bachmann
 Author-email: pypi@maxbachmann.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -147,14 +147,20 @@
 #### Token Set Ratio
 ```console
 > from rapidfuzz import fuzz
 > fuzz.token_sort_ratio("fuzzy was a bear", "fuzzy fuzzy was a bear")
 84.21052631578947
 > fuzz.token_set_ratio("fuzzy was a bear", "fuzzy fuzzy was a bear")
 100.0
+# Returns 100.0 if one string is a subset of the other, regardless of extra content in the longer string
+> fuzz.token_set_ratio("fuzzy was a bear but not a dog", "fuzzy was a bear")
+100.0
+# Score is reduced only when there is explicit disagreement in the two strings
+> fuzz.token_set_ratio("fuzzy was a bear but not a dog", "fuzzy was a bear but not a cat")
+92.3076923076923
 ```
 
 #### Weighted Ratio
 ```console
 > from rapidfuzz import fuzz
 > fuzz.WRatio("this is a test", "this is a new test!!!")
 85.5
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapidfuzz Version: 3.9.1 Summary: rapid fuzzy
+Metadata-Version: 2.1 Name: rapidfuzz Version: 3.9.2 Summary: rapid fuzzy
 string matching Home-page: https://github.com/rapidfuzz/RapidFuzz Author: Max
 Bachmann Author-email: pypi@maxbachmann.de License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.8 Description-Content-Type: text/
@@ -63,19 +63,24 @@
 Partial Ratio ```console > from rapidfuzz import fuzz > fuzz.partial_ratio
 ("this is a test", "this is a test!") 100.0 ``` #### Token Sort Ratio
 ```console > from rapidfuzz import fuzz > fuzz.ratio("fuzzy wuzzy was a bear",
 "wuzzy fuzzy was a bear") 90.9090909090909 > fuzz.token_sort_ratio("fuzzy wuzzy
 was a bear", "wuzzy fuzzy was a bear") 100.0 ``` #### Token Set Ratio
 ```console > from rapidfuzz import fuzz > fuzz.token_sort_ratio("fuzzy was a
 bear", "fuzzy fuzzy was a bear") 84.21052631578947 > fuzz.token_set_ratio
-("fuzzy was a bear", "fuzzy fuzzy was a bear") 100.0 ``` #### Weighted Ratio
-```console > from rapidfuzz import fuzz > fuzz.WRatio("this is a test", "this
-is a new test!!!") 85.5 > from rapidfuzz import fuzz, utils > # Removing non
-alpha numeric characters("!") from the string > fuzz.WRatio("this is a test",
-"this is a new test!!!", processor=utils.default_process) # here "this is a new
+("fuzzy was a bear", "fuzzy fuzzy was a bear") 100.0 # Returns 100.0 if one
+string is a subset of the other, regardless of extra content in the longer
+string > fuzz.token_set_ratio("fuzzy was a bear but not a dog", "fuzzy was a
+bear") 100.0 # Score is reduced only when there is explicit disagreement in the
+two strings > fuzz.token_set_ratio("fuzzy was a bear but not a dog", "fuzzy was
+a bear but not a cat") 92.3076923076923 ``` #### Weighted Ratio ```console >
+from rapidfuzz import fuzz > fuzz.WRatio("this is a test", "this is a new
+test!!!") 85.5 > from rapidfuzz import fuzz, utils > # Removing non alpha
+numeric characters("!") from the string > fuzz.WRatio("this is a test", "this
+is a new test!!!", processor=utils.default_process) # here "this is a new
 test!!!" is converted to "this is a new test" 95.0 > fuzz.WRatio("this is a
 test", "this is a new test") 95.0 > # Converting string to lower case >
 fuzz.WRatio("this is a word", "THIS IS A WORD") 21.42857142857143 > fuzz.WRatio
 ("this is a word", "THIS IS A WORD", processor=utils.default_process) # here
 "THIS IS A WORD" is converted to "this is a word" 100.0 ``` #### Quick Ratio
 ```console > from rapidfuzz import fuzz > fuzz.QRatio("this is a test", "this
 is a new test!!!") 80.0 > from rapidfuzz import fuzz, utils > # Removing non
```

### Comparing `rapidfuzz-3.9.1/README.md` & `rapidfuzz-3.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -126,14 +126,20 @@
 #### Token Set Ratio
 ```console
 > from rapidfuzz import fuzz
 > fuzz.token_sort_ratio("fuzzy was a bear", "fuzzy fuzzy was a bear")
 84.21052631578947
 > fuzz.token_set_ratio("fuzzy was a bear", "fuzzy fuzzy was a bear")
 100.0
+# Returns 100.0 if one string is a subset of the other, regardless of extra content in the longer string
+> fuzz.token_set_ratio("fuzzy was a bear but not a dog", "fuzzy was a bear")
+100.0
+# Score is reduced only when there is explicit disagreement in the two strings
+> fuzz.token_set_ratio("fuzzy was a bear but not a dog", "fuzzy was a bear but not a cat")
+92.3076923076923
 ```
 
 #### Weighted Ratio
 ```console
 > from rapidfuzz import fuzz
 > fuzz.WRatio("this is a test", "this is a new test!!!")
 85.5
```

#### html2text {}

```diff
@@ -53,19 +53,24 @@
 Partial Ratio ```console > from rapidfuzz import fuzz > fuzz.partial_ratio
 ("this is a test", "this is a test!") 100.0 ``` #### Token Sort Ratio
 ```console > from rapidfuzz import fuzz > fuzz.ratio("fuzzy wuzzy was a bear",
 "wuzzy fuzzy was a bear") 90.9090909090909 > fuzz.token_sort_ratio("fuzzy wuzzy
 was a bear", "wuzzy fuzzy was a bear") 100.0 ``` #### Token Set Ratio
 ```console > from rapidfuzz import fuzz > fuzz.token_sort_ratio("fuzzy was a
 bear", "fuzzy fuzzy was a bear") 84.21052631578947 > fuzz.token_set_ratio
-("fuzzy was a bear", "fuzzy fuzzy was a bear") 100.0 ``` #### Weighted Ratio
-```console > from rapidfuzz import fuzz > fuzz.WRatio("this is a test", "this
-is a new test!!!") 85.5 > from rapidfuzz import fuzz, utils > # Removing non
-alpha numeric characters("!") from the string > fuzz.WRatio("this is a test",
-"this is a new test!!!", processor=utils.default_process) # here "this is a new
+("fuzzy was a bear", "fuzzy fuzzy was a bear") 100.0 # Returns 100.0 if one
+string is a subset of the other, regardless of extra content in the longer
+string > fuzz.token_set_ratio("fuzzy was a bear but not a dog", "fuzzy was a
+bear") 100.0 # Score is reduced only when there is explicit disagreement in the
+two strings > fuzz.token_set_ratio("fuzzy was a bear but not a dog", "fuzzy was
+a bear but not a cat") 92.3076923076923 ``` #### Weighted Ratio ```console >
+from rapidfuzz import fuzz > fuzz.WRatio("this is a test", "this is a new
+test!!!") 85.5 > from rapidfuzz import fuzz, utils > # Removing non alpha
+numeric characters("!") from the string > fuzz.WRatio("this is a test", "this
+is a new test!!!", processor=utils.default_process) # here "this is a new
 test!!!" is converted to "this is a new test" 95.0 > fuzz.WRatio("this is a
 test", "this is a new test") 95.0 > # Converting string to lower case >
 fuzz.WRatio("this is a word", "THIS IS A WORD") 21.42857142857143 > fuzz.WRatio
 ("this is a word", "THIS IS A WORD", processor=utils.default_process) # here
 "THIS IS A WORD" is converted to "this is a word" 100.0 ``` #### Quick Ratio
 ```console > from rapidfuzz import fuzz > fuzz.QRatio("this is a test", "this
 is a new test!!!") 80.0 > from rapidfuzz import fuzz, utils > # Removing non
```

### Comparing `rapidfuzz-3.9.1/_custom_build/backend.py` & `rapidfuzz-3.9.2/_custom_build/backend.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/cmake/CheckCPUArch.cmake` & `rapidfuzz-3.9.2/cmake/CheckCPUArch.cmake`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Contributing/index.rst` & `rapidfuzz-3.9.2/docs/Contributing/index.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Installation.rst` & `rapidfuzz-3.9.2/docs/Installation.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/distance/DamerauLevenshtein.rst` & `rapidfuzz-3.9.2/docs/Usage/distance/DamerauLevenshtein.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/distance/Indel.rst` & `rapidfuzz-3.9.2/docs/Usage/distance/Indel.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/distance/Jaro.rst` & `rapidfuzz-3.9.2/docs/Usage/distance/Jaro.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/distance/JaroWinkler.rst` & `rapidfuzz-3.9.2/docs/Usage/distance/JaroWinkler.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/distance/LCSseq.rst` & `rapidfuzz-3.9.2/docs/Usage/distance/LCSseq.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/distance/Levenshtein.rst` & `rapidfuzz-3.9.2/docs/Usage/distance/Levenshtein.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/distance/OSA.rst` & `rapidfuzz-3.9.2/docs/Usage/distance/OSA.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/distance/img/damerau_levenshtein.svg` & `rapidfuzz-3.9.2/docs/Usage/distance/img/damerau_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/distance/img/indel_levenshtein.svg` & `rapidfuzz-3.9.2/docs/Usage/distance/img/indel_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/distance/img/jaro.svg` & `rapidfuzz-3.9.2/docs/Usage/distance/img/jaro.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/distance/img/jaro_winkler.svg` & `rapidfuzz-3.9.2/docs/Usage/distance/img/jaro_winkler.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/distance/img/osa.svg` & `rapidfuzz-3.9.2/docs/Usage/distance/img/osa.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/distance/img/uniform_levenshtein.svg` & `rapidfuzz-3.9.2/docs/Usage/distance/img/uniform_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/fuzz.rst` & `rapidfuzz-3.9.2/docs/Usage/fuzz.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/img/WRatio.svg` & `rapidfuzz-3.9.2/docs/Usage/img/WRatio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/img/indel_levenshtein.svg` & `rapidfuzz-3.9.2/docs/Usage/img/indel_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/img/partial_ratio_long_needle.svg` & `rapidfuzz-3.9.2/docs/Usage/img/partial_ratio_long_needle.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/img/partial_ratio_short_needle.svg` & `rapidfuzz-3.9.2/docs/Usage/img/partial_ratio_short_needle.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/img/partial_token_ratio.svg` & `rapidfuzz-3.9.2/docs/Usage/img/partial_token_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/img/partial_token_set_ratio.svg` & `rapidfuzz-3.9.2/docs/Usage/img/partial_token_set_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/img/partial_token_sort_ratio.svg` & `rapidfuzz-3.9.2/docs/Usage/img/partial_token_sort_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/img/ratio.svg` & `rapidfuzz-3.9.2/docs/Usage/img/ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/img/token_ratio.svg` & `rapidfuzz-3.9.2/docs/Usage/img/token_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/img/token_set_ratio.svg` & `rapidfuzz-3.9.2/docs/Usage/img/token_set_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/img/token_sort_ratio.svg` & `rapidfuzz-3.9.2/docs/Usage/img/token_sort_ratio.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/Usage/img/uniform_levenshtein.svg` & `rapidfuzz-3.9.2/docs/Usage/img/uniform_levenshtein.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/conf.py` & `rapidfuzz-3.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/img/RapidFuzz.svg` & `rapidfuzz-3.9.2/docs/img/RapidFuzz.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/img/cdist.svg` & `rapidfuzz-3.9.2/docs/img/cdist.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/img/scorer.svg` & `rapidfuzz-3.9.2/docs/img/scorer.svg`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/index.rst` & `rapidfuzz-3.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/docs/refs.bib` & `rapidfuzz-3.9.2/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/CMakeLists.txt` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/LICENSE` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/CharSet.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/GrowingHashmap.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/Matrix.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/PatternMatchVector.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/Range.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/SplittedSentenceView.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/common.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/common_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/distance.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/intrinsics.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/simd.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/simd_avx2.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/simd_sse2.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/type_traits.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/details/types.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/DamerauLevenshtein_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Hamming_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Indel_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/JaroWinkler_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Jaro_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/LCSseq_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Levenshtein_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/OSA_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Postfix_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance/Prefix_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/distance.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/fuzz.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/rapidfuzz-cpp/rapidfuzz/fuzz_impl.hpp` & `rapidfuzz-3.9.2/extern/rapidfuzz-cpp/rapidfuzz/fuzz_impl.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/CMakeLists.txt` & `rapidfuzz-3.9.2/extern/taskflow/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/LICENSE` & `rapidfuzz-3.9.2/extern/taskflow/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/critical.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/critical.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/data_pipeline.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/data_pipeline.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/find.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/find.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/for_each.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/for_each.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/launch.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/launch.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/partitioner.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/partitioner.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/pipeline.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/pipeline.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/reduce.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/reduce.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/scan.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/scan.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/sort.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/sort.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/algorithm/transform.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/algorithm/transform.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/async.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/async.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/async_task.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/async_task.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/declarations.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/declarations.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/error.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/error.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/executor-module-opt.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/executor-module-opt.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/executor.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/executor.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/flow_builder.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/flow_builder.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/graph.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/graph.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/notifier.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/notifier.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/observer.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/observer.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/semaphore.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/semaphore.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/task.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/task.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/taskflow.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/taskflow.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/topology.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/topology.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/tsq.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/tsq.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/core/worker.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/core/worker.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/taskflow.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/taskflow.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/iterator.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/iterator.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/macros.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/macros.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/math.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/math.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/object_pool.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/object_pool.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/os.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/os.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/serializer.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/serializer.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/singleton.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/singleton.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/small_vector.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/small_vector.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/stream.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/stream.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/traits.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/traits.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/extern/taskflow/taskflow/utility/uuid.hpp` & `rapidfuzz-3.9.2/extern/taskflow/taskflow/utility/uuid.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/pyproject.toml` & `rapidfuzz-3.9.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/setup.py` & `rapidfuzz-3.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 with open("README.md", encoding="utf8") as f:
     readme = f.read()
 
 setup_args = {
     "name": "rapidfuzz",
-    "version": "3.9.1",
+    "version": "3.9.2",
     "extras_require": {"full": ["numpy"]},
     "url": "https://github.com/rapidfuzz/RapidFuzz",
     "author": "Max Bachmann",
     "author_email": "pypi@maxbachmann.de",
     "description": "rapid fuzzy string matching",
     "long_description": readme,
     "long_description_content_type": "text/markdown",
```

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/CMakeLists.txt` & `rapidfuzz-3.9.2/src/rapidfuzz/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/FeatureDetector/CpuInfo.cpp` & `rapidfuzz-3.9.2/src/rapidfuzz/FeatureDetector/CpuInfo.cpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/FeatureDetector/CpuInfo.hpp` & `rapidfuzz-3.9.2/src/rapidfuzz/FeatureDetector/CpuInfo.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/__init__.pxd` & `rapidfuzz-3.9.2/src/rapidfuzz/__init__.pxd`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/__init__.py` & `rapidfuzz-3.9.2/src/rapidfuzz/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 rapid string matching library
 """
 
 from __future__ import annotations
 
 __author__: str = "Max Bachmann"
 __license__: str = "MIT"
-__version__: str = "3.9.1"
+__version__: str = "3.9.2"
 
 from rapidfuzz import distance, fuzz, process, utils
 
 __all__ = ["distance", "fuzz", "process", "utils", "get_include"]
 
 
 def get_include():
```

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py` & `rapidfuzz-3.9.2/src/rapidfuzz/__pyinstaller/test_rapidfuzz_packaging.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/_common_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/_common_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/_feature_detector_cpp.cxx` & `rapidfuzz-3.9.2/src/rapidfuzz/_feature_detector_cpp.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/_utils.py` & `rapidfuzz-3.9.2/src/rapidfuzz/_utils.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/cpp_common.hpp` & `rapidfuzz-3.9.2/src/rapidfuzz/cpp_common.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/cpp_common.pxd` & `rapidfuzz-3.9.2/src/rapidfuzz/cpp_common.pxd`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/CMakeLists.txt` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/DamerauLevenshtein.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/DamerauLevenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/DamerauLevenshtein.pyi` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/DamerauLevenshtein.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/DamerauLevenshtein_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/DamerauLevenshtein_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Hamming.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Hamming.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Hamming.pyi` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Hamming.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Hamming_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Hamming_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Indel.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Indel.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Indel.pyi` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Indel.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Indel_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Indel_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Jaro.pyi` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Jaro.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/JaroWinkler.pyi` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/JaroWinkler.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/JaroWinkler_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/JaroWinkler_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Jaro_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Jaro_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/LCSseq.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/LCSseq.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/LCSseq.pyi` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/LCSseq.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/LCSseq_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/LCSseq_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Levenshtein.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Levenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Levenshtein.pyi` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Levenshtein.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Levenshtein_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Levenshtein_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/OSA.pyi` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/OSA.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/OSA_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/OSA_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Postfix.pyi` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Postfix.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Postfix_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Postfix_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Prefix.pyi` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Prefix.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/Prefix_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/Prefix_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/__init__.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/__init__.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/__init__.pyi` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/__init__.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/_initialize.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize.pyi` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/_initialize.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize_cpp.cxx` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/_initialize_cpp.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize_cpp.pyx` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/_initialize_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/_initialize_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/_initialize_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics.hpp` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/metrics.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp.cxx` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/metrics_cpp.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp.pyx` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/metrics_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp_avx2.cxx` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/metrics_cpp_avx2.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_cpp_sse2.cxx` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/metrics_cpp_sse2.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/distance/metrics_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/distance/metrics_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/fuzz.py` & `rapidfuzz-3.9.2/src/rapidfuzz/fuzz.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/fuzz.pyi` & `rapidfuzz-3.9.2/src/rapidfuzz/fuzz.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp.cxx` & `rapidfuzz-3.9.2/src/rapidfuzz/fuzz_cpp.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp.hpp` & `rapidfuzz-3.9.2/src/rapidfuzz/fuzz_cpp.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp.pyx` & `rapidfuzz-3.9.2/src/rapidfuzz/fuzz_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp_avx2.cxx` & `rapidfuzz-3.9.2/src/rapidfuzz/fuzz_cpp_avx2.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/fuzz_cpp_sse2.cxx` & `rapidfuzz-3.9.2/src/rapidfuzz/fuzz_cpp_sse2.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/fuzz_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/fuzz_py.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,14 +430,20 @@
 
     Examples
     --------
     >>> fuzz.token_sort_ratio("fuzzy was a bear", "fuzzy fuzzy was a bear")
     83.8709716796875
     >>> fuzz.token_set_ratio("fuzzy was a bear", "fuzzy fuzzy was a bear")
     100.0
+    # Returns 100.0 if one string is a subset of the other, regardless of extra content in the longer string
+    >>> fuzz.token_set_ratio("fuzzy was a bear but not a dog", "fuzzy was a bear")
+    100.0
+    # Score is reduced only when there is explicit disagreement in the two strings
+    >>> fuzz.token_set_ratio("fuzzy was a bear but not a dog", "fuzzy was a bear but not a cat")
+    92.3076923076923
     """
     setupPandas()
     if is_none(s1) or is_none(s2):
         return 0
 
     if processor is not None:
         s1 = processor(s1)
```

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/process.pyi` & `rapidfuzz-3.9.2/src/rapidfuzz/process.pyi`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/process_cpp.hpp` & `rapidfuzz-3.9.2/src/rapidfuzz/process_cpp.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/process_cpp.py` & `rapidfuzz-3.9.2/src/rapidfuzz/process_cpp.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/process_cpp_impl.cxx` & `rapidfuzz-3.9.2/src/rapidfuzz/process_cpp_impl.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/process_cpp_impl.pyx` & `rapidfuzz-3.9.2/src/rapidfuzz/process_cpp_impl.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/process_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/process_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/rapidfuzz.h` & `rapidfuzz-3.9.2/src/rapidfuzz/rapidfuzz.h`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/unicodetype_db.h` & `rapidfuzz-3.9.2/src/rapidfuzz/unicodetype_db.h`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/utils.cpp` & `rapidfuzz-3.9.2/src/rapidfuzz/utils.cpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/utils.hpp` & `rapidfuzz-3.9.2/src/rapidfuzz/utils.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/utils_cpp.cxx` & `rapidfuzz-3.9.2/src/rapidfuzz/utils_cpp.cxx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/utils_cpp.hpp` & `rapidfuzz-3.9.2/src/rapidfuzz/utils_cpp.hpp`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/utils_cpp.pyx` & `rapidfuzz-3.9.2/src/rapidfuzz/utils_cpp.pyx`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz/utils_py.py` & `rapidfuzz-3.9.2/src/rapidfuzz/utils_py.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz.egg-info/PKG-INFO` & `rapidfuzz-3.9.2/src/rapidfuzz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidfuzz
-Version: 3.9.1
+Version: 3.9.2
 Summary: rapid fuzzy string matching
 Home-page: https://github.com/rapidfuzz/RapidFuzz
 Author: Max Bachmann
 Author-email: pypi@maxbachmann.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -147,14 +147,20 @@
 #### Token Set Ratio
 ```console
 > from rapidfuzz import fuzz
 > fuzz.token_sort_ratio("fuzzy was a bear", "fuzzy fuzzy was a bear")
 84.21052631578947
 > fuzz.token_set_ratio("fuzzy was a bear", "fuzzy fuzzy was a bear")
 100.0
+# Returns 100.0 if one string is a subset of the other, regardless of extra content in the longer string
+> fuzz.token_set_ratio("fuzzy was a bear but not a dog", "fuzzy was a bear")
+100.0
+# Score is reduced only when there is explicit disagreement in the two strings
+> fuzz.token_set_ratio("fuzzy was a bear but not a dog", "fuzzy was a bear but not a cat")
+92.3076923076923
 ```
 
 #### Weighted Ratio
 ```console
 > from rapidfuzz import fuzz
 > fuzz.WRatio("this is a test", "this is a new test!!!")
 85.5
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: rapidfuzz Version: 3.9.1 Summary: rapid fuzzy
+Metadata-Version: 2.1 Name: rapidfuzz Version: 3.9.2 Summary: rapid fuzzy
 string matching Home-page: https://github.com/rapidfuzz/RapidFuzz Author: Max
 Bachmann Author-email: pypi@maxbachmann.de License: MIT Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Classifier: License :: OSI
 Approved :: MIT License Requires-Python: >=3.8 Description-Content-Type: text/
@@ -63,19 +63,24 @@
 Partial Ratio ```console > from rapidfuzz import fuzz > fuzz.partial_ratio
 ("this is a test", "this is a test!") 100.0 ``` #### Token Sort Ratio
 ```console > from rapidfuzz import fuzz > fuzz.ratio("fuzzy wuzzy was a bear",
 "wuzzy fuzzy was a bear") 90.9090909090909 > fuzz.token_sort_ratio("fuzzy wuzzy
 was a bear", "wuzzy fuzzy was a bear") 100.0 ``` #### Token Set Ratio
 ```console > from rapidfuzz import fuzz > fuzz.token_sort_ratio("fuzzy was a
 bear", "fuzzy fuzzy was a bear") 84.21052631578947 > fuzz.token_set_ratio
-("fuzzy was a bear", "fuzzy fuzzy was a bear") 100.0 ``` #### Weighted Ratio
-```console > from rapidfuzz import fuzz > fuzz.WRatio("this is a test", "this
-is a new test!!!") 85.5 > from rapidfuzz import fuzz, utils > # Removing non
-alpha numeric characters("!") from the string > fuzz.WRatio("this is a test",
-"this is a new test!!!", processor=utils.default_process) # here "this is a new
+("fuzzy was a bear", "fuzzy fuzzy was a bear") 100.0 # Returns 100.0 if one
+string is a subset of the other, regardless of extra content in the longer
+string > fuzz.token_set_ratio("fuzzy was a bear but not a dog", "fuzzy was a
+bear") 100.0 # Score is reduced only when there is explicit disagreement in the
+two strings > fuzz.token_set_ratio("fuzzy was a bear but not a dog", "fuzzy was
+a bear but not a cat") 92.3076923076923 ``` #### Weighted Ratio ```console >
+from rapidfuzz import fuzz > fuzz.WRatio("this is a test", "this is a new
+test!!!") 85.5 > from rapidfuzz import fuzz, utils > # Removing non alpha
+numeric characters("!") from the string > fuzz.WRatio("this is a test", "this
+is a new test!!!", processor=utils.default_process) # here "this is a new
 test!!!" is converted to "this is a new test" 95.0 > fuzz.WRatio("this is a
 test", "this is a new test") 95.0 > # Converting string to lower case >
 fuzz.WRatio("this is a word", "THIS IS A WORD") 21.42857142857143 > fuzz.WRatio
 ("this is a word", "THIS IS A WORD", processor=utils.default_process) # here
 "THIS IS A WORD" is converted to "this is a word" 100.0 ``` #### Quick Ratio
 ```console > from rapidfuzz import fuzz > fuzz.QRatio("this is a test", "this
 is a new test!!!") 80.0 > from rapidfuzz import fuzz, utils > # Removing non
```

### Comparing `rapidfuzz-3.9.1/src/rapidfuzz.egg-info/SOURCES.txt` & `rapidfuzz-3.9.2/src/rapidfuzz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/common.py` & `rapidfuzz-3.9.2/tests/common.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/distance/common.py` & `rapidfuzz-3.9.2/tests/distance/common.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/distance/test_DamerauLevenshtein.py` & `rapidfuzz-3.9.2/tests/distance/test_DamerauLevenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/distance/test_Hamming.py` & `rapidfuzz-3.9.2/tests/distance/test_Hamming.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/distance/test_Indel.py` & `rapidfuzz-3.9.2/tests/distance/test_Indel.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/distance/test_Jaro.py` & `rapidfuzz-3.9.2/tests/distance/test_Jaro.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/distance/test_JaroWinkler.py` & `rapidfuzz-3.9.2/tests/distance/test_JaroWinkler.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/distance/test_LCSseq.py` & `rapidfuzz-3.9.2/tests/distance/test_LCSseq.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/distance/test_Levenshtein.py` & `rapidfuzz-3.9.2/tests/distance/test_Levenshtein.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/distance/test_OSA.py` & `rapidfuzz-3.9.2/tests/distance/test_OSA.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/distance/test_Postfix.py` & `rapidfuzz-3.9.2/tests/distance/test_Postfix.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/distance/test_Prefix.py` & `rapidfuzz-3.9.2/tests/distance/test_Prefix.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/distance/test_distance.py` & `rapidfuzz-3.9.2/tests/distance/test_distance.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/distance/test_init.py` & `rapidfuzz-3.9.2/tests/distance/test_init.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/test_fuzz.py` & `rapidfuzz-3.9.2/tests/test_fuzz.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/test_hypothesis.py` & `rapidfuzz-3.9.2/tests/test_hypothesis.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/test_process.py` & `rapidfuzz-3.9.2/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `rapidfuzz-3.9.1/tests/test_utils.py` & `rapidfuzz-3.9.2/tests/test_utils.py`

 * *Files identical despite different names*

