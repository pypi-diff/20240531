# Comparing `tmp/damply-0.2.0.tar.gz` & `tmp/damply-0.3.0.tar.gz`

## Comparing `damply-0.2.0.tar` & `damply-0.3.0.tar`

### file list

```diff
@@ -1,55 +1,54 @@
--rw-r--r--   0        0        0   401603 2020-02-02 00:00:00.000000 damply-0.2.0/pixi.lock
--rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 damply-0.2.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 damply-0.2.0/config/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 damply-0.2.0/config/coverage.toml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 damply-0.2.0/config/hatch.toml
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 damply-0.2.0/config/mkdocs.yaml
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 damply-0.2.0/config/releaserc.toml
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 damply-0.2.0/config/ruff.toml
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 damply-0.2.0/devnotes/pixi-hatch-build.md
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 damply-0.2.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 damply-0.2.0/docs/about.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/src/damply/__init__.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 damply-0.2.0/src/damply/cli.py
--rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 damply-0.2.0/src/damply/metadata.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 damply-0.2.0/tests/test_general.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 damply-0.2.0/tests/test_metadata.py
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/invalid_.md
--rwxr-xr-x   0        0        0      968 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/README_gcsi.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file1.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file10.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file2.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file3.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file4.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file5.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file6.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file7.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file8.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file9.txt
--rwxr-xr-x   0        0        0     1210 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/kallisto/README_kallisto.md
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/README_simple.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file1.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file10.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file2.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file3.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file4.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file5.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file6.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file7.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file8.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file9.txt
--rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/README_vanderijn.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file1.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file10.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file2.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file3.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file4.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file5.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file6.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file7.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file8.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file9.txt
--rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 damply-0.2.0/.gitignore
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 damply-0.2.0/README.md
--rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 damply-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 damply-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0   401603 2020-02-02 00:00:00.000000 damply-0.3.0/pixi.lock
+-rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 damply-0.3.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 damply-0.3.0/config/coverage.toml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 damply-0.3.0/config/hatch.toml
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 damply-0.3.0/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 damply-0.3.0/config/releaserc.toml
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 damply-0.3.0/config/ruff.toml
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 damply-0.3.0/devnotes/pixi-hatch-build.md
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 damply-0.3.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 damply-0.3.0/docs/about.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 damply-0.3.0/src/damply/__init__.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 damply-0.3.0/src/damply/cli.py
+-rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 damply-0.3.0/src/damply/metadata.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 damply-0.3.0/tests/test_general.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 damply-0.3.0/tests/test_metadata.py
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/invalid_.md
+-rwxr-xr-x   0        0        0      963 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/README_gcsi.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file10.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file2.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file3.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file4.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file5.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file6.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file7.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file8.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/gcsi/test_dir_1/file9.txt
+-rwxr-xr-x   0        0        0     1210 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/kallisto/README_kallisto.md
+-rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/README_simple.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file10.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file2.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file3.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file4.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file5.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file6.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file7.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file8.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/simple/test_dir_1/file9.txt
+-rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/README_vanderijn.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file10.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file2.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file3.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file4.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file5.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file6.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file7.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file8.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.3.0/tests/examples/vanderijn/test_dir_1/file9.txt
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 damply-0.3.0/.gitignore
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 damply-0.3.0/README.md
+-rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 damply-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 damply-0.3.0/PKG-INFO
```

### Comparing `damply-0.2.0/pixi.lock` & `damply-0.3.0/pixi.lock`

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
-  version: 0.2.0
+  version: 0.3.0
   path: .
-  sha256: 3630ee5f39a1b9867c7b8c4922888289e61be29a7d0df4e9248a09fbebee3e84
+  sha256: 68e45ee159719618d131e851dbbc75bd63f04756ecc7911c8c8d0ae707ab77b0
   requires_dist:
   - rich
   - rich-click
   - pydantic
   - textual
   - trogon
   - dataclasses-json
