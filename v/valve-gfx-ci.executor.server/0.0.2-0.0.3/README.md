# Comparing `tmp/valve_gfx_ci.executor.server-0.0.2.tar.gz` & `tmp/valve_gfx_ci_executor_server-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valve_gfx_ci.executor.server-0.0.2.tar", last modified: Mon Jan 24 11:48:55 2022, max compression
+gzip compressed data, was "valve_gfx_ci_executor_server-0.0.3.tar", last modified: Fri May 31 05:50:40 2024, max compression
```

## Comparing `valve_gfx_ci.executor.server-0.0.2.tar` & `valve_gfx_ci_executor_server-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,86 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 11:48:55.781237 valve_gfx_ci.executor.server-0.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     1061 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5123 2022-01-24 11:48:55.781237 valve_gfx_ci.executor.server-0.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4515 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      126 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1892 2022-01-24 11:48:55.782237 valve_gfx_ci.executor.server-0.0.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 11:48:55.777237 valve_gfx_ci.executor.server-0.0.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 11:48:55.777237 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 11:48:55.777237 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 11:48:55.780237 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    13019 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/app.py
--rw-rw-rw-   0 root         (0) root         (0)    11588 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/boots.py
--rw-rw-rw-   0 root         (0) root         (0)     2047 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/config.py
--rwxrwxrwx   0 root         (0) root         (0)    31142 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/executor.py
--rw-rw-rw-   0 root         (0) root         (0)     1414 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)    14297 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/job.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/logger.py
--rw-rw-rw-   0 root         (0) root         (0)    13414 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/mars.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/message.py
--rw-rw-rw-   0 root         (0) root         (0)     7926 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/minioclient.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 11:48:55.780237 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/pdu/
--rw-rw-rw-   0 root         (0) root         (0)     4081 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/pdu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 11:48:55.780237 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/pdu/drivers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/pdu/drivers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      281 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/pdu/drivers/apc.py
--rw-rw-rw-   0 root         (0) root         (0)      842 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/pdu/drivers/cyberpower.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/pdu/drivers/dummy.py
--rw-rw-rw-   0 root         (0) root         (0)     7568 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/pdu/drivers/snmp.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/pdu/drivers/virtual.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 11:48:55.781237 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7545 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/tests/test_boots.py
--rw-rw-rw-   0 root         (0) root         (0)     2854 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/tests/test_gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)    15469 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/tests/test_job.py
--rw-rw-rw-   0 root         (0) root         (0)     3528 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/tests/test_message.py
--rw-rw-rw-   0 root         (0) root         (0)    12205 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/tests/test_minio.py
--rw-rw-rw-   0 root         (0) root         (0)    12796 2022-01-24 09:01:52.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/tests/test_pdu.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-24 11:48:55.779237 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci.executor.server.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5123 2022-01-24 11:48:55.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci.executor.server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1602 2022-01-24 11:48:55.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci.executor.server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-24 11:48:55.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci.executor.server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2022-01-24 11:48:55.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci.executor.server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      210 2022-01-24 11:48:55.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci.executor.server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-01-24 11:48:55.000000 valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci.executor.server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 05:50:40.122800 valve_gfx_ci_executor_server-0.0.3/
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1693 2024-05-31 05:50:40.122800 valve_gfx_ci_executor_server-0.0.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      538 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      126 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2274 2024-05-31 05:50:40.122800 valve_gfx_ci_executor_server-0.0.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 05:50:40.111800 valve_gfx_ci_executor_server-0.0.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 05:50:40.111800 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 05:50:40.111800 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 05:50:40.115800 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/
+-rw-rw-rw-   0 root         (0) root         (0)     1215 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 05:50:40.115800 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/android/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 05:49:59.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/android/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7276 2024-05-22 07:08:29.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/android/fastbootd.py
+-rw-rw-rw-   0 root         (0) root         (0)    26867 2024-05-22 07:08:29.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/android/mkbootimg.py
+-rwxrwxrwx   0 root         (0) root         (0)    22449 2024-05-10 12:28:40.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/app.py
+-rw-rw-rw-   0 root         (0) root         (0)    18076 2024-05-22 07:08:29.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/boots.py
+-rw-rw-rw-   0 root         (0) root         (0)     2550 2024-05-22 07:08:29.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/boots_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     3394 2024-05-22 07:08:29.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    20458 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/dhcpd.py
+-rw-rw-rw-   0 root         (0) root         (0)    28592 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/dut.py
+-rw-rw-rw-   0 root         (0) root         (0)    45473 2024-05-22 07:08:29.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/executor.py
+-rw-rw-rw-   0 root         (0) root         (0)     4228 2024-04-26 19:36:29.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)    21610 2024-05-22 07:08:29.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/job.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 05:50:40.116800 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/job_templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/job_templates/bootloop.yml.j2
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/job_templates/cache_reset.yml.j2
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/job_templates/interactive.yml.j2
+-rw-rw-rw-   0 root         (0) root         (0)      843 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/job_templates/register.yml.j2
+-rw-rw-rw-   0 root         (0) root         (0)      389 2024-05-10 12:28:40.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)    21687 2024-05-17 12:52:18.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/mars.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/message.py
+-rw-rw-rw-   0 root         (0) root         (0)    12154 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/minioclient.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 05:50:40.117800 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/
+-rw-rw-rw-   0 root         (0) root         (0)     6443 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5313 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/daemon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 05:50:40.118800 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 05:49:59.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/apc.py
+-rw-rw-rw-   0 root         (0) root         (0)      842 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/cyberpower.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/devantech.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/dummy.py
+-rw-rw-rw-   0 root         (0) root         (0)     5252 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/kernelchip.py
+-rw-rw-rw-   0 root         (0) root         (0)     3578 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/shelly.py
+-rw-rw-rw-   0 root         (0) root         (0)     9013 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/snmp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2981 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/tasmota.py
+-rw-rw-rw-   0 root         (0) root         (0)     7184 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/usbhub.py
+-rw-rw-rw-   0 root         (0) root         (0)     2132 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/virtual.py
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/socketactivation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 05:50:40.118800 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3239 2024-05-22 07:08:29.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/templates/boots_db.yml.j2
+-rw-rw-rw-   0 root         (0) root         (0)     2068 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/templates/gitlab_runner_config.toml.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 05:50:40.121800 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-31 05:49:59.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2076 2024-04-27 04:10:31.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/sample_job.yml
+-rw-rw-rw-   0 root         (0) root         (0)    14040 2024-04-27 04:10:31.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_boots.py
+-rw-rw-rw-   0 root         (0) root         (0)     3215 2024-05-22 07:08:29.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_boots_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     1227 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)    11215 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_dhcpd.py
+-rw-rw-rw-   0 root         (0) root         (0)     6852 2024-05-22 07:08:29.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_fastboot.py
+-rw-rw-rw-   0 root         (0) root         (0)    12549 2024-04-26 19:36:29.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)    29510 2024-05-22 07:08:29.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     3528 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_message.py
+-rw-rw-rw-   0 root         (0) root         (0)    15445 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_minio.py
+-rw-rw-rw-   0 root         (0) root         (0)     6140 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_pdu.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_pdu_apc_masterswitch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5054 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_pdu_basesnmp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7068 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_pdu_daemon.py
+-rw-rw-rw-   0 root         (0) root         (0)     7440 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_pdu_devantech.py
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_pdu_dummy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8869 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_pdu_kernelchip.py
+-rw-rw-rw-   0 root         (0) root         (0)     7166 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_pdu_manualsnmp.py
+-rw-rw-rw-   0 root         (0) root         (0)      898 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_pdu_pdu41004.py
+-rw-rw-rw-   0 root         (0) root         (0)    14797 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_pdu_shelly.py
+-rw-rw-rw-   0 root         (0) root         (0)     3697 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_pdu_tasmota.py
+-rw-rw-rw-   0 root         (0) root         (0)    11160 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_pdu_usbhub.py
+-rw-rw-rw-   0 root         (0) root         (0)     2092 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_socketactivation.py
+-rw-rw-rw-   0 root         (0) root         (0)    14838 2024-04-05 13:19:21.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tftpd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 05:50:40.121800 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci.executor.server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1693 2024-05-31 05:50:40.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci.executor.server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3716 2024-05-31 05:50:40.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci.executor.server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 05:50:40.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci.executor.server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2024-05-31 05:50:40.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci.executor.server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      338 2024-05-31 05:50:40.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci.executor.server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-31 05:50:40.000000 valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci.executor.server.egg-info/top_level.txt
```

### Comparing `valve_gfx_ci.executor.server-0.0.2/LICENSE` & `valve_gfx_ci_executor_server-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/executor.py` & `valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/dut.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,801 +1,744 @@
-#!/usr/bin/env python3
-
+from collections import defaultdict
+from dataclasses import asdict, field
 from datetime import datetime
+from subprocess import Popen, PIPE, DEVNULL
+from enum import Enum
+from typing import Dict, List, Optional
 from threading import Thread, Event
-from collections import defaultdict, namedtuple
-from urllib.parse import urlsplit, urlparse
-from enum import Enum, IntEnum
+import subprocess
+import traceback
+import tempfile
+import socket
+import requests
+import tarfile
+import fcntl
+import time
+import json
+import dataclasses
+import yaml
+import sys
+import os
+
+from pydantic import field_validator
+from pydantic.dataclasses import dataclass
+import requests_unixsocket
 
-from .message import LogLevel, JobIOMessage, ControlMessage, SessionEndMessage, Message, MessageType
-from .pdu import PDUState
-from .message import JobStatus
+from .boots import BootConfig
 from .job import Job
 from .logger import logger
-from .minioclient import MinioClient, MinIOPolicyStatement, generate_policy
+from .message import JobStatus, MessageType, Message
+from .pdu import PDUState
 from . import config
 
-import traceback
-import requests
-import tempfile
-import secrets
-import random
-import select
-import shutil
-import socket
-import json
-import time
+
+@dataclass
+class CallbackEndpoint:
+    host: str
+    port: int
+
+
+@dataclass
+class MinIOCredentials:
+    access_key: Optional[str] = None
+    secret_key: Optional[str] = None
 
 
-# Constants
-CONSOLE_DRAINING_DELAY = 1
+# WARNING: This class is duplicated from job.py until marshmallow gets replaced by pydantic dataclasses
+@dataclass
+class Target:
+    id: Optional[str] = None
+    tags: Optional[List[str]] = field(default_factory=list)
+
+    @field_validator('tags')
+    @classmethod
+    def tags_must_be_a_list(cls, v):
+        if v is None:
+            return []
+        else:
+            return v
 
 
-class MachineState(Enum):
+class DUTState(Enum):
     WAIT_FOR_CONFIG = 0
     IDLE = 1
     TRAINING = 2
     QUEUED = 3
     RUNNING = 4
+    RETIRED = 5
+    UNKNOWN = 6
+    QUICK_CHECK = 7
+    BORKED = 8
+
+
+@dataclass(kw_only=True)
+class JobRequest:
+    version: int
+    raw_job: str
+    target: Target
+    callback_endpoint: CallbackEndpoint
+    minio_credentials: MinIOCredentials
+
+    job_id: Optional[str]
+    http_headers: Dict[str, str] = field(default_factory=dict)
+    minio_groups: List[str] = field(default_factory=list)
+    job_bucket_initial_state_tarball_file_fd: int = 0
 
+    def cleanup(self):
+        if self.job_bucket_initial_state_tarball_file_fd > 0:
+            try:
+                os.close(self.job_bucket_initial_state_tarball_file_fd)
+            except Exception:
+                logger.error(f"ERROR: Failed to close the initial state tarball file fd!\n{traceback.format_exc()}")
+            finally:
+                # Unconditionally mark the fd as freed, even if we failed to
+                # close it because it is better to leak the fd than potentially
+                # closing someone else's fd later down the line when this object
+                # gets garbage collected.
+                self.job_bucket_initial_state_tarball_file_fd = 0
 
