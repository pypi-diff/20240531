# Comparing `tmp/scikit_build_core-0.9.4.tar.gz` & `tmp/scikit_build_core-0.9.5.tar.gz`

## Comparing `scikit_build_core-0.9.4.tar` & `scikit_build_core-0.9.5.tar`

### file list

```diff
@@ -1,335 +1,334 @@
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.gitattributes
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.packit.yaml
--rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.readthedocs.yml
--rw-r--r--   0        0        0     8617 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/noxfile.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/python-scikit-build-core.rpmlintrc
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/python-scikit-build-core.spec
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/.fmf/version
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/plans/examples.fmf
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/plans/main.fmf.dist-git
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/plans/rpminspect.fmf
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/plans/rpmlint.fmf
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/plans/smoke.fmf
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.distro/tests/smoke.fmf
--rw-r--r--   0        0        0    10258 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.github/codecov.yml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.github/dependabot.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.github/release.yml
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.github/workflows/cd.yml
--rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/build.md
--rw-r--r--   0        0        0    32025 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/changelog.md
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/cmakelists.md
--rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/conf.py
--rw-r--r--   0        0        0    19835 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/configuration.md
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/crosscompile.md
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/faqs.md
--rw-r--r--   0        0        0    10874 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/getting_started.md
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/index.md
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/man.md
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/migration_guide.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/.fmf/version
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.build.rst
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.builder.rst
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.file_api.model.rst
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.file_api.rst
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.hatch.rst
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.metadata.rst
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.resources.find_python.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.resources.rst
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.rst
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.settings.rst
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/api/scikit_build_core.setuptools.rst
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/main.fmf
--rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/test.sh
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/main.fmf
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/CMakeLists.txt
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/LICENSE
--rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/README.md
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/main.fmf
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/pyproject.toml
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/src/nanobind_example_ext.cpp
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/src/nanobind_example/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/tests/test_basic.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/CMakeLists.txt
--rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/LICENSE
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/README.md
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/main.fmf
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/pyproject.toml
--rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/src/main.cpp
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/src/scikit_build_example/__init__.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/tests/test_basic.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/test.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/abi3/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/abi3/example.c
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/abi3/main.fmf
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/abi3/pyproject.toml
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/c/CMakeLists.txt
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/c/example.c
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/c/main.fmf
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/c/pyproject.toml
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/cython/CMakeLists.txt
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/cython/example.pyx
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/cython/main.fmf
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/cython/pyproject.toml
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/fortran/CMakeLists.txt
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/fortran/example.f
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/fortran/main.fmf
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/fortran/pyproject.toml
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/nanobind/CMakeLists.txt
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/nanobind/example.cpp
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/nanobind/main.fmf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/nanobind/pyproject.toml
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/pybind11/CMakeLists.txt
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/pybind11/example.cpp
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/pybind11/main.fmf
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/pybind11/pyproject.toml
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/swig/CMakeLists.txt
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/swig/example.c
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/swig/example.i
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/swig/main.fmf
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/examples/getting_started/swig/pyproject.toml
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/ext/conftabs.py
--rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/plugins/hatchling.md
--rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/docs/plugins/setuptools.md
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/__init__.py
--rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_logging.py
--rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_shutil.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_version.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_version.pyi
--rw-r--r--   0        0        0    10019 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/cmake.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/errors.py
--rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/program_search.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/py.typed
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_compat/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_compat/builtins.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_compat/tomllib.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_compat/typing.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_compat/importlib/__init__.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_compat/importlib/metadata.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_compat/importlib/resources.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_vendor/pyproject_metadata/LICENSE
--rw-r--r--   0        0        0    20882 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/_vendor/pyproject_metadata/__init__.py
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/__init__.py
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/_editable.py
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/_file_processor.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/_init.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/_pathutil.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/_scripts.py
--rw-r--r--   0        0        0     8645 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/_wheelfile.py
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/generate.py
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/metadata.py
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/sdist.py
--rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/build/wheel.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/__init__.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/__main__.py
--rw-r--r--   0        0        0     9190 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/builder.py
--rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/generator.py
--rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/get_requires.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/macos.py
--rw-r--r--   0        0        0     6304 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/sysconfig.py
--rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/builder/wheel_tag.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/__init__.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/_cattrs_converter.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/query.py
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/reply.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/cache.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/cmakefiles.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/codemodel.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/common.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/directory.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/index.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/toolchains.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/hatch/__init__.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/hatch/hooks.py
--rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/hatch/plugin.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/metadata/__init__.py
--rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/metadata/fancy_pypi_readme.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/metadata/regex.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/metadata/setuptools_scm.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/__init__.py
--rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/_editable_redirect.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/known_wheels.toml
--rw-r--r--   0        0        0    21268 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/scikit-build.schema.json
--rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/Copyright.txt
--rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
--rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPython.cmake
--rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPython3.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/__init__.py
--rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/__init__.py
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/_load_provider.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/documentation.py
--rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/json_schema.py
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_docs.py
--rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_model.py
--rw-r--r--   0        0        0    15816 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_read_settings.py
--rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_schema.py
--rw-r--r--   0        0        0    21975 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/settings/sources.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/setuptools/__init__.py
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/setuptools/build_cmake.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/setuptools/build_meta.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/src/scikit_build_core/setuptools/wrapper.py
--rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/conftest.py
--rw-r--r--   0        0        0      373 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/constraints.txt
--rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_builder.py
--rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_cmake_config.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_custom_modules.py
--rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_dynamic_metadata.py
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_editable.py
--rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_editable_redirect.py
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_editable_unit.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_file_processor.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_fileapi.py
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_fortran.py
--rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_generator_default.py
--rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_get_requires.py
--rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_hatchling.py
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_json_schema.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_logging.py
--rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_module_dir.py
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_name_main.py
--rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_prepare_metadata.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_printouts.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_process_scripts.py
--rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_program_search.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_pyproject_abi3.py
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_pyproject_extra_dirs.py
--rw-r--r--   0        0        0    10864 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_pyproject_pep517.py
--rw-r--r--   0        0        0     7728 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_pyproject_pep518.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_pyproject_pep660.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_pyproject_purelib.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_schema.py
--rw-r--r--   0        0        0    19424 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_settings.py
--rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_settings_overrides.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_setuptools_abi3.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_setuptools_pep517.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_setuptools_pep518.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_shutil.py
--rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_simple_pure.py
--rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_simplest_c.py
--rw-r--r--   0        0        0    19242 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_skbuild_settings.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/test_wheelfile_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
--rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_pyproject_ext/abi3_example.c
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_setuptools_ext/abi3_example.c
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_setuptools_ext/setup.cfg
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/abi3_setuptools_ext/setup.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/CMakeLists.txt
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/pyproject.toml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/extern/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
--rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/custom_cmake/scripts/script1
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg1/CMakeLists.txt
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg1/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg1/src/pkg1/__init__.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg1/src/pkg1/one.pxd
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg1/src/pkg1/one.pyx
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg2/CMakeLists.txt
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg2/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg2/src/pkg2/__init__.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg2/src/pkg2/two.pyx
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/CMakeLists.txt
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/dual_project.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/faulty_dual_project.toml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/faulty_project.toml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/local_pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/plugin_project.toml
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/pyproject.toml
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/warn_project.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/src/module.c
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/dynamic_metadata/src/dynamic/__init__.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/filepath_pure/CMakeLists.txt
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/filepath_pure/pyproject.toml
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/fortran_example/CMakeLists.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/fortran_example/fib1.f
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/fortran_example/pyproject.toml
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/hatchling/.gitignore
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/hatchling/pyproject.toml
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/hatchling/cpp/CMakeLists.txt
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/hatchling/cpp/example.cpp
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/hatchling/src/hatchling_example/__init__.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/hatchling/src/hatchling_example/_core.pyi
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/mixed_setuptools/CMakeLists.txt
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/mixed_setuptools/pyproject.toml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/mixed_setuptools/setup.cfg
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/mixed_setuptools/setup.py
--rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/mixed_setuptools/src/main.cpp
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/CMakeLists.txt
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/pyproject.toml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/python/shared_pkg/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/python/shared_pkg/c_module.pyi
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/python/shared_pkg/py_module.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/python/shared_pkg/data/py_data.txt
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/src/shared_pkg/c_module.c
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/navigate_editable/src/shared_pkg/data/generated.txt.in
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/sdist_config/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/sdist_config/CMakeLists.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/sdist_config/input.cmake
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/sdist_config/main.cpp
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/sdist_config/pyproject.toml
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pure/CMakeLists.txt
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pure/simple_pure.cpp
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_purelib_package/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_purelib_package/src/purelib_example/__init__.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_ext/LICENSE
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_ext/pyproject.toml
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_ext/src/main.cpp
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_script_with_flags/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_script_with_flags/LICENSE
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_script_with_flags/pyproject.toml
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_script_with_flags/src/main.c
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_source_dir/LICENSE
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_source_dir/pyproject.toml
--rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_pyproject_source_dir/src/main.cpp
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_setuptools_ext/CMakeLists.txt
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_setuptools_ext/LICENSE
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_setuptools_ext/pyproject.toml
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_setuptools_ext/setup.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simple_setuptools_ext/src/main.cpp
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/.gitignore
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/CMakeLists.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/pyproject.toml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/module.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/not_a_package/simple.txt
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/_module.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/excluded.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/ignored.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/ignored_included.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/tests/packages/simplest_c/src/simplest/sdist_only.txt
--rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/.gitignore
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/LICENSE
--rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/README.md
--rw-r--r--   0        0        0    11393 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/pyproject.toml
--rw-r--r--   0        0        0    19948 2020-02-02 00:00:00.000000 scikit_build_core-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.gitattributes
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.packit.yaml
+-rw-r--r--   0        0        0     3809 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.readthedocs.yml
+-rw-r--r--   0        0        0     8612 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/noxfile.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.distro/python-scikit-build-core.rpmlintrc
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.distro/python-scikit-build-core.spec
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.distro/.fmf/version
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.distro/plans/examples.fmf
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.distro/plans/main.fmf.dist-git
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.distro/plans/rpminspect.fmf
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.distro/plans/rpmlint.fmf
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.distro/plans/smoke.fmf
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.distro/tests/smoke.fmf
+-rw-r--r--   0        0        0    10258 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.github/codecov.yml
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.github/dependabot.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.github/release.yml
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     9414 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     7621 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/build.md
+-rw-r--r--   0        0        0    32551 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/changelog.md
+-rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/cmakelists.md
+-rw-r--r--   0        0        0     4967 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/conf.py
+-rw-r--r--   0        0        0    19958 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/configuration.md
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/crosscompile.md
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/faqs.md
+-rw-r--r--   0        0        0    10874 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/getting_started.md
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/index.md
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/man.md
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/migration_guide.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/.fmf/version
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/api/scikit_build_core.build.rst
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/api/scikit_build_core.builder.rst
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/api/scikit_build_core.file_api.model.rst
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/api/scikit_build_core.file_api.rst
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/api/scikit_build_core.hatch.rst
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/api/scikit_build_core.metadata.rst
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/api/scikit_build_core.resources.find_python.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/api/scikit_build_core.resources.rst
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/api/scikit_build_core.rst
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/api/scikit_build_core.settings.rst
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/api/scikit_build_core.setuptools.rst
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/main.fmf
+-rwxr-xr-x   0        0        0     1074 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/test.sh
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/main.fmf
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/nanobind_example/CMakeLists.txt
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/nanobind_example/LICENSE
+-rw-r--r--   0        0        0     2208 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/nanobind_example/README.md
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/nanobind_example/main.fmf
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/nanobind_example/pyproject.toml
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/nanobind_example/src/nanobind_example_ext.cpp
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/nanobind_example/src/nanobind_example/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/nanobind_example/tests/test_basic.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/pybind11_example/CMakeLists.txt
+-rw-r--r--   0        0        0     2182 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/pybind11_example/LICENSE
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/pybind11_example/README.md
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/pybind11_example/main.fmf
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/pybind11_example/pyproject.toml
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/pybind11_example/src/main.cpp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/pybind11_example/src/scikit_build_example/__init__.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/downstream/pybind11_example/tests/test_basic.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/test.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/abi3/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/abi3/example.c
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/abi3/main.fmf
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/abi3/pyproject.toml
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/c/CMakeLists.txt
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/c/example.c
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/c/main.fmf
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/c/pyproject.toml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/cython/CMakeLists.txt
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/cython/example.pyx
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/cython/main.fmf
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/cython/pyproject.toml
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/fortran/CMakeLists.txt
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/fortran/example.f
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/fortran/main.fmf
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/fortran/pyproject.toml
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/nanobind/CMakeLists.txt
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/nanobind/example.cpp
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/nanobind/main.fmf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/nanobind/pyproject.toml
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/pybind11/CMakeLists.txt
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/pybind11/example.cpp
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/pybind11/main.fmf
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/pybind11/pyproject.toml
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/swig/CMakeLists.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/swig/example.c
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/swig/example.i
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/swig/main.fmf
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/examples/getting_started/swig/pyproject.toml
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/ext/conftabs.py
+-rw-r--r--   0        0        0     2432 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/plugins/hatchling.md
+-rw-r--r--   0        0        0     2284 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/docs/plugins/setuptools.md
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/__init__.py
+-rw-r--r--   0        0        0     3863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/_logging.py
+-rw-r--r--   0        0        0     3114 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/_shutil.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/_version.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/_version.pyi
+-rw-r--r--   0        0        0    10027 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/cmake.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/errors.py
+-rw-r--r--   0        0        0     5785 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/program_search.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/py.typed
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/_compat/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/_compat/builtins.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/_compat/tomllib.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/_compat/typing.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/_compat/importlib/__init__.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/_compat/importlib/metadata.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/_compat/importlib/resources.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/_vendor/pyproject_metadata/LICENSE
+-rw-r--r--   0        0        0    20882 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/_vendor/pyproject_metadata/__init__.py
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/build/__init__.py
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/build/_editable.py
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/build/_file_processor.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/build/_init.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/build/_pathutil.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/build/_scripts.py
+-rw-r--r--   0        0        0     8645 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/build/_wheelfile.py
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/build/generate.py
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/build/metadata.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/build/sdist.py
+-rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/build/wheel.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/builder/__init__.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/builder/__main__.py
+-rw-r--r--   0        0        0     9190 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/builder/builder.py
+-rw-r--r--   0        0        0     3855 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/builder/generator.py
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/builder/get_requires.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/builder/macos.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/builder/sysconfig.py
+-rw-r--r--   0        0        0     5806 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/builder/wheel_tag.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/file_api/__init__.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/file_api/_cattrs_converter.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/file_api/query.py
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/file_api/reply.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/file_api/model/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/file_api/model/cache.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/file_api/model/cmakefiles.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/file_api/model/codemodel.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/file_api/model/common.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/file_api/model/directory.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/file_api/model/index.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/file_api/model/toolchains.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/hatch/__init__.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/hatch/hooks.py
+-rw-r--r--   0        0        0    10786 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/hatch/plugin.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/metadata/__init__.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/metadata/fancy_pypi_readme.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/metadata/regex.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/metadata/setuptools_scm.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/resources/__init__.py
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/resources/_editable_redirect.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/resources/known_wheels.toml
+-rw-r--r--   0        0        0    21268 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/resources/scikit-build.schema.json
+-rw-r--r--   0        0        0     5477 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/resources/find_python/Copyright.txt
+-rw-r--r--   0        0        0    23174 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake
+-rw-r--r--   0        0        0    22536 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/resources/find_python/FindPython.cmake
+-rw-r--r--   0        0        0    19036 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/resources/find_python/FindPython3.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/resources/find_python/__init__.py
+-rw-r--r--   0        0        0   198528 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/resources/find_python/FindPython/Support.cmake
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/settings/__init__.py
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/settings/_load_provider.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/settings/documentation.py
+-rw-r--r--   0        0        0     5009 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/settings/json_schema.py
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/settings/skbuild_docs.py
+-rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/settings/skbuild_model.py
+-rw-r--r--   0        0        0    15816 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/settings/skbuild_read_settings.py
+-rw-r--r--   0        0        0     6577 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/settings/skbuild_schema.py
+-rw-r--r--   0        0        0    21975 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/settings/sources.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/setuptools/__init__.py
+-rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/setuptools/build_cmake.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/setuptools/build_meta.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/src/scikit_build_core/setuptools/wrapper.py
+-rw-r--r--   0        0        0    10427 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/conftest.py
+-rw-r--r--   0        0        0     9106 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_builder.py
+-rw-r--r--   0        0        0     4556 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_cmake_config.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_custom_modules.py
+-rw-r--r--   0        0        0     9172 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_dynamic_metadata.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_editable.py
+-rw-r--r--   0        0        0     2206 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_editable_redirect.py
+-rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_editable_unit.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_file_processor.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_fileapi.py
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_fortran.py
+-rw-r--r--   0        0        0    15811 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_generator_default.py
+-rw-r--r--   0        0        0     4859 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_get_requires.py
+-rw-r--r--   0        0        0     2246 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_hatchling.py
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_json_schema.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_logging.py
+-rw-r--r--   0        0        0     1937 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_module_dir.py
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_name_main.py
+-rw-r--r--   0        0        0     2489 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_prepare_metadata.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_printouts.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_process_scripts.py
+-rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_program_search.py
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_pyproject_abi3.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_pyproject_extra_dirs.py
+-rw-r--r--   0        0        0    10864 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_pyproject_pep517.py
+-rw-r--r--   0        0        0     7728 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_pyproject_pep518.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_pyproject_pep660.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_pyproject_purelib.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_schema.py
+-rw-r--r--   0        0        0    19424 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_settings.py
+-rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_settings_overrides.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_setuptools_abi3.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_setuptools_pep517.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_setuptools_pep518.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_shutil.py
+-rw-r--r--   0        0        0     3073 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_simple_pure.py
+-rw-r--r--   0        0        0     5035 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_simplest_c.py
+-rw-r--r--   0        0        0    19242 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_skbuild_settings.py
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/test_wheelfile_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/query/cache-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/query/cmakeFiles-v1
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/query/codemodel-v2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/query/toolchains-v1
+-rw-r--r--   0        0        0    20671 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/abi3_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/abi3_pyproject_ext/abi3_example.c
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/abi3_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/abi3_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/abi3_setuptools_ext/abi3_example.c
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/abi3_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/abi3_setuptools_ext/setup.cfg
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/abi3_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/custom_cmake/CMakeLists.txt
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/custom_cmake/pyproject.toml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/custom_cmake/extern/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/__init__.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/ExampleInclude.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_modules/__init__.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/ExamplePkgConfig.cmake
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/custom_cmake/extern/custom_cmake_testing_stuff/cmake_prefix/__init__.py
+-rwxr-xr-x   0        0        0       82 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/custom_cmake/scripts/script1
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/cython_pxd_editable/pkg1/CMakeLists.txt
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/cython_pxd_editable/pkg1/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/cython_pxd_editable/pkg1/src/pkg1/__init__.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/cython_pxd_editable/pkg1/src/pkg1/one.pxd
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/cython_pxd_editable/pkg1/src/pkg1/one.pyx
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/cython_pxd_editable/pkg2/CMakeLists.txt
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/cython_pxd_editable/pkg2/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/cython_pxd_editable/pkg2/src/pkg2/__init__.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/cython_pxd_editable/pkg2/src/pkg2/two.pyx
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/dynamic_metadata/CMakeLists.txt
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/dynamic_metadata/dual_project.toml
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/dynamic_metadata/faulty_dual_project.toml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/dynamic_metadata/faulty_project.toml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/dynamic_metadata/local_pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/dynamic_metadata/plugin_project.toml
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/dynamic_metadata/pyproject.toml
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/dynamic_metadata/warn_project.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/dynamic_metadata/plugins/local/version/__init__.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/dynamic_metadata/plugins/local/version/nested/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/dynamic_metadata/src/module.c
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/dynamic_metadata/src/dynamic/__init__.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/filepath_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/filepath_pure/pyproject.toml
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/fortran_example/CMakeLists.txt
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/fortran_example/fib1.f
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/fortran_example/pyproject.toml
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/hatchling/.gitignore
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/hatchling/pyproject.toml
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/hatchling/cpp/CMakeLists.txt
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/hatchling/cpp/example.cpp
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/hatchling/src/hatchling_example/__init__.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/hatchling/src/hatchling_example/_core.pyi
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/mixed_setuptools/CMakeLists.txt
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/mixed_setuptools/pyproject.toml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/mixed_setuptools/setup.cfg
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/mixed_setuptools/setup.py
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/mixed_setuptools/src/main.cpp
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/mixed_setuptools/src/mixed_setuptools/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/mixed_setuptools/src/mixed_setuptools/_core.pyi
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/navigate_editable/CMakeLists.txt
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/navigate_editable/pyproject.toml
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/navigate_editable/python/shared_pkg/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/navigate_editable/python/shared_pkg/c_module.pyi
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/navigate_editable/python/shared_pkg/py_module.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/navigate_editable/python/shared_pkg/data/py_data.txt
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/navigate_editable/src/shared_pkg/c_module.c
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/navigate_editable/src/shared_pkg/data/generated.txt.in
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/sdist_config/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/sdist_config/CMakeLists.txt
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/sdist_config/input.cmake
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/sdist_config/main.cpp
+-rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/sdist_config/pyproject.toml
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_pure/CMakeLists.txt
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_pure/simple_pure.cpp
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_purelib_package/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_purelib_package/src/purelib_example/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_pyproject_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_pyproject_ext/LICENSE
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_pyproject_ext/pyproject.toml
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_pyproject_ext/src/main.cpp
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_pyproject_script_with_flags/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_pyproject_script_with_flags/LICENSE
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_pyproject_script_with_flags/pyproject.toml
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_pyproject_script_with_flags/src/main.c
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_pyproject_source_dir/LICENSE
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_pyproject_source_dir/pyproject.toml
+-rw-r--r--   0        0        0      465 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_pyproject_source_dir/src/CMakeLists.txt
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_pyproject_source_dir/src/main.cpp
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_setuptools_ext/CMakeLists.txt
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_setuptools_ext/LICENSE
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_setuptools_ext/pyproject.toml
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_setuptools_ext/setup.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simple_setuptools_ext/src/main.cpp
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simplest_c/.gitignore
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simplest_c/CMakeLists.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simplest_c/pyproject.toml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simplest_c/src/module.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simplest_c/src/not_a_package/simple.txt
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simplest_c/src/simplest/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simplest_c/src/simplest/_module.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simplest_c/src/simplest/artifact_ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simplest_c/src/simplest/data.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simplest_c/src/simplest/excluded.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simplest_c/src/simplest/ignored.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simplest_c/src/simplest/ignored_included.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/tests/packages/simplest_c/src/simplest/sdist_only.txt
+-rw-r--r--   0        0        0     2519 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/.gitignore
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/LICENSE
+-rw-r--r--   0        0        0    15572 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/README.md
+-rw-r--r--   0        0        0    11391 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0    19946 2020-02-02 00:00:00.000000 scikit_build_core-0.9.5/PKG-INFO
```

