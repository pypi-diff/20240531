# Comparing `tmp/damply-0.3.0.tar.gz` & `tmp/damply-0.4.0.tar.gz`

## Comparing `damply-0.3.0.tar` & `damply-0.4.0.tar`

### file list

```diff
@@ -1,54 +1,56 @@
--rw-r--r--   0        0        0   401603 2020-02-02 00:00:00.000000 damply-0.3.0/pixi.lock
--rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 damply-0.3.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 damply-0.3.0/config/coverage.toml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 damply-0.3.0/config/hatch.toml
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 damply-0.3.0/config/mkdocs.yaml
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 damply-0.3.0/config/releaserc.toml
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 damply-0.3.0/config/ruff.toml
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 damply-0.3.0/devnotes/pixi-hatch-build.md
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 damply-0.3.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 damply-0.3.0/docs/about.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 damply-0.3.0/src/damply/__init__.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 damply-0.3.0/src/damply/cli.py
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 damply-0.3.0/src/damply/metadata.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 damply-0.3.0/tests/test_general.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 damply-0.3.0/tests/test_metadata.py
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/invalid_.md
--rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/README_gcsi.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file1.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file10.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file2.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file3.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file4.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file5.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file6.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file7.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file8.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file9.txt
--rwxr-xr-x   0        0        0     1210 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/kallisto/README_kallisto.md
--rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/README_simple.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file1.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file10.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file2.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file3.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file4.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file5.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file6.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file7.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file8.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file9.txt
--rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/README_vanderijn.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file1.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file10.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file2.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file3.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file4.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file5.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file6.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file7.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file8.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file9.txt
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 damply-0.3.0/.gitignore
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 damply-0.3.0/README.md
--rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 damply-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 damply-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0   401603 2020-02-02 00:00:00.000000 damply-0.4.0/pixi.lock
+-rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 damply-0.4.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 damply-0.4.0/config/coverage.toml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 damply-0.4.0/config/hatch.toml
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 damply-0.4.0/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 damply-0.4.0/config/releaserc.toml
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 damply-0.4.0/config/ruff.toml
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 damply-0.4.0/devnotes/pixi-hatch-build.md
+-rw-r--r--   0        0        0     2292 2020-02-02 00:00:00.000000 damply-0.4.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 damply-0.4.0/docs/about.md
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 damply-0.4.0/src/damply/__init__.py
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 damply-0.4.0/src/damply/cli.py
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 damply-0.4.0/src/damply/metadata.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 damply-0.4.0/src/damply/utils/byte_size.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 damply-0.4.0/src/damply/utils/whose.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 damply-0.4.0/tests/test_general.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 damply-0.4.0/tests/test_metadata.py
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/invalid_.md
+-rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/README_gcsi.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file10.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file2.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file3.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file4.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file5.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file6.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file7.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file8.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/gcsi/test_dir_1/file9.txt
+-rwxr-xr-x   0        0        0     1210 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/kallisto/README_kallisto.md
+-rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/README_simple.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file10.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file2.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file3.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file4.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file5.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file6.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file7.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file8.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/simple/test_dir_1/file9.txt
+-rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/README_vanderijn.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file10.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file2.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file3.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file4.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file5.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file6.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file7.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file8.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.4.0/tests/examples/vanderijn/test_dir_1/file9.txt
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 damply-0.4.0/.gitignore
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 damply-0.4.0/README.md
+-rw-r--r--   0        0        0     5848 2020-02-02 00:00:00.000000 damply-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 damply-0.4.0/PKG-INFO
```

### Comparing `damply-0.3.0/pixi.lock` & `damply-0.4.0/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2853,17 +2853,17 @@
   license_family: BSD
   purls:
   - pkg:pypi/cryptography?source=conda-forge-mapping
   size: 1978679
   timestamp: 1715044173081
 - kind: pypi
   name: damply
-  version: 0.3.0
+  version: 0.4.0
   path: .