-def str_to_int(string, default):
-    try:
-        return int(string)
-    except Exception:
-        return default
-
-
-class JobConsoleState(IntEnum):
-    CREATED = 0
-    ACTIVE = 1
-    DUT_DONE = 2
-    TEAR_DOWN = 3
-    OVER = 4
-
-
-class JobConsole(Thread):
-    def __init__(self, machine_id, client_endpoint, console_patterns,
-                 client_version=None, log_level=LogLevel.INFO):
-        super().__init__(name='ConsoleThread')
-
-        self.machine_id = machine_id
-
-        self.client_endpoint = client_endpoint
-        self.console_patterns = console_patterns
-        self.client_version = client_version
-        self.log_level = log_level
-
-        # Sockets
-        self.client_sock = None
-        self.salad_sock = self.connect_to_salad()
-
-        # Job-long state
-        self._state = JobConsoleState.CREATED
-        self.start_time = None
-        self.line_buffer = bytearray()
-        self._user_session_state = dict()
-
-        self.reset_per_boot_state()
+    def __del__(self):
+        self.cleanup()
 
-    @property
-    def salad_url(self):
-        return f"{config.SALAD_URL}/api/v1/machine/{self.machine_id}"
+    @field_validator("job_id")
+    @classmethod
+    def job_id_isnt_empty(cls, v):
+        if not v:
+            now = int(datetime.utcnow().timestamp())
+            v = f"untitled-{now}"
+        return v
 
-    def connect_to_salad(self):
-        parsed_url = urlsplit(config.SALAD_URL)
+    @field_validator("callback_endpoint")
+    @classmethod
+    def callback_endpoint_is_set(cls, v):
+        if v.host is None:
+            raise ValueError("callback's host cannot be None. Leave empty to get the default value")
+        if v.port is None:
+            raise ValueError("callback's port cannot be None")
+        return v
 
-        r = requests.get(self.salad_url)
-        r.raise_for_status()
+    @classmethod
+    def parse(cls, request):
+        if request.mimetype == "application/json":
+            return JSONJobRequest(request)
+        elif request.mimetype == "multipart/form-data":
+            return MultipartJobRequest(request)
+        else:
+            raise ValueError("Unknown job request format")
 
-        machine = r.json()
-        port = machine.get("tcp_port")
 
-        return socket.create_connection((parsed_url.hostname, port))
+# DEPRECATED: To be removed when we are sure all the clients out there have been updated
+class JSONJobRequest(JobRequest):
+    def __init__(self, request):
+        job_params = request.json
+        metadata = job_params["metadata"]
+        job = Job.render_with_resources(job_params["job"])
 
-    def reset_per_boot_state(self):
-        self.last_activity_from_machine = None
-        self.last_activity_from_client = None
+        # Use the client-provided host callback if available, or default to the remote addr
+        remote_addr = metadata.get("callback_host", request.remote_addr)
+        endpoint = CallbackEndpoint(remote_addr, metadata.get("callback_port"))
 
-        self.console_patterns.reset_per_boot_state()
-        self.needs_reboot = self.console_patterns.needs_reboot
+        super().__init__(http_headers=dict(request.headers), version=0, raw_job=job_params["job"],
+                         target=job.target, callback_endpoint=endpoint,
+                         minio_credentials=MinIOCredentials())
 
-    def close_salad(self):
-        try:
-            self.salad_sock.shutdown(socket.SHUT_RDWR)
-            self.salad_sock.close()
-        except OSError:
-            pass
 
-    def close_client(self):
-        if self.client_version:
-            try:
-                self.client_sock.shutdown(socket.SHUT_RDWR)
-                self.client_sock.close()
-            except OSError:
-                pass
+class InvalidTarballFile(Exception):
+    pass
 
-    def close(self):
-        self.set_state(JobConsoleState.OVER)
 
-    @property
-    def state(self):
-        if self._state == JobConsoleState.ACTIVE:
-            return self._state if self.is_alive() else JobConsoleState.OVER
+class MultipartJobRequest(JobRequest):
+    def __init__(self, request):
+        metadata_file = request.files.get('metadata')
+        if metadata_file is None:
+            raise ValueError("No metadata file found")
 
-        return self._state
+        if metadata_file.mimetype != "application/json":
+            raise ValueError("The metadata file has the wrong mimetype: "
+                             "{metadata_file.mimetype}} instead of application/json")
 
-    def set_state(self, state, **kwargs):
-        prev_state = self._state
-        if state < prev_state:
-            raise ValueError("The state can only move forward")
-        elif state == prev_state:
-            return
+        try:
+            metadata = json.loads(metadata_file.read())
+        except json.JSONDecodeError as e:
+            raise ValueError(f"The metadata file is not a valid JSON file: {e.msg}")
+
+        version = metadata.get('version')
+        if version == 1:
+            self.parse_v1(request, metadata)
         else:
-            self._state = state
-
-        self.log(f"Job console state changed from {prev_state.name} -> {state.name}\n")
-
-        if state == JobConsoleState.ACTIVE:
-            self.start_time = datetime.now()
+            raise ValueError(f"Invalid request version {version}")
 
-        elif state == JobConsoleState.DUT_DONE:
-            # Skip the entire tear-down if we do not have a client
-            if not self.client_version:
-                self.set_state(JobConsoleState.OVER)
-
-        elif state == JobConsoleState.TEAR_DOWN:
-            # Kill the connection to SALAD
-            self.close_salad()
-
-            # Notify the client
-            if self.client_version:
-                if self.client_version == 0:
-                    self.log(f"<-- End of the session: {self.console_patterns.job_status} -->\n")
-                elif self.client_version == 1:
-                    try:
-                        status = JobStatus.from_str(self.console_patterns.job_status)
-                        SessionEndMessage.create(job_bucket=kwargs.get('job_bucket'),
-                                                 status=status).send(self.client_sock)
-                    except (ConnectionResetError, BrokenPipeError, OSError):
-                        traceback.print_exc()
-                try:
-                    self.client_sock.shutdown(socket.SHUT_WR)
-                except (ConnectionResetError, BrokenPipeError, OSError):
-                    pass
-
-        elif state == JobConsoleState.OVER:
-            # Make sure the connections to SALAD and the client are killed
-            self.close_salad()
-            self.close_client()
-
-    def start(self):
-        if self.client_version:
-            logger.info(f"Connecting to the client endpoint {self.client_endpoint}")
-            self.client_sock = socket.create_connection(self.client_endpoint)
-        super().start()
-
-    def match_console_patterns(self, buf):
-        patterns_matched = set()
-
-        # Process the buffer, line by line
-        to_process = self.line_buffer + buf
-        cur = 0
-        while True:
-            idx = to_process.find(b'\n', cur)
-            if idx > 0:
-                line = to_process[cur:idx+1]
-                logger.info(f"{self.machine_id} -> {bytes(line)}")
-                patterns_matched |= self.console_patterns.process_line(line)
-                cur = idx + 1
-            else:
-                break
-        self.line_buffer = to_process[cur:]
+    def parse_v1(self, request, metadata):
+        # Get the job file, and check its mimetype
+        job_file = request.files['job']
+        if job_file.mimetype != "application/x-yaml":
+            raise ValueError("The metadata file has the wrong mimetype: "
+                             "{job_file.mimetype}} instead of application/x-yaml")
+
+        # Get the initial state tarball.
+        # Since flask files can be either in memory or on the disk, let's write its content
+        # to a temporary file, keep a reference open by tying it to the lifetime of this object,
+        # then store the fd in job_bucket_initial_state_tarball_file_fd. This file descriptor
+        # will then be passed to the executor instance that will execute the job at which point
+        # the object can be deleted automatically and the filedescriptor will get closed.
+        initial_state_tarball_file = request.files.get('job_bucket_initial_state_tarball_file', None)
+        if initial_state_tarball_file and initial_state_tarball_file.mimetype != "application/octet-stream":
+            raise ValueError("The job_bucket_initial_state_tarball file has the wrong mimetype: "
+                             "{initial_state_tarball_file.mimetype}} instead of application/octet-stream")
+        if initial_state_tarball_file:
+            job_bucket_initial_state_tarball_file_fd, file_path = tempfile.mkstemp()
 
-        # Tell the user what happened
-        if len(patterns_matched) > 0:
-            self.log(f"Matched the following patterns: {', '.join(patterns_matched)}\n")
-
-        # Check if the state changed
-        self.needs_reboot = self.console_patterns.needs_reboot
-
-    def log(self, msg, log_level=LogLevel.INFO):
-        # Ignore messages with a log level lower than the minimum set
-        if log_level < self.log_level:
-            return
+            # Make sure the file doesn't linger on the disk even if everything crashes
+            os.unlink(file_path)
 
-        if self.start_time is not None:
-            relative_time = (datetime.now() - self.start_time).total_seconds()
+            with os.fdopen(job_bucket_initial_state_tarball_file_fd, 'w+b', closefd=False) as tmp_file:
+                while chunk := initial_state_tarball_file.read(1000000):
+                    tmp_file.write(chunk)
+
+                # Check if the file passed is a valid tarball, or raise InvalidTarballFile
+                # NOTE: We make sure to rewind the file before and after the check!
+                tmp_file.seek(0)
+                if not tarfile.is_tarfile(tmp_file):
+                    raise InvalidTarballFile()
+                tmp_file.seek(0)
         else:
-            relative_time = 0.0
-
-        log_msg = f"+{relative_time:.3f}s: {msg}"
-        logger.info(log_msg.rstrip("\r\n"))
-
-        if self.client_version:
-            try:
-                if self.client_version == 0:
-                    self.client_sock.send(log_msg.encode())
-                elif self.client_version == 1:
-                    ControlMessage.create(log_msg, severity=log_level).send(self.client_sock)
-            except OSError:
-                pass
-
-    def stop(self):
-        self.set_state(JobConsoleState.OVER)
-        self.join()
-
-    def run(self):
-        self.set_state(JobConsoleState.ACTIVE)
+            job_bucket_initial_state_tarball_file_fd = -1
 
-        while self.state < JobConsoleState.OVER:
-            fds = []
-            if self.state < JobConsoleState.TEAR_DOWN:
-                fds.extend([self.salad_sock.fileno()])
-            if self.client_version:
-                fds.extend([self.client_sock.fileno()])
-
-            # Make sure all the FDs are valid, or exit!
-            if any([fd < 0 for fd in fds]):
-                self.log("Found a negative fd, aborting!")
-                self.close()
+        # Create a Job object
+        raw_job = job_file.read().decode()
+        job = Job.render_with_resources(raw_job)
+
+        # Get the target that will run the job. Use the job's target by default,
+        # but allow the client to override the target
+        if "target" in metadata:
+            target = metadata.get('target', {})
+            job_target = Target(target.get('id'), target.get('tags', []))
+        else:
+            job_target = Target(id=job.target.id, tags=job.target.tags)
 