### Comparing `scikit_build_core-0.9.4/.packit.yaml` & `scikit_build_core-0.9.5/.packit.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -29,22 +29,17 @@
 
 jobs:
   - &copr_build
     job: copr_build
     trigger: release
     owner: "@scikit-build"
     project: release
-    # Drop F38 due to dependency
     targets: &targets
-      - fedora-latest-x86_64
-      - fedora-latest-aarch64
-      - fedora-latest-stable-x86_64
-      - fedora-latest-stable-aarch64
-      - fedora-development-x86_64
-      - fedora-development-aarch64
+      - fedora-all-x86_64
+      - fedora-all-aarch64
   - &tests
     job: tests
     trigger: release
     targets: *targets
     fmf_path: .distro
   - <<: *copr_build
     trigger: commit
```

### Comparing `scikit_build_core-0.9.4/.pre-commit-config.yaml` & `scikit_build_core-0.9.5/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         args: ["--pytest-test-first"]
         exclude: "^tests/packages/"
       - id: requirements-txt-fixer
       - id: trailing-whitespace
         exclude: "^tests"
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.4.4
+    rev: v0.4.5
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
       - id: ruff-format
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.10.0
@@ -93,15 +93,15 @@
       - id: check-sdist
         args: [--inject-junk]
         additional_dependencies:
           - hatchling
           - hatch-vcs
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.6
+    rev: v2.3.0
     hooks:
       - id: codespell
         exclude: ^(LICENSE$|src/scikit_build_core/resources/find_python|tests/test_skbuild_settings.py$)
 
   - repo: https://github.com/shellcheck-py/shellcheck-py
     rev: v0.10.0.1
     hooks:
@@ -117,19 +117,19 @@
       - id: disallow-expressions
         name: Disallow expressions
         language: pygrep
         entry: tool\.cmake
         exclude: .pre-commit-config.yaml
 
   - repo: https://github.com/henryiii/validate-pyproject-schema-store
-    rev: 2024.04.29
+    rev: 2024.05.24
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.28.3
+    rev: 0.28.4
     hooks:
       - id: check-dependabot
       - id: check-github-workflows
       - id: check-readthedocs
       - id: check-metaschema
         files: \.schema\.json
```

### Comparing `scikit_build_core-0.9.4/noxfile.py` & `scikit_build_core-0.9.5/noxfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,16 +66,15 @@
 
     _extras = ["test", *extras]
     if "--cov" in posargs:
         _extras.append("cov")
         posargs.append("--cov-config=pyproject.toml")
 
     install_arg = f"-e.[{','.join(_extras)}]"
-    session.install(install_arg, *install_args)
-    session.run("pip", "list")
+    session.install(install_arg, *install_args, silent=False)
     session.run("pytest", *run_args, *posargs, env=env)
 
 
 @nox.session(reuse_venv=True)
 def generate_schema(session: nox.Session) -> None:
     """
     (Re)generate src/scikit_build_core/resources/scikit-build.schema.json from model.
@@ -105,22 +104,23 @@
 
     args = session.posargs or ["-r"]
 
     session.install("-e.", "cogapp")
     session.run("cog", "-P", *args, "README.md")
 
 
-@nox.session
+@nox.session(venv_backend="uv")
 def minimums(session: nox.Session) -> None:
     """
     Test the minimum versions of dependencies.
     """
+
     _run_tests(
         session,
-        install_args=["--constraint=tests/constraints.txt"],
+        install_args=["--resolution=lowest-direct"],
         run_args=["-Wdefault"],
     )
 
 
 @nox.session(reuse_venv=True)
 def docs(session: nox.Session) -> None:
     """
