# Comparing `tmp/swh_objstorage-3.1.1.tar.gz` & `tmp/swh_objstorage-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh_objstorage-3.1.1.tar", last modified: Wed May 29 14:23:25 2024, max compression
+gzip compressed data, was "swh_objstorage-3.1.2.tar", last modified: Fri May 31 10:40:51 2024, max compression
```

## Comparing `swh_objstorage-3.1.1.tar` & `swh_objstorage-3.1.2.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.524975 swh_objstorage-3.1.1/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/.copier-answers.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) jenkins    (120)      388 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/AUTHORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/LICENSE
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/Makefile
--rw-r--r--   0 jenkins    (115) jenkins    (120)       37 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/Makefile.local
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4479 2024-05-29 14:23:25.524975 swh_objstorage-3.1.1/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2275 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/README.rst
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.496976 swh_objstorage-3.1.1/bin/
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     3435 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/bin/swh-objstorage-azure
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3948 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/conftest.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.496976 swh_objstorage-3.1.1/docs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/.gitignore
--rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.496976 swh_objstorage-3.1.1/docs/_static/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.496976 swh_objstorage-3.1.1/docs/_templates/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/cli.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/conf.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      284 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/index.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5513 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/docs/winery.rst
--rw-r--r--   0 jenkins    (115) jenkins    (120)      629 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/mypy.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2004 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/pyproject.toml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/pytest.ini
--rw-r--r--   0 jenkins    (115) jenkins    (120)      125 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/requirements-azure.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       16 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/requirements-libcloud.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      172 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/requirements-test.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/requirements-winery.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      308 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-05-29 14:23:25.524975 swh_objstorage-3.1.1/setup.cfg
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.488976 swh_objstorage-3.1.1/swh/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.500976 swh_objstorage-3.1.1/swh/objstorage/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.504976 swh_objstorage-3.1.1/swh/objstorage/api/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2546 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/api/client.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5259 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/api/server.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.504976 swh_objstorage-3.1.1/swh/objstorage/backends/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17552 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/azure.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5306 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/generator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3294 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1855 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8398 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/libcloud.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1258 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/noop.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12102 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/pathslicing.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.504976 swh_objstorage-3.1.1/swh/objstorage/backends/seaweedfs/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/seaweedfs/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4060 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/seaweedfs/http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     5043 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/seaweedfs/objstorage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.508976 swh_objstorage-3.1.1/swh/objstorage/backends/winery/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      191 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2076 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/database.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2857 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/gunicorn.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15484 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/objstorage.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16122 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/roshard.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6856 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/rwshard.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    17191 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/sharedbase.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      944 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/sleep.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.508976 swh_objstorage-3.1.1/swh/objstorage/backends/winery/sql/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1170 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/sql/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2810 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/stats.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6455 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/backends/winery/throttler.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12642 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/cli.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1115 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/constants.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1971 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/exc.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3472 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/factory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8960 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    16931 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/multiplexer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     8303 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/objstorage.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.508976 swh_objstorage-3.1.1/swh/objstorage/proxies/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2367 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/proxies/readonly.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/py.typed
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1493 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.512976 swh_objstorage-3.1.1/swh/objstorage/tests/
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    15606 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/objstorage_testing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1519 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_interface.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2169 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_api.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    12670 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_azure.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7640 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_cloud.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4729 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_http.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      466 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_in_memory.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      794 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_instantiation.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    13803 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_multiplexer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      512 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_noop.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     7192 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_pathslicing.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1630 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_random_generator.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    10093 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_seaweedfs.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    45626 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_winery.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2761 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_pathslicer.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3148 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_readonly_filter.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4017 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/test_server.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)    19921 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/winery_benchmark.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     6882 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/tests/winery_testing_helpers.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      903 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/swh/objstorage/utils.py
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.520975 swh_objstorage-3.1.1/swh.objstorage.egg-info/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4479 2024-05-29 14:23:25.000000 swh_objstorage-3.1.1/swh.objstorage.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) jenkins    (120)     4064 2024-05-29 14:23:25.000000 swh_objstorage-3.1.1/swh.objstorage.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-29 14:23:25.000000 swh_objstorage-3.1.1/swh.objstorage.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-05-29 14:23:25.000000 swh_objstorage-3.1.1/swh.objstorage.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      487 2024-05-29 14:23:25.000000 swh_objstorage-3.1.1/swh.objstorage.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-29 14:23:25.000000 swh_objstorage-3.1.1/swh.objstorage.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1253 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/tox.ini
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.516975 swh_objstorage-3.1.1/winery-test-environment/
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/README.md
--rw-r--r--   0 jenkins    (115) jenkins    (120)      209 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/ansible.cfg
--rw-r--r--   0 jenkins    (115) jenkins    (120)      955 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/bootstrap.yml
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     4204 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/build-vms.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2038 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/ceph.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     3932 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/fed4fire.rspec
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)      844 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/fed4fire.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1836 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/grid5000.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.520975 swh_objstorage-3.1.1/winery-test-environment/inventory/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.488976 swh_objstorage-3.1.1/winery-test-environment/inventory/group_vars/
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.520975 swh_objstorage-3.1.1/winery-test-environment/inventory/group_vars/all/
--rw-r--r--   0 jenkins    (115) jenkins    (120)      108 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/inventory/group_vars/all/rw.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       91 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/inventory/groups.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      822 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/inventory/hosts.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       84 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/inventory/osd.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)       75 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/libvirt.yml
-drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:25.520975 swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/
--rw-r--r--   0 jenkins    (115) jenkins    (120)       80 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/README.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/__init__.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2757 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2763 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen_free.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2895 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2765 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen_linear.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)      824 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/osd.yml
--rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1333 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/remote-tox.sh
--rw-r--r--   0 jenkins    (115) jenkins    (120)     1733 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/render-stats.py
--rw-r--r--   0 jenkins    (115) jenkins    (120)       40 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/requirements.txt
--rw-r--r--   0 jenkins    (115) jenkins    (120)      198 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/rng.xml
--rw-r--r--   0 jenkins    (115) jenkins    (120)     2727 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/rw.yml
--rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-05-29 14:23:19.000000 swh_objstorage-3.1.1/winery-test-environment/tests.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.491515 swh_objstorage-3.1.2/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      360 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/.copier-answers.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      140 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      388 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1538 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      112 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/AUTHORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3397 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       15 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    35147 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/LICENSE
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/Makefile
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       37 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/Makefile.local
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4479 2024-05-31 10:40:51.491515 swh_objstorage-3.1.2/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2275 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/README.rst
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.463516 swh_objstorage-3.1.2/bin/
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     3435 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/bin/swh-objstorage-azure
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3948 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/conftest.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.463516 swh_objstorage-3.1.2/docs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       24 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.463516 swh_objstorage-3.1.2/docs/_static/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.467516 swh_objstorage-3.1.2/docs/_templates/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      163 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       43 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/docs/conf.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      284 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/docs/index.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5513 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/docs/winery.rst
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      629 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/mypy.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2004 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/pyproject.toml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       96 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/pytest.ini
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      125 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/requirements-azure.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       16 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/requirements-libcloud.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       69 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      172 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       31 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/requirements-winery.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      308 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      210 2024-05-31 10:40:51.491515 swh_objstorage-3.1.2/setup.cfg
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.455516 swh_objstorage-3.1.2/swh/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.471516 swh_objstorage-3.1.2/swh/objstorage/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.471516 swh_objstorage-3.1.2/swh/objstorage/api/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2546 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/api/client.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5259 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/api/server.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.471516 swh_objstorage-3.1.2/swh/objstorage/backends/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    19300 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/azure.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5306 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/generator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3294 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1855 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8398 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/libcloud.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1258 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/noop.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12102 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/pathslicing.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.471516 swh_objstorage-3.1.2/swh/objstorage/backends/seaweedfs/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       61 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/seaweedfs/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4060 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/seaweedfs/http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     5043 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/seaweedfs/objstorage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.475516 swh_objstorage-3.1.2/swh/objstorage/backends/winery/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      191 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/winery/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2076 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/winery/database.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2857 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/winery/gunicorn.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15484 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/winery/objstorage.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16122 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/winery/roshard.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6856 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/winery/rwshard.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    17191 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/winery/sharedbase.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      944 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/winery/sleep.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.475516 swh_objstorage-3.1.2/swh/objstorage/backends/winery/sql/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1170 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/winery/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/winery/sql/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2810 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/winery/stats.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6455 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/backends/winery/throttler.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12642 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/cli.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1115 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/constants.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1971 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/exc.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3472 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/factory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8960 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    16931 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/multiplexer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     8303 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/objstorage.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.475516 swh_objstorage-3.1.2/swh/objstorage/proxies/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2367 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/proxies/readonly.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       27 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/py.typed
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1493 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.479516 swh_objstorage-3.1.2/swh/objstorage/tests/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    15606 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/objstorage_testing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1519 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_interface.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2169 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_api.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    12787 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_azure.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7640 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_cloud.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4729 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_http.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      466 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_in_memory.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      794 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_instantiation.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    13803 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_multiplexer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      512 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_noop.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     7192 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_pathslicing.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1630 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_random_generator.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    10093 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_seaweedfs.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    45626 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_winery.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2761 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_pathslicer.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3148 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_readonly_filter.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4017 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)    19921 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/winery_benchmark.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     6882 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/tests/winery_testing_helpers.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      903 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/swh/objstorage/utils.py
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.487516 swh_objstorage-3.1.2/swh.objstorage.egg-info/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4479 2024-05-31 10:40:51.000000 swh_objstorage-3.1.2/swh.objstorage.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     4064 2024-05-31 10:40:51.000000 swh_objstorage-3.1.2/swh.objstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        1 2024-05-31 10:40:51.000000 swh_objstorage-3.1.2/swh.objstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       58 2024-05-31 10:40:51.000000 swh_objstorage-3.1.2/swh.objstorage.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      487 2024-05-31 10:40:51.000000 swh_objstorage-3.1.2/swh.objstorage.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        4 2024-05-31 10:40:51.000000 swh_objstorage-3.1.2/swh.objstorage.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1253 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/tox.ini
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.483516 swh_objstorage-3.1.2/winery-test-environment/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2649 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/README.md
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      209 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/ansible.cfg
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      955 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/bootstrap.yml
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     4204 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/build-vms.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2038 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/ceph.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     3932 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/fed4fire.rspec
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)      844 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/fed4fire.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1836 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/grid5000.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.487516 swh_objstorage-3.1.2/winery-test-environment/inventory/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.455516 swh_objstorage-3.1.2/winery-test-environment/inventory/group_vars/
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.487516 swh_objstorage-3.1.2/winery-test-environment/inventory/group_vars/all/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      108 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/inventory/group_vars/all/rw.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       91 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/inventory/groups.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      822 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/inventory/hosts.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       84 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/inventory/osd.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       75 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/libvirt.yml
+drwxr-xr-x   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:51.487516 swh_objstorage-3.1.2/winery-test-environment/mitogen-strategy/
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       80 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/mitogen-strategy/README.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)        0 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/mitogen-strategy/__init__.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2757 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/mitogen-strategy/mitogen.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2763 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/mitogen-strategy/mitogen_free.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2895 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2765 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/mitogen-strategy/mitogen_linear.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      824 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/osd.yml
+-rwxr-xr-x   0 jenkins    (115) jenkins    (120)     1333 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/remote-tox.sh
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     1733 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/render-stats.py
+-rw-r--r--   0 jenkins    (115) jenkins    (120)       40 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/requirements.txt
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      198 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/rng.xml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)     2727 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/rw.yml
+-rw-r--r--   0 jenkins    (115) jenkins    (120)      632 2024-05-31 10:40:46.000000 swh_objstorage-3.1.2/winery-test-environment/tests.yml
```

### Comparing `swh_objstorage-3.1.1/.pre-commit-config.yaml` & `swh_objstorage-3.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/CODE_OF_CONDUCT.md` & `swh_objstorage-3.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/LICENSE` & `swh_objstorage-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/PKG-INFO` & `swh_objstorage-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage
-Version: 3.1.1
+Version: 3.1.2
 Summary: Software Heritage object storage
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-objstorage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage.git
```

### Comparing `swh_objstorage-3.1.1/README.rst` & `swh_objstorage-3.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/bin/swh-objstorage-azure` & `swh_objstorage-3.1.2/bin/swh-objstorage-azure`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/conftest.py` & `swh_objstorage-3.1.2/conftest.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/docs/winery.rst` & `swh_objstorage-3.1.2/docs/winery.rst`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/mypy.ini` & `swh_objstorage-3.1.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/pyproject.toml` & `swh_objstorage-3.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/api/client.py` & `swh_objstorage-3.1.2/swh/objstorage/api/client.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/api/server.py` & `swh_objstorage-3.1.2/swh/objstorage/api/server.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/azure.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/azure.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (C) 2016-2024  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import asyncio
 import contextlib
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 from itertools import product
 import string
 from typing import Iterable, Iterator, Mapping, Optional, Union