-  sha256: 68e45ee159719618d131e851dbbc75bd63f04756ecc7911c8c8d0ae707ab77b0
+  sha256: b2811d5009d9ac733800bddaa30d3d134178741e59d03d7a9083f3ed7df25897
   requires_dist:
   - rich
   - rich-click
   - pydantic
   - textual
   - trogon
   - dataclasses-json
@@ -5812,88 +5812,88 @@
   purls:
   - pkg:pypi/pydantic?source=conda-forge-mapping
   size: 282316
   timestamp: 1716962269411
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/c2/9f/e2f17d24aee5406a8e8e57784fa737abde9ac538d18028b523268796bcce/pydantic_core-2.18.3-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 24b214b7ee3bd3b865e963dbed0f8bc5375f49449d70e8d407b567af3222aae4
+  url: https://files.pythonhosted.org/packages/e3/5c/477dac00c0d6d34921fec2507ae6aea2cd7c84072eab1dca5bcbbf86c4a2/pydantic_core-2.18.3-cp312-none-win_amd64.whl
+  sha256: 2c8333f6e934733483c7eddffdb094c143b9463d2af7e6bd85ebcb2d4a1b82c6
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/94/bc/e5d1938f36cad75525e923ecfef6f544970d4f14800716728ea5555fc574/pydantic_core-2.18.3-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: 0bee9bb305a562f8b9271855afb6ce00223f545de3d68560b3c1649c7c5295e9
+  url: https://files.pythonhosted.org/packages/77/72/3ce28b58f3d9c9a8bb59984d810be3eabba4455e92de806a4edacd4e5c0b/pydantic_core-2.18.3-cp312-cp312-macosx_10_12_x86_64.whl
+  sha256: f0928cde2ae416a2d1ebe6dee324709c6f73e93494d8c7aea92df99aab1fc40f
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/77/72/3ce28b58f3d9c9a8bb59984d810be3eabba4455e92de806a4edacd4e5c0b/pydantic_core-2.18.3-cp312-cp312-macosx_10_12_x86_64.whl
-  sha256: f0928cde2ae416a2d1ebe6dee324709c6f73e93494d8c7aea92df99aab1fc40f
+  url: https://files.pythonhosted.org/packages/94/bc/e5d1938f36cad75525e923ecfef6f544970d4f14800716728ea5555fc574/pydantic_core-2.18.3-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: 0bee9bb305a562f8b9271855afb6ce00223f545de3d68560b3c1649c7c5295e9
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/e3/5c/477dac00c0d6d34921fec2507ae6aea2cd7c84072eab1dca5bcbbf86c4a2/pydantic_core-2.18.3-cp312-none-win_amd64.whl
-  sha256: 2c8333f6e934733483c7eddffdb094c143b9463d2af7e6bd85ebcb2d4a1b82c6
+  url: https://files.pythonhosted.org/packages/c2/9f/e2f17d24aee5406a8e8e57784fa737abde9ac538d18028b523268796bcce/pydantic_core-2.18.3-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 24b214b7ee3bd3b865e963dbed0f8bc5375f49449d70e8d407b567af3222aae4
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/82/ff/61c330412137b46a55b2269d0a49fd8b90e29fb57b72760b8e09b49db896/pydantic_core-2.18.3-cp310-cp310-macosx_10_12_x86_64.whl
-  sha256: 744697428fcdec6be5670460b578161d1ffe34743a5c15656be7ea82b008197c
+  url: https://files.pythonhosted.org/packages/a0/27/aeade6d7b2f2bcc8fc835bdf6aa705f6f34508da380f170e13cd37477dd4/pydantic_core-2.18.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: c6ac9ffccc9d2e69d9fba841441d4259cb668ac180e51b30d3632cd7abca2b9b
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/a0/27/aeade6d7b2f2bcc8fc835bdf6aa705f6f34508da380f170e13cd37477dd4/pydantic_core-2.18.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: c6ac9ffccc9d2e69d9fba841441d4259cb668ac180e51b30d3632cd7abca2b9b
+  url: https://files.pythonhosted.org/packages/7d/3d/1640253d1da28910b02b00bf6af4a80f1de27f561879128f76bbacb8436d/pydantic_core-2.18.3-cp310-cp310-macosx_11_0_arm64.whl
+  sha256: 37b40c05ced1ba4218b14986fe6f283d22e1ae2ff4c8e28881a70fb81fbfcda7
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
   url: https://files.pythonhosted.org/packages/e2/67/85ee8a54220139159b14088dd40f4d43e60822f8d64bb2a5b9b04d673bd2/pydantic_core-2.18.3-cp310-none-win_amd64.whl
   sha256: 45e4ffbae34f7ae30d0047697e724e534a7ec0a82ef9994b7913a412c21462a0
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/7d/3d/1640253d1da28910b02b00bf6af4a80f1de27f561879128f76bbacb8436d/pydantic_core-2.18.3-cp310-cp310-macosx_11_0_arm64.whl
-  sha256: 37b40c05ced1ba4218b14986fe6f283d22e1ae2ff4c8e28881a70fb81fbfcda7
+  url: https://files.pythonhosted.org/packages/82/ff/61c330412137b46a55b2269d0a49fd8b90e29fb57b72760b8e09b49db896/pydantic_core-2.18.3-cp310-cp310-macosx_10_12_x86_64.whl
+  sha256: 744697428fcdec6be5670460b578161d1ffe34743a5c15656be7ea82b008197c
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/d2/c7/e01cb2017c4b7b274258694f73e8bbbb0988a28b49802e569d1d9bfd51cb/pydantic_core-2.18.3-cp311-none-win_amd64.whl
-  sha256: 58ff8631dbab6c7c982e6425da8347108449321f61fe427c52ddfadd66642af7
+  url: https://files.pythonhosted.org/packages/0c/84/a14457b3cb1ec1f5d1567395abe11ab420dd76733bc79dd0124a874e9eac/pydantic_core-2.18.3-cp311-cp311-macosx_11_0_arm64.whl
+  sha256: b8e20e15d18bf7dbb453be78a2d858f946f5cdf06c5072453dace00ab652e2b2
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/0c/84/a14457b3cb1ec1f5d1567395abe11ab420dd76733bc79dd0124a874e9eac/pydantic_core-2.18.3-cp311-cp311-macosx_11_0_arm64.whl
-  sha256: b8e20e15d18bf7dbb453be78a2d858f946f5cdf06c5072453dace00ab652e2b2
+  url: https://files.pythonhosted.org/packages/d2/c7/e01cb2017c4b7b274258694f73e8bbbb0988a28b49802e569d1d9bfd51cb/pydantic_core-2.18.3-cp311-none-win_amd64.whl
+  sha256: 58ff8631dbab6c7c982e6425da8347108449321f61fe427c52ddfadd66642af7
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
   url: https://files.pythonhosted.org/packages/4a/cf/2847167bab3e7676ba6f0b49963ba04112b1e4281d8c70e302c2fd29e08c/pydantic_core-2.18.3-cp311-cp311-macosx_10_12_x86_64.whl