```

### Comparing `scikit_build_core-0.9.4/.distro/python-scikit-build-core.spec` & `scikit_build_core-0.9.5/.distro/python-scikit-build-core.spec`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/.github/CONTRIBUTING.md` & `scikit_build_core-0.9.5/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/.github/workflows/cd.yml` & `scikit_build_core-0.9.5/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/.github/workflows/ci.yml` & `scikit_build_core-0.9.5/.github/workflows/ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     timeout-minutes: 8
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - uses: actions/setup-python@v5
         with:
-          python-version: "3.11"
+          python-version: "3.12"
       - uses: pre-commit/action@v3.0.1
         with:
           extra_args: --hook-stage manual --all-files
       - name: Run PyLint
         run: pipx run nox -s pylint -- --output-format=github
       - name: Run nox generator
         run: |
@@ -115,18 +115,30 @@
       - name: Install package (pip)
         if:
           matrix.python-version == '3.7' || matrix.python-version == 'pypy-3.8'
           || matrix.python-version == 'pypy-3.7'
         run: pip install -e.[test,test-meta,test-numpy,test-schema,wheels,cov]
 
       - name: Test package
+        if: "!contains(matrix.python_version, 'pypy')"
         run: >-
           pytest -ra --showlocals --cov --cov-report=xml --cov-report=term
           --durations=20
 
+      - name: Test package (two attempts)
+        uses: nick-fields/retry@v3
+        if: "contains(matrix.python_version, 'pypy')"
+        with:
+          max_attempts: 2
+          retry_on: error
+          timeout_seconds: 5
+          command: >-
+            pytest -ra --showlocals --cov --cov-report=xml --cov-report=term
+            --durations=20
+
       - name: Upload coverage report
         uses: codecov/codecov-action@v4
         with:
           name:
             ${{ runner.os }}-${{ matrix.python-version }}-${{
             matrix.cmake-version }}
           verbose: true
@@ -135,28 +147,34 @@
   min:
     name: Min 🐍 ${{ matrix.python-version }} on ${{ matrix.runs-on }}
     runs-on: ${{ matrix.runs-on }}
     timeout-minutes: 40
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.7", "3.11"]
+        python-version: ["3.8", "3.11"]
         runs-on: [ubuntu-latest, macos-13, windows-latest]
 
     steps:
       - uses: actions/checkout@v4
 
       - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
+      - uses: yezz123/setup-uv@v4
+
       # The min requirements are not compatible with some of the extra test
       # deps, so limit to just built-in deps.
-      - name: Min requirements
-        run: pip install --constraint tests/constraints.txt .[test] ninja
+      - name: Install extra helpers
+        run: uv pip install ninja --system
+
+      - name: Install min requirements
+        run: |
+          uv pip install -e .[test,pyproject] --resolution=lowest-direct --system
 
       - name: Setup CMake 3.15
         uses: jwlawson/actions-setup-cmake@v2.0
         if: runner.os != 'Windows'
         with:
           cmake-version: "3.15.x"
```