@@ -5844,22 +5844,14 @@
   sha256: 2c8333f6e934733483c7eddffdb094c143b9463d2af7e6bd85ebcb2d4a1b82c6
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/7d/3d/1640253d1da28910b02b00bf6af4a80f1de27f561879128f76bbacb8436d/pydantic_core-2.18.3-cp310-cp310-macosx_11_0_arm64.whl
-  sha256: 37b40c05ced1ba4218b14986fe6f283d22e1ae2ff4c8e28881a70fb81fbfcda7
-  requires_dist:
-  - typing-extensions>=4.6.0,!=4.7.0
-  requires_python: '>=3.8'
-- kind: pypi
-  name: pydantic-core
-  version: 2.18.3
   url: https://files.pythonhosted.org/packages/82/ff/61c330412137b46a55b2269d0a49fd8b90e29fb57b72760b8e09b49db896/pydantic_core-2.18.3-cp310-cp310-macosx_10_12_x86_64.whl
   sha256: 744697428fcdec6be5670460b578161d1ffe34743a5c15656be7ea82b008197c
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
@@ -5876,40 +5868,48 @@
   sha256: 45e4ffbae34f7ae30d0047697e724e534a7ec0a82ef9994b7913a412c21462a0
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/4a/cf/2847167bab3e7676ba6f0b49963ba04112b1e4281d8c70e302c2fd29e08c/pydantic_core-2.18.3-cp311-cp311-macosx_10_12_x86_64.whl
-  sha256: b9ebe8231726c49518b16b237b9fe0d7d361dd221302af511a83d4ada01183ab
+  url: https://files.pythonhosted.org/packages/7d/3d/1640253d1da28910b02b00bf6af4a80f1de27f561879128f76bbacb8436d/pydantic_core-2.18.3-cp310-cp310-macosx_11_0_arm64.whl
+  sha256: 37b40c05ced1ba4218b14986fe6f283d22e1ae2ff4c8e28881a70fb81fbfcda7
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/08/6b/391098a7f0863b5e54c60244c069acfca969af56af4eb7cf52e08b009560/pydantic_core-2.18.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: bd7df92f28d351bb9f12470f4c533cf03d1b52ec5a6e5c58c65b183055a60106
+  url: https://files.pythonhosted.org/packages/d2/c7/e01cb2017c4b7b274258694f73e8bbbb0988a28b49802e569d1d9bfd51cb/pydantic_core-2.18.3-cp311-none-win_amd64.whl
+  sha256: 58ff8631dbab6c7c982e6425da8347108449321f61fe427c52ddfadd66642af7
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
+  url: https://files.pythonhosted.org/packages/4a/cf/2847167bab3e7676ba6f0b49963ba04112b1e4281d8c70e302c2fd29e08c/pydantic_core-2.18.3-cp311-cp311-macosx_10_12_x86_64.whl
+  sha256: b9ebe8231726c49518b16b237b9fe0d7d361dd221302af511a83d4ada01183ab
+  requires_dist:
+  - typing-extensions>=4.6.0,!=4.7.0
+  requires_python: '>=3.8'
+- kind: pypi
+  name: pydantic-core
+  version: 2.18.3
+  url: https://files.pythonhosted.org/packages/08/6b/391098a7f0863b5e54c60244c069acfca969af56af4eb7cf52e08b009560/pydantic_core-2.18.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: bd7df92f28d351bb9f12470f4c533cf03d1b52ec5a6e5c58c65b183055a60106
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: conda
   name: pydantic-core
   version: 2.18.3
   build: py312h2615798_0
```

### Comparing `damply-0.2.0/.github/workflows/main.yaml` & `damply-0.3.0/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `damply-0.2.0/config/mkdocs.yaml` & `damply-0.3.0/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `damply-0.2.0/config/releaserc.toml` & `damply-0.3.0/config/releaserc.toml`

 * *Files identical despite different names*

### Comparing `damply-0.2.0/config/ruff.toml` & `damply-0.3.0/config/ruff.toml`

 * *Files identical despite different names*

### Comparing `damply-0.2.0/devnotes/pixi-hatch-build.md` & `damply-0.3.0/devnotes/pixi-hatch-build.md`

 * *Files identical despite different names*

### Comparing `damply-0.2.0/docs/CHANGELOG.md` & `damply-0.3.0/docs/CHANGELOG.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # CHANGELOG
 
 
 