-            rlist, _, _ = select.select(fds, [], [], 1.0)
-
-            for fd in rlist:
-                try:
-                    if fd == self.salad_sock.fileno():
-                        # DUT's stdout/err: Salad -> Client
-                        buf = self.salad_sock.recv(8192)
-                        if len(buf) == 0:
-                            self.set_state(JobConsoleState.DUT_DONE)
-
-                        # Match the console patterns
-                        try:
-                            self.match_console_patterns(buf)
-                        except Exception:
-                            self.log(traceback.format_exc())
-
-                        # Update the last console activity if we already had activity,
-                        # or when we get the first newline character as serial
-                        # consoles may sometimes send unwanted characters at power up
-                        if self.last_activity_from_machine is not None or b'\n' in buf:
-                            self.last_activity_from_machine = datetime.now()
-
-                        # Forward to the client
-                        if self.client_version:
-                            if self.client_version == 0:
-                                self.client_sock.send(buf)
-                            elif self.client_version == 1:
-                                JobIOMessage.create(buf).send(self.client_sock)
-
-                        # The message got forwarded, close the session if it ended
-                        if self.console_patterns.session_has_ended:
-                            self.set_state(JobConsoleState.DUT_DONE)
-
-                    elif fd == self.client_sock.fileno():
-                        # DUT's stdin: Client -> Salad
-                        if self.client_version == 0:
-                            buf = self.client_sock.recv(8192)
-                            if len(buf) == 0:
-                                self.close()
-
-                            # Forward to the salad
-                            self.salad_sock.send(buf)
-                        elif self.client_version == 1:
-                            try:
-                                msg = Message.next_message(self.client_sock)
-                                if msg.msg_type == MessageType.JOB_IO:
-                                    self.salad_sock.send(msg.buffer)
-                            except EOFError:
-                                # Do not warn when we are expecting the client to close its socket
-                                if self.state < JobConsoleState.TEAR_DOWN:
-                                    self.log(traceback.format_exc())
-
-                                self.log("The client closed its connection")
-
-                                # Clean up everything on our side
-                                self.close()
-
-                        self.last_activity_from_client = datetime.now()
-                except (ConnectionResetError, BrokenPipeError, OSError):
-                    self.log(traceback.format_exc())
-                    self.close()
-                except Exception:
-                    logger.error(traceback.format_exc())
+        # Use the client-provided host callback if available, or default to the remote addr
+        callback = metadata.get('callback', {})
+        remote_addr = callback.get("host", request.remote_addr)
+        endpoint = CallbackEndpoint(remote_addr, callback.get("port"))
+
+        # Parse the minio-related arguments request
+        minio = metadata.get('minio', {})
+        minio_credentials = minio.get('credentials', {})
+        credentials = MinIOCredentials(access_key=minio_credentials.get("access_key"),
+                                       secret_key=minio_credentials.get("secret_key"))
+
+        super().__init__(http_headers=dict(request.headers), version=1, raw_job=raw_job,
+                         target=job_target, callback_endpoint=endpoint,
+                         job_bucket_initial_state_tarball_file_fd=job_bucket_initial_state_tarball_file_fd,
+                         job_id=metadata.get('job_id'),
+                         minio_credentials=credentials,
+                         minio_groups=minio.get('groups', []))
+
+
+class SergentHartmanState(Enum):
+    IDLE = 0
+    ENROLLING = 1
+    QUICK_CHECK = 2
+    REGISTRATION_FAILED = 3
 
 
 class SergentHartman:
-    def __init__(self, machine, boot_loop_counts=None, qualifying_rate=None):
+    def __init__(self, machine, boot_loop_counts=None, qualifying_rate=None, quick_check=None):
         super().__init__()
 
         if boot_loop_counts is None:
             boot_loop_counts = int(config.SERGENT_HARTMAN_BOOT_COUNT)
 
         if qualifying_rate is None:
             qualifying_rate = int(config.SERGENT_HARTMAN_QUALIFYING_BOOT_COUNT)
 
+        if quick_check is None:
+            quick_check = config.as_boolean("SERGENT_HARTMAN_QUICK_CHECK")
+
         self.machine = machine
         self.boot_loop_counts = boot_loop_counts
         self.qualifying_rate = qualifying_rate
+        self.quick_check = quick_check
+        self._state = None
+        self.registration_failed_at = None
 
-        self.reset()
+        # Tri-state boolean
+        self.result = None
+
+        self.set_state(SergentHartmanState.IDLE)
 
     @property
-    def is_machine_registered(self):
-        return self.cur_loop > 0
+    def is_active(self):
+        return self.state != SergentHartmanState.IDLE
 
-    def reset(self):
-        self.is_active = False
-        self.cur_loop = 0
-        self.statuses = defaultdict(int)
+    @property
+    def state(self):
+        def registration_failed_expiration_time():
+            delay = int(config.SERGENT_HARTMAN_REGISTRATION_RETRIAL_DELAY)
+            return self.registration_failed_at + delay if self.registration_failed_at is not None else 0
 
-    def next_task(self):
-        mid = self.machine.id
+        if self._state == SergentHartmanState.ENROLLING and registration_failed_expiration_time() > time.monotonic():
+            return SergentHartmanState.REGISTRATION_FAILED
+        else:
+            return self._state
 
-        if not self.is_active:
-            # Start by forcing the machine to register itself to make sure the
-            # its configuration is up to date (especially the serial console
-            # port). Loop until it succeeds!
-            self.reset()
+    def set_state(self, state):
+        def reset():
+            self.is_machine_registered = False
+            self.cur_loop = 0
+            self.statuses = defaultdict(int)
+            self.result = None
+            self.registration_failed_at = None
 
-            logger.info("SergentHartman/%s - Try registering the machine", mid)
+        if self.state == state:
+            return
+        elif state == SergentHartmanState.IDLE:
+            reset()
+        elif self.state == SergentHartmanState.IDLE and state == SergentHartmanState.ENROLLING:
+            pass
+        elif self.state == SergentHartmanState.IDLE and state == SergentHartmanState.QUICK_CHECK:
+            pass
+        elif state == SergentHartmanState.REGISTRATION_FAILED:
+            reset()
+            self.registration_failed_at = time.monotonic()
+            state = SergentHartmanState.ENROLLING
+        else:
+            raise ValueError(f"{self.state} -> {state} is an invalid transition")
 
-            self.is_active = True
+        self._state = state
 
-            return Job.from_path(config.EXECUTOR_REGISTRATION_JOB, self.machine)
+    def _next_task(self, callback_port):
+        mid = self.machine.id
+
+        if self.state == SergentHartmanState.ENROLLING:
+            if not self.is_machine_registered:
+                # Start by forcing the machine to register itself to make sure the
+                # its configuration is up to date (especially the serial console
+                # port). Loop until it succeeds!
+                job_path = config.EXECUTOR_REGISTRATION_JOB
+
+                logger.info("SergentHartman/%s - Try registering the machine", mid)
+            else:
+                # Check that we got the expected amount of reports
+                if self.cur_loop != sum(self.statuses.values()):
+                    raise ValueError("The previous next_task() call was not followed by a call to report()")
+
+                # The registration went well, let's start the boot loop!
+                self.cur_loop += 1
+
+                statuses_str = [f"{status.name}: {values}" for status, values in self.statuses.items()]
+                logger.info("SergentHartman/%s - loop %s/%s - statuses %s: "
+                            "Execute one more round!",
+                            mid,
+                            self.cur_loop,
+                            self.boot_loop_counts,
+                            statuses_str)
+
+                job_path = config.EXECUTOR_BOOTLOOP_JOB
+        elif self.state == SergentHartmanState.QUICK_CHECK:
+            logger.info("SergentHartman/%s - Initial check", mid)
+            job_path = config.EXECUTOR_BOOTLOOP_JOB
         else:
-            # Check that we got the expected amount of reports
-            if self.cur_loop != sum(self.statuses.values()):
-                raise ValueError("The previous next_task() call was not followed by a call to report()")
-
-            # The registration went well, let's start the boot loop!
-            self.cur_loop += 1
-
-            statuses_str = [f"{status.name}: {values}" for status, values in self.statuses.items()]
-            logger.info("SergentHartman/%s - loop %s/%s - statuses %s: "
-                        "Execute one more round!",
-                        mid,
-                        self.cur_loop,
-                        self.boot_loop_counts,
-                        statuses_str)
+            raise ValueError(f"There are no next tasks when the state is {self.state.name}")
 
-            return Job.from_path(config.EXECUTOR_BOOTLOOP_JOB, self.machine)
+        with open(job_path, "r") as f:
+            raw_job = f.read()
 
-    def report(self, job_status):
+            callback_endpoint = CallbackEndpoint(host="127.0.0.1", port=callback_port)
+            return JobRequest(version=1, job_id=None, raw_job=raw_job,
+                              target=Target(), callback_endpoint=callback_endpoint,
+                              minio_credentials=MinIOCredentials())
+
+    def _report(self, job_status, execution_time):
         mid = self.machine.id
 
-        if self.cur_loop == 0:
-            if job_status != JobStatus.PASS:
-                delay = int(config.SERGENT_HARTMAN_REGISTRATION_RETRIAL_DELAY)
-                logger.warning((f"SergentHartman/{mid} - Registration failed with status {job_status.name}. "
-                                f"Retrying in {delay} second(s)"))
-                self.reset()
-                return delay
+        if self.state == SergentHartmanState.ENROLLING:
+            if self.cur_loop == 0:
+                if job_status != JobStatus.PASS:
+                    delay = int(config.SERGENT_HARTMAN_REGISTRATION_RETRIAL_DELAY)
+                    logger.warning((f"SergentHartman/{mid} - Registration failed with status {job_status.name}. "
+                                    f"Retrying in {delay} second(s)"))
+                    self.set_state(SergentHartmanState.REGISTRATION_FAILED)
+                else:
+                    self.is_machine_registered = True
+                    if self.boot_loop_counts >= 1:
+                        logger.info(f"SergentHartman/{mid} - Registration succeeded, moving on to the boot loop")
+                    else:
+                        logger.info(f"SergentHartman/{mid} - Registration succeeded, boot loops disabled")
+                        self.result = True
             else:
-                logger.info(f"SergentHartman/{mid} - Registration succeeded, moving on to the boot loop")
+                # We are in the boot loop
+                self.statuses[job_status] += 1
+
+                if self.cur_loop >= self.boot_loop_counts:
+                    self.result = self.statuses[JobStatus.PASS] >= self.qualifying_rate
+        elif self.state == SergentHartmanState.QUICK_CHECK:
+            self.result = (job_status == JobStatus.PASS)
+
+            if job_status == JobStatus.PASS:
+                logger.info(f"SergentHartman/{mid} - Initial check successful after {execution_time:.2f} seconds")
+            else:
+                logger.error(f"SergentHartman/{mid} - Initial check failed after {execution_time:.2f} seconds")
         else:
-            # We are in the boot loop
-            self.statuses[job_status] += 1
+            raise ValueError(f"Reporting unsupported on the state {self.state.name}")
 
-            if self.cur_loop == self.boot_loop_counts:
-                self.is_active = False
+    def execute_next_task(self, stop_event):
+        if self.state in [SergentHartmanState.IDLE, SergentHartmanState.REGISTRATION_FAILED]:
+            # Nothing to do here
+            return
 
-                # Update MaRS
-                ready_for_service = self.statuses[JobStatus.PASS] >= self.qualifying_rate
-                self.machine.ready_for_service = ready_for_service
+        if stop_event.is_set():
+            return
 
-        return 0
+        # If we are asked for fewer than 0 bootloops, consider Sergent Hartman disabled
+        if self.boot_loop_counts < 0:
+            self.result = True
+            return
 
-    @property
-    def is_available(self):
-        return config.EXECUTOR_REGISTRATION_JOB or config.EXECUTOR_BOOTLOOP_JOB
+        # If we were asked to quick check but quick check was disabled, pretend we ran it
+        # already
+        if self.state == SergentHartmanState.QUICK_CHECK and not self.quick_check:
+            self.result = True
+            return
 
+        start_time = time.monotonic()
+        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as tcp_server:
+            tcp_server.bind(('', 0))
+            tcp_server.listen(1)
+            local_port = tcp_server.getsockname()[1]
 
-class JobBucket:
-    Credentials = namedtuple('Credentials', ['username', 'password', 'policy_name'])
+            # Queue the job
+            status = DUTState.UNKNOWN
+            try:
+                proc = self.machine.start_job(self._next_task(callback_port=local_port), quiet=True)
 
-    def __init__(self, minio, bucket_name, initial_state_tarball_file=None):
-        self.minio = minio
-        self.name = bucket_name
+                print(f"Waiting for the executor to connect to our local port {local_port}")
+                tcp_server.settimeout(5)
+                try:
+                    job_socket, _ = tcp_server.accept()
+                except socket.timeout:
+                    proc.kill()
+                    proc.wait(timeout=10)
+                    raise ValueError("The server failed to initiate a connection")
 
-        self._credentials = dict()
+                # Set the resulting socket's timeout to blocking
+                job_socket.settimeout(None)
 