### Comparing `scikit_build_core-0.9.4/docs/build.md` & `scikit_build_core-0.9.5/docs/build.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/changelog.md` & `scikit_build_core-0.9.5/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,43 @@
 # Changelog
 
+This release fixes building for the the Windows variant of free-threaded Python
+3.13.
+
+Fixes:
+
+- Support Windows free-threading by @henryiii in #759
+- Strip whitespace around generator so that it's passed through correctly by
+  @vyasr in #748
+
+Documentation:
+
+- Note that `-C` options can be prefixed with `skbuild.` by @KyleFromNVIDIA in
+  #754
+
+CI and testing:
+
+- Retry pypy if fails by @henryiii in #746
+- Disable rpminspect on rawhide by @LecrisUT in #753
+- Use uv for minimum version check by @henryiii in #679
+
 ## Version 0.9.4
 
 This version supports the newly available free-threading variant of Python
 3.13b1 (mostly related to skipping the stable ABI). We test this via the
 manylinux/musllinux images. There's also a new feature requested by third-party
 packagers; the ability to pass args directly to the build tool
 
 Features:
 
 - Add `build.tool-args` by @henryiii in #733
 
 Fixes:
 
-- Support free-threaded builds of Python 3.13+ by @henryiii in #741
+- Support free-threaded builds of Python 3.13+ on Linux by @henryiii in #741
 - Slightly better stable ABI behavior using PyPy by @henryiii in #741
 
 Documentation:
 
 - Fix example of configuration overrides in configuration.md by @wu-vincent in
   #739
 - Update stable ABI instructions by @henryiii in #740
```

### Comparing `scikit_build_core-0.9.4/docs/cmakelists.md` & `scikit_build_core-0.9.5/docs/cmakelists.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/conf.py` & `scikit_build_core-0.9.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/configuration.md` & `scikit_build_core-0.9.5/docs/configuration.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # Configuration
 
 Scikit-build-core supports a powerful unified configuration system. Every option
 in scikit-build-core can be specified in one of three ways: as a
 `pyproject.toml` option (preferred if static), as a config-settings options
-(preferred if dynamic), or as an environment variable.
+(preferred if dynamic), or as an environment variable. Note that config-settings
+options can optionally be prefixed with `skbuild.`, for example
+`-C skbuild.logging.level=INFO`.
 
 (verbosity)=
 
 ## Verbosity
 
 You can increase the verbosity of the build with two settings - `cmake.verbose`
 is a shortcut for verbose build output, and logging.level controls
