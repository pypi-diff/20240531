# Comparing `tmp/damply-0.1.1.tar.gz` & `tmp/damply-0.2.0.tar.gz`

## Comparing `damply-0.1.1.tar` & `damply-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,55 @@
--rw-r--r--   0        0        0   401603 2020-02-02 00:00:00.000000 damply-0.1.1/pixi.lock
--rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 damply-0.1.1/.github/workflows/main.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 damply-0.1.1/config/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 damply-0.1.1/config/coverage.toml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 damply-0.1.1/config/hatch.toml
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 damply-0.1.1/config/mkdocs.yaml
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 damply-0.1.1/config/releaserc.toml
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 damply-0.1.1/config/ruff.toml
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 damply-0.1.1/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 damply-0.1.1/docs/about.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.1.1/src/damply/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 damply-0.1.1/src/damply/cli.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 damply-0.1.1/tests/test_general.py
--rw-r--r--   0        0        0     3247 2020-02-02 00:00:00.000000 damply-0.1.1/.gitignore
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 damply-0.1.1/README.md
--rw-r--r--   0        0        0     5765 2020-02-02 00:00:00.000000 damply-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 damply-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0   401603 2020-02-02 00:00:00.000000 damply-0.2.0/pixi.lock
+-rw-r--r--   0        0        0     9354 2020-02-02 00:00:00.000000 damply-0.2.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 damply-0.2.0/config/.pypackage-builder-answers.yml
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 damply-0.2.0/config/coverage.toml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 damply-0.2.0/config/hatch.toml
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 damply-0.2.0/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 damply-0.2.0/config/releaserc.toml
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 damply-0.2.0/config/ruff.toml
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 damply-0.2.0/devnotes/pixi-hatch-build.md
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 damply-0.2.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 damply-0.2.0/docs/about.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/src/damply/__init__.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 damply-0.2.0/src/damply/cli.py
+-rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 damply-0.2.0/src/damply/metadata.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 damply-0.2.0/tests/test_general.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 damply-0.2.0/tests/test_metadata.py
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/invalid_.md
+-rwxr-xr-x   0        0        0      968 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/README_gcsi.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file10.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file2.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file3.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file4.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file5.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file6.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file7.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file8.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/gcsi/test_dir_1/file9.txt
+-rwxr-xr-x   0        0        0     1210 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/kallisto/README_kallisto.md
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/README_simple.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file10.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file2.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file3.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file4.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file5.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file6.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file7.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file8.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/simple/test_dir_1/file9.txt
+-rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/README_vanderijn.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file1.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file10.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file2.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file3.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file4.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file5.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file6.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file7.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file8.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 damply-0.2.0/tests/examples/vanderijn/test_dir_1/file9.txt
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 damply-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 damply-0.2.0/README.md
+-rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 damply-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3691 2020-02-02 00:00:00.000000 damply-0.2.0/PKG-INFO
```

### Comparing `damply-0.1.1/pixi.lock` & `damply-0.2.0/pixi.lock`

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
-  version: 0.1.1
+  version: 0.2.0
   path: .
-  sha256: fbe3e7786c541551a0549533a070128b6a1c8d8604bac8f7fa32127c8a74d975
+  sha256: 3630ee5f39a1b9867c7b8c4922888289e61be29a7d0df4e9248a09fbebee3e84
   requires_dist:
   - rich
   - rich-click
   - pydantic
   - textual
   - trogon
   - dataclasses-json
@@ -5828,48 +5828,48 @@
   sha256: 0bee9bb305a562f8b9271855afb6ce00223f545de3d68560b3c1649c7c5295e9
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/e3/5c/477dac00c0d6d34921fec2507ae6aea2cd7c84072eab1dca5bcbbf86c4a2/pydantic_core-2.18.3-cp312-none-win_amd64.whl
-  sha256: 2c8333f6e934733483c7eddffdb094c143b9463d2af7e6bd85ebcb2d4a1b82c6
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
+  url: https://files.pythonhosted.org/packages/e3/5c/477dac00c0d6d34921fec2507ae6aea2cd7c84072eab1dca5bcbbf86c4a2/pydantic_core-2.18.3-cp312-none-win_amd64.whl
+  sha256: 2c8333f6e934733483c7eddffdb094c143b9463d2af7e6bd85ebcb2d4a1b82c6
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/82/ff/61c330412137b46a55b2269d0a49fd8b90e29fb57b72760b8e09b49db896/pydantic_core-2.18.3-cp310-cp310-macosx_10_12_x86_64.whl
-  sha256: 744697428fcdec6be5670460b578161d1ffe34743a5c15656be7ea82b008197c
+  url: https://files.pythonhosted.org/packages/7d/3d/1640253d1da28910b02b00bf6af4a80f1de27f561879128f76bbacb8436d/pydantic_core-2.18.3-cp310-cp310-macosx_11_0_arm64.whl
+  sha256: 37b40c05ced1ba4218b14986fe6f283d22e1ae2ff4c8e28881a70fb81fbfcda7
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/a0/27/aeade6d7b2f2bcc8fc835bdf6aa705f6f34508da380f170e13cd37477dd4/pydantic_core-2.18.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: c6ac9ffccc9d2e69d9fba841441d4259cb668ac180e51b30d3632cd7abca2b9b
+  url: https://files.pythonhosted.org/packages/82/ff/61c330412137b46a55b2269d0a49fd8b90e29fb57b72760b8e09b49db896/pydantic_core-2.18.3-cp310-cp310-macosx_10_12_x86_64.whl
+  sha256: 744697428fcdec6be5670460b578161d1ffe34743a5c15656be7ea82b008197c
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
-  url: https://files.pythonhosted.org/packages/7d/3d/1640253d1da28910b02b00bf6af4a80f1de27f561879128f76bbacb8436d/pydantic_core-2.18.3-cp310-cp310-macosx_11_0_arm64.whl
-  sha256: 37b40c05ced1ba4218b14986fe6f283d22e1ae2ff4c8e28881a70fb81fbfcda7
+  url: https://files.pythonhosted.org/packages/a0/27/aeade6d7b2f2bcc8fc835bdf6aa705f6f34508da380f170e13cd37477dd4/pydantic_core-2.18.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: c6ac9ffccc9d2e69d9fba841441d4259cb668ac180e51b30d3632cd7abca2b9b
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.3
   url: https://files.pythonhosted.org/packages/e2/67/85ee8a54220139159b14088dd40f4d43e60822f8d64bb2a5b9b04d673bd2/pydantic_core-2.18.3-cp310-none-win_amd64.whl
@@ -5892,24 +5892,24 @@
   sha256: bd7df92f28d351bb9f12470f4c533cf03d1b52ec5a6e5c58c65b183055a60106
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
-  url: https://files.pythonhosted.org/packages/d2/c7/e01cb2017c4b7b274258694f73e8bbbb0988a28b49802e569d1d9bfd51cb/pydantic_core-2.18.3-cp311-none-win_amd64.whl
-  sha256: 58ff8631dbab6c7c982e6425da8347108449321f61fe427c52ddfadd66642af7
+  url: https://files.pythonhosted.org/packages/0c/84/a14457b3cb1ec1f5d1567395abe11ab420dd76733bc79dd0124a874e9eac/pydantic_core-2.18.3-cp311-cp311-macosx_11_0_arm64.whl
+  sha256: b8e20e15d18bf7dbb453be78a2d858f946f5cdf06c5072453dace00ab652e2b2
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: conda
   name: pydantic-core
   version: 2.18.3
   build: py312h2615798_0
```