+## v0.3.0 (2024-05-31)
+
+### Chore
+
+* chore: Delete config/.pypackage-builder-answers.yml ([`a04cabd`](https://github.com/jjjermiah/damply/commit/a04cabd468901e3b47e236a31d9eb867feea7719))
+
+### Feature
+
+* feat: add cli tool ([`077e52b`](https://github.com/jjjermiah/damply/commit/077e52bf1e3c529685a631aee6978e59676b0165))
+
+* feat: add cli ([`1e825d1`](https://github.com/jjjermiah/damply/commit/1e825d1e71293cb46fcb8abe6498b5a695982e39))
+
+
 ## v0.2.0 (2024-05-31)
 
 ### Feature
 
 * feat: Refactor metadata.py for improved readability and maintainability ([`cf909e0`](https://github.com/jjjermiah/damply/commit/cf909e0f1824fdc9275171d10c3c2a87049521e7))
 
 * feat: add tests and major class ([`569177b`](https://github.com/jjjermiah/damply/commit/569177b476047cadb22ae84d0eeb92ad1fb370ea))
```

### Comparing `damply-0.2.0/docs/about.md` & `damply-0.3.0/docs/about.md`

 * *Files identical despite different names*

### Comparing `damply-0.2.0/src/damply/metadata.py` & `damply-0.3.0/src/damply/metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 import re
 import stat
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Type
 
 from rich import print
+import rich.repr
 
 def is_file_writable(file_path: Path) -> bool:
     import os
+
     return file_path.exists() and os.access(file_path, os.W_OK)
 
+
 @dataclass
 class DMPMetadata:
     fields: dict = field(default_factory=dict)
     content: str = field(default_factory=str, repr=False)
     path: Path = field(default=Path().cwd())
     permissions: str = field(default="---------")
     logs: list = field(default_factory=list, repr=True)
@@ -38,15 +41,14 @@
 
         return metadata
 
     def log_change(self, description: str) -> None:
         timestamp = datetime.datetime.now().strftime("%Y-%m-%d %H:%M")
         self.logs.append(f"{timestamp}: {description}")
 
-
     def write_to_file(self, newpath: Path | None = None) -> None:
         newpath = newpath or self.path.with_name(self.path.stem + ".dmp")
 
         if not is_file_writable(newpath):
             raise PermissionError(f"{newpath} is not writable: {self.permissions}")
 
         # with newpath.open(mode='w') as file:
@@ -149,14 +151,20 @@
 
     def is_writeable(self) -> bool:
         return "w" in self.permissions
 
     def is_readable(self) -> bool:
         return "r" in self.permissions
 
+    def __rich_repr__(self) -> rich.repr.Result:
+        yield "path", self.path
+        yield "fields", self.fields
+        yield "content", self.content
+        yield "permissions", self.permissions
+        yield "logs", self.logs
 
 if __name__ == "__main__":
     # test the function
     cwd = Path.cwd()
     readme_example_dir = cwd / "tests" / "examples"
 
     all_dirs = list(readme_example_dir.glob("*"))
@@ -165,13 +173,12 @@
 
     dmps = []
     for file in all_files:
         dmp = DMPMetadata.from_path(file)
         print()
         dmps.append(dmp)
 
-
     print(dmps[3])
     dmps[3].log_change("Added a log entry.")
     dmps[3].log_change("Added another log entry.")
     print(dmps[3])
     dmps[3].write_to_file()
```

### Comparing `damply-0.2.0/tests/test_metadata.py` & `damply-0.3.0/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `damply-0.2.0/tests/examples/gcsi/README_gcsi.md` & `damply-0.3.0/tests/examples/gcsi/README_gcsi.md`

 * *Files 12% similar despite different names*

```diff
@@ -10,19 +10,16 @@
 [Link to Data Page](http://research-pub.gene.com/gCSI_GRvalues2019/)
 
 - Drugs and Cell Lines per drug
   - http://research-pub.gene.com/gCSI_GRvalues2019/Cell_lines_per_drug.txt
 - http://research-pub.gene.com/gCSI_GRvalues2019/gCSI_GRdata_v1.3.rds.tar.gz
 - http://research-pub.gene.com/gCSI_GRvalues2019/gCSI_GRdata_v1.3.tsv.tar.gz
 
-
-
 conda environment starting off with 
-``` bash
+```bash
 mamba create -n gcsi -c conda-forge -c bioconda r-base=4.3.1  r-essentials=4.3.0 r-data.table=1.14.8 bioconductor-CoreGx bioconductor-PharmacoGx bioconductor-annotationdbi -y 
-
 ```
 
 Download pset
-``` R
+```R
 PharmacoGx::downloadPSet(name = "gCSI_2019", saveDir = ".", verbose = TRUE, timeout=3600) 
 ```
```

### Comparing `damply-0.2.0/tests/examples/kallisto/README_kallisto.md` & `damply-0.3.0/tests/examples/kallisto/README_kallisto.md`

 * *Files identical despite different names*

### Comparing `damply-0.2.0/tests/examples/vanderijn/README_vanderijn.md` & `damply-0.3.0/tests/examples/vanderijn/README_vanderijn.md`

 * *Files identical despite different names*

### Comparing `damply-0.2.0/.gitignore` & `damply-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `damply-0.2.0/README.md` & `damply-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `damply-0.2.0/pyproject.toml` & `damply-0.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "damply"
-version = "0.2.0"
+version = "0.3.0"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["damply", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
```

### Comparing `damply-0.2.0/PKG-INFO` & `damply-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: damply
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Quick Tool For Sorting Dicom Files
 Project-URL: homepage, https://github.com/jjjermiah/damply
 Project-URL: repository, https://github.com/jjjermiah/damply
 Project-URL: documentation, https://jjjermiah.github.io/damply/
 Project-URL: changelog, https://github.com/jjjermiah/damply/blob/main/docs/CHANGELOG.md
 Project-URL: issues, https://github.com/jjjermiah/damply/issues
 Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
```