+from urllib.parse import parse_qs, urlparse
 import warnings
 
 from azure.core.exceptions import ResourceExistsError, ResourceNotFoundError
 from azure.storage.blob import (
     BlobSasPermissions,
     ContainerClient,
     ContainerSasPermissions,
@@ -201,19 +202,55 @@
         """Internal id is the hex version in objstorage."""
         if isinstance(obj_id, dict):
             obj_id = obj_id[self.PRIMARY_HASH]
         return hashutil.hash_to_hex(obj_id)
 
     def check_config(self, *, check_write):
         """Check the configuration for this object storage"""
+        now = datetime.now(tz=timezone.utc).isoformat()
         for container_client in self.get_all_container_clients():
-            props = container_client.get_container_properties()
+            parsed = urlparse(container_client.url)
+            # The query string for the container_client url contains a bunch of
+            # fields that are associated with the permissions given by the
+            # shared access signature. We treat all fields as optional, this is
+            # not a 100% bullet-proof set of checks, for instance if a
+            # connection_string is used
+            qs = parse_qs(parsed.query)
+
+            # st is the "signed start" (the signature is only valid after that
+            # date) as an ISO-8601 encoded datetime
+            if "st" in qs and qs["st"][0] > now:
+                raise ValueError(
+                    "Shared access signature is not valid yet: %s" % qs["st"][0]
+                )
+
+            # se is the "signed expiry" (the signature is invalid after that
+            # date) as an ISO-8601 encoded datetime
+            if "se" in qs and qs["se"][0] < now:
+                raise ValueError(
+                    "Shared access signature has expired: %s" % qs["se"][0]
+                )
+
+            # sr is the "signed resource". "c" means container.
+            if "sr" in qs and "c" not in qs["sr"][0]:
+                raise ValueError(
+                    "Shared access signature is not for a container service"
+                )
 
-            # FIXME: check_write is ignored here
-            if not props:
+            # sp is the "signed permissions"
+            if (
+                "sp" in qs
+                and check_write
+                # "c" allows to create new objects
+                and "c" not in qs["sp"][0]
+                # "w" allows to write to objects. Either permission is valid to
+                # write to an objstorage
+                and "w" not in qs["sp"][0]
+            ):
+                # We have neither "c" or "w" permissions, this is read-only
                 return False
 
         return True
 
     @timed
     def __contains__(self, obj_id: ObjId) -> bool:
         """Does the storage contains the obj_id."""
```

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/generator.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/generator.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/http.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/http.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/in_memory.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/in_memory.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/libcloud.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/libcloud.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/noop.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/noop.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/pathslicing.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/pathslicing.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/seaweedfs/http.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/seaweedfs/http.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/seaweedfs/objstorage.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/seaweedfs/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/winery/database.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/winery/database.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/winery/gunicorn.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/winery/gunicorn.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/winery/objstorage.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/winery/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/winery/roshard.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/winery/roshard.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/winery/rwshard.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/winery/rwshard.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/winery/sharedbase.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/winery/sharedbase.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/winery/sleep.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/winery/sleep.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/winery/sql/30-schema.sql` & `swh_objstorage-3.1.2/swh/objstorage/backends/winery/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/winery/stats.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/winery/stats.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/backends/winery/throttler.py` & `swh_objstorage-3.1.2/swh/objstorage/backends/winery/throttler.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/cli.py` & `swh_objstorage-3.1.2/swh/objstorage/cli.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/constants.py` & `swh_objstorage-3.1.2/swh/objstorage/constants.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/exc.py` & `swh_objstorage-3.1.2/swh/objstorage/exc.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/factory.py` & `swh_objstorage-3.1.2/swh/objstorage/factory.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/interface.py` & `swh_objstorage-3.1.2/swh/objstorage/interface.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/multiplexer.py` & `swh_objstorage-3.1.2/swh/objstorage/multiplexer.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/objstorage.py` & `swh_objstorage-3.1.2/swh/objstorage/objstorage.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/proxies/readonly.py` & `swh_objstorage-3.1.2/swh/objstorage/proxies/readonly.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/pytest_plugin.py` & `swh_objstorage-3.1.2/swh/objstorage/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/objstorage_testing.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/objstorage_testing.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_interface.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_api.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_api.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_azure.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_azure.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,20 +181,24 @@
     blobs = collections.defaultdict(dict)  # {container_url: {blob_id: blob}}
 
     class MockContainerClient:
         def __init__(self, container_url):
             self.container_url = container_url
             self.blobs = blobs[self.container_url]
 
+        @property
+        def url(self):
+            return self.container_url
+
         @classmethod
         def from_container_url(cls, container_url):
             return cls(container_url)
 
         def get_container_properties(self):
-            return {"exists": True}
+            raise EnvironmentError("This raises an error in production")
 
         def get_blob_client(self, blob):
             return MockBlobClient(self, blob)
 
         def list_blobs(self):
             for obj in sorted(self.blobs):
                 yield MockListedObject(obj)
```

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_cloud.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_cloud.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_http.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_http.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_instantiation.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_instantiation.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_multiplexer.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_multiplexer.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_noop.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_noop.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_pathslicing.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_pathslicing.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_random_generator.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_random_generator.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_seaweedfs.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_seaweedfs.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_objstorage_winery.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_objstorage_winery.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_pathslicer.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_pathslicer.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_readonly_filter.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_readonly_filter.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/test_server.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/winery_benchmark.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/winery_benchmark.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/tests/winery_testing_helpers.py` & `swh_objstorage-3.1.2/swh/objstorage/tests/winery_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh/objstorage/utils.py` & `swh_objstorage-3.1.2/swh/objstorage/utils.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/swh.objstorage.egg-info/PKG-INFO` & `swh_objstorage-3.1.2/swh.objstorage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.objstorage
-Version: 3.1.1
+Version: 3.1.2
 Summary: Software Heritage object storage
 Author-email: Software Heritage developers <swh-devel@inria.fr>
 Project-URL: Homepage, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage
 Project-URL: Bug Reports, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage/-/issues
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Documentation, https://docs.softwareheritage.org/devel/swh-objstorage/
 Project-URL: Source, https://gitlab.softwareheritage.org/swh/devel/swh-objstorage.git
```

### Comparing `swh_objstorage-3.1.1/swh.objstorage.egg-info/SOURCES.txt` & `swh_objstorage-3.1.2/swh.objstorage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/tox.ini` & `swh_objstorage-3.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/README.md` & `swh_objstorage-3.1.2/winery-test-environment/README.md`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/bootstrap.yml` & `swh_objstorage-3.1.2/winery-test-environment/bootstrap.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/build-vms.sh` & `swh_objstorage-3.1.2/winery-test-environment/build-vms.sh`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/ceph.yml` & `swh_objstorage-3.1.2/winery-test-environment/ceph.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/fed4fire.rspec` & `swh_objstorage-3.1.2/winery-test-environment/fed4fire.rspec`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/fed4fire.sh` & `swh_objstorage-3.1.2/winery-test-environment/fed4fire.sh`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/grid5000.yml` & `swh_objstorage-3.1.2/winery-test-environment/grid5000.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/inventory/hosts.yml` & `swh_objstorage-3.1.2/winery-test-environment/inventory/hosts.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen.py` & `swh_objstorage-3.1.2/winery-test-environment/mitogen-strategy/mitogen.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen_free.py` & `swh_objstorage-3.1.2/winery-test-environment/mitogen-strategy/mitogen_free.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py` & `swh_objstorage-3.1.2/winery-test-environment/mitogen-strategy/mitogen_host_pinned.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/mitogen-strategy/mitogen_linear.py` & `swh_objstorage-3.1.2/winery-test-environment/mitogen-strategy/mitogen_linear.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/osd.yml` & `swh_objstorage-3.1.2/winery-test-environment/osd.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/remote-tox.sh` & `swh_objstorage-3.1.2/winery-test-environment/remote-tox.sh`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/render-stats.py` & `swh_objstorage-3.1.2/winery-test-environment/render-stats.py`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/rw.yml` & `swh_objstorage-3.1.2/winery-test-environment/rw.yml`

 * *Files identical despite different names*

### Comparing `swh_objstorage-3.1.1/winery-test-environment/tests.yml` & `swh_objstorage-3.1.2/winery-test-environment/tests.yml`

 * *Files identical despite different names*