```

### Comparing `scikit_build_core-0.9.4/docs/crosscompile.md` & `scikit_build_core-0.9.5/docs/crosscompile.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/faqs.md` & `scikit_build_core-0.9.5/docs/faqs.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/getting_started.md` & `scikit_build_core-0.9.5/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/index.md` & `scikit_build_core-0.9.5/docs/index.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/migration_guide.md` & `scikit_build_core-0.9.5/docs/migration_guide.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/api/scikit_build_core.build.rst` & `scikit_build_core-0.9.5/docs/api/scikit_build_core.build.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/api/scikit_build_core.builder.rst` & `scikit_build_core-0.9.5/docs/api/scikit_build_core.builder.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/api/scikit_build_core.file_api.model.rst` & `scikit_build_core-0.9.5/docs/api/scikit_build_core.file_api.model.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/api/scikit_build_core.file_api.rst` & `scikit_build_core-0.9.5/docs/api/scikit_build_core.file_api.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/api/scikit_build_core.hatch.rst` & `scikit_build_core-0.9.5/docs/api/scikit_build_core.hatch.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/api/scikit_build_core.metadata.rst` & `scikit_build_core-0.9.5/docs/api/scikit_build_core.metadata.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/api/scikit_build_core.rst` & `scikit_build_core-0.9.5/docs/api/scikit_build_core.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/api/scikit_build_core.settings.rst` & `scikit_build_core-0.9.5/docs/api/scikit_build_core.settings.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/api/scikit_build_core.setuptools.rst` & `scikit_build_core-0.9.5/docs/api/scikit_build_core.setuptools.rst`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/examples/test.sh` & `scikit_build_core-0.9.5/docs/examples/test.sh`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/CMakeLists.txt` & `scikit_build_core-0.9.5/docs/examples/downstream/nanobind_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/LICENSE` & `scikit_build_core-0.9.5/docs/examples/downstream/nanobind_example/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/README.md` & `scikit_build_core-0.9.5/docs/examples/downstream/nanobind_example/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/examples/downstream/nanobind_example/pyproject.toml` & `scikit_build_core-0.9.5/docs/examples/downstream/nanobind_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/LICENSE` & `scikit_build_core-0.9.5/docs/examples/downstream/pybind11_example/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/README.md` & `scikit_build_core-0.9.5/docs/examples/downstream/pybind11_example/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/pyproject.toml` & `scikit_build_core-0.9.5/docs/examples/downstream/pybind11_example/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/examples/downstream/pybind11_example/src/main.cpp` & `scikit_build_core-0.9.5/docs/examples/downstream/pybind11_example/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/examples/getting_started/abi3/example.c` & `scikit_build_core-0.9.5/docs/examples/getting_started/abi3/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/examples/getting_started/c/example.c` & `scikit_build_core-0.9.5/docs/examples/getting_started/c/example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/examples/getting_started/cython/CMakeLists.txt` & `scikit_build_core-0.9.5/docs/examples/getting_started/cython/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/examples/getting_started/fortran/CMakeLists.txt` & `scikit_build_core-0.9.5/docs/examples/getting_started/fortran/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/examples/getting_started/swig/CMakeLists.txt` & `scikit_build_core-0.9.5/docs/examples/getting_started/swig/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/ext/conftabs.py` & `scikit_build_core-0.9.5/docs/ext/conftabs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/plugins/hatchling.md` & `scikit_build_core-0.9.5/docs/plugins/hatchling.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/docs/plugins/setuptools.md` & `scikit_build_core-0.9.5/docs/plugins/setuptools.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/_logging.py` & `scikit_build_core-0.9.5/src/scikit_build_core/_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/_shutil.py` & `scikit_build_core-0.9.5/src/scikit_build_core/_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/cmake.py` & `scikit_build_core-0.9.5/src/scikit_build_core/cmake.py`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
     def get_generator(self, *args: str) -> str | None:
         """
         Try to get the generator that will be used to build the project. If it's
         not set, return None (default generator will be used).
         """
         generators = [g for g in args if g.startswith("-G")]
         if generators:
-            return generators[-1][2:]
+            return generators[-1][2:].strip()
         return self.env.get("CMAKE_GENERATOR", None)
 
     def configure(
         self,
         *,
         defines: Mapping[str, str | os.PathLike[str] | bool] | None = None,
         cmake_args: Sequence[str] = (),
```

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/errors.py` & `scikit_build_core-0.9.5/src/scikit_build_core/errors.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/program_search.py` & `scikit_build_core-0.9.5/src/scikit_build_core/program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/_compat/typing.py` & `scikit_build_core-0.9.5/src/scikit_build_core/_compat/typing.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/_compat/importlib/metadata.py` & `scikit_build_core-0.9.5/src/scikit_build_core/_compat/importlib/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/_vendor/pyproject_metadata/LICENSE` & `scikit_build_core-0.9.5/src/scikit_build_core/_vendor/pyproject_metadata/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/_vendor/pyproject_metadata/__init__.py` & `scikit_build_core-0.9.5/src/scikit_build_core/_vendor/pyproject_metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/build/__init__.py` & `scikit_build_core-0.9.5/src/scikit_build_core/build/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/build/_editable.py` & `scikit_build_core-0.9.5/src/scikit_build_core/build/_editable.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/build/_file_processor.py` & `scikit_build_core-0.9.5/src/scikit_build_core/build/_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/build/_init.py` & `scikit_build_core-0.9.5/src/scikit_build_core/build/_init.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/build/_pathutil.py` & `scikit_build_core-0.9.5/src/scikit_build_core/build/_pathutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/build/_scripts.py` & `scikit_build_core-0.9.5/src/scikit_build_core/build/_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/build/_wheelfile.py` & `scikit_build_core-0.9.5/src/scikit_build_core/build/_wheelfile.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/build/generate.py` & `scikit_build_core-0.9.5/src/scikit_build_core/build/generate.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/build/metadata.py` & `scikit_build_core-0.9.5/src/scikit_build_core/build/metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/build/sdist.py` & `scikit_build_core-0.9.5/src/scikit_build_core/build/sdist.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/build/wheel.py` & `scikit_build_core-0.9.5/src/scikit_build_core/build/wheel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/builder/__main__.py` & `scikit_build_core-0.9.5/src/scikit_build_core/builder/__main__.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/builder/builder.py` & `scikit_build_core-0.9.5/src/scikit_build_core/builder/builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/builder/generator.py` & `scikit_build_core-0.9.5/src/scikit_build_core/builder/generator.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/builder/get_requires.py` & `scikit_build_core-0.9.5/src/scikit_build_core/builder/get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/builder/macos.py` & `scikit_build_core-0.9.5/src/scikit_build_core/builder/macos.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/builder/sysconfig.py` & `scikit_build_core-0.9.5/src/scikit_build_core/builder/sysconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,20 +47,24 @@
     if config_file and Path(config_file).is_file():
         cp = configparser.ConfigParser()
         cp.read(config_file)
         result = cp.get("build_ext", "library_dirs", fallback="")
         if result:
             logger.info("Reading DIST_EXTRA_CONFIG:build_ext.library_dirs={}", result)
             minor = "" if abi3 else sys.version_info[1]
+            if env.get("SETUPTOOLS_EXT_SUFFIX", "").endswith("t.pyd"):
+                return Path(result) / f"python3{minor}t.lib"
             return Path(result) / f"python3{minor}.lib"
 
     libdirstr = sysconfig.get_config_var("LIBDIR")
     ldlibrarystr = sysconfig.get_config_var("LDLIBRARY")
+    librarystr = sysconfig.get_config_var("LDLIBRARY")
     libdir: Path | None = libdirstr and Path(libdirstr)
     ldlibrary: Path | None = ldlibrarystr and Path(ldlibrarystr)
+    library: Path | None = librarystr and Path(librarystr)
     multiarch: str | None = sysconfig.get_config_var("MULTIARCH")
     masd: str | None = sysconfig.get_config_var("multiarchsubdir")
 
     log_func = logger.warning if sys.platform.startswith("win") else logger.debug
 
     if libdir and ldlibrary:
         try:
@@ -73,15 +77,21 @@
                     masd = masd[len(os.sep) :]
                 libdir_masd = libdir / masd
                 if libdir_masd.is_dir():
                     libdir = libdir_masd
             libpath = libdir / ldlibrary
             if Path(os.path.expandvars(libpath)).is_file():
                 return libpath
-            log_func("libdir/ldlibrary: {} is not a real file!", libpath)
+            if library:
+                libpath = libdir / library
+                if sys.platform.startswith("win") and libpath.suffix == ".dll":
+                    libpath = libpath.with_suffix(".lib")
+                if Path(os.path.expandvars(libpath)).is_file():
+                    return libpath
+            log_func("libdir/(ld)library: {} is not a real file!", libpath)
         else:
             log_func("libdir: {} is not a directory", libdir)
 
     framework_prefix = sysconfig.get_config_var("PYTHONFRAMEWORKPREFIX")
     if framework_prefix and Path(framework_prefix).is_dir() and ldlibrary:
         libpath = Path(framework_prefix) / ldlibrary
         if libpath.is_file():