-        if initial_state_tarball_file:
-            self.initial_state_tarball_file = tempfile.NamedTemporaryFile("w+b")
-            shutil.copyfileobj(initial_state_tarball_file, self.initial_state_tarball_file)
-            self.initial_state_tarball_file.seek(0)
-        else:
-            self.initial_state_tarball_file = None
+                # Wait for the end message
+                status_msg = JobStatus.UNKNOWN
+                try:
+                    while not stop_event.is_set():
+                        msg = Message.next_message(job_socket)
 
-        self.minio.make_bucket(bucket_name)
+                        if msg.msg_type == MessageType.SESSION_END:
+                            status_msg = msg.status
+                            break
+                except Exception:
+                    traceback.print_exc()
 
-    def remove(self):
-        self.minio.remove_bucket(self.name)
+                # Close the socket to signal we are done
+                job_socket.shutdown(socket.SHUT_RDWR)
+                job_socket.close()
 
-        for credentials in self._credentials.values():
-            self.minio.remove_user_policy(credentials.policy_name, credentials.username)
-            self.minio.remove_user(credentials.username)
+                # Wait for the process to die
+                status_exit_code = JobStatus.UNKNOWN
+                try:
+                    proc.wait(timeout=10)
+                    status_exit_code = JobStatus(proc.returncode)
+                except subprocess.TimeoutExpired:
+                    proc.kill()
+                    raise ValueError("The process never finished")
+                except ValueError:
+                    logger.error(f"The exit status {proc.returncode} is an invalid value for JobStatus")
+
+                # Check that the status reported by the SESSION_END message matches
+                # the one we got from
+                if status_msg != JobStatus.UNKNOWN and \
+                   status_exit_code != JobStatus.UNKNOWN and \
+                   status_msg != status_exit_code:
+                    raise ValueError("Mismatch detected between the END_MESSAGE's and the exit code's status")
+
+                # report the status
+                status = status_msg if status_msg != JobStatus.UNKNOWN else status_exit_code
+            finally:
+                execution_time = time.monotonic() - start_time
+                self._report(job_status=status, execution_time=execution_time)
 
-    def __del__(self):
-        try:
-            self.remove()
-        except Exception:
-            traceback.print_exc()
+    @property
+    def is_available(self):
+        return config.EXECUTOR_REGISTRATION_JOB or config.EXECUTOR_BOOTLOOP_JOB
 
-    def credentials(self, role):
-        return self._credentials.get(role)
 
-    def create_owner_credentials(self, role, user_name=None, password=None,
-                                 groups=None, whitelisted_ips=None):
-        if user_name is None:
-            user_name = f"{self.name}-{role}"
-
-        if password is None:
-            password = secrets.token_hex(16)
-
-        if groups is None:
-            groups = []
-
-        if whitelisted_ips is None:
-            whitelisted_ips = []
-
-        policy_name = f"policy_{user_name}"
-
-        self.minio.add_user(user_name, password)
-
-        policy_statements = [
-            MinIOPolicyStatement(buckets=[self.name], source_ips=whitelisted_ips)
-        ]
-        if len(whitelisted_ips) > 0:
-            restrict_to_whitelisted_ips = MinIOPolicyStatement(allow=False, not_source_ips=whitelisted_ips)
-            policy_statements.append(restrict_to_whitelisted_ips)
-        policy = json.dumps(generate_policy(policy_statements))
-        logger.debug(f"Applying the MinIO policy: {policy}")
+def lock_fd(fd, attempts=100):
+    last_exc = None
 
+    for i in range(attempts):
         try:
-            self.minio.apply_user_policy(policy_name, user_name, policy_statements)
-        except Exception as e:
-            self.minio.remove_user(user_name)
-            raise e from None
-
-        # Add the user to the wanted list of groups
-        for group_name in groups:
-            self.minio.add_user_to_group(user_name, group_name)
-
-        credentials = self.Credentials(user_name, password, policy_name)
-        self._credentials[role] = credentials
-
-        return credentials
-
-    def setup(self):
-        if self.initial_state_tarball_file:
-            self.minio.extract_archive(self.initial_state_tarball_file, self.name)
-
-    def access_url(self, role=None):
-        endpoint = urlparse(self.minio.url)
-
-        role_creds = self.credentials(role)
-        if role_creds:
-            credentials = f"{role_creds[0]}:{role_creds[1]}@"
-        else:
-            credentials = ""
-        return f'{endpoint.scheme}://{credentials}{endpoint.netloc}'
+            fcntl.flock(fd, fcntl.LOCK_EX | fcntl.LOCK_NB)
+            return
+        except BlockingIOError as e:
+            if e.errno == 11:
+                last_exc = e
+                time.sleep(0.01)
+                continue
+            else:
+                raise e
 
-    @classmethod
-    def from_job_request(cls, minio, request, machine):
-        # Generate a job id
-        bucket_name = MinioClient.create_valid_bucket_name(f"job-{machine.id}-{request.job_id}")
+    raise last_exc
 
-        try:
-            # BUG: It seems like this is not a reliable way to detect re-use of existing buckets...
-            return cls(minio, bucket_name=bucket_name,
-                       initial_state_tarball_file=request.job_bucket_initial_state_tarball_file)
-        except ValueError:
-            # The bucket already exists, let's try to make it more unique!
-            now = int(datetime.utcnow().timestamp())
-            rand_int = random.randrange(10e6)
-            return cls(minio, bucket_name=f"{bucket_name}-{now}-{rand_int}",
-                       initial_state_tarball_file=request.job_bucket_initial_state_tarball_file)
 
+@dataclass
+class PduPortStats:
+    last_polled: Optional[datetime] = None
+    last_known_state: Optional[PDUState] = None
+    last_shutdown: Optional[datetime] = None
 
-class Executor(Thread):
-    def __init__(self, machine):
-        super().__init__(name=f'ExecutorThread-{machine.id}')
+    def serialize(self):
+        fields = asdict(self)
+        fields['last_known_state'] = fields['last_known_state'].value
+        return fields
+
+    @classmethod
+    def from_pdu_port(cls, port):
+        fields = {f.name: getattr(port, f.name) for f in dataclasses.fields(cls)}
+        return cls(**fields)
 
-        self.machine = machine
 
-        self.state = MachineState.WAIT_FOR_CONFIG
-        self.minio = MinioClient()
+class DUT(Thread):
+    def __init__(self, mars, db_dut):
+        self.mars = mars
+        self.config_changed(db_dut)
 
         # Training / Qualifying process
-        self.sergent_hartman = SergentHartman(machine)
+        self.sergent_hartman = SergentHartman(self)
 
-        # Outside -> Inside communication
-        self.job_ready = Event()
-        self.job_config = None
-        self.job_console = None
-        self.job_bucket = None
-
-        # Remote artifacts (typically over HTTPS) are stored in our
-        # local minio instance which is exposed over HTTP to the
-        # private LAN. This makes such artifacts amenable to PXE
-        # booting, for which HTTPS clients are not available.  Less
-        # critically, it makes access easier for the boards in our
-        # private LAN, for which HTTPS offers no advantage.
-        self.remote_url_to_local_cache_mapping = {}
+        # Queue a quick check
+        self.quick_check_queued = Event()
+        if self.ready_for_service and not self.is_retired:
+            self.quick_check_queued.set()
 
         # Start the background thread that will manage the machine
+        super().__init__(name=f'ExecutorThread-{self.id}')
         self.stop_event = Event()
         self.start()
 
-    def start_job(self, job_request):
-        if self.state != MachineState.IDLE:
-            raise ValueError(f"The machine isn't idle: Current state is {self.state.name}")
-
-        # Prepare the job bucket
-        self.job_bucket = JobBucket.from_job_request(self.minio, job_request, self.machine)
-        if self.job_bucket:
-            self.job_bucket.create_owner_credentials("dut", groups=job_request.minio_groups,
-                                                     whitelisted_ips=[f'{self.machine.ip_address}/32'])
-
-        # Bit nasty to render twice, but better than duplicating
-        # template render in the various call-sites within
-        # executor. Rendering it up front reduces the chances for
-        # mistakes. (Meta-point: using an HTTP query to specify the
-        # "target" could avoid this duplication of work, and might
-        # actually make more sense)
-        job = Job.render_with_resources(job_request.raw_job, self.machine, self.job_bucket)
-        logger.debug("rendered job:\n%s", job)
-
-        self.state = MachineState.QUEUED
-        self.job_request = job_request
-        self.job_config = job
-        self.job_console = JobConsole(self.machine.id,
-                                      client_endpoint=job_request.callback_endpoint,
-                                      console_patterns=self.job_config.console_patterns,
-                                      client_version=job_request.version)
-        self.job_ready.set()
-
-    def log(self, msg, log_level=LogLevel.INFO):
-        if self.job_console is not None:
-            self.job_console.log(msg, log_level=log_level)
-
-    def _cache_remote_artifact(self, artifact_name, start_url, continue_url):
-        artifact_prefix = f"{artifact_name}-{self.machine.id}"
-
-        # Assume the remote artifacts already exist locally
-        self.remote_url_to_local_cache_mapping[start_url] = start_url
-        self.remote_url_to_local_cache_mapping[continue_url] = continue_url
-
-        def cache_it(url, suffix):
-            if self.minio.is_local_url(url):
-                logger.debug(f"Ignore caching {url} as it is already hosted by our minio cache")
-                return
-            self.remote_url_to_local_cache_mapping[url] = f"http://10.42.0.1:9000/boot/{artifact_prefix}-{suffix}"
-            self.log(f'Caching {url} into minio...\n')
-            self.minio.save_boot_artifact(start_url, f"{artifact_prefix}-start")
-
-        cache_it(start_url, 'start')
-        if start_url != continue_url:
-            cache_it(continue_url, 'continue')
-
-    def _cache_remote_artifacts(self):
-        deploy_strt = self.job_config.deployment_start
-        deploy_cnt = self.job_config.deployment_start
-
-        logger.info("Caching the kernel...")
-        self._cache_remote_artifact("kernel", deploy_strt.kernel_url,
-                                    deploy_cnt.kernel_url)
-
-        logger.info("Caching the initramfs...")
-        self._cache_remote_artifact("initramfs", deploy_strt.initramfs_url,
-                                    deploy_cnt.initramfs_url)
-
-        if self.job_bucket:
-            logger.info("Initializing the job bucket with the client's data")
-            self.job_bucket.setup()
+    def stop_machine(self):
+        self.stop_event.set()
+        self.cancel_job()
+        self.join()
 
-    def run(self):
-        def session_init():
-            # Reset the state
-            self.job_config = None
-            self.job_console = None
-            self.machine.boots.remove_pxelinux_config(self.machine.mac_address)
-
-            # Pick a job
-            if self.sergent_hartman.is_available and not self.machine.ready_for_service:
-                self.state = MachineState.TRAINING
-
-                self.job_config = self.sergent_hartman.next_task()
-                self.job_console = JobConsole(self.machine.id,
-                                              client_endpoint=None,
-                                              client_version=None,
-                                              console_patterns=self.job_config.console_patterns)
-            else:
-                self.sergent_hartman.reset()
+    # Expose all the fields of the associated ConfigDUT object
+    def __getattr__(self, attr):
+        return getattr(self.db_dut, attr)
 
-                # Wait for a job to be set
-                self.state = MachineState.IDLE
-                if not self.job_ready.wait(1):
-                    return False
-                self.job_ready.clear()
+    @property
+    def ready_for_service(self):
+        return self.db_dut.ready_for_service
 
-                self.state = MachineState.RUNNING
+    @ready_for_service.setter
+    def ready_for_service(self, val):
+        self.update_fields({"ready_for_service": val})
 
-            # Cut the power to the machine, we do not need it
-            self.machine.pdu_port.set(PDUState.OFF)
+    @property
+    def is_retired(self):
+        return self.db_dut.is_retired
 
-            # Mark the start time to now()
-            self.job_start_time = datetime.now()
+    @is_retired.setter
+    def is_retired(self, val):
+        self.update_fields({"is_retired": val})
 