```

### Comparing `damply-0.3.0/.github/workflows/main.yaml` & `damply-0.4.0/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `damply-0.3.0/config/mkdocs.yaml` & `damply-0.4.0/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `damply-0.3.0/config/releaserc.toml` & `damply-0.4.0/config/releaserc.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 [semantic_release]
 version_variables = ["src/damply/__init__.py:version"]
-version_toml = ["pyproject.toml:project.version"]
+version_toml = [
+  "pyproject.toml:project.version",
+  "pyproject.toml:tool.pixi.version",
+]
 commit_parser = "angular"
 logging_use_named_masks = false
 major_on_zero = true
 allow_zero_version = true
 tag_format = "v{version}"
 
 [semantic_release.branches.main]
```

### Comparing `damply-0.3.0/config/ruff.toml` & `damply-0.4.0/config/ruff.toml`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 fix = true
 
 # extend-exclude is used to exclude directories from the flake8 checks
 extend-exclude = [
   "docs/*",
   "tests/*",
   ".pixi/",
+  "src/damply/utils/**/*.py"
   ]
 
 extend-include = []
 
 [lint]
 select = [
   "E",
```

### Comparing `damply-0.3.0/devnotes/pixi-hatch-build.md` & `damply-0.4.0/devnotes/pixi-hatch-build.md`

 * *Files identical despite different names*