```

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/builder/wheel_tag.py` & `scikit_build_core-0.9.5/src/scikit_build_core/builder/wheel_tag.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/file_api/_cattrs_converter.py` & `scikit_build_core-0.9.5/src/scikit_build_core/file_api/_cattrs_converter.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/file_api/query.py` & `scikit_build_core-0.9.5/src/scikit_build_core/file_api/query.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/file_api/reply.py` & `scikit_build_core-0.9.5/src/scikit_build_core/file_api/reply.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/codemodel.py` & `scikit_build_core-0.9.5/src/scikit_build_core/file_api/model/codemodel.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/directory.py` & `scikit_build_core-0.9.5/src/scikit_build_core/file_api/model/directory.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/index.py` & `scikit_build_core-0.9.5/src/scikit_build_core/file_api/model/index.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/file_api/model/toolchains.py` & `scikit_build_core-0.9.5/src/scikit_build_core/file_api/model/toolchains.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/hatch/plugin.py` & `scikit_build_core-0.9.5/src/scikit_build_core/hatch/plugin.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/metadata/fancy_pypi_readme.py` & `scikit_build_core-0.9.5/src/scikit_build_core/metadata/fancy_pypi_readme.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/metadata/regex.py` & `scikit_build_core-0.9.5/src/scikit_build_core/metadata/regex.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/metadata/setuptools_scm.py` & `scikit_build_core-0.9.5/src/scikit_build_core/metadata/setuptools_scm.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/resources/_editable_redirect.py` & `scikit_build_core-0.9.5/src/scikit_build_core/resources/_editable_redirect.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/resources/known_wheels.toml` & `scikit_build_core-0.9.5/src/scikit_build_core/resources/known_wheels.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/resources/scikit-build.schema.json` & `scikit_build_core-0.9.5/src/scikit_build_core/resources/scikit-build.schema.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/Copyright.txt` & `scikit_build_core-0.9.5/src/scikit_build_core/resources/find_python/Copyright.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake` & `scikit_build_core-0.9.5/src/scikit_build_core/resources/find_python/FindPackageHandleStandardArgs.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake` & `scikit_build_core-0.9.5/src/scikit_build_core/resources/find_python/FindPackageMessage.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPython.cmake` & `scikit_build_core-0.9.5/src/scikit_build_core/resources/find_python/FindPython.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPython3.cmake` & `scikit_build_core-0.9.5/src/scikit_build_core/resources/find_python/FindPython3.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/resources/find_python/FindPython/Support.cmake` & `scikit_build_core-0.9.5/src/scikit_build_core/resources/find_python/FindPython/Support.cmake`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/settings/_load_provider.py` & `scikit_build_core-0.9.5/src/scikit_build_core/settings/_load_provider.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/settings/documentation.py` & `scikit_build_core-0.9.5/src/scikit_build_core/settings/documentation.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/settings/json_schema.py` & `scikit_build_core-0.9.5/src/scikit_build_core/settings/json_schema.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_docs.py` & `scikit_build_core-0.9.5/src/scikit_build_core/settings/skbuild_docs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_model.py` & `scikit_build_core-0.9.5/src/scikit_build_core/settings/skbuild_model.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_read_settings.py` & `scikit_build_core-0.9.5/src/scikit_build_core/settings/skbuild_read_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/settings/skbuild_schema.py` & `scikit_build_core-0.9.5/src/scikit_build_core/settings/skbuild_schema.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/settings/sources.py` & `scikit_build_core-0.9.5/src/scikit_build_core/settings/sources.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/setuptools/build_cmake.py` & `scikit_build_core-0.9.5/src/scikit_build_core/setuptools/build_cmake.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/setuptools/build_meta.py` & `scikit_build_core-0.9.5/src/scikit_build_core/setuptools/build_meta.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/src/scikit_build_core/setuptools/wrapper.py` & `scikit_build_core-0.9.5/src/scikit_build_core/setuptools/wrapper.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/conftest.py` & `scikit_build_core-0.9.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_builder.py` & `scikit_build_core-0.9.5/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_cmake_config.py` & `scikit_build_core-0.9.5/tests/test_cmake_config.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_custom_modules.py` & `scikit_build_core-0.9.5/tests/test_custom_modules.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_dynamic_metadata.py` & `scikit_build_core-0.9.5/tests/test_dynamic_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_editable.py` & `scikit_build_core-0.9.5/tests/test_editable.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,16 @@
     ninja = [
         "ninja" for f in isolated.wheelhouse.iterdir() if f.name.startswith("ninja-")
     ]
     cmake = [
         "cmake" for f in isolated.wheelhouse.iterdir() if f.name.startswith("cmake-")
     ]
 