-            # Connect to the client's endpoint, to relay the serial console
-            self.job_console.start()
+    @property
+    def pdu_port(self):
+        if self._pdu_port is None:
+            self._pdu_port = self.mars.get_pdu_port_by_name(self.db_dut.pdu,
+                                                            self.db_dut.pdu_port_id,
+                                                            raise_if_missing=False,
+                                                            timeout=0)
+            if self._pdu_port:
+                self._pdu_port.min_off_time = self.db_dut.pdu_off_delay
+
+        return self._pdu_port
+
+    def config_changed(self, db_dut=None):
+        self.db_dut = db_dut
+
+        # Invalidate the PDU port cache
+        self._pdu_port = None
+
+    def update_fields(self, fields):
+        with self.mars.db as mars_db:
+            db_dut = mars_db.duts[self.id]
+
+            updated_fields = set()
+            for k, v in fields.items():
+                if getattr(self.db_dut, k, None) == v:
+                    continue
 
-            return True
+                if k == 'is_retired':
+                    if self.is_retired and not v:
+                        self.quick_check_queued.set()
 
-        def session_end():
-            cooldown_delay_s = 0
+                setattr(db_dut, k, v)
 
-            if self.sergent_hartman.is_active and self.job_config is not None:
-                status = JobStatus.from_str(self.job_config.console_patterns.job_status)
-                cooldown_delay_s = int(self.sergent_hartman.report(status))
-
-            self.job_config = None
-
-            # Signal to the job that we reached the end of the execution
-            if self.job_console is not None:
-                self.job_console.close()
-                self.job_console = None
-                self.machine.boots.remove_pxelinux_config(self.machine.mac_address)
-                if self.job_bucket:
-                    del self.job_bucket
-
-            # Interruptible sleep
-            for i in range(cooldown_delay_s):
-                if self.stop_event.is_set():
-                    return
-                time.sleep(1)
-
-        def log_exception():
-            logger.debug("Exception caught:\n%s", traceback.format_exc())
-            self.log(f"An exception got caught: {traceback.format_exc()}\n", LogLevel.ERROR)
-            # If exceptions start firing, throttle the parent loop, since it's
-            # very heavy spam if left to run at full speed.
-            time.sleep(2)
-
-        def execute_job():
-            # Start the overall timeout
-            timeouts = self.job_config.timeouts
-            timeouts.overall.start()
-
-            # Download the kernel/initramfs
-            self.log("Setup the infrastructure\n")
-            timeouts.infra_setup.start()
-            self._cache_remote_artifacts()
-            self.log(f"Completed setup of the infrastructure, after {timeouts.infra_setup.active_for} s\n")
-            timeouts.infra_setup.stop()
-
-            # Keep on resuming until success, timeouts' retry limits is hit, or the entire executor is going down
-            deployment = self.job_config.deployment_start
-            while (not self.stop_event.is_set() and not timeouts.overall.has_expired and
-                   self.job_console.state < JobConsoleState.DUT_DONE):
-                self.job_console.reset_per_boot_state()
-
-                # Make sure the machine shuts down
-                self.machine.pdu_port.set(PDUState.OFF)
-
-                # Set up the deployment
-                self.log("Setting up the boot configuration\n")
-                self.machine.boots.write_pxelinux_config(
-                    mac_addr=self.machine.id,
-                    kernel_path=self.remote_url_to_local_cache_mapping.get(deployment.kernel_url),
-                    cmdline=deployment.kernel_cmdline,
-                    initrd_path=self.remote_url_to_local_cache_mapping.get(deployment.initramfs_url))
-
-                self.log(f"Power up the machine, enforcing {self.machine.pdu_port.min_off_time} seconds of down time\n")
-                self.machine.pdu_port.set(PDUState.ON)
-
-                # Start the boot, and enable the timeouts!
-                self.log("Boot the machine\n")
-                timeouts.boot_cycle.start()
-                timeouts.first_console_activity.start()
-                timeouts.console_activity.stop()
-
-                while (self.job_console.state < JobConsoleState.DUT_DONE and
-                       not self.job_console.needs_reboot and
-                       not self.stop_event.is_set() and not timeouts.has_expired):
-                    # Update the activity timeouts, based on when was the
-                    # last time we sent it data
-                    if self.job_console.last_activity_from_machine is not None:
-                        timeouts.first_console_activity.stop()
-                        timeouts.console_activity.reset(when=self.job_console.last_activity_from_machine)
-
-                    # Wait a little bit before checking again
-                    time.sleep(0.1)
-
-                # Cut the power
-                self.machine.pdu_port.set(PDUState.OFF)
-
-                # Increase the retry count of the timeouts that expired, and
-                # abort the job if we exceeded their limits.
-                abort = False
-                for timeout in timeouts.expired_list:
-                    retry = timeout.retry()
-                    decision = "Try again!" if retry else "Abort!"
-                    self.log(f"Hit the timeout {timeout} --> {decision}\n", LogLevel.ERROR)
-                    abort = abort or not retry
-
-                # Check if the DUT asked us to reboot
-                if self.job_console.needs_reboot:
-                    retry = timeouts.boot_cycle.retry()
-                    retries_str = f"{timeouts.boot_cycle.retried}/{timeouts.boot_cycle.retries}"
-                    dec = f"Boot cycle {retries_str}, go ahead!" if retry else "Exceeded boot loop count, aborting!"
-                    self.log(f"The DUT asked us to reboot: {dec}\n", LogLevel.WARN)
-                    abort = abort or not retry
-
-                if abort:
-                    return
-
-                # Stop all the timeouts, except the overall
-                timeouts.first_console_activity.stop()
-                timeouts.console_activity.stop()
-                timeouts.boot_cycle.stop()
-
-                # We went through one boot cycle, update the
-                deployment = self.job_config.deployment_continue
-
-            # We either reached the end of the job, or the client got disconnected
-            if self.job_console.state == JobConsoleState.DUT_DONE:
-                # Tearing down the job
-                self.log("The job has finished executing, starting tearing down\n")
-                timeouts.infra_teardown.start()
-
-                # Delay to make sure messages are read before the end of the job
-                time.sleep(CONSOLE_DRAINING_DELAY)
-
-                # Start the tear down, which will create and send the credentials
-                # for the job bucket to the client
-                self.log("Creating credentials to the job bucket for the client\n")
-                self.job_console.set_state(JobConsoleState.TEAR_DOWN, job_bucket=self.job_bucket)
-
-                # Wait for the client to close the connection
-                self.log("Waiting for the client to download the job bucket\n")
-                while (self.job_console.state < JobConsoleState.OVER and
-                       not self.stop_event.is_set() and
-                       not timeouts.infra_teardown.has_expired):
-                    # Wait a little bit before checking again
-                    time.sleep(0.1)
+                updated_fields.add(k)
 
-                self.log(f"Completed the tear down procedure in {timeouts.infra_teardown.active_for} s\n")
-                timeouts.infra_teardown.stop()
-            else:
-                self.log("The job is over, skipping sharing the job bucket with the client")
+            if len(updated_fields) > 0:
+                self.config_changed(db_dut)
 
-            # We are done!
+    @property
+    def _executor_socket_path(self):
+        dut_id = self.id.replace(":", "_")
+        return f"/var/run/executor/{dut_id}.sock"
 
-        while not self.stop_event.is_set():
+    @property
+    def _executor_lock_path(self):
+        return f"{self._executor_socket_path}.lock"
+
+    def _executor_query(self, path, method="get"):
+        session = requests_unixsocket.Session()
+        r = getattr(session, method)(f'http+unix://{self._executor_socket_path.replace("/", "%2F")}{path}')
+        return r
+
+    @property
+    def state(self):
+        def job_process_state():
             try:
-                # Wait for the machine to have an assigned PDU port
-                if self.machine.pdu_port is None:
-                    time.sleep(1)
-                    continue
+                r = self._executor_query("/api/v1/state")
+                if r.status_code == 200:
+                    q = r.json()
+                    state = q.get("state")
+                    try:
+                        return DUTState[state]
+                    except KeyError:
+                        return DUTState.UNKNOWN
+                else:
+                    return DUTState.QUEUED
+            except (requests.exceptions.ConnectionError, FileNotFoundError):
+                # Verify that the lock is not held by anyone before declaring
+                # the machine is IDLE
                 try:
-                    if not session_init():
-                        # No jobs for us to run!
-                        continue
+                    with open(self._executor_lock_path, "r") as f:
+                        lock_fd(f, attempts=5)
+
+                        # The lock was available, the machine can be considered IDLE
+                        return DUTState.IDLE
+                except BlockingIOError:
+                    # The lock was not available, the machine may still be in use
+                    return DUTState.BORKED
+                except FileNotFoundError:
+                    # The lock file does not exist, the machine must be idle
+                    return DUTState.IDLE
+
+            return DUTState.IDLE
+
+        state = job_process_state()
+
+        if state == DUTState.IDLE:
+            # If the state is IDLE, check what state we should give it
+            if self.pdu_port is None:
+                return DUTState.WAIT_FOR_CONFIG
+            elif self.is_retired:
+                return DUTState.RETIRED
+            elif not self.ready_for_service:
+                return DUTState.TRAINING
+            elif self.quick_check_queued.is_set():
+                return DUTState.QUICK_CHECK
+        elif self.sergent_hartman.state == SergentHartmanState.ENROLLING:
+            return DUTState.TRAINING
+        elif self.sergent_hartman.state == SergentHartmanState.QUICK_CHECK:
+            return DUTState.QUICK_CHECK
+
+        return state
+
+    def start_job(self, job_request, quiet=False):
+        if self.pdu_port is None:
+            raise ValueError("Can't start a job until the PDU port is properly setup")
+
+        # Create the configuration for the run
+        config = {
+            "executor_job_version": 1,
+            "mars_db": asdict(self.mars_db),
+            "job_request": asdict(job_request),
+            "machine_id": self.id,
+            "pdu_port_stats": PduPortStats.from_pdu_port(self.pdu_port).serialize()
+
+        }
+
+        # Compute the list of file descriptors to pass to the next client
+        if job_request.job_bucket_initial_state_tarball_file_fd > 0:
+            pass_fds = [job_request.job_bucket_initial_state_tarball_file_fd]
+        else:
+            pass_fds = []
+
+        # Execute the job
+        proc = Popen(["executor", "run-job", "-s", self._executor_socket_path,
+                      "-l", self._executor_lock_path],
+                     stdin=PIPE, stdout=sys.stdout if not quiet else DEVNULL,
+                     stderr=sys.stderr if not quiet else DEVNULL,
+                     pass_fds=pass_fds)
+        yaml.dump(config, proc.stdin, sort_keys=False, encoding='utf-8')
+        proc.stdin.flush()
+        proc.stdin.close()
+
+        # Wait for 15s for the unix socket to appear, or kill the process
+        start = time.monotonic()
+        while time.monotonic() - start < 15:
+            try:
+                self._executor_query("/api/v1/state")
+                return proc
+            except requests.exceptions.ConnectionError:
+                pass
+
+        # Seems like the start-up process did not work, kill the process!
+        proc.kill()
+        proc.wait()
+        raise ValueError("The job process failed to start")
+
+    def cancel_job(self):
+        try:
+            r = self._executor_query("/api/v1/job/cancel", method="post")
+            return r.status_code == 200
+        except requests.exceptions.ConnectionError:
+            # Nothing to do
+            return True
+
+    def boot_config_query(self, platform=None, buildarch=None, bootloader=None):
+        try:
+            url = f"/api/v1/boot/config?platform={platform}&buildarch={buildarch}&bootloader={bootloader}"
+            q = self._executor_query(url)
+            if q.status_code == 200:
+                return BootConfig(**q.json())
+        except Exception:
+            traceback.print_exc()
+            return None
+
+    def run(self):
+        while not self.stop_event.is_set():
+            try:
+                if self.state == DUTState.TRAINING and self.sergent_hartman.state == SergentHartmanState.IDLE:
+                    self.sergent_hartman.set_state(SergentHartmanState.ENROLLING)
+                elif self.state == DUTState.QUICK_CHECK and self.sergent_hartman.state == SergentHartmanState.IDLE:
+                    self.sergent_hartman.set_state(SergentHartmanState.QUICK_CHECK)
+                elif self.sergent_hartman.state == SergentHartmanState.ENROLLING and (self.ready_for_service or
+                                                                                      self.is_retired):
+                    # Cancel enrollment
+                    self.sergent_hartman.set_state(SergentHartmanState.IDLE)
+
+                if self.sergent_hartman.is_active:
+                    self.sergent_hartman.execute_next_task(stop_event=self.stop_event)
+
+                    # Check if we are done
+                    if self.sergent_hartman.result is not None and not self.stop_event.is_set():
+                        if self.sergent_hartman.state == SergentHartmanState.ENROLLING:
+                            self.ready_for_service = self.sergent_hartman.result
+                        elif self.sergent_hartman.state == SergentHartmanState.QUICK_CHECK:
+                            if not self.sergent_hartman.result:
+                                self.ready_for_service = False
+                            self.quick_check_queued.clear()
+
+                        self.sergent_hartman.set_state(SergentHartmanState.IDLE)
 