### Comparing `damply-0.3.0/docs/CHANGELOG.md` & `damply-0.4.0/docs/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # CHANGELOG
 
 
 
+## v0.4.0 (2024-05-31)
+
+### Feature
+
+* feat: add cli whose ([`b15ec32`](https://github.com/jjjermiah/damply/commit/b15ec32b551533aab892b3b3227e2091c643dfe1))
+
+* feat: Update CLI help messages and add &#39;whose&#39; command ([`620f209`](https://github.com/jjjermiah/damply/commit/620f209656ab91d5f8ae4e11608eaa6aef05e3f9))
+
+### Fix
+
+* fix: Refactor get_file_owner_full_name function for improved error handling and platform compatibility ([`f4fca58`](https://github.com/jjjermiah/damply/commit/f4fca58d63e4667f8c3fc60b51776a038757c669))
+
+* fix: lint ([`64944d3`](https://github.com/jjjermiah/damply/commit/64944d3025cc20721aa5415c882b42e737daa3da))
+
+
 ## v0.3.0 (2024-05-31)
 
 ### Chore
 
 * chore: Delete config/.pypackage-builder-answers.yml ([`a04cabd`](https://github.com/jjjermiah/damply/commit/a04cabd468901e3b47e236a31d9eb867feea7719))
 
 ### Feature
```

### Comparing `damply-0.3.0/docs/about.md` & `damply-0.4.0/docs/about.md`

 * *Files identical despite different names*

### Comparing `damply-0.3.0/src/damply/cli.py` & `damply-0.4.0/src/damply/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,95 +1,118 @@
-from typing import Literal
-
 from pathlib import Path
+from typing import Literal
 
 import rich_click as click
 from rich import print
+
 from damply.metadata import DMPMetadata
+from damply.utils import whose as whose_util
 
 click.rich_click.OPTION_GROUPS = {
     "damply": [
         {
             "name": "Basic options",
             "options": ["--help"],
         },
     ]
 }
 
 click.rich_click.COMMAND_GROUPS = {
     "damply": [
         {
             "name": "Subcommands",
-            "commands": ["version", "view"],
+            "commands": ["version", "view", "whose"],
         }
     ]
 }
 
 help_config = click.RichHelpConfiguration(
     show_arguments=True,
-    option_groups={"damply": [{"name": "Arguments", "panel_styles": {"box": "ASCII"}}]}
+    option_groups={"damply": [{"name": "Arguments", "panel_styles": {"box": "ASCII"}}]},
 )
 
 
 @click.group(name="damply", context_settings={"help_option_names": ["-h", "--help"]})
 def cli() -> None:
-    """damply tool"""
+    """A tool to interact with systems implementing the Data Management Plan (DMP) standard."""
     pass
 
 
 @cli.command()
 def version() -> None:
     """Print the version of damply."""
     from . import __version__ as ver
 
     print(f"damply version {ver}")
 
 
 @cli.command(context_settings={"help_option_names": ["-h", "--help"]})
 @click.argument(
-    "directory", 
+    "directory",
     type=click.Path(
         exists=True,
         path_type=Path,
         file_okay=False,
         dir_okay=True,
         readable=True,
     ),
     default=Path().cwd(),
 )
 @click.rich_config(help_config=help_config)
 def view(directory: Path) -> None:
-    """Create a DMP file from a directory."""
+    """View the DMP Metadata of a valid DMP Directory."""
     readmes = [f for f in directory.glob("README*") if f.is_file()]
 
     if len(readmes) == 0:
         print("No README file found.")
         return
     elif len(readmes) > 1:
         print("Multiple README files found. Using the first one.")
         readme = readmes[0]
     else:
         readme = readmes[0]
 
     metadata = DMPMetadata.from_path(readme)
 
     from rich.console import Console
-    from rich.table import Table
     from rich.markdown import Markdown
+    from rich.table import Table
 
     console = Console()
 
-    table = Table.grid(padding=1, pad_edge=True, expand = True)
+    table = Table.grid(padding=1, pad_edge=True, expand=True)
     table.title = f"[bold]Metadata for {metadata.path.name}[/bold]"
     table.add_column("Field", justify="right", style="cyan")
     table.add_column("Value", style="yellow")
 
     for field, value in metadata.fields.items():
         table.add_row(field, value)
 
     console.print(table)
     console.print(Markdown(metadata.content))
     console.print(Markdown("\n".join(metadata.logs)))
 
 
+@cli.command(context_settings={"help_option_names": ["-h", "--help"]})
+@click.argument(
+    "path",
+    type=click.Path(
+        exists=True,
+        path_type=Path,
+        file_okay=True,
+        dir_okay=True,
+        readable=True,
+    ),
+    default=Path().cwd(),
+)
+@click.rich_config(help_config=help_config)
+def whose(path: Path) -> None:
+    """Print the owner of the file or directory."""
+    result = whose_util.get_file_owner_full_name(path)
+
+    print(
+        f"The owner of [bold magenta]{path}[/bold magenta] is [bold cyan]{result}[/bold cyan]"
+    )
+
+
 def hello() -> Literal["Hello, World!"]:
     return "Hello, World!"
```

### Comparing `damply-0.3.0/src/damply/metadata.py` & `damply-0.4.0/src/damply/metadata.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime  # Add this import
 import re
 import stat
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Type
 
-from rich import print
 import rich.repr
+from rich import print
 
 def is_file_writable(file_path: Path) -> bool:
     import os
 
     return file_path.exists() and os.access(file_path, os.W_OK)
```

### Comparing `damply-0.3.0/tests/test_metadata.py` & `damply-0.4.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `damply-0.3.0/tests/examples/gcsi/README_gcsi.md` & `damply-0.4.0/tests/examples/gcsi/README_gcsi.md`

 * *Files identical despite different names*

### Comparing `damply-0.3.0/tests/examples/kallisto/README_kallisto.md` & `damply-0.4.0/tests/examples/kallisto/README_kallisto.md`

 * *Files identical despite different names*

### Comparing `damply-0.3.0/tests/examples/vanderijn/README_vanderijn.md` & `damply-0.4.0/tests/examples/vanderijn/README_vanderijn.md`

 * *Files identical despite different names*

### Comparing `damply-0.3.0/.gitignore` & `damply-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `damply-0.3.0/README.md` & `damply-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `damply-0.3.0/pyproject.toml` & `damply-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "damply"
-version = "0.3.0"
+version = "0.4.0"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["damply", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
@@ -44,14 +44,15 @@
 ############################################## PIXI ################################################
 #__________________________________________________________________________________________________#
 
 [tool.pixi.system-requirements]
 linux = "3.10.0"
 
 [tool.pixi.project]
+version = "0.3.0"
 channels = ["conda-forge"]
 platforms = ["osx-arm64", "linux-64", "win-64", "osx-64"]
 # platforms = ["linux-64", "osx-arm64", "osx-64"]
 # platforms = ["osx-arm64"]
 
 [tool.pixi.dependencies]
```

### Comparing `damply-0.3.0/PKG-INFO` & `damply-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: damply
-Version: 0.3.0
+Version: 0.4.0
 Summary: A Quick Tool For Sorting Dicom Files
 Project-URL: homepage, https://github.com/jjjermiah/damply
 Project-URL: repository, https://github.com/jjjermiah/damply
 Project-URL: documentation, https://jjjermiah.github.io/damply/
 Project-URL: changelog, https://github.com/jjjermiah/damply/blob/main/docs/CHANGELOG.md
 Project-URL: issues, https://github.com/jjjermiah/damply/issues
 Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
```