### Comparing `damply-0.1.1/.github/workflows/main.yaml` & `damply-0.2.0/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `damply-0.1.1/config/mkdocs.yaml` & `damply-0.2.0/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `damply-0.1.1/config/releaserc.toml` & `damply-0.2.0/config/releaserc.toml`

 * *Files identical despite different names*

### Comparing `damply-0.1.1/config/ruff.toml` & `damply-0.2.0/config/ruff.toml`

 * *Files 27% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 fix = true
 
 # extend-exclude is used to exclude directories from the flake8 checks
 extend-exclude = [
   "docs/*",
   "tests/*",
   ".pixi/",
-  "src/damply/textual/*.py",
-  "src/damply/subcommands/*.py",
-  "src/damply/sandbox/*.py",
-  "src/damply/*.py"
   ]
 
 extend-include = []
 
 [lint]
 select = [
   "E",
```

### Comparing `damply-0.1.1/docs/CHANGELOG.md` & `damply-0.2.0/docs/CHANGELOG.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # CHANGELOG
 
 
 
+## v0.2.0 (2024-05-31)
+
+### Feature
+
+* feat: Refactor metadata.py for improved readability and maintainability ([`cf909e0`](https://github.com/jjjermiah/damply/commit/cf909e0f1824fdc9275171d10c3c2a87049521e7))
+
+* feat: add tests and major class ([`569177b`](https://github.com/jjjermiah/damply/commit/569177b476047cadb22ae84d0eeb92ad1fb370ea))
+
+### Fix
+
+* fix: tests so it makes file ([`69d4e54`](https://github.com/jjjermiah/damply/commit/69d4e54ea76ef75dde242e28261ee79b60bc2093))
+
+
 ## v0.1.1 (2024-05-31)
 
 ### Fix
 
 * fix: some pypi issues ([`c6f810e`](https://github.com/jjjermiah/damply/commit/c6f810ea4859a45b4d9f1b3432cca1f45dc29f30))
```

### Comparing `damply-0.1.1/docs/about.md` & `damply-0.2.0/docs/about.md`

 * *Files identical despite different names*

### Comparing `damply-0.1.1/.gitignore` & `damply-0.2.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -167,7 +167,12 @@
 src/testmypixipkg/__pycache__/__init__.cpython-312.pyc
 **/__pycache__/*
 *./**/.pyc
 **.pyc
 
 **/__pycache__/*
 **/.DS_Store
+
+**/*.dmp
+**/*.log
+**/*.success
+**/*.tar.gz
```

### Comparing `damply-0.1.1/pyproject.toml` & `damply-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "damply"
-version = "0.1.1"
+version = "0.2.0"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["damply", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
@@ -36,18 +36,14 @@
 documentation = "https://jjjermiah.github.io/damply/"
 changelog = "https://github.com/jjjermiah/damply/blob/main/docs/CHANGELOG.md"
 issues = "https://github.com/jjjermiah/damply/issues"
 
 [project.scripts]
 dmp = "damply.cli:cli"
 
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
 #--------------------------------------------------------------------------------------------------#
 ############################################## PIXI ################################################
 #__________________________________________________________________________________________________#
 
 [tool.pixi.system-requirements]
 linux = "3.10.0"
 
@@ -149,41 +145,50 @@
 # Semver task will only work on the main or dev/develop branch (see releaserc.toml:branches)
 semver = 'echo "Next Version is: $(semantic-release -c config/releaserc.toml version --print)"'
 release = "semantic-release -c config/releaserc.toml version"
 
 [tool.pixi.feature.build.dependencies]
 hatch = "*"
 
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
 [tool.pixi.feature.build.tasks]
 # Builds the package
 build = { cmd = [
   "hatch",
   "build",
   "--clean",
 ], inputs = [
   "src",
   "config/hatch.toml",
   "pyproject.toml",
 ], outputs = [
   "dist/*",
 ], env = { HATCH_CONFIG = "config/hatch.toml" } }
 
-# Publishes the package to the main repository, depends on the build task
+# Publishes the package to the main PYPI repository, depends on the build task
 publish-pypi = { cmd = [
   "hatch",
   "publish",
   "--yes",
   "--repo",
   "main",
 ], inputs = [
   "dist/*",
-  "config/hatch.toml",
 ], depends-on = [
   "build",
 ], env = { HATCH_CONFIG = "config/hatch.toml" } }
 
-publish-test = { cmd = "hatch publish --yes --repo test", inputs = [
+# Publishes the package to the TEST-PYPI repository, depends on the build task
+publish-test = { cmd = [
+  "hatch",
+  "publish",
+  "--yes",
+  "--repo",
+  "test",
+], inputs = [
   "dist/*",
-  "config/hatch.toml",
 ], depends-on = [
   "build",
 ], env = { HATCH_CONFIG = "config/hatch.toml" } }
```

### Comparing `damply-0.1.1/PKG-INFO` & `damply-0.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,41 @@
-Metadata-Version: 2.3
-Name: damply
-Version: 0.1.1
-Summary: A Quick Tool For Sorting Dicom Files
-Project-URL: homepage, https://github.com/jjjermiah/damply
-Project-URL: repository, https://github.com/jjjermiah/damply
-Project-URL: documentation, https://jjjermiah.github.io/damply/
-Project-URL: changelog, https://github.com/jjjermiah/damply/blob/main/docs/CHANGELOG.md
-Project-URL: issues, https://github.com/jjjermiah/damply/issues
-Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
-Maintainer-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
-License-Expression: MIT
-Keywords: damply,package,pixi,python
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.10
-Requires-Dist: dataclasses-json
-Requires-Dist: pydantic
-Requires-Dist: rich
-Requires-Dist: rich-click
-Requires-Dist: textual
-Requires-Dist: trogon
-Description-Content-Type: text/markdown
-
 # damply
 
 [![codecov](https://codecov.io/gh/jjjermiah/damply/graph/badge.svg?token=tCcajRIGz9)](https://codecov.io/gh/jjjermiah/damply)
 [![CI-CD](https://github.com/jjjermiah/damply/actions/workflows/main.yaml/badge.svg)](https://github.com/jjjermiah/damply/actions/workflows/main.yaml)
 [![CodeFactor](https://www.codefactor.io/repository/github/jjjermiah/damply/badge)](https://www.codefactor.io/repository/github/jjjermiah/damply)
 
 [![pixi-badge](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/prefix-dev/pixi/main/assets/badge/v0.json&style=flat-square)](https://github.com/prefix-dev/pixi)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&style=flat-square)](https://github.com/pre-commit/pre-commit)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json&style=flat-square)](https://github.com/astral-sh/ruff)
 [![Built with Material for MkDocs](https://img.shields.io/badge/mkdocs--material-gray?logo=materialformkdocs&style=flat-square)](https://github.com/squidfunk/mkdocs-material)
 
-
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/damply)](https://pypi.org/project/damply/)
 [![PyPI - Version](https://img.shields.io/pypi/v/damply)](https://pypi.org/project/damply/)
 [![PyPI - Format](https://img.shields.io/pypi/format/damply)](https://pypi.org/project/damply/)
 [![Downloads](https://static.pepy.tech/badge/damply)](https://pepy.tech/project/damply)
 
+## Overview
+
+DaMPly (Data Management Plan) is a Python module designed to streamline the process of managing and packaging directories. 
+
+This tool is particularly useful for archiving project directories while leaving behind a README file to provide context and instructions for future users.
+
+## Features
+TODO
+- [ ] README Check: Verifies the presence of a README file in the specified directory.
+- [ ] User Interaction: Prompts the user for necessary information to enhance the archiving process.
+- [ ] Directory Compression: Compresses all files and sub
+
+
+## Development
+
+This project uses [`pixi`](pixi.sh) for managing the development environment.
+A set of convenient `tasks` are defined in the `pyproject.toml` file to streamline the development process.
+
+The `build` feature contains the following tasks:
+
+- `build`: Builds the package.
+- `publish-pypi`: Publishes the package to the main PYPI repository.
+- `publish-test`: Publishes the package to the TEST-PYPI repository.
+  
+For more details, view the [devnotes on pixi + hatch](devnotes/pixi-hatch-build.md).
```