-                    self.log(f"Starting the job: {self.job_config}\n\n", LogLevel.DEBUG)
-                    execute_job()
-                except Exception:
-                    log_exception()
-                finally:
-                    session_end()
             except Exception:
-                # Capture any further exceptions from session_end
-                # TODO: Refactor to avoid the cyclomatic complexity.
-                # Note: Do not be tempted to log_exception() here! Any
-                # exceptions thrown by *that* method could crash our
-                # thread.
                 traceback.print_exc()
 
-            # TODO: Keep the state of the job in memory for later querying
+            # Wait for a second before starting a new round of testing
+            self.stop_event.wait(1)
```

### Comparing `valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/message.py` & `valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/message.py`

 * *Files identical despite different names*

### Comparing `valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/pdu/drivers/cyberpower.py` & `valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/cyberpower.py`

 * *Files identical despite different names*

### Comparing `valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/pdu/drivers/dummy.py` & `valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/dummy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .. import PDU, PDUPort, PDUState
 
 
 class DummyPDU(PDU):
-    def __init__(self, name, config):
+    def __init__(self, name, config, reserved_port_ids=[]):
         self._ports = []
 
         for i, port_label in enumerate(config.get('ports', [])):
             port = PDUPort(self, i, port_label)
             port._state = PDUState.ON
             self._ports.append(port)
 
-        super().__init__(name)
+        super().__init__(name, config, reserved_port_ids)
 
     @property
     def ports(self):
         return self._ports
 
     def set_port_state(self, port_id, state):
         port = self.ports[int(port_id)]
```

### Comparing `valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/pdu/drivers/snmp.py` & `valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/snmp.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from easysnmp import snmp_get, snmp_set, snmp_walk
+from easysnmp import Session
+import easysnmp.exceptions
 from .. import logger, PDU, PDUPort, PDUState
+from functools import cached_property
 from typing import Dict
 
 import random
 import time
 
 
 def _is_int(s):
@@ -11,67 +13,102 @@
         s = int(s)
         return True
     except ValueError:
         return False
 
 
 def retry_on_known_errors(func):
-    retriable_errors = [
-        "<built-in function set> returned NULL without setting an error",
-        "<built-in function get> returned NULL without setting an error",
-        "<built-in function walk> returned NULL without setting an error",
-    ]
-
     def retry(*args, **kwargs):
         retries = 3
 
         for i in range(retries):
             try:
                 return func(*args, **kwargs)
-            except SystemError as e:
-                if str(e) in retriable_errors:
-                    logger.warning(f"Caught the re-triable error '{str(e)}', retrying ({i+1}/{retries})")
-
-                    # Wait a minimum of 1 second, plus a random delay to reduce the chances of concurrent requests
-                    time.sleep(1 + random.random())
-                    continue
-                raise e
+            except (SystemError, easysnmp.exceptions.EasySNMPError) as e:
+                logger.warning(f"Caught the error '{str(e)}', retrying ({i+1}/{retries})")
+                # Wait 1 second, plus a random [0,1] second delay to reduce the chances of concurrent requests
+                time.sleep(1 + random.random())
+                continue
 
         raise ValueError(f"The function {func} failed {retries} times in a row")
 
     return retry
 
 
 class SnmpPDU(PDU):
     oid_enterprise = '1.3.6.1.4.1'
 
-    def __init__(self, name, config):
-        self.hostname = config.get('hostname', None)
-        if not self.hostname:
-            raise ValueError('SnmpPDU requires a "hostname" configuration key')
-        self.community = config.get('community', 'private')
+    @property
+    def __port_labels(self):
+        try:
+            return [x.value for x in self.session.walk(self.outlet_labels_oid)]
+        except SystemError as e:
+            raise ValueError(f"The snmp_walk() call failed with the following error: {e}")
+
+    def __init__(self, name, config, reserved_port_ids=[]):
+        super().__init__(name, config, reserved_port_ids)
 
         assert self.system_id
         assert self.outlet_labels
         assert self.outlet_status
 
         if not hasattr(self, 'outlet_ctrl'):
             # Some PDUs offer a RW status tree, others require a separate
             # tree for writes. Default to the seemingly more common case
             # of a RW tree.
             self.outlet_ctrl = self.outlet_status
 
-        # FIXME: THe UNKNOWN status is a bit of an odd one, not all PDUs expose such a concept.
+        # FIXME: The UNKNOWN status is a bit of an odd one, not all PDUs expose such a concept.
         assert self.state_mapping.keys() == set([PDUState.ON, PDUState.OFF, PDUState.REBOOT])
         if not hasattr(self, 'inverse_state_mapping'):
             self.inverse_state_mapping: Dict[int, PDUState] = \
                 dict([(value, key) for key, value in self.state_mapping.items()])
         else:
             assert self.inverse_state_mapping.keys() == set([PDUState.ON, PDUState.OFF, PDUState.REBOOT])
-        super().__init__(name)
+
+        # Validate the configuration by getting the list of ports
+        self._ports = []
+        self.ports
+
+    @cached_property
+    def session(self):
+        config = self.config
+
+        if 'hostname' not in config:
+            raise ValueError('SnmpPDU requires a "hostname" configuration key')
+
+        version = config.get('version', 1)
+        if version in [1, 2]:
+            session = Session(hostname=config['hostname'], community=config.get('community', 'private'),
+                              version=version)
+        elif version == 3:
+            # Only keep the keys
+            supported_keys = {'hostname', 'security_username', 'privacy_protocol', 'privacy_password',
+                              'auth_protocol', 'auth_password', 'context_engine_id', 'security_engine_id', 'version'}
+            session_cfg = {k: v for k, v in config.items() if k in supported_keys}
+
+            auth_protocol = session_cfg.get('auth_protocol')
+            privacy_protocol = session_cfg.get('privacy_protocol')
+            if auth_protocol is not None and privacy_protocol is not None:
+                session_cfg['security_level'] = 'auth_with_privacy'
+            elif auth_protocol is not None and privacy_protocol is None:
+                session_cfg['security_level'] = 'auth_without_privacy'
+            elif auth_protocol is None and privacy_protocol is None:
+                session_cfg['security_level'] = 'no_auth_or_privacy'
+            else:
+                raise ValueError("Unsupported security level: Can't have a privacy protocol with no auth protocol")
+
+            session = Session(**session_cfg)
+        else:
+            raise ValueError(f"SNMP version {version} is unsupported")
+
+        # Validate the configuration by reading the state of the first port
+        session.get(self.outlet_status_oid(1))
+
+        return session
 
     @property
     def outlet_system_id(self):
         return f'{self.oid_enterprise}.{self.system_id}'
 
     @property
     def outlet_labels_oid(self):
@@ -83,29 +120,29 @@
 
     def outlet_ctrl_oid(self, port_id: int):
         assert isinstance(port_id, int)
         return f'{self.outlet_system_id}.{self.outlet_ctrl}.{port_id}'
 
     @property
     def ports(self):
-        ports = []
+        labels = self.__port_labels
+        for i, label in enumerate(labels):
+            if len(self._ports) <= i:
+                port = PDUPort(pdu=self, port_id=i+1)
+                self._ports.append(port)
+            else:
+                port = self._ports[i]
 
-        try:
-            names = [x.value for x in
-                     snmp_walk(self.outlet_labels_oid,
-                               hostname=self.hostname,
-                               community=self.community,
-                               version=1)]
-        except SystemError as e:
-            raise ValueError(f"The snmp_walk() call failed with the following error: {e}")
+            # Update the label
+            port.label = labels[i]
 
-        for i, name in enumerate(names):
-            ports.append(PDUPort(self, i+1, name))
+        # Truncate the list of ports if it shrank
+        self._ports = self._ports[0:len(labels)]
 
-        return ports
+        return self._ports
 
     def _port_spec_to_int(self, port_spec):
         if _is_int(port_spec):
             return port_spec
         else:
             for port in self.ports:
                 if port.label == port_spec:
@@ -118,20 +155,17 @@
         SNMP_INTEGER_TYPE = 'i'
 
         port_id = self._port_spec_to_int(port_spec)
         logger.debug('setting OID %s to state %s with value %d',
                      self.outlet_ctrl_oid(port_id),
                      state,
                      self.state_mapping[state])
-        ret = snmp_set(self.outlet_ctrl_oid(port_id),
-                       self.state_mapping[state],
-                       SNMP_INTEGER_TYPE,
-                       hostname=self.hostname,
-                       version=1,
-                       community=self.community)
+        ret = self.session.set(self.outlet_ctrl_oid(port_id),
+                               self.state_mapping[state],
+                               SNMP_INTEGER_TYPE)
 
         if self.state_transition_delay_seconds is not None:
             logger.debug("Enforcing %s seconds of delay for state change", self.state_transition_delay_seconds)
             # TODO: keep track of state changes to avoid a forced sleep.
             # TODO: Polling for the state change would be better in general.
             # The root cause of this is because PDUs maintain their
             # own configurables how long to delay between
@@ -140,61 +174,72 @@
             time.sleep(self.state_transition_delay_seconds)
 
         return ret
 
     @retry_on_known_errors
     def get_port_state(self, port_spec):
         port_id = self._port_spec_to_int(port_spec)
-        vs = snmp_get(self.outlet_status_oid(port_id),
-                      hostname=self.hostname,
-                      version=1,
-                      community=self.community)
+        vs = self.session.get(self.outlet_status_oid(port_id))
         value = int(vs.value)
         logger.debug('retrieved OID %s with value %d, maps to state %s',
                      self.outlet_status_oid(port_id),
                      value,
                      self.inverse_state_mapping[value])
         return self.inverse_state_mapping[value]
 
     def __eq__(self, other):
         return not any([
             getattr(self, attr, None) != getattr(other, attr, None)
             for attr in ["name",
-                         "hostname",
-                         "community",
+                         "config",
                          "system_id",
                          "outlet_labels",
                          "outlet_status",
                          "outlet_ctrl",
                          "state_mapping",
                          "inverse_state_mapping"]])
 
 
 class ManualSnmpPDU(SnmpPDU):