-    isolated.install("pip>23", "cython", "scikit-build-core", *ninja, *cmake)
+    isolated.install("pip>23")
+    isolated.install("cython", "scikit-build-core", *ninja, *cmake)
 
     isolated.install(
         "-v",
         *config_mode_flags,
         "--no-build-isolation",
         *editable_flag,
         ".",
```

### Comparing `scikit_build_core-0.9.4/tests/test_editable_redirect.py` & `scikit_build_core-0.9.5/tests/test_editable_redirect.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_editable_unit.py` & `scikit_build_core-0.9.5/tests/test_editable_unit.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_file_processor.py` & `scikit_build_core-0.9.5/tests/test_file_processor.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_fileapi.py` & `scikit_build_core-0.9.5/tests/test_fileapi.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_fortran.py` & `scikit_build_core-0.9.5/tests/test_fortran.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_generator_default.py` & `scikit_build_core-0.9.5/tests/test_generator_default.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_get_requires.py` & `scikit_build_core-0.9.5/tests/test_get_requires.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_hatchling.py` & `scikit_build_core-0.9.5/tests/test_hatchling.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_json_schema.py` & `scikit_build_core-0.9.5/tests/test_json_schema.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_logging.py` & `scikit_build_core-0.9.5/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_module_dir.py` & `scikit_build_core-0.9.5/tests/test_module_dir.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_name_main.py` & `scikit_build_core-0.9.5/tests/test_name_main.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_prepare_metadata.py` & `scikit_build_core-0.9.5/tests/test_prepare_metadata.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_process_scripts.py` & `scikit_build_core-0.9.5/tests/test_process_scripts.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_program_search.py` & `scikit_build_core-0.9.5/tests/test_program_search.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_pyproject_abi3.py` & `scikit_build_core-0.9.5/tests/test_pyproject_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_pyproject_extra_dirs.py` & `scikit_build_core-0.9.5/tests/test_pyproject_extra_dirs.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_pyproject_pep517.py` & `scikit_build_core-0.9.5/tests/test_pyproject_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_pyproject_pep518.py` & `scikit_build_core-0.9.5/tests/test_pyproject_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_pyproject_pep660.py` & `scikit_build_core-0.9.5/tests/test_pyproject_pep660.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_pyproject_purelib.py` & `scikit_build_core-0.9.5/tests/test_pyproject_purelib.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_schema.py` & `scikit_build_core-0.9.5/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_settings.py` & `scikit_build_core-0.9.5/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_settings_overrides.py` & `scikit_build_core-0.9.5/tests/test_settings_overrides.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_setuptools_abi3.py` & `scikit_build_core-0.9.5/tests/test_setuptools_abi3.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_setuptools_pep517.py` & `scikit_build_core-0.9.5/tests/test_setuptools_pep517.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_setuptools_pep518.py` & `scikit_build_core-0.9.5/tests/test_setuptools_pep518.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_shutil.py` & `scikit_build_core-0.9.5/tests/test_shutil.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_simple_pure.py` & `scikit_build_core-0.9.5/tests/test_simple_pure.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_simplest_c.py` & `scikit_build_core-0.9.5/tests/test_simplest_c.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_skbuild_settings.py` & `scikit_build_core-0.9.5/tests/test_skbuild_settings.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/test_wheelfile_utils.py` & `scikit_build_core-0.9.5/tests/test_wheelfile_utils.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json` & `scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/reply/cache-v2-2dececcab32f1eda138d.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json` & `scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/reply/cmakeFiles-v1-74870fd87af7f965b597.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json` & `scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/reply/codemodel-v2-ea39b5a28cb1a3e0a069.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json` & `scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/reply/directory-.-5e7a28751b0c9235cbe7.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json` & `scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/reply/index-2022-09-12T15-23-13-0135.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json` & `scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/reply/target-simple_pure-7eb73eb5c359b881e083.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json` & `scikit_build_core-0.9.5/tests/api/simple_pure/.cmake/api/v1/reply/toolchains-v1-06b92b86597808b5f980.json`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/abi3_pyproject_ext/abi3_example.c` & `scikit_build_core-0.9.5/tests/packages/abi3_pyproject_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/abi3_setuptools_ext/abi3_example.c` & `scikit_build_core-0.9.5/tests/packages/abi3_setuptools_ext/abi3_example.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg1/CMakeLists.txt` & `scikit_build_core-0.9.5/tests/packages/cython_pxd_editable/pkg1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/cython_pxd_editable/pkg2/CMakeLists.txt` & `scikit_build_core-0.9.5/tests/packages/cython_pxd_editable/pkg2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/dynamic_metadata/plugin_project.toml` & `scikit_build_core-0.9.5/tests/packages/dynamic_metadata/plugin_project.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/dynamic_metadata/src/module.c` & `scikit_build_core-0.9.5/tests/packages/dynamic_metadata/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/filepath_pure/CMakeLists.txt` & `scikit_build_core-0.9.5/tests/packages/filepath_pure/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/fortran_example/CMakeLists.txt` & `scikit_build_core-0.9.5/tests/packages/fortran_example/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/hatchling/.gitignore` & `scikit_build_core-0.9.5/tests/packages/hatchling/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/hatchling/cpp/CMakeLists.txt` & `scikit_build_core-0.9.5/tests/packages/hatchling/cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/hatchling/cpp/example.cpp` & `scikit_build_core-0.9.5/tests/packages/hatchling/cpp/example.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/mixed_setuptools/CMakeLists.txt` & `scikit_build_core-0.9.5/tests/packages/mixed_setuptools/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/navigate_editable/CMakeLists.txt` & `scikit_build_core-0.9.5/tests/packages/navigate_editable/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/navigate_editable/python/shared_pkg/py_module.py` & `scikit_build_core-0.9.5/tests/packages/navigate_editable/python/shared_pkg/py_module.py`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/navigate_editable/src/shared_pkg/c_module.c` & `scikit_build_core-0.9.5/tests/packages/navigate_editable/src/shared_pkg/c_module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/sdist_config/CMakeLists.txt` & `scikit_build_core-0.9.5/tests/packages/sdist_config/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/sdist_config/pyproject.toml` & `scikit_build_core-0.9.5/tests/packages/sdist_config/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/simple_pyproject_ext/LICENSE` & `scikit_build_core-0.9.5/tests/packages/simple_pyproject_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/simple_pyproject_ext/src/main.cpp` & `scikit_build_core-0.9.5/tests/packages/simple_pyproject_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/simple_pyproject_script_with_flags/LICENSE` & `scikit_build_core-0.9.5/tests/packages/simple_pyproject_script_with_flags/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/simple_pyproject_source_dir/LICENSE` & `scikit_build_core-0.9.5/tests/packages/simple_pyproject_source_dir/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/simple_pyproject_source_dir/src/main.cpp` & `scikit_build_core-0.9.5/tests/packages/simple_pyproject_source_dir/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/simple_setuptools_ext/LICENSE` & `scikit_build_core-0.9.5/tests/packages/simple_setuptools_ext/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/simple_setuptools_ext/src/main.cpp` & `scikit_build_core-0.9.5/tests/packages/simple_setuptools_ext/src/main.cpp`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/simplest_c/CMakeLists.txt` & `scikit_build_core-0.9.5/tests/packages/simplest_c/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/tests/packages/simplest_c/src/module.c` & `scikit_build_core-0.9.5/tests/packages/simplest_c/src/module.c`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/.gitignore` & `scikit_build_core-0.9.5/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/LICENSE` & `scikit_build_core-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/README.md` & `scikit_build_core-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `scikit_build_core-0.9.4/pyproject.toml` & `scikit_build_core-0.9.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     "pybind11 >=2.11",
     "pytest >=7.0",  # 7.2+ recommended for better tracebacks with ExceptionGroup
     "pytest-subprocess >=1.5",
     'setuptools >=43; python_version<"3.9"',
     'setuptools >=45; python_version=="3.9"',
     'setuptools >=49; python_version>="3.10" and python_version<"3.12"',
     'setuptools >=66.1; python_version>="3.12"',
-    "virtualenv >=20.0.28",
+    "virtualenv >=20.20",
     "wheel >=0.40",
 ]
 test-hatchling = [
     "hatchling >=1.24.0",
 ]
 test-meta = [
     "hatch-fancy-pypi-readme>=22.3",
```

### Comparing `scikit_build_core-0.9.4/PKG-INFO` & `scikit_build_core-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scikit_build_core
-Version: 0.9.4
+Version: 0.9.5
 Summary: Build backend for CMake based projects
 Project-URL: Changelog, https://scikit-build-core.readthedocs.io/en/latest/changelog.html
 Project-URL: Discussions, https://github.com/orgs/scikit-build/discussions
 Project-URL: Documentation, https://scikit-build-core.readthedocs.io
 Project-URL: Homepage, https://github.com/scikit-build/scikit-build-core
 Project-URL: Issues, https://github.com/scikit-build/scikit-build-core/issues
 Author-email: Henry Schreiner <henryfs@princeton.edu>
@@ -58,15 +58,15 @@
 Requires-Dist: pybind11>=2.11; extra == 'test'
 Requires-Dist: pytest-subprocess>=1.5; extra == 'test'
 Requires-Dist: pytest>=7.0; extra == 'test'
 Requires-Dist: setuptools>=43; (python_version < '3.9') and extra == 'test'
 Requires-Dist: setuptools>=45; (python_version == '3.9') and extra == 'test'
 Requires-Dist: setuptools>=49; (python_version >= '3.10' and python_version < '3.12') and extra == 'test'
 Requires-Dist: setuptools>=66.1; (python_version >= '3.12') and extra == 'test'
-Requires-Dist: virtualenv>=20.0.28; extra == 'test'
+Requires-Dist: virtualenv>=20.20; extra == 'test'
 Requires-Dist: wheel>=0.40; extra == 'test'
 Provides-Extra: test-hatchling
 Requires-Dist: hatchling>=1.24.0; extra == 'test-hatchling'
 Provides-Extra: test-meta
 Requires-Dist: hatch-fancy-pypi-readme>=22.3; extra == 'test-meta'
 Requires-Dist: setuptools-scm; extra == 'test-meta'
 Provides-Extra: test-numpy
```