-    def __init__(self, name, config):
-        self.system_id = config.get('system_id')
-        self.outlet_labels = config.get('outlet_labels')
-        self.outlet_status = config.get('outlet_status')
-        # Some PDUs offer a RW status tree, others require a separate
-        # tree for writes. Default to the seemingly more common case
-        # of a RW tree.
-        self.outlet_ctrl = config.get('outlet_ctrl', self.outlet_status)
-
-        def populate_state_mapping(state_mapping, d):
-            for state, internal_value in d.items():
-                v = int(internal_value)
-                if state.lower() == "on":
-                    state_mapping[PDUState.ON] = v
-                elif state.lower() == "off":
-                    state_mapping[PDUState.OFF] = v
-                elif state.lower() == "reboot":
-                    state_mapping[PDUState.REBOOT] = v
-                    # Unknown deliberately excluded.
-        self.state_mapping = {}
-        populate_state_mapping(self.state_mapping,
-                               config.get('state_mapping', {}))
-        if 'inverse_state_mapping' in config:
-            self.inverse_state_mapping = {}
-            populate_state_mapping(self.inverse_state_mapping,
-                                   config.get('inverse_state_mapping'))
+    def __init__(self, name, config, reserved_port_ids=[]):
+        if inverse_state_mapping := config.get('inverse_state_mapping'):
+            self.inverse_state_mapping = self.__generate_state_mapping(inverse_state_mapping)
+
+        super().__init__(name, config, reserved_port_ids)
+
+    @property
+    def system_id(self):
+        return self.config['system_id']
+
+    @property
+    def outlet_labels(self):
+        return self.config['outlet_labels']
 
-        super().__init__(name, config)
+    @property
+    def outlet_status(self):
+        return self.config['outlet_status']
+
+    # Some PDUs offer a RW status tree, others require a separate
+    # tree for writes. Default to the seemingly more common case
+    # of a RW tree.
+    @property
+    def outlet_ctrl(self):
+        return self.config.get('outlet_ctrl', self.outlet_status)
+
+    def __generate_state_mapping(self, d):
+        state_mapping = dict()
+
+        for state, internal_value in d.items():
+            v = int(internal_value)
+            if state.lower() == "on":
+                state_mapping[PDUState.ON] = v
+            elif state.lower() == "off":
+                state_mapping[PDUState.OFF] = v
+            elif state.lower() == "reboot":
+                state_mapping[PDUState.REBOOT] = v
+                # Unknown deliberately excluded.
+
+        return state_mapping
+
+    @property
+    def state_mapping(self):
+        return self.__generate_state_mapping(self.config.get('state_mapping', {}))
```

### Comparing `valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/pdu/drivers/virtual.py` & `valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/pdu/drivers/virtual.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,64 +1,60 @@
 from .. import logger, PDU, PDUPort, PDUState
 
-import time
 import socket
 from contextlib import contextmanager
 
 
 class VirtualPDU(PDU):  # pragma: nocover
-    def __init__(self, name, config):
-        logger.info("Creating a virtual PDU named %s", name)
+    def __init__(self, name, config, reserved_port_ids=[]):
+        logger.debug("Creating a virtual PDU named %s", name)
         self.host, self.port = config.get('hostname', 'localhost:9191').split(':')
         self.port = int(self.port)
-        logger.info("Connecting to %s:%d", self.host, self.port)
+        logger.debug("Connecting to %s:%d", self.host, self.port)
         with self.conn() as s:
             s.sendall((0).to_bytes(4, byteorder='big'))
             num_ports = int(s.recv(1)[0])
             self._ports = [PDUPort(self, i) for i in range(num_ports)]
-        super().__init__(name)
+        super().__init__(name, config, reserved_port_ids)
+
+    @property
+    def default_min_off_time(self):
+        return 0.1
 
     @property
     def ports(self):
         return self._ports
 
     @contextmanager
     def conn(self, *args, **kw):
-        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
+            s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
-        s.connect((self.host, self.port))
-        try:
+            s.connect((self.host, self.port))
             yield s
-        finally:
-            s.close()
 
     def set_port_state(self, port_id, state):
         if state == PDUState.OFF or state == PDUState.REBOOT:
             cmd = (port_id << 2) | 0x02
             with self.conn() as s:
                 s.sendall(cmd.to_bytes(4, byteorder='big'))
-                assert(s.recv(1)[0] == 0x01)
-        if self.state_transition_delay_seconds:
-            time.sleep(self.state_transition_delay_seconds)
+                assert (s.recv(1)[0] == 0x01)
         if state == PDUState.ON or state == PDUState.REBOOT:
             cmd = (port_id << 2) | 0x01
             with self.conn() as s:
                 s.sendall(cmd.to_bytes(4, byteorder='big'))
-                assert(s.recv(1)[0] == 0x01)
-        if self.state_transition_delay_seconds:
-            time.sleep(self.state_transition_delay_seconds)
+                assert (s.recv(1)[0] == 0x01)
 
     def get_port_state(self, port_id):
         cmd = port_id << 2 | 0x03
         with self.conn() as s:
             s.sendall(cmd.to_bytes(4, byteorder='big'))
             state = int(s.recv(1)[0])
-            logger.info("port state %x", state)
+            logger.debug("port state %x", state)
             if state == 0x03:
                 return PDUState.ON
             elif state == 0x04:
                 return PDUState.OFF
             elif state == 0x05:
                 return PDUState.UNKNOWN
             else:
-                assert(False)
+                assert (False)
```

### Comparing `valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/tests/test_message.py` & `valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `valve_gfx_ci.executor.server-0.0.2/src/valve_gfx_ci/executor/server/tests/test_minio.py` & `valve_gfx_ci_executor_server-0.0.3/src/valve_gfx_ci/executor/server/tests/test_minio.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from unittest.mock import call, patch, MagicMock
 from urllib.parse import urlparse
+import subprocess
+import tarfile
 import json
 
 from minio.error import S3Error
 import pytest
 
 from server.minioclient import MinioClient, MinIOPolicyStatement, generate_policy
 import server.config as config
@@ -54,112 +56,133 @@
 @patch("server.minioclient.Minio", autospec=True)
 @patch("subprocess.check_call")
 def test_client_instantiation__defaults(subproc_mock, minio_mock):
     MinioClient()
     minio_mock.assert_called_once_with(endpoint=urlparse(config.MINIO_URL).netloc,
                                        access_key=config.MINIO_ROOT_USER, secret_key=config.MINIO_ROOT_PASSWORD,
                                        secure=False)
-    subproc_mock.assert_called_once_with(['mcli', '-q', '--no-color', 'alias', 'set',
+    subproc_mock.assert_called_once_with(['mcli', '--no-color', 'alias', 'set',
                                           config.MINIO_ADMIN_ALIAS, config.MINIO_URL,
                                           config.MINIO_ROOT_USER, config.MINIO_ROOT_PASSWORD])
 
 
 @patch("server.minioclient.Minio", autospec=True)
 @patch("subprocess.check_call")
 def test_client_instantiation__custom_params(subproc_mock, minio_mock):
     MinioClient(url="http://hello-world", user="accesskey", secret_key="secret_key", alias="toto")
     minio_mock.assert_called_once_with(endpoint="hello-world", access_key="accesskey",
                                        secret_key="secret_key", secure=False)
-    subproc_mock.assert_called_once_with(['mcli', '-q', '--no-color', 'alias', 'set',
+    subproc_mock.assert_called_once_with(['mcli', '--no-color', 'alias', 'set',
                                           "toto", "http://hello-world", "accesskey", "secret_key"])
 
 
 @patch("server.minioclient.Minio", autospec=True)
 @patch("subprocess.check_call")
 def test_client_instantiation__no_aliases(subproc_mock, minio_mock):
     MinioClient(url="http://hello-world", user="accesskey", secret_key="secret_key", alias=None)
     minio_mock.assert_called_once_with(endpoint="hello-world", access_key="accesskey",
                                        secret_key="secret_key", secure=False)
     subproc_mock.assert_not_called()
 
 
 @patch("server.minioclient.Minio", autospec=True)
 @patch("subprocess.check_call")
-def test_client_remove_alias(subproc_mock, minio_mock):
+@patch("subprocess.check_output")
+def test_client_remove_alias(check_output_mock, subproc_mock, minio_mock):
     client = MinioClient(url="http://hello-world", user="accesskey", secret_key="secret_key", alias="toto")
-    subproc_mock.assert_called_once_with(['mcli', '-q', '--no-color', 'alias', 'set',
+    subproc_mock.assert_called_once_with(['mcli', '--no-color', 'alias', 'set',
                                           "toto", "http://hello-world", "accesskey", "secret_key"])
 
     client.remove_alias()
-    subproc_mock.assert_called_with(['mcli', '-q', '--no-color', 'alias', 'rm', "toto"])
+    check_output_mock.assert_called_with(['mcli', '--no-color', 'alias', 'rm', "toto"])
 
 
 @patch("subprocess.check_call")
 def test_is_local_url(subproc_mock):
     minio = MinioClient(url="http://10.42.0.1:9000")
 
     assert minio.is_local_url("http://10.42.0.1:9000/toto")
     assert not minio.is_local_url("http://hello-world/toto")
 
     minio = MinioClient(url="http://hello-world")
     assert not minio.is_local_url("http://10.42.0.1:9000/toto")
     assert minio.is_local_url("http://hello-world/toto")
 
 
-class MockStream:
-    def iter_content(self, _):
-        yield b'hello world'
+class MockResponse:
+    content = b'hello world'
+    from_cache = True
 
     def raise_for_status(self):
         pass
 
-    def __enter__(self):
-        return self
 
-    def __exit__(self, *args):
-        pass
-
-
-@patch("server.minioclient.requests.get", return_value=MockStream())
+@patch("server.minioclient.requests.get", return_value=MockResponse())
 @patch("server.minioclient.Minio", autospec=True)
 @patch("server.minioclient.tempfile.NamedTemporaryFile", autospec=True)
 @patch("subprocess.check_call")
 def test_save_boot_artifact(subproc_mock, named_temp_mock, minio_mock, get_mock):
     client = MinioClient()
 
     named_temp_mock().__enter__().name = "/tmp/temp_file"
     client.save_boot_artifact("https://toto.com/path", "/toto/path")
 
     client._client.fput_object.assert_called_once_with("boot", "/toto/path", "/tmp/temp_file")
 
 
+@patch("requests.sessions.Session.get", return_value=MockResponse())
+@patch("server.minioclient.Minio", autospec=True)
+@patch("server.minioclient.tempfile.NamedTemporaryFile", autospec=True)
+@patch("subprocess.check_call")
+def test_save_boot_artifact_cached(subproc_mock, named_temp_mock, minio_mock, get_mock, tmp_path):
+    client = MinioClient(artifact_cache_root=f"{tmp_path}/artifact_cache_root")
+
+    named_temp_mock().__enter__().name = "/tmp/temp_file"
+    client.save_boot_artifact("https://toto.com/path", "/toto/path")
+
+    client._client.fput_object.assert_called_once_with("boot", "/toto/path", "/tmp/temp_file")
+
+
 @patch("server.minioclient.Minio", autospec=True)
 @patch("server.minioclient.TarFile.open", autospec=True)
 @patch("subprocess.check_call")
 def test_extract_archive(subproc_mock, tarfile_mock, minio_mock):
     client = MinioClient()
 
     archive_mock = tarfile_mock.return_value.__enter__.return_value
     file_obj = MagicMock()
-    members = [MagicMock(isfile=MagicMock(return_value=True), size=42),
-               MagicMock(isfile=MagicMock(return_value=False)),
-               None]
+
+    member1 = MagicMock(spec=tarfile.TarInfo)
+    member1.isfile = MagicMock(return_value=True)
+    member1.size.return_value = 42
+    member1.mode = 0o777
+    member1.get_info.return_value = {
+        'gid': 1,
+        'gname': 'group',
+        'mtime': 42,
+        'uid': 2,
+        'uname': 'frank'
+    }
+
+    members = [member1, MagicMock(isfile=MagicMock(return_value=False)), None]
     members[0].name = "toto"
     archive_mock.next = MagicMock(side_effect=members)
 
     client.extract_archive(file_obj, "bucket/rootpath")
 
     tarfile_mock.assert_called_once_with(fileobj=file_obj, mode='r')
     archive_mock.extractfile.assert_called_once_with(members[0])
 
-    client._client.put_object.assert_called_once_with("bucket/rootpath",
-                                                      "toto",
-                                                      archive_mock.extractfile(),
-                                                      members[0].size,
-                                                      num_parallel_uploads=1)
+    client._client.put_object.assert_called_once_with(
+        "bucket/rootpath",
+        "toto",
+        archive_mock.extractfile(),
+        members[0].size,
+        num_parallel_uploads=1,
+        metadata={'X-Amz-Meta-Mc-Attrs': 'gid:1/gname:group/mode:2384495103/mtime:42/uid:2/uname:frank'})
 
 
 @patch("server.minioclient.Minio", autospec=True)
 @patch("subprocess.check_call")
 def test_make_bucket(subproc_mock, minio_mock):
     client = MinioClient()
     client._client = MagicMock()
@@ -173,108 +196,169 @@
     with pytest.raises(ValueError) as exc:
         client.make_bucket('test-id')
     assert "The bucket already exists" in str(exc.value)
 
 
 @patch("server.minioclient.Minio", autospec=True)
 @patch("subprocess.check_call")
-def test_remove_bucket(subproc_mock, minio_mock):
+def test_bucket_exists(subproc_mock, minio_mock):
+    client = MinioClient()
+    client._client = MagicMock()
+    ret = client.bucket_exists('test-id')
+    client._client.bucket_exists.assert_called_once_with('test-id')
+
+    assert ret == client._client.bucket_exists.return_value
+
+
+@patch("server.minioclient.Minio", autospec=True)
+@patch("subprocess.check_call")
+@patch("subprocess.check_output")
+def test_remove_bucket(check_output_mock, _, minio_mock):
     client = MinioClient(url='http://test.invalid', user='test', secret_key='test', alias="local")
     client.remove_bucket('test-id')
-    subproc_mock.assert_has_calls([
-        call(['mcli', '-q', '--no-color', 'alias', 'set', 'local', 'http://test.invalid', 'test', 'test']),
-        call(['mcli', '-q', '--no-color', 'rb', '--force', 'local/test-id'])])
+    check_output_mock.assert_called_with(['mcli', '--no-color', 'rb', '--force', 'local/test-id'])
 
 
 @patch("server.minioclient.Minio", autospec=True)
 @patch("subprocess.check_call")
-def test_minio_add_user(subproc_mock, minio_mock):
+@patch("subprocess.check_output")
+def test_minio_add_user(check_output_mock, _, minio_mock):
     client = MinioClient(url='http://test.invalid', user='test', secret_key='test', alias="local")
     client.add_user('job-id-c', 'job-password')
-    subproc_mock.assert_has_calls([
-        call(['mcli', '-q', '--no-color', 'alias', 'set', 'local', 'http://test.invalid', 'test', 'test']),
-        call(['mcli', '-q', '--no-color', 'admin', 'user', 'add', 'local', 'job-id-c', 'job-password']),
-    ])
+    check_output_mock.assert_called_with(['mcli', '--no-color', 'admin', 'user', 'add', 'local',
+                                          'job-id-c', 'job-password'])
 
 
 @patch("server.minioclient.Minio", autospec=True)
 @patch("subprocess.check_call")
-def test_minio_remove_user(subproc_mock, minio_mock):
+@patch("subprocess.check_output")
+def test_minio_remove_user(check_output_mock, _, minio_mock):
     client = MinioClient(url='http://test.invalid', user='test', secret_key='test', alias="local")
     client.remove_user('username')
-    subproc_mock.assert_has_calls([
-        call(['mcli', '-q', '--no-color', 'alias', 'set', 'local', 'http://test.invalid', 'test', 'test']),
-        call(['mcli', '-q', '--no-color', 'admin', 'user', 'remove', 'local', 'username']),
-    ])
+    check_output_mock.assert_called_with(['mcli', '--no-color', 'admin', 'user', 'remove', 'local', 'username'])
 
 
 @patch("server.minioclient.Minio", autospec=True)
 @patch("subprocess.check_call")
 @patch("subprocess.check_output", return_value="""{"status": "success", "accessKey": "username",
     "userStatus": "enabled", "memberOf": ["group1", "group2"]}""")
 def test_minio_groups_user_is_in(subproc_mock, _, minio_mock):
     client = MinioClient(url='http://test.invalid', user='test', secret_key='test', alias="local")
-    assert client.groups_user_is_in() == ["group1", "group2"]
-    assert client.groups_user_is_in('username') == ["group1", "group2"]
+    assert client.groups_user_is_in() == {"group1", "group2"}
+    assert client.groups_user_is_in('username') == {"group1", "group2"}
     subproc_mock.assert_has_calls([
-        call(['mcli', '-q', '--no-color', '--json', 'admin', 'user', 'info', 'local', 'test']),
-        call(['mcli', '-q', '--no-color', '--json', 'admin', 'user', 'info', 'local', 'username'])
+        call(['mcli', '--no-color', '--json', 'admin', 'user', 'info', 'local', 'test']),
+        call(['mcli', '--no-color', '--json', 'admin', 'user', 'info', 'local', 'username'])
     ])
 
 
 @patch("server.minioclient.Minio", autospec=True)
 @patch("subprocess.check_call")
-def test_minio_add_user_to_group(subproc_mock, minio_mock):
+@patch("subprocess.check_output", return_value="""{"status": "success", "accessKey": "username",
+    "userStatus": "enabled", "memberOf": [{"name": "group1"}, {"name": "group2"}]}""")
+def test_minio_groups_user_is_in__newformat(subproc_mock, _, minio_mock):
+    client = MinioClient(url='http://test.invalid', user='test', secret_key='test', alias="local")
+    assert client.groups_user_is_in() == {"group1", "group2"}
+
+
+@patch("server.minioclient.Minio", autospec=True)
+@patch("subprocess.check_call")
+@patch("subprocess.check_output",
+       side_effect=subprocess.CalledProcessError(1, ["cmd", "arg"], output="An error message"))
+def test_minio_groups_user_is_in__callprocess_error(subproc_mock, _, minio_mock):
+    client = MinioClient(url='http://test.invalid', user='test', secret_key='test', alias="local")
+    with pytest.raises(ValueError) as e:
+        client.groups_user_is_in()
+    assert "Failed to query information about the user" in str(e)
+
+
+@patch("server.minioclient.Minio", autospec=True)
+@patch("subprocess.check_call")
+@patch("subprocess.check_output")
+def test_minio_add_user_to_group(check_output_mock, _, minio_mock):
     client = MinioClient(url='http://test.invalid', user='test', secret_key='test', alias="local")
     client.add_user_to_group('username', 'groupname')
-    subproc_mock.assert_has_calls([
-        call(['mcli', '-q', '--no-color', 'alias', 'set', 'local', 'http://test.invalid', 'test', 'test']),
-        call(['mcli', '-q', '--no-color', 'admin', 'group', 'add', 'local', 'groupname', 'username']),
-    ])
+    check_output_mock.assert_called_with(['mcli', '--no-color', 'admin', 'group', 'add', 'local',
+                                          'groupname', 'username'])
 
 
 @patch("subprocess.check_call")
 @patch("server.minioclient.tempfile.NamedTemporaryFile", autospec=True)
-def test_minio_add_user_policy_add(named_temp_mock, subproc_mock):
+@patch("subprocess.check_output")
+def test_minio_apply_user_policy(check_output_mock, named_temp_mock, _):
     temp_mock = MagicMock()
     temp_mock.name = '/tmp/temp_file'
     named_temp_mock.return_value.__enter__.return_value = temp_mock
 
     policy_statements = [MinIOPolicyStatement(['bucket'])]
     expected_policy = generate_policy(policy_statements)
 
     client = MinioClient(url='http://test.invalid', user='test', secret_key='test', alias="local")
     client.apply_user_policy('policy_name', 'username', policy_statements=policy_statements)
 
     temp_mock.write.assert_called_once_with(json.dumps(expected_policy).encode())
 
-    subproc_mock.assert_has_calls([
-        call(['mcli', '-q', '--no-color', 'alias', 'set', 'local', 'http://test.invalid', 'test', 'test']),
-        call(['mcli', '-q', '--no-color', 'admin', 'policy', 'add', 'local', 'policy_name', '/tmp/temp_file']),
-        call(['mcli', '-q', '--no-color', 'admin', 'policy', 'set', 'local', 'policy_name', 'user=username'])])
+    check_output_mock.assert_has_calls([
+        call(['mcli', '--no-color', 'admin', 'policy', 'create', 'local', 'policy_name', '/tmp/temp_file']),
+        call(['mcli', '--no-color', '--json', 'admin', 'policy', 'attach', 'local', 'policy_name',
+              '--user', 'username'])])
+
+
+def mcli_mock(cmd, error_code):
+    if 'attach' in cmd:
+        output = {
+            "error": {
+                "cause": {
+                    "error": {
+                        "Code": error_code
+                    }
+                }
+            }
+        }
+        raise subprocess.CalledProcessError(returncode=1, cmd=[], output=json.dumps(output))
+
+
+@patch("subprocess.check_call")
+@patch("server.minioclient.tempfile.NamedTemporaryFile", autospec=True)
+@patch("subprocess.check_output", side_effect=lambda cmd: mcli_mock(cmd, "XMinioPolicyAlreadyAttached"))
+def test_minio_apply_user_policy__already_attached(check_output_mock, __, _):
+    client = MinioClient(url='http://test.invalid', user='test', secret_key='test', alias="local")
+    client.apply_user_policy('policy_name', 'username', policy_statements=[MinIOPolicyStatement(['bucket'])])
 
 
 @patch("subprocess.check_call")
-def test_minio_remove_user_policy(subproc_mock):
+@patch("server.minioclient.tempfile.NamedTemporaryFile", autospec=True)
+@patch("subprocess.check_output", side_effect=lambda cmd: mcli_mock(cmd, "Unknownerror"))
+def test_minio_apply_user_policy__unknown_error(check_output_mock, __, _):
+    client = MinioClient(url='http://test.invalid', user='test', secret_key='test', alias="local")
+
+    with pytest.raises(ValueError) as e:
+        client.apply_user_policy('policy_name', 'username', policy_statements=[MinIOPolicyStatement(['bucket'])])
+
+    assert "Applying policy failed: Error: Unknownerror" in str(e)
+
+
+@patch("subprocess.check_call")
+@patch("subprocess.check_output")
+def test_minio_remove_user_policy(check_output_mock, _):
     client = MinioClient(url='http://test.invalid', user='test', secret_key='test', alias="local")
     client.remove_user_policy('policy_name', 'username')
 
-    subproc_mock.assert_has_calls([
-        call(['mcli', '-q', '--no-color', 'alias', 'set', 'local', 'http://test.invalid', 'test', 'test']),
-        call(['mcli', '-q', '--no-color', 'admin', 'policy', 'unset', 'local', 'policy_name', 'user=username']),
-        call(['mcli', '-q', '--no-color', 'admin', 'policy', 'remove', 'local', 'policy_name'])])
+    check_output_mock.assert_has_calls([
+        call(['mcli', '--no-color', 'admin', 'policy', 'detach', 'local', 'policy_name', '--user', 'username']),
+        call(['mcli', '--no-color', 'admin', 'policy', 'remove', 'local', 'policy_name'])])
 
 
 def test_create_valid_bucket_name():
     # Name is too short
     assert MinioClient.create_valid_bucket_name("") == "b--x"
     assert MinioClient.create_valid_bucket_name("ab") == "b--ab"
 
     # Name is too long
-    bucket_name = "rhjfklsahjfkdlsahuifeohwuiafohuiofhueioahufieohauiefohuaieofhuiffdsarewfgdsa"
+    bucket_name = ".rhjfklsahjfkdlsahuifeohwuiafohuiofhueioahufieohauiefohuaieof-"
     assert len(MinioClient.create_valid_bucket_name(bucket_name)) == 63
 
     # Wrong characters
-    assert MinioClient.create_valid_bucket_name("/*_~!@#$%^&*()_+|") == "x-----------------x"
+    assert MinioClient.create_valid_bucket_name("/*_~!@#$%^&*()_+|.---........") == 'x-----------------------x'
 
     # IP address
     assert MinioClient.create_valid_bucket_name("192.168.5.4") == "ip-192.168.5.4"
```

