# Comparing `tmp/pynetdicom-2.0.2.tar.gz` & `tmp/pynetdicom-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynetdicom-2.0.2.tar", last modified: Sat Apr 23 05:56:12 2022, max compression
+gzip compressed data, was "pynetdicom-2.1.0.tar", max compression
```

## Comparing `pynetdicom-2.0.2.tar` & `pynetdicom-2.1.0.tar`

### file list

```diff
@@ -1,151 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.059456 pynetdicom-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1091 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (121)      147 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    22880 2022-04-23 05:56:12.059456 pynetdicom-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    21650 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.039456 pynetdicom-2.0.2/pynetdicom/
--rw-r--r--   0 runner    (1001) docker     (121)     2685 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      737 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9590 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3789 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/_globals.py
--rw-r--r--   0 runner    (1001) docker     (121)   161001 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/_handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/_validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1588 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    32463 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/acse.py
--rw-r--r--   0 runner    (1001) docker     (121)    59655 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/ae.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.039456 pynetdicom-2.0.2/pynetdicom/apps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21133 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/common.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.043456 pynetdicom-2.0.2/pynetdicom/apps/echoscp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/echoscp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6053 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/echoscp/echoscp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.043456 pynetdicom-2.0.2/pynetdicom/apps/echoscu/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/echoscu/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6483 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/echoscu/echoscu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.043456 pynetdicom-2.0.2/pynetdicom/apps/findscu/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/findscu/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11492 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/findscu/findscu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.043456 pynetdicom-2.0.2/pynetdicom/apps/getscu/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/getscu/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9931 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/getscu/getscu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.043456 pynetdicom-2.0.2/pynetdicom/apps/movescu/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/movescu/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11001 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/movescu/movescu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.043456 pynetdicom-2.0.2/pynetdicom/apps/qrscp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/qrscp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26305 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/qrscp/db.py
--rw-r--r--   0 runner    (1001) docker     (121)      957 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/qrscp/default.ini
--rw-r--r--   0 runner    (1001) docker     (121)    11499 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/qrscp/handlers.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    12418 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/qrscp/qrscp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.043456 pynetdicom-2.0.2/pynetdicom/apps/storescp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/storescp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6796 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/storescp/storescp.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.043456 pynetdicom-2.0.2/pynetdicom/apps/storescu/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/storescu/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     9173 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/storescu/storescu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.047456 pynetdicom-2.0.2/pynetdicom/apps/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31470 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     8260 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/test_echoscp.py
--rw-r--r--   0 runner    (1001) docker     (121)    15912 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/test_echoscu.py
--rw-r--r--   0 runner    (1001) docker     (121)    17216 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/test_findscu.py
--rw-r--r--   0 runner    (1001) docker     (121)    17178 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/test_getscu.py
--rw-r--r--   0 runner    (1001) docker     (121)    23359 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/test_movescu.py
--rw-r--r--   0 runner    (1001) docker     (121)    26283 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/test_qrscp_db.py
--rw-r--r--   0 runner    (1001) docker     (121)     6636 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/test_qrscp_echo.py
--rw-r--r--   0 runner    (1001) docker     (121)    17949 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/test_qrscp_find.py
--rw-r--r--   0 runner    (1001) docker     (121)     4175 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/test_qrscp_get.py
--rw-r--r--   0 runner    (1001) docker     (121)     4201 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/test_qrscp_move.py
--rw-r--r--   0 runner    (1001) docker     (121)     2949 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/test_qrscp_store.py
--rw-r--r--   0 runner    (1001) docker     (121)    11069 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/test_storescp.py
--rw-r--r--   0 runner    (1001) docker     (121)    17592 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/apps/tests/test_storescu.py
--rw-r--r--   0 runner    (1001) docker     (121)   168041 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/association.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.047456 pynetdicom-2.0.2/pynetdicom/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2454 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/benchmarks/bench_c_send.py
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/benchmarks/bench_dimse_message.py
--rw-r--r--   0 runner    (1001) docker     (121)     3580 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/benchmarks/bench_pdu.py
--rw-r--r--   0 runner    (1001) docker     (121)     6592 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/benchmarks/bench_presentation.py
--rw-r--r--   0 runner    (1001) docker     (121)    13205 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/dimse.py
--rw-r--r--   0 runner    (1001) docker     (121)    31944 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/dimse_messages.py
--rw-r--r--   0 runner    (1001) docker     (121)    82438 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/dimse_primitives.py
--rw-r--r--   0 runner    (1001) docker     (121)     9308 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/dsutils.py
--rw-r--r--   0 runner    (1001) docker     (121)    18712 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/dul.py
--rw-r--r--   0 runner    (1001) docker     (121)    37353 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/events.py
--rw-r--r--   0 runner    (1001) docker     (121)    35803 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/fsm.py
--rw-r--r--   0 runner    (1001) docker     (121)    72105 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/pdu.py
--rw-r--r--   0 runner    (1001) docker     (121)   128085 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/pdu_items.py
--rw-r--r--   0 runner    (1001) docker     (121)    72788 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/pdu_primitives.py
--rw-r--r--   0 runner    (1001) docker     (121)    41850 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/presentation.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    98760 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/service_class.py
--rw-r--r--   0 runner    (1001) docker     (121)    11896 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/service_class_n.py
--rw-r--r--   0 runner    (1001) docker     (121)    27493 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/sop_class.py
--rw-r--r--   0 runner    (1001) docker     (121)    21641 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.055456 pynetdicom-2.0.2/pynetdicom/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    16541 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/benchmark_script.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.059456 pynetdicom-2.0.2/pynetdicom/tests/cert_files/
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/cert_files/client.crt
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/cert_files/client.key
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/cert_files/server.crt
--rw-r--r--   0 runner    (1001) docker     (121)     1704 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/cert_files/server.key
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.059456 pynetdicom-2.0.2/pynetdicom/tests/dicom_files/
--rw-r--r--   0 runner    (1001) docker     (121)    39122 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/dicom_files/CTImageStorage.dcm
--rw-r--r--   0 runner    (1001) docker     (121)    39088 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/dicom_files/CTImageStorage_bad_meta.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     9712 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/dicom_files/MRImageStorage_ExplicitVRBigEndian.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     6008 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/dicom_files/MRImageStorage_JPG2000_Lossless.dcm
--rw-r--r--   0 runner    (1001) docker     (121)  2098468 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/dicom_files/RTImageStorage.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     4637 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/dicom_files/SCImageStorage_Deflated.dcm
--rw-r--r--   0 runner    (1001) docker     (121)     9922 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/encoded_dimse_msg.py
--rw-r--r--   0 runner    (1001) docker     (121)    15444 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/encoded_dimse_n_msg.py
--rw-r--r--   0 runner    (1001) docker     (121)    30013 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/encoded_pdu_items.py
--rw-r--r--   0 runner    (1001) docker     (121)     3732 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/hide_modules.py
--rw-r--r--   0 runner    (1001) docker     (121)     8895 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/parrot.py
--rw-r--r--   0 runner    (1001) docker     (121)    96264 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_acse.py
--rw-r--r--   0 runner    (1001) docker     (121)    65977 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_ae.py
--rw-r--r--   0 runner    (1001) docker     (121)   243982 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_assoc.py
--rw-r--r--   0 runner    (1001) docker     (121)    98883 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_assoc_n.py
--rw-r--r--   0 runner    (1001) docker     (121)   103595 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_assoc_user.py
--rw-r--r--   0 runner    (1001) docker     (121)      636 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    44764 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_dimse_c.py
--rw-r--r--   0 runner    (1001) docker     (121)    31590 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_dimse_msg.py
--rw-r--r--   0 runner    (1001) docker     (121)    58250 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_dimse_n.py
--rw-r--r--   0 runner    (1001) docker     (121)    30387 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_dimse_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)    22308 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_dsutils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12681 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_dul.py
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_environment.py
--rw-r--r--   0 runner    (1001) docker     (121)    17056 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (121)   293413 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_fsm.py
--rw-r--r--   0 runner    (1001) docker     (121)    56614 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (121)    74927 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_pdu.py
--rw-r--r--   0 runner    (1001) docker     (121)    99960 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_pdu_items.py
--rw-r--r--   0 runner    (1001) docker     (121)    86019 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_presentation.py
--rw-r--r--   0 runner    (1001) docker     (121)    44419 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_primitives.py
--rw-r--r--   0 runner    (1001) docker     (121)     4929 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_service_class.py
--rw-r--r--   0 runner    (1001) docker     (121)    78424 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_service_n.py
--rw-r--r--   0 runner    (1001) docker     (121)    12227 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_service_non_patient.py
--rw-r--r--   0 runner    (1001) docker     (121)   221884 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_service_qr.py
--rw-r--r--   0 runner    (1001) docker     (121)    23629 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_service_relevant_patient.py
--rw-r--r--   0 runner    (1001) docker     (121)    25053 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_service_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     7645 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_service_substance_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)    12658 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_service_verification.py
--rw-r--r--   0 runner    (1001) docker     (121)    18807 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_sop.py
--rw-r--r--   0 runner    (1001) docker     (121)    10827 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     3448 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_timer.py
--rw-r--r--   0 runner    (1001) docker     (121)    69674 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (121)    10852 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2725 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4050 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/timer.py
--rw-r--r--   0 runner    (1001) docker     (121)    30702 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/transport.py
--rw-r--r--   0 runner    (1001) docker     (121)    10106 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/pynetdicom/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-23 05:56:12.039456 pynetdicom-2.0.2/pynetdicom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22880 2022-04-23 05:56:12.000000 pynetdicom-2.0.2/pynetdicom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4379 2022-04-23 05:56:12.000000 pynetdicom-2.0.2/pynetdicom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-23 05:56:12.000000 pynetdicom-2.0.2/pynetdicom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-23 05:56:12.000000 pynetdicom-2.0.2/pynetdicom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-04-23 05:56:12.000000 pynetdicom-2.0.2/pynetdicom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-04-23 05:56:12.000000 pynetdicom-2.0.2/pynetdicom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-04-23 05:56:12.063456 pynetdicom-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-04-23 05:56:08.000000 pynetdicom-2.0.2/setup.py
+-rw-r--r--   0        0        0     1091 2024-05-31 01:07:48.587077 pynetdicom-2.1.0/LICENCE
+-rw-r--r--   0        0        0    21837 2024-05-31 01:07:48.587077 pynetdicom-2.1.0/README.rst
+-rw-r--r--   0        0        0     2747 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/__init__.py
+-rw-r--r--   0        0        0      737 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/__main__.py
+-rw-r--r--   0        0        0     9588 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/_config.py
+-rw-r--r--   0        0        0     5196 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/_globals.py
+-rw-r--r--   0        0        0   161448 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/_handlers.py
+-rw-r--r--   0        0        0     1961 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/_validators.py
+-rw-r--r--   0        0        0     1588 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/_version.py
+-rw-r--r--   0        0        0    32454 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/acse.py
+-rw-r--r--   0        0        0    59645 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/ae.py
+-rw-r--r--   0        0        0        0 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/__init__.py
+-rw-r--r--   0        0        0    21177 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/common.py
+-rw-r--r--   0        0        0        0 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/echoscp/__init__.py
+-rwxr-xr-x   0        0        0     6053 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/echoscp/echoscp.py
+-rw-r--r--   0        0        0        0 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/echoscu/__init__.py
+-rwxr-xr-x   0        0        0     6483 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/echoscu/echoscu.py
+-rw-r--r--   0        0        0        0 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/findscu/__init__.py
+-rwxr-xr-x   0        0        0    11838 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/findscu/findscu.py
+-rw-r--r--   0        0        0        0 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/getscu/__init__.py
+-rwxr-xr-x   0        0        0     9930 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/getscu/getscu.py
+-rw-r--r--   0        0        0        0 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/movescu/__init__.py
+-rwxr-xr-x   0        0        0    11000 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/movescu/movescu.py
+-rw-r--r--   0        0        0        0 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/qrscp/__init__.py
+-rw-r--r--   0        0        0    26289 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/qrscp/db.py
+-rw-r--r--   0        0        0      957 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/qrscp/default.ini
+-rw-r--r--   0        0        0    11846 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/qrscp/handlers.py
+-rwxr-xr-x   0        0        0    12791 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/qrscp/qrscp.py
+-rw-r--r--   0        0        0        0 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/storescp/__init__.py
+-rwxr-xr-x   0        0        0     6796 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/storescp/storescp.py
+-rw-r--r--   0        0        0        0 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/storescu/__init__.py
+-rwxr-xr-x   0        0        0     9148 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/storescu/storescu.py
+-rw-r--r--   0        0        0        0 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/tests/__init__.py
+-rw-r--r--   0        0        0    31471 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/tests/test_common.py
+-rw-r--r--   0        0        0     8258 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/tests/test_echoscp.py
+-rw-r--r--   0        0        0    15935 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/tests/test_echoscu.py
+-rw-r--r--   0        0        0    18295 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/tests/test_findscu.py
+-rw-r--r--   0        0        0    17206 2024-05-31 01:07:48.595077 pynetdicom-2.1.0/pynetdicom/apps/tests/test_getscu.py
+-rw-r--r--   0        0        0    23387 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/apps/tests/test_movescu.py
+-rw-r--r--   0        0        0    26337 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/apps/tests/test_qrscp_db.py
+-rw-r--r--   0        0        0     6626 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/apps/tests/test_qrscp_echo.py
+-rw-r--r--   0        0        0    18241 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/apps/tests/test_qrscp_find.py
+-rw-r--r--   0        0        0     4267 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/apps/tests/test_qrscp_get.py
+-rw-r--r--   0        0        0     4293 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/apps/tests/test_qrscp_move.py
+-rw-r--r--   0        0        0     3041 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/apps/tests/test_qrscp_store.py
+-rw-r--r--   0        0        0    11097 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/apps/tests/test_storescp.py
+-rw-r--r--   0        0        0    17620 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/apps/tests/test_storescu.py
+-rw-r--r--   0        0        0   171589 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/association.py
+-rw-r--r--   0        0        0        0 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/benchmarks/__init__.py
+-rw-r--r--   0        0        0     2482 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/benchmarks/bench_c_send.py
+-rw-r--r--   0        0        0     1948 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/benchmarks/bench_dimse_message.py
+-rw-r--r--   0        0        0     3594 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/benchmarks/bench_pdu.py
+-rw-r--r--   0        0        0     6627 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/benchmarks/bench_presentation.py
+-rw-r--r--   0        0        0    13290 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/dimse.py
+-rw-r--r--   0        0        0    31790 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/dimse_messages.py
+-rw-r--r--   0        0        0    82594 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/dimse_primitives.py
+-rw-r--r--   0        0        0     9601 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/dsutils.py
+-rw-r--r--   0        0        0    18665 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/dul.py
+-rw-r--r--   0        0        0    39088 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/events.py
+-rw-r--r--   0        0        0    35798 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/fsm.py
+-rw-r--r--   0        0        0    72101 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/pdu.py
+-rw-r--r--   0        0        0   127831 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/pdu_items.py
+-rw-r--r--   0        0        0    72770 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/pdu_primitives.py
+-rw-r--r--   0        0        0    51404 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/presentation.py
+-rw-r--r--   0        0        0        0 2024-05-31 01:07:48.599077 pynetdicom-2.1.0/pynetdicom/py.typed
+-rw-r--r--   0        0        0    99629 2024-05-31 01:07:48.603077 pynetdicom-2.1.0/pynetdicom/service_class.py
+-rw-r--r--   0        0        0    12959 2024-05-31 01:07:48.603077 pynetdicom-2.1.0/pynetdicom/service_class_n.py
+-rw-r--r--   0        0        0    33201 2024-05-31 01:07:48.603077 pynetdicom-2.1.0/pynetdicom/sop_class.py
+-rw-r--r--   0        0        0    22159 2024-05-31 01:07:48.603077 pynetdicom-2.1.0/pynetdicom/status.py
+-rw-r--r--   0        0        0        0 2024-05-31 01:07:48.603077 pynetdicom-2.1.0/pynetdicom/tests/__init__.py
+-rwxr-xr-x   0        0        0    15951 2024-05-31 01:07:48.603077 pynetdicom-2.1.0/pynetdicom/tests/benchmark_script.py
+-rw-r--r--   0        0        0     1233 2024-05-31 01:07:48.603077 pynetdicom-2.1.0/pynetdicom/tests/cert_files/client.crt
+-rw-r--r--   0        0        0     1704 2024-05-31 01:07:48.603077 pynetdicom-2.1.0/pynetdicom/tests/cert_files/client.key
+-rw-r--r--   0        0        0     1302 2024-05-31 01:07:48.603077 pynetdicom-2.1.0/pynetdicom/tests/cert_files/server.crt
+-rw-r--r--   0        0        0     1704 2024-05-31 01:07:48.603077 pynetdicom-2.1.0/pynetdicom/tests/cert_files/server.key
+-rw-r--r--   0        0        0    39122 2024-05-31 01:07:48.603077 pynetdicom-2.1.0/pynetdicom/tests/dicom_files/CTImageStorage.dcm
+-rw-r--r--   0        0        0    39088 2024-05-31 01:07:48.603077 pynetdicom-2.1.0/pynetdicom/tests/dicom_files/CTImageStorage_bad_meta.dcm
+-rw-r--r--   0        0        0     9712 2024-05-31 01:07:48.603077 pynetdicom-2.1.0/pynetdicom/tests/dicom_files/MRImageStorage_ExplicitVRBigEndian.dcm
+-rw-r--r--   0        0        0     6008 2024-05-31 01:07:48.603077 pynetdicom-2.1.0/pynetdicom/tests/dicom_files/MRImageStorage_JPG2000_Lossless.dcm
+-rw-r--r--   0        0        0  2098468 2024-05-31 01:07:48.611077 pynetdicom-2.1.0/pynetdicom/tests/dicom_files/RTImageStorage.dcm
+-rw-r--r--   0        0        0     4637 2024-05-31 01:07:48.611077 pynetdicom-2.1.0/pynetdicom/tests/dicom_files/SCImageStorage_Deflated.dcm
+-rw-r--r--   0        0        0     9922 2024-05-31 01:07:48.611077 pynetdicom-2.1.0/pynetdicom/tests/encoded_dimse_msg.py
+-rw-r--r--   0        0        0    15444 2024-05-31 01:07:48.611077 pynetdicom-2.1.0/pynetdicom/tests/encoded_dimse_n_msg.py
+-rw-r--r--   0        0        0    30013 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/encoded_pdu_items.py
+-rw-r--r--   0        0        0     3561 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/hide_modules.py
+-rw-r--r--   0        0        0     8861 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/parrot.py
+-rw-r--r--   0        0        0    96404 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_acse.py
+-rw-r--r--   0        0        0    66153 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_ae.py
+-rw-r--r--   0        0        0   253175 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_assoc.py
+-rw-r--r--   0        0        0    98967 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_assoc_n.py
+-rw-r--r--   0        0        0   103803 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_assoc_user.py
+-rw-r--r--   0        0        0      659 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_cli.py
+-rw-r--r--   0        0        0    44830 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_dimse_c.py
+-rw-r--r--   0        0        0    31593 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_dimse_msg.py
+-rw-r--r--   0        0        0    58328 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_dimse_n.py
+-rw-r--r--   0        0        0    30422 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_dimse_provider.py
+-rw-r--r--   0        0        0    22315 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_dsutils.py
+-rw-r--r--   0        0        0    12695 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_dul.py
+-rw-r--r--   0        0        0     1452 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_environment.py
+-rw-r--r--   0        0        0    18572 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_events.py
+-rw-r--r--   0        0        0   293971 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_fsm.py
+-rw-r--r--   0        0        0    56656 2024-05-31 01:07:48.615077 pynetdicom-2.1.0/pynetdicom/tests/test_logging.py
+-rw-r--r--   0        0        0    75630 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_pdu.py
+-rw-r--r--   0        0        0   100058 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_pdu_items.py
+-rw-r--r--   0        0        0    86437 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_presentation.py
+-rw-r--r--   0        0        0    44485 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_primitives.py
+-rw-r--r--   0        0        0     4929 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_service_class.py
+-rw-r--r--   0        0        0    78647 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_service_n.py
+-rw-r--r--   0        0        0    12242 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_service_non_patient.py
+-rw-r--r--   0        0        0   228627 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_service_qr.py
+-rw-r--r--   0        0        0    23644 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_service_relevant_patient.py
+-rw-r--r--   0        0        0    26337 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_service_storage.py
+-rw-r--r--   0        0        0     9121 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_service_substance_admin.py
+-rw-r--r--   0        0        0    12672 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_service_verification.py
+-rw-r--r--   0        0        0    25526 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_sop.py
+-rw-r--r--   0        0        0    10823 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_status.py
+-rw-r--r--   0        0        0     3444 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_timer.py
+-rw-r--r--   0        0        0    70584 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_transport.py
+-rw-r--r--   0        0        0    10952 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_utils.py
+-rw-r--r--   0        0        0     2725 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/test_validators.py
+-rw-r--r--   0        0        0      813 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/tests/utils.py
+-rw-r--r--   0        0        0     4041 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/timer.py
+-rw-r--r--   0        0        0    30616 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/transport.py
+-rw-r--r--   0        0        0    10096 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pynetdicom/utils.py
+-rw-r--r--   0        0        0     3753 2024-05-31 01:07:48.619077 pynetdicom-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0    23966 1970-01-01 00:00:00.000000 pynetdicom-2.1.0/PKG-INFO
```

### Comparing `pynetdicom-2.0.2/LICENCE.txt` & `pynetdicom-2.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/PKG-INFO` & `pynetdicom-2.1.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,74 +1,96 @@
 Metadata-Version: 2.1
 Name: pynetdicom
-Version: 2.0.2
+Version: 2.1.0
 Summary: A Python implementation of the DICOM networking protocol
 Home-page: https://github.com/pydicom/pynetdicom
-Author: 
-Author-email: scaramallion@users.noreply.github.com
 License: MIT
-Project-URL: Documentation, https://pydicom.github.io/pynetdicom/
-Keywords: dicom network python medicalimaging radiotherapy oncology pydicom imaging
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
+Keywords: dicom,networking,pydicom
+Author: pynetdicom contributors
+Maintainer: scaramallion
+Maintainer-email: scaramallion@users.noreply.github.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
-Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
 Provides-Extra: apps
+Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
-License-File: LICENCE.txt
+Requires-Dist: asv (>=0.6,<0.7) ; extra == "dev"
+Requires-Dist: black (>=23.1,<25.0) ; extra == "dev"
+Requires-Dist: codespell (>=2.2,<3.0) ; extra == "dev"
+Requires-Dist: coverage (>=7.3,<8.0) ; extra == "dev" or extra == "tests"
+Requires-Dist: mypy (>=1.7,<2.0) ; extra == "dev"
+Requires-Dist: numpydoc (>=1.6,<2.0) ; extra == "docs"
+Requires-Dist: pydicom (>=2.4,<2.5)
+Requires-Dist: pyfakefs (>=5.3,<6.0) ; extra == "dev" or extra == "tests"
+Requires-Dist: pytest (>=7.4,<8.0) ; extra == "dev" or extra == "tests"
+Requires-Dist: pytest-cov (>=4.1,<5.0) ; extra == "dev" or extra == "tests"
+Requires-Dist: ruff (==0.1.5) ; extra == "dev"
+Requires-Dist: sphinx (>=7.2,<8.0) ; extra == "docs"
+Requires-Dist: sphinx-copybutton (>=0.5,<0.6) ; extra == "docs"
+Requires-Dist: sphinx-rtd-theme (>=1.3,<2.0) ; extra == "docs"
+Requires-Dist: sqlalchemy (>=2.0,<3.0) ; extra == "apps" or extra == "dev" or extra == "tests"
+Project-URL: Documentation, https://pydicom.github.io/pynetdicom
+Description-Content-Type: text/x-rst
+
+|coverage| |unit-tests| |type-hints| |docs| |black| |pypi-versions| |python-versions| |conda| |zenodo|
+
+.. |coverage| image:: https://codecov.io/gh/pydicom/pynetdicom/branch/main/graph/badge.svg 
+   :target: https://codecov.io/gh/pydicom/pynetdicom
+
+.. |unit-tests| image:: https://github.com/pydicom/pynetdicom/workflows/unit-tests/badge.svg
+   :target: https://github.com/pydicom/pynetdicom/actions?query=workflow%3Aunit-tests
 
-.. class:: center
-.. image:: https://codecov.io/gh/pydicom/pynetdicom/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/pydicom/pynetdicom
-.. image:: https://github.com/pydicom/pynetdicom/workflows/unit-tests/badge.svg
-    :target: https://github.com/pydicom/pynetdicom/actions?query=workflow%3Aunit-tests
-.. image:: https://github.com/pydicom/pynetdicom/workflows/type-hints/badge.svg
-    :target: https://github.com/pydicom/pynetdicom/actions?query=workflow%3Atype-hints
-.. image:: https://circleci.com/gh/pydicom/pynetdicom/tree/master.svg?style=shield
-    :target: https://circleci.com/gh/pydicom/pynetdicom/tree/master
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-.. image:: https://badge.fury.io/py/pynetdicom.svg
-    :target: https://badge.fury.io/py/pynetdicom
-.. image:: https://img.shields.io/pypi/pyversions/pynetdicom.svg
-    :target: https://img.shields.io/pypi/pyversions/pynetdicom.svg
-.. image:: https://img.shields.io/conda/vn/conda-forge/pynetdicom.svg
+.. |type-hints| image:: https://github.com/pydicom/pynetdicom/workflows/type-hints/badge.svg
+   :target: https://github.com/pydicom/pynetdicom/actions?query=workflow%3Atype-hints
+
+.. |docs| image:: https://circleci.com/gh/pydicom/pynetdicom/tree/main.svg?style=shield
+   :target: https://circleci.com/gh/pydicom/pynetdicom/tree/main
+
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+
+.. |pypi-versions| image:: https://badge.fury.io/py/pynetdicom.svg
+   :target: https://badge.fury.io/py/pynetdicom
+
+.. |python-versions| image:: https://img.shields.io/pypi/pyversions/pynetdicom.svg
+   :target: https://img.shields.io/pypi/pyversions/pynetdicom.svg
+
+.. |conda| image:: https://img.shields.io/conda/vn/conda-forge/pynetdicom.svg
    :target: https://anaconda.org/conda-forge/pynetdicom
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3880767.svg
+
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3880767.svg
    :target: https://doi.org/10.5281/zenodo.3880767
-.. image:: https://badges.gitter.im/pydicom/Lobby.svg
-    :target: https://gitter.im/pydicom/Lobby
 
 
 pynetdicom
 ==========
 
-A Python implementation of the `DICOM <http://dicom.nema.org>`_
+A Python implementation of the `DICOM <https://www.dicomstandard.org>`_
 networking protocol, originally based on (legacy)
 `pynetdicom <https://github.com/patmun/pynetdicom_legacy>`_.
 
 
 Description
 -----------
 
-`DICOM <http://dicom.nema.org>`_ is the international standard for medical
-images and related information. It defines the formats and communication
+`DICOM <https://www.dicomstandard.org>`_ is the international standard for
+medical images and related information. It defines the formats and communication
 protocols for media exchange in radiology, cardiology, radiotherapy and other
 medical domains.
 
 *pynetdicom* is a pure Python 3.7+ package that implements the DICOM
 networking protocol. Working with
 `pydicom <https://github.com/pydicom/pydicom>`_, it allows the easy creation
 of DICOM *Service Class Users* (SCUs) and *Service Class Providers* (SCPs).
@@ -87,17 +109,17 @@
   `AE.associate() <https://pydicom.github.io/pynetdicom/stable/reference/generated/pynetdicom.ae.ApplicationEntity.html#pynetdicom.ae.ApplicationEntity.associate>`_
   method, which returns an
   `Association <https://pydicom.github.io/pynetdicom/stable/reference/generated/pynetdicom.association.Association.html#pynetdicom.association.Association>`_
   thread.
 
 Once associated, the services available to the association can
 be used by sending
-`DIMSE-C <http://dicom.nema.org/medical/dicom/current/output/html/part07.html#chapter_9>`_
+`DIMSE-C <https://dicom.nema.org/medical/dicom/current/output/html/part07.html#chapter_9>`_
 and
-`DIMSE-N <http://dicom.nema.org/medical/dicom/current/output/html/part07.html#chapter_10>`_
+`DIMSE-N <https://dicom.nema.org/medical/dicom/current/output/html/part07.html#chapter_10>`_
 messages.
 
 Documentation
 -------------
 The *pynetdicom*
 `tutorials <https://pydicom.github.io/pynetdicom/stable/tutorials/index.html>`_,
 `user guide <https://pydicom.github.io/pynetdicom/stable/user/index.html>`_,
@@ -116,28 +138,25 @@
 
 Installing current release
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 Using pip:
 
 .. code-block:: sh
 
-    $ pip install pynetdicom
+    pip install -U pynetdicom
 
 Using conda:
 
 .. code-block:: sh
 
-    $ conda install -c conda-forge pynetdicom
-
+    conda install -c conda-forge pynetdicom
 
-Installing development version
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-.. code-block:: sh
-
-    $ pip install git+https://github.com/pydicom/pynetdicom.git
+For more detailed instructions, including how to install the
+current development version, please see the `installation guide
+<https://pydicom.github.io/pynetdicom/stable/tutorials/installation.html>`_.
 
 
 Supported DIMSE Services
 ------------------------
 SCU Services
 ~~~~~~~~~~~~
 
@@ -267,14 +286,15 @@
 Some basic DICOM applications are included with *pynetdicom*:
 
 * `echoscp <https://pydicom.github.io/pynetdicom/stable/apps/echoscp.html>`_
 * `echoscu <https://pydicom.github.io/pynetdicom/stable/apps/echoscu.html>`_
 * `findscu <https://pydicom.github.io/pynetdicom/stable/apps/findscu.html>`_
 * `getscu <https://pydicom.github.io/pynetdicom/stable/apps/getscu.html>`_
 * `qrscp <https://pydicom.github.io/pynetdicom/stable/apps/qrscp.html>`_
+  (requires `sqlalchemy <https://www.sqlalchemy.org/>`_)
 * `movescu <https://pydicom.github.io/pynetdicom/stable/apps/movescu.html>`_
 * `storescp <https://pydicom.github.io/pynetdicom/stable/apps/storescp.html>`_
 * `storescu <https://pydicom.github.io/pynetdicom/stable/apps/storescu.html>`_
 
 Code Examples
 -------------
 
@@ -287,15 +307,15 @@
 Send a C-ECHO request to a Verification SCP (at TCP/IP address
 *addr*, listen port number *port*):
 
 .. code-block:: python
 
         from pynetdicom import AE
 
-        ae = AE(ae_title=b'MY_ECHO_SCU')
+        ae = AE(ae_title='MY_ECHO_SCU')
         # Verification SOP Class has a UID of 1.2.840.10008.1.1
         #   we can use the UID str directly when adding the requested
         #   presentation context
         ae.add_requested_context('1.2.840.10008.1.1')
 
         # Associate with a peer AE
         assoc = ae.associate(addr, port)
@@ -317,15 +337,15 @@
 bind a handler to the ``evt.EVT_C_ECHO`` event if you want to return something
 other than an ``0x0000`` *Success* status):
 
 .. code-block:: python
 
         from pynetdicom import AE, VerificationPresentationContexts
 
-        ae = AE(ae_title=b'MY_ECHO_SCP')
+        ae = AE(ae_title='MY_ECHO_SCP')
         # Or we can use the inbuilt VerificationPresentationContexts list,
         #   there's one for each of the supported Service Classes
         # In this case, we are supporting any requests to use Verification SOP
         #   Class in the association
         ae.supported_contexts = VerificationPresentationContexts
 
         # Start the SCP on (host, port) in blocking mode
@@ -340,21 +360,21 @@
 requestor's address and port number and the timestamp for the event.
 
 .. code-block:: python
 
         import logging
 
         from pynetdicom import AE, evt, debug_logger
-        from pynetdicom.sop_class import VerificationSOPClass
+        from pynetdicom.sop_class import Verification
 
         # Setup logging to use the StreamHandler at the debug level
         debug_logger()
 
-        ae = AE(ae_title=b'MY_ECHO_SCP')
-        ae.add_supported_context(VerificationSOPClass)
+        ae = AE(ae_title='MY_ECHO_SCP')
+        ae.add_supported_context(Verification)
 
         # Implement the EVT_C_ECHO handler
         def handle_echo(event, logger):
             """Handle a C-ECHO service request.
 
             Parameters
             ----------
@@ -390,15 +410,15 @@
         #   the handler
         handlers = [(evt.EVT_C_ECHO, handle_echo, [logging.getLogger('pynetdicom')])]
 
         # Start the SCP in non-blocking mode
         scp = ae.start_server(("localhost", 11112), block=False, evt_handlers=handlers)
 
         # Associate and send a C-ECHO request to our own Verification SCP
-        ae.add_requested_context(VerificationSOPClass)
+        ae.add_requested_context(Verification)
         assoc = ae.associate('localhost', 11112)
         if assoc.is_established:
             status = assoc.send_c_echo()
             assoc.release()
 
         # Shutdown the SCP
         scp.shutdown()
@@ -412,15 +432,15 @@
 
         from pydicom import dcmread
         from pydicom.uid import ImplicitVRLittleEndian
 
         from pynetdicom import AE, VerificationPresentationContexts
         from pynetdicom.sop_class import CTImageStorage, MRImageStorage
 
-        ae = AE(ae_title=b'MY_STORAGE_SCU')
+        ae = AE(ae_title='MY_STORAGE_SCU')
         # We can also do the same thing with the requested contexts
         ae.requested_contexts = VerificationPresentationContexts
         # Or we can use inbuilt objects like CTImageStorage.
         # The requested presentation context's transfer syntaxes can also
         #   be specified using a str/UID or list of str/UIDs
         ae.add_requested_context(CTImageStorage,
                                  transfer_syntax=ImplicitVRLittleEndian)
@@ -435,8 +455,7 @@
             # `status` is the response from the peer to the store request
             # but may be an empty pydicom Dataset if the peer timed out or
             # sent an invalid dataset.
             status = assoc.send_c_store(dataset)
 
             assoc.release()
 
-
```

### Comparing `pynetdicom-2.0.2/README.rst` & `pynetdicom-2.1.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,50 @@
-.. class:: center
-.. image:: https://codecov.io/gh/pydicom/pynetdicom/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/pydicom/pynetdicom
-.. image:: https://github.com/pydicom/pynetdicom/workflows/unit-tests/badge.svg
-    :target: https://github.com/pydicom/pynetdicom/actions?query=workflow%3Aunit-tests
-.. image:: https://github.com/pydicom/pynetdicom/workflows/type-hints/badge.svg
-    :target: https://github.com/pydicom/pynetdicom/actions?query=workflow%3Atype-hints
-.. image:: https://circleci.com/gh/pydicom/pynetdicom/tree/master.svg?style=shield
-    :target: https://circleci.com/gh/pydicom/pynetdicom/tree/master
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-.. image:: https://badge.fury.io/py/pynetdicom.svg
-    :target: https://badge.fury.io/py/pynetdicom
-.. image:: https://img.shields.io/pypi/pyversions/pynetdicom.svg
-    :target: https://img.shields.io/pypi/pyversions/pynetdicom.svg
-.. image:: https://img.shields.io/conda/vn/conda-forge/pynetdicom.svg
+|coverage| |unit-tests| |type-hints| |docs| |black| |pypi-versions| |python-versions| |conda| |zenodo|
+
+.. |coverage| image:: https://codecov.io/gh/pydicom/pynetdicom/branch/main/graph/badge.svg 
+   :target: https://codecov.io/gh/pydicom/pynetdicom
+
+.. |unit-tests| image:: https://github.com/pydicom/pynetdicom/workflows/unit-tests/badge.svg
+   :target: https://github.com/pydicom/pynetdicom/actions?query=workflow%3Aunit-tests
+
+.. |type-hints| image:: https://github.com/pydicom/pynetdicom/workflows/type-hints/badge.svg
+   :target: https://github.com/pydicom/pynetdicom/actions?query=workflow%3Atype-hints
+
+.. |docs| image:: https://circleci.com/gh/pydicom/pynetdicom/tree/main.svg?style=shield
+   :target: https://circleci.com/gh/pydicom/pynetdicom/tree/main
+
+.. |black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+
+.. |pypi-versions| image:: https://badge.fury.io/py/pynetdicom.svg
+   :target: https://badge.fury.io/py/pynetdicom
+
+.. |python-versions| image:: https://img.shields.io/pypi/pyversions/pynetdicom.svg
+   :target: https://img.shields.io/pypi/pyversions/pynetdicom.svg
+
+.. |conda| image:: https://img.shields.io/conda/vn/conda-forge/pynetdicom.svg
    :target: https://anaconda.org/conda-forge/pynetdicom
-.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3880767.svg
+
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3880767.svg
    :target: https://doi.org/10.5281/zenodo.3880767
-.. image:: https://badges.gitter.im/pydicom/Lobby.svg
-    :target: https://gitter.im/pydicom/Lobby
 
 
 pynetdicom
 ==========
 
-A Python implementation of the `DICOM <http://dicom.nema.org>`_
+A Python implementation of the `DICOM <https://www.dicomstandard.org>`_
 networking protocol, originally based on (legacy)
 `pynetdicom <https://github.com/patmun/pynetdicom_legacy>`_.
 
 
 Description
 -----------
 
-`DICOM <http://dicom.nema.org>`_ is the international standard for medical
-images and related information. It defines the formats and communication
+`DICOM <https://www.dicomstandard.org>`_ is the international standard for
+medical images and related information. It defines the formats and communication
 protocols for media exchange in radiology, cardiology, radiotherapy and other
 medical domains.
 
 *pynetdicom* is a pure Python 3.7+ package that implements the DICOM
 networking protocol. Working with
 `pydicom <https://github.com/pydicom/pydicom>`_, it allows the easy creation
 of DICOM *Service Class Users* (SCUs) and *Service Class Providers* (SCPs).
@@ -56,17 +63,17 @@
   `AE.associate() <https://pydicom.github.io/pynetdicom/stable/reference/generated/pynetdicom.ae.ApplicationEntity.html#pynetdicom.ae.ApplicationEntity.associate>`_
   method, which returns an
   `Association <https://pydicom.github.io/pynetdicom/stable/reference/generated/pynetdicom.association.Association.html#pynetdicom.association.Association>`_
   thread.
 
 Once associated, the services available to the association can
 be used by sending
-`DIMSE-C <http://dicom.nema.org/medical/dicom/current/output/html/part07.html#chapter_9>`_
+`DIMSE-C <https://dicom.nema.org/medical/dicom/current/output/html/part07.html#chapter_9>`_
 and
-`DIMSE-N <http://dicom.nema.org/medical/dicom/current/output/html/part07.html#chapter_10>`_
+`DIMSE-N <https://dicom.nema.org/medical/dicom/current/output/html/part07.html#chapter_10>`_
 messages.
 
 Documentation
 -------------
 The *pynetdicom*
 `tutorials <https://pydicom.github.io/pynetdicom/stable/tutorials/index.html>`_,
 `user guide <https://pydicom.github.io/pynetdicom/stable/user/index.html>`_,
@@ -85,28 +92,25 @@
 
 Installing current release
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 Using pip:
 
 .. code-block:: sh
 
-    $ pip install pynetdicom
+    pip install -U pynetdicom
 
 Using conda:
 
 .. code-block:: sh
 
-    $ conda install -c conda-forge pynetdicom
-
-
-Installing development version
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-.. code-block:: sh
+    conda install -c conda-forge pynetdicom
 
-    $ pip install git+https://github.com/pydicom/pynetdicom.git
+For more detailed instructions, including how to install the
+current development version, please see the `installation guide
+<https://pydicom.github.io/pynetdicom/stable/tutorials/installation.html>`_.
 
 
 Supported DIMSE Services
 ------------------------
 SCU Services
 ~~~~~~~~~~~~
 
@@ -236,14 +240,15 @@
 Some basic DICOM applications are included with *pynetdicom*:
 
 * `echoscp <https://pydicom.github.io/pynetdicom/stable/apps/echoscp.html>`_
 * `echoscu <https://pydicom.github.io/pynetdicom/stable/apps/echoscu.html>`_
 * `findscu <https://pydicom.github.io/pynetdicom/stable/apps/findscu.html>`_
 * `getscu <https://pydicom.github.io/pynetdicom/stable/apps/getscu.html>`_
 * `qrscp <https://pydicom.github.io/pynetdicom/stable/apps/qrscp.html>`_
+  (requires `sqlalchemy <https://www.sqlalchemy.org/>`_)
 * `movescu <https://pydicom.github.io/pynetdicom/stable/apps/movescu.html>`_
 * `storescp <https://pydicom.github.io/pynetdicom/stable/apps/storescp.html>`_
 * `storescu <https://pydicom.github.io/pynetdicom/stable/apps/storescu.html>`_
 
 Code Examples
 -------------
 
@@ -256,15 +261,15 @@
 Send a C-ECHO request to a Verification SCP (at TCP/IP address
 *addr*, listen port number *port*):
 
 .. code-block:: python
 
         from pynetdicom import AE
 
-        ae = AE(ae_title=b'MY_ECHO_SCU')
+        ae = AE(ae_title='MY_ECHO_SCU')
         # Verification SOP Class has a UID of 1.2.840.10008.1.1
         #   we can use the UID str directly when adding the requested
         #   presentation context
         ae.add_requested_context('1.2.840.10008.1.1')
 
         # Associate with a peer AE
         assoc = ae.associate(addr, port)
@@ -286,15 +291,15 @@
 bind a handler to the ``evt.EVT_C_ECHO`` event if you want to return something
 other than an ``0x0000`` *Success* status):
 
 .. code-block:: python
 
         from pynetdicom import AE, VerificationPresentationContexts
 
-        ae = AE(ae_title=b'MY_ECHO_SCP')
+        ae = AE(ae_title='MY_ECHO_SCP')
         # Or we can use the inbuilt VerificationPresentationContexts list,
         #   there's one for each of the supported Service Classes
         # In this case, we are supporting any requests to use Verification SOP
         #   Class in the association
         ae.supported_contexts = VerificationPresentationContexts
 
         # Start the SCP on (host, port) in blocking mode
@@ -309,21 +314,21 @@
 requestor's address and port number and the timestamp for the event.
 
 .. code-block:: python
 
         import logging
 
         from pynetdicom import AE, evt, debug_logger
-        from pynetdicom.sop_class import VerificationSOPClass
+        from pynetdicom.sop_class import Verification
 
         # Setup logging to use the StreamHandler at the debug level
         debug_logger()
 
-        ae = AE(ae_title=b'MY_ECHO_SCP')
-        ae.add_supported_context(VerificationSOPClass)
+        ae = AE(ae_title='MY_ECHO_SCP')
+        ae.add_supported_context(Verification)
 
         # Implement the EVT_C_ECHO handler
         def handle_echo(event, logger):
             """Handle a C-ECHO service request.
 
             Parameters
             ----------
@@ -359,15 +364,15 @@
         #   the handler
         handlers = [(evt.EVT_C_ECHO, handle_echo, [logging.getLogger('pynetdicom')])]
 
         # Start the SCP in non-blocking mode
         scp = ae.start_server(("localhost", 11112), block=False, evt_handlers=handlers)
 
         # Associate and send a C-ECHO request to our own Verification SCP
-        ae.add_requested_context(VerificationSOPClass)
+        ae.add_requested_context(Verification)
         assoc = ae.associate('localhost', 11112)
         if assoc.is_established:
             status = assoc.send_c_echo()
             assoc.release()
 
         # Shutdown the SCP
         scp.shutdown()
@@ -381,15 +386,15 @@
 
         from pydicom import dcmread
         from pydicom.uid import ImplicitVRLittleEndian
 
         from pynetdicom import AE, VerificationPresentationContexts
         from pynetdicom.sop_class import CTImageStorage, MRImageStorage
 
-        ae = AE(ae_title=b'MY_STORAGE_SCU')
+        ae = AE(ae_title='MY_STORAGE_SCU')
         # We can also do the same thing with the requested contexts
         ae.requested_contexts = VerificationPresentationContexts
         # Or we can use inbuilt objects like CTImageStorage.
         # The requested presentation context's transfer syntaxes can also
         #   be specified using a str/UID or list of str/UIDs
         ae.add_requested_context(CTImageStorage,
                                  transfer_syntax=ImplicitVRLittleEndian)
```

### Comparing `pynetdicom-2.0.2/pynetdicom/__init__.py` & `pynetdicom-2.1.0/pynetdicom/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 
 PYNETDICOM_IMPLEMENTATION_UID: UID = UID(f"{PYNETDICOM_UID_PREFIX}{'.'.join(_version)}")
 """The (0002,0012) *Implementation Class UID* used by *pynetdicom*"""
 assert PYNETDICOM_IMPLEMENTATION_UID.is_valid
 
 
 # Convenience imports
+# ruff: noqa: E402,F401
 from pynetdicom import events as evt
 from pynetdicom.ae import ApplicationEntity as AE
 from pynetdicom.association import Association
 from pynetdicom._globals import (
     ALL_TRANSFER_SYNTAXES,
     DEFAULT_TRANSFER_SYNTAXES,
 )
@@ -59,23 +60,24 @@
     RTMachineVerificationPresentationContexts,
     StoragePresentationContexts,
     StorageCommitmentPresentationContexts,
     SubstanceAdministrationPresentationContexts,
     UnifiedProcedurePresentationContexts,
     VerificationPresentationContexts,
 )
+from pynetdicom.sop_class import register_uid
 
 
 # Setup default logging
-logging.getLogger("pynetdicom").addHandler(logging.NullHandler())
+logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 
 def debug_logger() -> None:
     """Setup the logging for debugging."""
-    logger = logging.getLogger("pynetdicom")
+    logger = logging.getLogger(__name__)
     # Ensure only have one StreamHandler
     logger.handlers = []
     handler = logging.StreamHandler()
     logger.setLevel(logging.DEBUG)
     formatter = logging.Formatter("%(levelname).1s: %(message)s")
     handler.setFormatter(formatter)
     logger.addHandler(handler)
```

### Comparing `pynetdicom-2.0.2/pynetdicom/__main__.py` & `pynetdicom-2.1.0/pynetdicom/__main__.py`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/_config.py` & `pynetdicom-2.1.0/pynetdicom/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 .. versionadded:: 1.3
 
 If ``True`` then UIDs will be checked to ensure they're conformant to the
 DICOM Standard and if not then an appropriate response sent, otherwise
 UIDs will only be checked to ensure they're no longer then 64 characters and
 if not then an appropriate response sent.
 
-Default: ``True``
+Default: ``False``
 
 Examples
 --------
 
 >>> from pynetdicom import _config
 >>> _config.ENFORCE_UID_CONFORMANCE = True
 """
@@ -284,25 +284,27 @@
   Where `value` is the :class:`~pydicom.uid.UID` to be validated.
 
   The function should return a :class:`tuple` of (:class:`bool`,
   :class:`str`) as the ``(result, msg)``. If the `result` is ``True``
   then `msg` is ignored, otherwise `msg` will be used to provide feedback
   about why validation has failed.
 
-The default validation functions can be found `here
-<https://github.com/pydicom/pynetdicom/blob/master/pynetdicom/_validators.py>`_
+The default validation functions can be found :gh:`here
+<pynetdicom/blob/master/pynetdicom/_validators.py>`
 .
 
 Examples
 --------
 
 Perform no validation of **AE** DIMSE elements and AE title PDU parameters:
 
 >>> from pynetdicom import _config
->>> _config.VALIDATORS['AE'] = def my_validator(value): return (True, "")
+>>> def my_validator(value): return (True, "")
+...
+>>> _config.VALIDATORS['AE'] = my_validator
 """
 
 
 UNRESTRICTED_STORAGE_SERVICE: bool = False
 """When acting as an SCP assume all presentation contexts with private or
 unknown public abstract syntaxes belong to the storage service and accept all
 storage service requests.
```

### Comparing `pynetdicom-2.0.2/pynetdicom/_globals.py` & `pynetdicom-2.1.0/pynetdicom/_globals.py`

 * *Files 25% similar despite different names*

```diff
@@ -28,35 +28,46 @@
 """
 
 ALL_TRANSFER_SYNTAXES: List[str] = [
     "1.2.840.10008.1.2",  # Implicit VR Little Endian,
     "1.2.840.10008.1.2.1",  # Explicit VR Little Endian,
     "1.2.840.10008.1.2.1.99",  # Deflated Explicit VR Little Endian
     "1.2.840.10008.1.2.2",  # Explicit VR Big Endian,
-    "1.2.840.10008.1.2.4.50",  # JPEG Baseline
-    "1.2.840.10008.1.2.4.51",  # JPEG Extended
-    "1.2.840.10008.1.2.4.57",  # JPEG Lossless P14
-    "1.2.840.10008.1.2.4.70",  # JPEG Lossless
+    "1.2.840.10008.1.2.4.50",  # JPEG Baseline 8 Bit
+    "1.2.840.10008.1.2.4.51",  # JPEG Extended 12 Bit
+    "1.2.840.10008.1.2.4.57",  # JPEG Lossless
+    "1.2.840.10008.1.2.4.70",  # JPEG Lossless SV1
     "1.2.840.10008.1.2.4.80",  # JPEG-LS Lossless
     "1.2.840.10008.1.2.4.81",  # JPEG-LS Lossy
     "1.2.840.10008.1.2.4.90",  # JPEG 2000 Lossless
     "1.2.840.10008.1.2.4.91",  # JPEG 2000
     "1.2.840.10008.1.2.4.92",  # JPEG 2000 Multi-Component Lossless
     "1.2.840.10008.1.2.4.93",  # JPEG 2000 Multi-Component
     "1.2.840.10008.1.2.4.94",  # JPIP Referenced
     "1.2.840.10008.1.2.4.95",  # JPIP Referenced Deflate
     "1.2.840.10008.1.2.4.100",  # MPEG2 Main Profile / Main Level
     "1.2.840.10008.1.2.4.101",  # MPEG2 Main Profile / High Level
+    "1.2.840.10008.1.2.4.101.1",  # Fragmentable MPEG2 Main Profile / High Level
     "1.2.840.10008.1.2.4.102",  # MPEG-4 AVC/H.264 High Profile / Level 4.1
+    "1.2.840.10008.1.2.4.102.1",  # Fragmentable MPEG-4 AVC/H.264 High Profile / Level 4.1
     "1.2.840.10008.1.2.4.103",  # MPEG-4 AVC/H.264 BD-compatible High Profile
+    "1.2.840.10008.1.2.4.103.1",  # Fragmentable MPEG-4 AVC/H.264 BD-compatible High Profile
     "1.2.840.10008.1.2.4.104",  # MPEG-4 AVC/H.264 High Profile For 2D Video
+    "1.2.840.10008.1.2.4.104.1",  # Fragmentable MPEG-4 AVC/H.264 High Profile For 2D Video
     "1.2.840.10008.1.2.4.105",  # MPEG-4 AVC/H.264 High Profile For 3D Video
+    "1.2.840.10008.1.2.4.105.1",  # Fragmentable MPEG-4 AVC/H.264 High Profile For 3D Video
     "1.2.840.10008.1.2.4.106",  # MPEG-4 AVC/H.264 Stereo High Profile
+    "1.2.840.10008.1.2.4.106.1",  # Fragmentable MPEG-4 AVC/H.264 Stereo High Profile
     "1.2.840.10008.1.2.4.107",  # HEVC/H.265 Main Profile / Level 5.1
     "1.2.840.10008.1.2.4.108",  # HEVC/H.265 Main 10 Profile / Level 5.1
+    "1.2.840.10008.1.2.4.201",  # High-Throughput JPEG 2000 Lossless
+    "1.2.840.10008.1.2.4.202",  # High-Throughput JPEG 2000 RPCL
+    "1.2.840.10008.1.2.4.203",  # High-Throughput JPEG 2000
+    "1.2.840.10008.1.2.4.204",  # JPIP HT2K Referenced
+    "1.2.840.10008.1.2.4.205",  # JPIP HTJ2k Referenced Deflate
     "1.2.840.10008.1.2.5",  # RLE Lossless
 ]
 """All current transfer syntaxes and explicit VR big endian.
 
 * Implicit VR Little Endian
 * Explicit VR Little Endian
 * Deflated Explicit VR Little Endian
@@ -70,22 +81,34 @@
 * JPEG 2000 Lossless
 * JPEG 2000
 * JPEG 2000 Multi-component Lossless
 * JPEG 2000 Multi-component
 * JPIP Referenced
 * JPIP Referenced Deflate
 * MPEG2 Main Profile / Main Level
+* Fragmentable MPEG2 Main Profile / Main Level
 * MPEG2 Main Profile / High Level
+* Fragmentable MPEG2 Main Profile / High Level
 * MPEG-4 AVC/H.264 High Profile / Level 4.1
+* Fragmentable MPEG-4 AVC/H.264 High Profile / Level 4.1
 * MPEG-4 AVC/H.264 BD-compatible High Profile
+* Fragmentable MPEG-4 AVC/H.264 BD-compatible High Profile
 * MPEG-4 AVC/H.264 High Profile For 2D Video
+* Fragmentable MPEG-4 AVC/H.264 High Profile For 2D Video
 * MPEG-4 AVC/H.264 High Profile For 3D Video
+* Fragmentable MPEG-4 AVC/H.264 High Profile For 3D Video
 * MPEG-4 AVC/H.264 Stereo High Profile
+* Fragmentable MPEG-4 AVC/H.264 Stereo High Profile
 * HEVC/H.265 Main Profile / Level 5.1
 * HEVC/H.265 Main 10 Profile / Level 5.1
+* High-Throughput JPEG 2000 Lossless
+* High-Throughput JPEG 2000 with RPCL Lossless
+* High-Throughput JPEG 2000
+* JPIP HTK2K Referenced
+* JPIP HTK2K Referenced Deflate
 * RLE Lossless
 """
 
 # The association operation modes
 MODE_ACCEPTOR: str = "acceptor"
 MODE_REQUESTOR: str = "requestor"
```

### Comparing `pynetdicom-2.0.2/pynetdicom/_handlers.py` & `pynetdicom-2.1.0/pynetdicom/_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 if TYPE_CHECKING:  # pragma: no cover
     from pynetdicom.events import Event
     from pynetdicom.pdu_items import UserInformationItem, UserIdentitySubItemRQ
     from pynetdicom.pdu_items import SOPClassCommonExtendedNegotiation
 
 
-LOGGER = logging.getLogger("pynetdicom.events")
+LOGGER = logging.getLogger(__name__)
 
 
 # Debugging handlers
 def debug_fsm(event: "Event") -> None:
     """Debugging handler for the FSM."""
     LOGGER.debug(
         "{}: {} + {} -> {} -> {}".format(
@@ -634,25 +634,25 @@
         LOGGER.debug(line)
 
     return s
 
 
 def _receive_data_tf(event: "Event") -> List[str]:
     """Standard logging handler for receiving a P-DATA-TF PDU."""
-    pass
+    return []
 
 
 def _receive_release_rp(event: "Event") -> List[str]:
     """Standard logging handler for receiving an A-RELEASE-RP PDU."""
-    pass
+    return []
 
 
 def _receive_release_rq(event: "Event") -> List[str]:
     """Standard logging handler for receiving an A-RELEASE-RQ PDU."""
-    pass
+    return []
 
 
 def _send_abort(event: "Event") -> List[str]:
     """Standard logging handler for sending an A-ABORT PDU."""
     pdu = cast("A_ABORT_RQ", event.pdu)
     s = [
         "Abort Parameters:",
@@ -902,25 +902,25 @@
         LOGGER.debug(line)
 
     return s
 
 
 def _send_data_tf(event: "Event") -> List[str]:
     """Standard logging handler for sending a P-DATA-TF PDU."""
-    pass
+    return []
 
 
 def _send_release_rp(event: "Event") -> List[str]:
     """Standard logging handler for sending an A-RELEASE-RP PDU."""
-    pass
+    return []
 
 
 def _send_release_rq(event: "Event") -> List[str]:
     """Standard logging handler for sending an A-RELEASE-RQ PDU."""
-    pass
+    return []
 
 
 # DIMSE sub-handlers
 def _send_c_echo_rq(event: "Event") -> List[str]:
     """Logging handler for when a C-ECHO-RQ is sent.
 
     **C-ECHO Request Parameters**
@@ -929,15 +929,15 @@
     | (M) Affected SOP Class UID
 
     Parameters
     ----------
     event : events.Event
         The evt.EVT_DIMSE_SENT event that occurred.
     """
-    pass
+    return []
 
 
 def _send_c_echo_rsp(event: "Event") -> List[str]:
     """Logging handler for when a C-ECHO-RSP is sent.
 
     **C-ECHO Response Parameters**
 
@@ -947,15 +947,15 @@
     | (M) Status
 
     Parameters
     ----------
     event : events.Event
         The evt.EVT_DIMSE_SENT event that occurred.
     """
-    pass
+    return []
 
 
 def _send_c_store_rq(event: "Event") -> List[str]:
     """Logging handler when a C-STORE-RQ is sent.
 
     **C-STORE Request Elements**
 
@@ -1021,15 +1021,15 @@
     | (M) Status
 
     Parameters
     ----------
     event : events.Event
         The evt.EVT_DIMSE_SENT event that occurred.
     """
-    pass
+    return []
 
 
 def _send_c_find_rq(event: "Event") -> List[str]:
     """Logging handler when a C-FIND-RQ is sent.
 
     **C-FIND Request Parameters**
 
@@ -1281,15 +1281,15 @@
     Covers C-CANCEL-FIND-RQ, C-CANCEL-GET-RQ and C-CANCEL-MOVE-RQ.
 
     Parameters
     ----------
     event : events.Event
         The evt.EVT_DIMSE_SENT event that occurred.
     """
-    pass
+    return []
 
 
 def _recv_c_echo_rq(event: "Event") -> List[str]:
     """Logging handler when a C-ECHO-RQ is received.
 
     **C-ECHO Request Parameters**
 
@@ -2275,15 +2275,15 @@
 
     * DICOM Standard, Part 4, :dcm:`Annex A<part04/chapter_A.html>`
     * DICOM Standard, Part 7, Sections
       :dcm:`9.1.5<part07/chapter_9.html#sect_9.1.5>`,
       :dcm:`9.3.5<part07/sect_9.3.5.html>`, and
       :dcm:`Annex C<part07/chapter_C.html>`
     """
-    pass
+    return 0  # pragma: no cover
 
 
 def doc_handle_find(event: "Event", *args: Sequence[Any]) -> CFindType:
     """Documentation for handlers bound to ``evt.EVT_C_FIND``.
 
     User implementation of this event handler is required if one or more
     services that use C-FIND are to be supported. If a handler is
@@ -2427,15 +2427,15 @@
     * DICOM Standard, Part 4, :dcm:`Annex HH<part04/chapter_HH.html>`
     * DICOM Standard, Part 4, :dcm:`Annex II<part04/chapter_II.html>`
     * DICOM Standard, Part 7, Sections
       :dcm:`9.1.2<part07/chapter_9.html#sect_9.1.2>`,
       :dcm:`9.3.2<part07/sect_9.3.2.html>` and
       :dcm:`Annex C<part07/chapter_C.html>`
     """
-    pass
+    yield 0, None  # pragma: no cover
 
 
 def doc_handle_c_get(event: "Event", *args: Sequence[Any]) -> CGetType:
     """Documentation for handlers bound to ``evt.EVT_C_GET``.
 
     User implementation of this event handler is required if one or more
     services that use C-GET are to be supported. If a handler is
@@ -2585,15 +2585,15 @@
     * DICOM Standard, Part 4, :dcm:`Annex HH<part04/chapter_HH.html>`
     * DICOM Standard, Part 4, :dcm:`Annex II<part04/chapter_II.html>`
     * DICOM Standard, Part 7, Sections
       :dcm:`9.1.3<part07/chapter_9.html#sect_9.1.3>`,
       :dcm:`9.3.3<part07/sect_9.3.3.html>` and
       :dcm:`Annex C<part07/chapter_C.html>`
     """
-    pass
+    yield 0  # pragma: no cover
 
 
 def doc_handle_move(event: "Event", *args: Sequence[Any]) -> CMoveType:
     """Documentation for handlers bound to ``evt.EVT_C_MOVE``.
 
     User implementation of this event handler is required if one or more
     services that use C-MOVE are to be supported. If a handler is
@@ -2771,15 +2771,15 @@
     * DICOM Standard, Part 4, :dcm:`Annex HH<part04/chapter_HH.html>`
     * DICOM Standard, Part 4, :dcm:`Annex II<part04/chapter_II.html>`
     * DICOM Standard, Part 7, Sections
       :dcm:`9.1.4<part07/chapter_9.html#sect_9.1.4>`,
       :dcm:`9.3.4<part07/sect_9.3.4.html>` and
       :dcm:`Annex C<part07/chapter_C.html>`
     """
-    pass
+    yield 0  # pragma: no cover
 
 
 def doc_handle_store(event: "Event", *args: Sequence[Any]) -> StatusType:
     """Documentation for handlers bound to ``evt.EVT_C_STORE``.
 
     User implementation of this event handler is required if one or more
     services that use C-STORE are to be supported. If a handler is
@@ -2897,15 +2897,15 @@
     * DICOM Standard, Part 4, :dcm:`Annex B<part04/chapter_B.html>`
     * DICOM Standard, Part 4, :dcm:`Annex GG<part04/chapter_GG.html>`
     * DICOM Standard, Part 7, Sections
       :dcm:`9.1.1<part07/chapter_9.html#sect_9.1.1>`,
       :dcm:`9.3.1<part07/sect_9.3.html#sect_9.3.1>` and
       :dcm:`Annex C<part07/chapter_C.html>`
     """
-    pass
+    return 0  # pragma: no cover
 
 
 def doc_handle_action(event: "Event", *args: Sequence[Any]) -> UserReturnType:
     """Documentation for handlers bound to ``evt.EVT_N_ACTION``.
 
     User implementation of this event handler is required if one or more
     services that use N-ACTION are to be supported. If a handler is
@@ -3088,15 +3088,15 @@
     * DICOM Standard, Part 4, :dcm:`Annex CC<part04/chapter_CC.html>`
     * DICOM Standard, Part 4, :dcm:`Annex DD<part04/chapter_DD.html>`
     * DICOM Standard, Part 7, Sections
       :dcm:`10.1.4<part07/chapter_10.html#sect_10.1.4>`,
       :dcm:`10.3.4<part07/sect_10.3.4.html>` and
       :dcm:`Annex C<part07/chapter_C.html>`
     """
-    pass
+    return 0, None  # pragma: no cover
 
 
 def doc_handle_create(event: "Event", *args: Sequence[Any]) -> UserReturnType:
     """Documentation for handlers bound to ``evt.EVT_N_CREATE``.
 
     User implementation of this event handler is required if one or more
     services that use N-CREATE are to be supported. If a handler is
@@ -3245,15 +3245,15 @@
     * DICOM Standard, Part 4, :dcm:`Annex CC<part04/chapter_CC.html>`
     * DICOM Standard, Part 4, :dcm:`Annex DD<part04/chapter_DD.html>`
     * DICOM Standard, Part 7, Sections
       :dcm:`10.1.5<part07/chapter_10.html#sect_10.1.5>`,
       :dcm:`10.3.5<part07/sect_10.3.5.html>`
       and :dcm:`Annex C<part07/chapter_C.html>`
     """
-    pass
+    return 0, None  # pragma: no cover
 
 
 def doc_handle_delete(event: "Event", *args: Sequence[Any]) -> StatusType:
     """Documentation for handlers bound to ``evt.EVT_N_DELETE``.
 
     User implementation of this event handler is required if one or more
     services that use N-DELETE are to be supported. If a handler is
@@ -3349,15 +3349,15 @@
     * DICOM Standard, Part 4, :dcm:`Annex H <part04/chapter_H.html>`
     * DICOM Standard, Part 4, :dcm:`Annex DD <part04/chapter_DD.html>`
     * DICOM Standard, Part 7, Sections
       :dcm:`10.1.6<part07/chapter_10.html#sect_10.1.6>`,
       :dcm:`10.3.6<part07/sect_10.3.6.html>`
       and :dcm:`Annex C<part07/chapter_C.html>`
     """
-    pass
+    return 0  # pragma: no cover
 
 
 def doc_handle_event_report(event: "Event", *args: Sequence[Any]) -> UserReturnType:
     """Documentation for handlers bound to ``evt.EVT_N_EVENT_REPORT``.
 
     User implementation of this event handler is required if one or more
     services that use N-EVENT-REPORT are to be supported. If a handler is
@@ -3482,15 +3482,15 @@
     * DICOM Standard, Part 4, :dcm:`Annex CC <part04/chapter_CC.html>`
     * DICOM Standard, Part 4, :dcm:`Annex DD <part04/chapter_DD.html>`
     * DICOM Standard, Part 7, Sections
       :dcm:`10.1.1 <part07/chapter_10.html#sect_10.1.1>`,
       :dcm:`10.3.1 <part07/sect_10.3.html#sect_10.3.1>`
       and :dcm:`Annex C <part07/chapter_C.html>`
     """
-    pass
+    return 0, None  # pragma: no cover
 
 
 def doc_handle_n_get(event: "Event", *args: Sequence[Any]) -> UserReturnType:
     """Documentation for handlers bound to ``evt.EVT_N_GET``.
 
     User implementation of this event handler is required if one or more
     services that use N-GET are to be supported. If a handler is
@@ -3505,15 +3505,15 @@
     **Supported Service Classes**
 
     * :dcm:`Procedure Step<part04/chapter_F.html>`
     * :dcm:`Print Management<part04/chapter_H.html>`
     * :dcm:`Media Creation Management<part04/chapter_S.html>`
     * :dcm:`Unified Procedure Step<part04/chapter_CC.html>`
     * :dcm:`RT Machine Verification<part04/chapter_DD.html>`
-    * :dcm:`Dispaly System Management<part04/chapter_EE.html>`
+    * :dcm:`Display System Management<part04/chapter_EE.html>`
 
     **Status**
 
     Success
       | ``0x0000`` - Success
 
     Failure
@@ -3610,15 +3610,15 @@
     * DICOM Standard, Part 4, :dcm:`Annex DD <part04/chapter_DD.html>`
     * DICOM Standard, Part 4, :dcm:`Annex EE <part04/chapter_EE.html>`
     * DICOM Standard, Part 7, Sections
       :dcm:`10.1.2 <part07/chapter_10.html#sect_10.1.2>`,
       :dcm:`10.3.2 <part07/sect_10.3.2.html>`
       and :dcm:`Annex C <part07/chapter_C.html>`
     """
-    pass
+    return 0, None  # pragma: no cover
 
 
 def doc_handle_set(event: "Event", *args: Sequence[Any]) -> UserReturnType:
     """Documentation for handlers bound to ``evt.EVT_N_SET``.
 
     User implementation of this event handler is required if one or more
     services that use N-SET are to be supported. If a handler is
@@ -3771,15 +3771,15 @@
     * DICOM Standard, Part 4, :dcm:`Annex CC <part04/chapter_CC.html>`
     * DICOM Standard, Part 4, :dcm:`Annex DD <part04/chapter_DD.html>`
     * DICOM Standard, Part 7, Sections
       :dcm:`10.1.3 <part07/chapter_10.html#sect_10.1.3>`,
       :dcm:`10.3.3 <part07/sect_10.3.3.html>`
       and :dcm:`Annex C <part07/chapter_C.html>`
     """
-    pass
+    return 0, None  # pragma: no cover
 
 
 def doc_handle_async(event: "Event", *args: Sequence[Any]) -> Tuple[int, int]:
     """Documentation for handlers bound to ``evt.EVT_ASYNC_OPS``.
 
     User implementation of this event handler is optional. If a handler is
     not implemented and bound to ``evt.EVT_ASYNC_OPS`` then no response to the
@@ -3836,15 +3836,15 @@
         response.
 
     References
     ----------
 
     * DICOM Standard, Part 7, :dcm:`Annex D.3.3.3 <part07/sect_D.3.3.3.html>`
     """
-    pass
+    return 1, 1  # pragma: no cover
 
 
 def doc_handle_sop_common(
     event: "Event", *args: Sequence[Any]
 ) -> Dict[UID, "SOPClassCommonExtendedNegotiation"]:
     """Documentation for handlers bound to ``evt.EVT_SOP_COMMON``.
 
@@ -3893,15 +3893,15 @@
         the corresponding Service Class will be used (if available).
 
     References
     ----------
 
     * DICOM Standard, Part 7, :dcm:`Annex D.3.3.6 <part07/sect_D.3.3.6.html>`
     """
-    pass
+    return {}  # pragma: no cover
 
 
 def doc_handle_sop_extended(event: "Event", *args: Sequence[Any]) -> Dict[UID, bytes]:
     """Documentation for handlers bound to ``evt.EVT_SOP_EXTENDED``.
 
     User implementation of this event handler is required only if
     :dcm:`SOP Class Extended Negotiation<part07/sect_D.3.3.5.html>`
@@ -3950,15 +3950,15 @@
         response is to be sent.
 
     References
     ----------
 
     * DICOM Standard, Part 7, :dcm:`Annex D.3.3.5 <part07/sect_D.3.3.5.html>`
     """
-    pass
+    return {}  # pragma: no cover
 
 
 def doc_handle_userid(
     event: "Event", *args: Sequence[Any]
 ) -> Tuple[bool, Optional[bytes]]:
     """Documentation for handlers bound to ``evt.EVT_USER_ID``.
 
@@ -4026,15 +4026,15 @@
         * ``5`` then return the JSON web token as :class:`bytes`
 
     References
     ----------
 
     * DICOM Standard, Part 7, :dcm:`Annex D.3.3.7 <part07/sect_D.3.3.7.html>`
     """
-    pass
+    return False, None  # pragma: no cover
 
 
 # Notification event handler documentation
 def doc_handle_acse(event: "Event", *args: Sequence[Any]) -> None:
     """Documentation for handlers bound to ``evt.EVT_ACSE_RECV`` or
     ``evt.EVT_ACSE_SENT``.
```

### Comparing `pynetdicom-2.0.2/pynetdicom/_validators.py` & `pynetdicom-2.1.0/pynetdicom/_validators.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 from typing import Tuple
 import unicodedata
 
 from pydicom.uid import UID
 
 
-LOGGER = logging.getLogger("pynetdicom._validators")
+LOGGER = logging.getLogger(__name__)
 
 
 def validate_ae(value: str) -> Tuple[bool, str]:
     """Return ``True`` if `value` is a conformant **AE** value.
 
     An **AE** value:
 
@@ -48,15 +48,14 @@
     if invalid or "\\" in value:
         return False, "must not contain control characters or backslashes"
 
     return True, ""
 
 
 def validate_ui(value: UID) -> Tuple[bool, str]:
-
     from pynetdicom import _config
 
     if not isinstance(value, str):
         return False, "must be pydicom.uid.UID"
 
     value = UID(value)
```

### Comparing `pynetdicom-2.0.2/pynetdicom/_version.py` & `pynetdicom-2.1.0/pynetdicom/_version.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Version information for pynetdicom based on PEP396 and 440"""
 
 import re
 
 
 # pynetdicom version
-__version__ = "2.0.2"
+__version__ = "2.1.0"
 
 # DICOM Standard version used for SOP classes and instances
-__dicom_version__: str = "2021e"
+__dicom_version__: str = "2024b"
 
 VERSION_PATTERN = r"""
     v?
     (?:
         (?:(?P<epoch>[0-9]+)!)?                           # epoch
         (?P<release>[0-9]+(?:\.[0-9]+)*)                  # release segment
         (?P<pre>                                          # pre-release
```

### Comparing `pynetdicom-2.0.2/pynetdicom/acse.py` & `pynetdicom-2.1.0/pynetdicom/acse.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 if TYPE_CHECKING:  # pragma: no cover
     from pynetdicom.association import Association, ServiceUser
     from pynetdicom.dul import DULServiceProvider
     from pynetdicom.transport import AssociationSocket
 
 
-LOGGER = logging.getLogger("pynetdicom.acse")
+LOGGER = logging.getLogger(__name__)
 
 
 class ACSE:
     """The Association Control Service Element (ACSE) service provider.
 
     The ACSE protocol handles association negotiation and establishment, and
     normal and abnormal release of an association.
```

### Comparing `pynetdicom-2.0.2/pynetdicom/ae.py` & `pynetdicom-2.1.0/pynetdicom/ae.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The main user class, represents a DICOM Application Entity
 """
+
 from copy import deepcopy
 from datetime import datetime
 import logging
 from ssl import SSLContext
 import threading
 from typing import (
     Union,
@@ -37,20 +38,20 @@
     MODE_REQUESTOR,
     DEFAULT_MAX_LENGTH,
     DEFAULT_TRANSFER_SYNTAXES,
     BIND_ADDRESS,
 )
 
 
-LOGGER = logging.getLogger("pynetdicom.ae")
+LOGGER = logging.getLogger(__name__)
 
 
 _T = TypeVar("_T")
-ListCXType = List[PresentationContext]
-TSyntaxType = Optional[Union[str, UID, Sequence[Union[str, UID]]]]
+ListCXType = list[PresentationContext]
+TSyntaxType = None | str | UID | Sequence[str] | Sequence[UID]
 
 
 class ApplicationEntity:
     """Represents a DICOM Application Entity (AE).
 
     An AE may be a *Service Class Provider* (SCP), a *Service Class User* (SCU)
     or both.
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/common.py` & `pynetdicom-2.1.0/pynetdicom/apps/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """Utility classes and functions for the apps."""
 
 import logging
 import os
+import re
 from struct import pack
 
 from pydicom import dcmread
 from pydicom.datadict import tag_for_keyword, repeater_has_keyword, get_entry
 from pydicom.dataset import Dataset
-from pydicom.filewriter import write_file_meta_info
 from pydicom.tag import Tag
 from pydicom.uid import DeflatedExplicitVRLittleEndian
 
-from pynetdicom.dsutils import encode
-
 
 def create_dataset(args, logger=None):
     """Return a new or updated dataset.
 
     The DICOM dataset at ``args.file='path/to/file'`` will be read and updated
     using the values in ``args.keyword`` (if specified). If ``args.file=None``
     then a new dataset will be created using the values in ``args.keyword``.
@@ -186,15 +184,15 @@
         self._components = path.split(".")
 
         # Parse current component and set attributes accordingly
         tag = self.tag
         try:
             # Try DICOM dictionary for public elements
             self._entry = get_entry(tag)
-        except Exception as exc:
+        except Exception:
             # Private element
             self._entry = ("UN", "1", "Unknown", False, "Unknown")
 
         # Try to convert value to appropriate type
         self.value = value
 
     @property
@@ -501,21 +499,24 @@
     logger : logging.Logger, optional
         The logger to use for logging.
     """
     formatter = logging.Formatter("%(levelname).1s: %(message)s")
 
     # Setup pynetdicom library's logging
     pynd_logger = logging.getLogger("pynetdicom")
-    handler = logging.StreamHandler()
-    handler.setFormatter(formatter)
-    pynd_logger.addHandler(handler)
-    pynd_logger.setLevel(logging.ERROR)
+    if not any(isinstance(h, logging.StreamHandler) for h in pynd_logger.handlers):
+        handler = logging.StreamHandler()
+        handler.setFormatter(formatter)
+        pynd_logger.addHandler(handler)
+        pynd_logger.setLevel(logging.ERROR)
 
     # Setup application's logging
-    app_logger = logging.Logger(app_name)
+    app_logger = logging.getLogger(app_name)
+    if app_logger.hasHandlers():
+        return app_logger
     handler = logging.StreamHandler()
     handler.setFormatter(formatter)
     app_logger.addHandler(handler)
     app_logger.setLevel(logging.ERROR)
 
     if args.log_type == "q":
         app_logger.handlers = []
@@ -578,15 +579,16 @@
     # Add the file meta information elements
     ds.file_meta = event.file_meta
 
     # Because pydicom uses deferred reads for its decoding, decoding errors
     #   are hidden until encountered by accessing a faulty element
     try:
         sop_class = ds.SOPClassUID
-        sop_instance = ds.SOPInstanceUID
+        # sanitize filename by replacing all illegal characters with underscores
+        sop_instance = re.sub(r"[^\d.]", "_", ds.SOPInstanceUID)
     except Exception as exc:
         app_logger.error(
             "Unable to decode the received dataset or missing 'SOP Class "
             "UID' and/or 'SOP Instance UID' elements"
         )
         app_logger.exception(exc)
         # Unable to decode dataset
@@ -609,40 +611,37 @@
         filename = os.path.join(args.output_directory, filename)
         try:
             os.makedirs(args.output_directory, exist_ok=True)
         except Exception as exc:
             app_logger.error("Unable to create the output directory:")
             app_logger.error(f"    {args.output_directory}")
             app_logger.exception(exc)
-            # Failed - Out of Resources - IOError
+            # Failed - Out of Resources - OSError
             status_ds.Status = 0xA700
             return status_ds
 
     if os.path.exists(filename):
         app_logger.warning("DICOM file already exists, overwriting")
 
     try:
         if event.context.transfer_syntax == DeflatedExplicitVRLittleEndian:
             # Workaround for pydicom issue #1086
             with open(filename, "wb") as f:
-                f.write(b"\x00" * 128)
-                f.write(b"DICM")
-                write_file_meta_info(f, event.file_meta)
-                f.write(encode(ds, False, True, True))
+                f.write(event.encoded_dataset())
         else:
             # We use `write_like_original=False` to ensure that a compliant
             #   File Meta Information Header is written
             ds.save_as(filename, write_like_original=False)
 
         status_ds.Status = 0x0000  # Success
-    except IOError as exc:
+    except OSError as exc:
         app_logger.error("Could not write file to specified directory:")
         app_logger.error(f"    {os.path.dirname(filename)}")
         app_logger.exception(exc)
-        # Failed - Out of Resources - IOError
+        # Failed - Out of Resources - OSError
         status_ds.Status = 0xA700
     except Exception as exc:
         app_logger.error("Could not write file to specified directory:")
         app_logger.error(f"    {os.path.dirname(filename)}")
         app_logger.exception(exc)
         # Failed - Out of Resources - Miscellaneous error
         status_ds.Status = 0xA701
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/echoscp/echoscp.py` & `pynetdicom-2.1.0/pynetdicom/apps/echoscp/echoscp.py`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/echoscu/echoscu.py` & `pynetdicom-2.1.0/pynetdicom/apps/echoscu/echoscu.py`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/findscu/findscu.py` & `pynetdicom-2.1.0/pynetdicom/apps/findscu/findscu.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,22 @@
 from pynetdicom import (
     AE,
     BasicWorklistManagementPresentationContexts,
     QueryRetrievePresentationContexts,
     PYNETDICOM_IMPLEMENTATION_UID,
     PYNETDICOM_IMPLEMENTATION_VERSION,
     PYNETDICOM_UID_PREFIX,
+    UnifiedProcedurePresentationContexts,
 )
 from pynetdicom.apps.common import create_dataset, setup_logging
 from pynetdicom._globals import DEFAULT_MAX_LENGTH
 from pynetdicom.pdu_primitives import SOPClassExtendedNegotiation
 from pynetdicom.sop_class import (
     ModalityWorklistInformationFind,
+    UnifiedProcedureStepPull,
     PatientRootQueryRetrieveInformationModelFind,
     StudyRootQueryRetrieveInformationModelFind,
     PatientStudyOnlyQueryRetrieveInformationModelFind,
 )
 
 
 __version__ = "0.2.0"
@@ -169,14 +171,20 @@
     )
     qr_model.add_argument(
         "-W",
         "--worklist",
         help="use modality worklist information model",
         action="store_true",
     )
+    qr_model.add_argument(
+        "-U",
+        "--ups",
+        help="use unified procedure step information model",
+        action="store_true",
+    )
 
     qr_query = parser.add_argument_group("Query Options")
     qr_query.add_argument(
         "-k",
         "--keyword",
         metavar="[k]eyword: (gggg,eeee)=str, keyword=str",
         help=(
@@ -278,15 +286,15 @@
 
     APP_LOGGER = setup_logging(args, "findscu")
     APP_LOGGER.debug(f"findscu.py v{__version__}")
     APP_LOGGER.debug("")
 
     # Create query (identifier) dataset
     try:
-        # If you're looking at this to see how QR Find works then `identifer`
+        # If you're looking at this to see how QR Find works then `identifier`
         # is a pydicom Dataset instance with your query keys, e.g.:
         #     identifier = Dataset()
         #     identifier.QueryRetrieveLevel = 'PATIENT'
         #     identifier.PatientName = ''
         identifier = create_dataset(args, APP_LOGGER)
     except Exception as exc:
         APP_LOGGER.exception(exc)
@@ -299,20 +307,24 @@
     # Set timeouts
     ae.acse_timeout = args.acse_timeout
     ae.dimse_timeout = args.dimse_timeout
     ae.network_timeout = args.network_timeout
 
     # Set the Presentation Contexts we are requesting the Find SCP support
     ae.requested_contexts = (
-        QueryRetrievePresentationContexts + BasicWorklistManagementPresentationContexts
+        QueryRetrievePresentationContexts
+        + BasicWorklistManagementPresentationContexts
+        + UnifiedProcedurePresentationContexts
     )
 
     # Query/Retrieve Information Models
     if args.worklist:
         query_model = ModalityWorklistInformationFind
+    elif args.ups:
+        query_model = UnifiedProcedureStepPull
     elif args.study:
         query_model = StudyRootQueryRetrieveInformationModelFind
     elif args.psonly:
         query_model = PatientStudyOnlyQueryRetrieveInformationModelFind
     else:
         query_model = PatientRootQueryRetrieveInformationModelFind
 
@@ -353,15 +365,15 @@
         ext_neg=ext_neg,
     )
     if assoc.is_established:
         # Send C-FIND request, `responses` is a generator
         responses = assoc.send_c_find(identifier, query_model)
         # Used to generate filenames if args.write used
         fname = generate_filename()
-        for (status, rsp_identifier) in responses:
+        for status, rsp_identifier in responses:
             # If `status.Status` is one of the 'Pending' statuses then
             #   `rsp_identifier` is the C-FIND response's Identifier dataset
             if status and status.Status in [0xFF00, 0xFF01]:
                 if args.write:
                     rsp_identifier.file_meta = get_file_meta(assoc, query_model)
                     rsp_identifier.save_as(next(fname), write_like_original=False)
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/getscu/getscu.py` & `pynetdicom-2.1.0/pynetdicom/apps/getscu/getscu.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
 
     APP_LOGGER = setup_logging(args, "getscu")
     APP_LOGGER.debug(f"getscu.py v{__version__}")
     APP_LOGGER.debug("")
 
     # Create query (identifier) dataset
     try:
-        # If you're looking at this to see how QR Get works then `identifer`
+        # If you're looking at this to see how QR Get works then `identifier`
         # is a pydicom Dataset instance with your query keys, e.g.:
         #     identifier = Dataset()
         #     identifier.QueryRetrieveLevel = 'PATIENT'
         #     identifier.PatientName = '*'
         identifier = create_dataset(args, APP_LOGGER)
     except Exception as exc:
         APP_LOGGER.exception(exc)
@@ -306,15 +306,15 @@
         evt_handlers=[(evt.EVT_C_STORE, handle_store, [args, APP_LOGGER])],
         max_pdu=args.max_pdu,
     )
 
     if assoc.is_established:
         # Send query
         responses = assoc.send_c_get(identifier, query_model)
-        for (status, rsp_identifier) in responses:
+        for status, rsp_identifier in responses:
             # If `status.Status` is one of the 'Pending' statuses then
             #   `rsp_identifier` is the C-GET response's Identifier dataset
             if status and status.Status in [0xFF00, 0xFF01]:
                 # `rsp_identifier` is a pydicom Dataset containing a query
                 # response. You may want to do something interesting here...
                 pass
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/movescu/movescu.py` & `pynetdicom-2.1.0/pynetdicom/apps/movescu/movescu.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
     APP_LOGGER = setup_logging(args, "movescu")
     APP_LOGGER.debug(f"movescu.py v{__version__}")
     APP_LOGGER.debug("")
 
     # Create query (identifier) dataset
     try:
-        # If you're looking at this to see how QR Move works then `identifer`
+        # If you're looking at this to see how QR Move works then `identifier`
         # is a pydicom Dataset instance with your query keys, e.g.:
         #     identifier = Dataset()
         #     identifier.QueryRetrieveLevel = 'PATIENT'
         #     identifier.PatientName = '*'
         identifier = create_dataset(args, APP_LOGGER)
     except Exception as exc:
         APP_LOGGER.exception(exc)
@@ -335,15 +335,15 @@
         max_pdu=args.max_pdu,
         ext_neg=ext_neg,
     )
     if assoc.is_established:
         # Send query
         move_aet = args.move_aet or args.calling_aet
         responses = assoc.send_c_move(identifier, move_aet, query_model)
-        for (status, rsp_identifier) in responses:
+        for status, rsp_identifier in responses:
             # If `status.Status` is one of the 'Pending' statuses then
             #   `rsp_identifier` is the C-MOVE response's Identifier dataset
             if status and status.Status in [0xFF00, 0xFF01]:
                 # `rsp_identifier` is a pydicom Dataset containing a query
                 # response. You may want to do something interesting here...
                 pass
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/qrscp/db.py` & `pynetdicom-2.1.0/pynetdicom/apps/qrscp/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import sys
 
 try:
     from sqlalchemy import create_engine, Column, ForeignKey, Integer, String
 except ImportError:
     sys.exit("qrscp requires the sqlalchemy package")
 
-from sqlalchemy.ext.declarative import declarative_base
+from sqlalchemy.orm import declarative_base
 
 from pydicom.dataset import Dataset
 
 from pynetdicom import build_context
 from pynetdicom.sop_class import (
     PatientRootQueryRetrieveInformationModelFind,
     PatientRootQueryRetrieveInformationModelMove,
@@ -170,15 +170,15 @@
         instance = result[0]
     else:
         instance = Instance()
 
     # Unique or Required attributes
     required = [
         # (Instance attribute, DICOM keyword, max length, req'd)
-        ("patient_id", "PatientID", 16, True),
+        ("patient_id", "PatientID", 64, True),
         ("patient_name", "PatientName", 64, False),
         ("study_instance_uid", "StudyInstanceUID", 64, True),
         ("study_date", "StudyDate", 8, False),
         ("study_time", "StudyTime", 14, False),
         ("accession_number", "AccessionNumber", 16, False),
         ("study_id", "StudyID", 16, False),
         ("series_instance_uid", "SeriesInstanceUID", 64, True),
@@ -213,15 +213,15 @@
 
     # Transfer Syntax UID
     try:
         tsyntax = ds.file_meta.TransferSyntaxUID
         if tsyntax:
             assert len(tsyntax) < 64
             instance.transfer_syntax_uid = tsyntax
-    except (AttributeError, AssertionError) as exc:
+    except (AttributeError, AssertionError):
         pass
 
     # SOP Class UID
     try:
         uid = ds.SOPClassUID
         if uid:
             assert len(uid) < 64
@@ -695,15 +695,15 @@
     # Absolute path to the stored SOP Instance
     filename = Column(String)
     # Transfer Syntax UID of the SOP Instance
     transfer_syntax_uid = Column(String(64))
     sop_class_uid = Column(String(64))
 
     patient_id = Column(String, ForeignKey("patient.patient_id"))
-    patient_name = Column(String, ForeignKey("patient.patient_id"))
+    patient_name = Column(String, ForeignKey("patient.patient_name"))
 
     study_instance_uid = Column(String, ForeignKey("study.study_instance_uid"))
     study_date = Column(String, ForeignKey("study.study_date"))
     study_time = Column(String, ForeignKey("study.study_time"))
     accession_number = Column(String, ForeignKey("study.accession_number"))
     study_id = Column(String, ForeignKey("study.study_id"))
 
@@ -779,17 +779,17 @@
 
         return build_context(self.sop_class_uid, self.transfer_syntax_uid)
 
 
 class Patient(Base):
     __tablename__ = "patient"
     # (0010,0020) Patient ID | VR LO, VM 1, U
-    patient_id = Column(String(16), primary_key=True)
+    patient_id = Column(String(64), primary_key=True)
     # (0010,0010) Patient's Name | VR PN, VM 1, R
-    patient_name = Column(String(64))
+    patient_name = Column(String(400))
 
 
 class Series(Base):
     __tablename__ = "series"
     # (0020,000E) Series Instance UID | VR UI, VM 1, U
     series_instance_uid = Column(String(64), primary_key=True)
     # (0008,0060) Modality | VR CS, VM 1, R
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/qrscp/default.ini` & `pynetdicom-2.1.0/pynetdicom/apps/qrscp/default.ini`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/qrscp/handlers.py` & `pynetdicom-2.1.0/pynetdicom/apps/qrscp/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,51 +58,58 @@
     requestor = event.assoc.requestor
     timestamp = event.timestamp.strftime("%Y-%m-%d %H:%M:%S")
     addr, port = requestor.address, requestor.port
     logger.info(f"Received C-FIND request from {addr}:{port} at {timestamp}")
 
     model = event.request.AffectedSOPClassUID
 
-    engine = create_engine(db_path)
-    with engine.connect() as conn:
-        Session = sessionmaker(bind=engine)
-        session = Session()
-        # Search database using Identifier as the query
-        try:
-            matches = search(model, event.identifier, session)
-        except InvalidIdentifier as exc:
-            session.rollback()
-            logger.error("Invalid C-FIND Identifier received")
-            logger.error(str(exc))
-            yield 0xA900, None
-            return
-        except Exception as exc:
-            session.rollback()
-            logger.error("Exception occurred while querying database")
-            logger.exception(exc)
-            yield 0xC320, None
-            return
-        finally:
-            session.close()
-
-    # Yield results
-    for match in matches:
-        if event.is_cancelled:
-            yield 0xFE00, None
-            return
-
-        try:
-            response = match.as_identifier(event.identifier, model)
-            response.RetrieveAETitle = event.assoc.ae.ae_title
-        except Exception as exc:
-            logger.error("Error creating response Identifier")
-            logger.exception(exc)
-            yield 0xC322, None
+    if model.keyword in (
+        "UnifiedProcedureStepPull",
+        "ModalityWorklistInformationModelFind",
+    ):
+        yield 0x0000, None
+    else:
+        engine = create_engine(db_path)
+        with engine.connect() as conn:  # noqa: F841
+            Session = sessionmaker(bind=engine)
+            session = Session()
+            # Search database using Identifier as the query
+            try:
+                matches = search(model, event.identifier, session)
+
+            except InvalidIdentifier as exc:
+                session.rollback()
+                logger.error("Invalid C-FIND Identifier received")
+                logger.error(str(exc))
+                yield 0xA900, None
+                return
+            except Exception as exc:
+                session.rollback()
+                logger.error("Exception occurred while querying database")
+                logger.exception(exc)
+                yield 0xC320, None
+                return
+            finally:
+                session.close()
+
+        # Yield results
+        for match in matches:
+            if event.is_cancelled:
+                yield 0xFE00, None
+                return
+
+            try:
+                response = match.as_identifier(event.identifier, model)
+                response.RetrieveAETitle = event.assoc.ae.ae_title
+            except Exception as exc:
+                logger.error("Error creating response Identifier")
+                logger.exception(exc)
+                yield 0xC322, None
 
-        yield 0xFF00, response
+            yield 0xFF00, response
 
 
 def handle_get(event, db_path, cli_config, logger):
     """Handler for evt.EVT_C_GET.
 
     Parameters
     ----------
@@ -127,15 +134,15 @@
     timestamp = event.timestamp.strftime("%Y-%m-%d %H:%M:%S")
     addr, port = requestor.address, requestor.port
     logger.info(f"Received C-GET request from {addr}:{port} at {timestamp}")
 
     model = event.request.AffectedSOPClassUID
 
     engine = create_engine(db_path)
-    with engine.connect() as conn:
+    with engine.connect() as conn:  # noqa: F841
         Session = sessionmaker(bind=engine)
         session = Session()
         # Search database using Identifier as the query
         try:
             matches = search(model, event.identifier, session)
         except InvalidIdentifier as exc:
             session.rollback()
@@ -212,15 +219,15 @@
     except KeyError:
         logger.info("No matching move destination in the configuration")
         yield None, None
         return
 
     model = event.request.AffectedSOPClassUID
     engine = create_engine(db_path)
-    with engine.connect() as conn:
+    with engine.connect() as conn:  # noqa: F841
         Session = sessionmaker(bind=engine)
         session = Session()
         # Search database using Identifier as the query
         try:
             matches = search(model, event.identifier, session)
         except InvalidIdentifier as exc:
             session.rollback()
@@ -322,15 +329,15 @@
         # Failed - Out of Resources
         return 0xA700
 
     logger.info("Instance written to storage directory")
 
     # Dataset successfully written, try to add to/update database
     engine = create_engine(db_path)
-    with engine.connect() as conn:
+    with engine.connect() as conn:  # noqa: F841
         Session = sessionmaker(bind=engine)
         session = Session()
 
         try:
             # Path is relative to the database file
             matches = (
                 session.query(Instance)
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/qrscp/qrscp.py` & `pynetdicom-2.1.0/pynetdicom/apps/qrscp/qrscp.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 
 from pynetdicom import (
     AE,
     _config,
     evt,
+    _handlers,
     AllStoragePresentationContexts,
     ALL_TRANSFER_SYNTAXES,
+    UnifiedProcedurePresentationContexts,
 )
-from pynetdicom import _config, _handlers
 from pynetdicom.apps.common import setup_logging
 from pynetdicom.sop_class import (
     Verification,
+    ModalityWorklistInformationFind,
     PatientRootQueryRetrieveInformationModelFind,
     PatientRootQueryRetrieveInformationModelMove,
     PatientRootQueryRetrieveInformationModelGet,
     StudyRootQueryRetrieveInformationModelFind,
     StudyRootQueryRetrieveInformationModelMove,
     StudyRootQueryRetrieveInformationModelGet,
 )
@@ -40,27 +42,28 @@
 from pynetdicom.apps.qrscp import db
 
 # Use `None` for empty values
 pydicom.config.use_none_as_empty_text_VR_value = True
 # Don't log identifiers
 _config.LOG_RESPONSE_IDENTIFIERS = False
 
+
 # Override the standard logging handlers
 def _dont_log(event):
     pass
 
 
 _handlers._send_c_find_rsp = _dont_log
 _handlers._send_c_get_rsp = _dont_log
 _handlers._send_c_move_rsp = _dont_log
 _handlers._send_c_store_rq = _dont_log
 _handlers._recv_c_store_rsp = _dont_log
 
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 
 
 def _log_config(config, logger):
     """Log the configuration settings.
 
     Parameters
     ----------
@@ -234,15 +237,15 @@
     Returns
     -------
     bool
         ``True`` if the storage directory and database were both cleaned
         successfully, ``False`` otherwise.
     """
     engine = create_engine(db_path)
-    with engine.connect() as conn:
+    with engine.connect() as conn:  # noqa: F841
         Session = sessionmaker(bind=engine)
         session = Session()
         query_success = True
         try:
             fpaths = [ii.filename for ii in session.query(db.Instance).all()]
         except Exception as exc:
             logger.error("Exception raised while querying the database")
@@ -381,14 +384,23 @@
     ae.add_supported_context(PatientRootQueryRetrieveInformationModelFind)
     ae.add_supported_context(PatientRootQueryRetrieveInformationModelMove)
     ae.add_supported_context(PatientRootQueryRetrieveInformationModelGet)
     ae.add_supported_context(StudyRootQueryRetrieveInformationModelFind)
     ae.add_supported_context(StudyRootQueryRetrieveInformationModelMove)
     ae.add_supported_context(StudyRootQueryRetrieveInformationModelGet)
 
+    # Unified Procedure Step SCP
+    for cx in UnifiedProcedurePresentationContexts:
+        ae.add_supported_context(
+            cx.abstract_syntax, ALL_TRANSFER_SYNTAXES, scp_role=True, scu_role=False
+        )
+
+    # Modality Worklist SCP
+    ae.add_supported_context(ModalityWorklistInformationFind)
+
     # Set our handler bindings
     handlers = [
         (evt.EVT_C_ECHO, handle_echo, [args, APP_LOGGER]),
         (evt.EVT_C_FIND, handle_find, [db_path, args, APP_LOGGER]),
         (evt.EVT_C_GET, handle_get, [db_path, args, APP_LOGGER]),
         (evt.EVT_C_MOVE, handle_move, [dests, db_path, args, APP_LOGGER]),
         (evt.EVT_C_STORE, handle_store, [instance_dir, db_path, args, APP_LOGGER]),
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/storescp/storescp.py` & `pynetdicom-2.1.0/pynetdicom/apps/storescp/storescp.py`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/storescu/storescu.py` & `pynetdicom-2.1.0/pynetdicom/apps/storescu/storescu.py`

 * *Files 5% similar despite different names*

```diff
@@ -209,32 +209,32 @@
     """
     good, bad = [], []
     contexts = {}
     for fpath in fpaths:
         path = os.fspath(Path(fpath).resolve())
         try:
             ds = dcmread(path)
-        except Exception as exc:
+        except Exception:
             bad.append(("Bad DICOM file", path))
             continue
 
         try:
             sop_class = ds.SOPClassUID
             tsyntax = ds.file_meta.TransferSyntaxUID
-        except Exception as exc:
+        except Exception:
             bad.append(("Unknown SOP Class or Transfer Syntax UID", path))
             continue
 
         tsyntaxes = contexts.setdefault(sop_class, [])
         if tsyntax not in tsyntaxes:
             tsyntaxes.append(tsyntax)
 
         good.append(path)
 
-    for (reason, path) in bad:
+    for reason, path in bad:
         app_logger.error(f"{reason}: {path}")
 
     return good, contexts
 
 
 def main(args=None):
     """Run the application."""
@@ -303,15 +303,15 @@
     )
     if assoc.is_established:
         ii = 1
         for fpath in lfiles:
             APP_LOGGER.info(f"Sending file: {fpath}")
             try:
                 ds = dcmread(fpath)
-                status = assoc.send_c_store(ds, ii)
+                assoc.send_c_store(ds, ii)
                 ii += 1
             except InvalidDicomError:
                 APP_LOGGER.error(f"Bad DICOM file: {fpath}")
             except Exception as exc:
                 APP_LOGGER.error(f"Store failed: {fpath}")
                 APP_LOGGER.exception(exc)
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/tests/test_common.py` & `pynetdicom-2.1.0/pynetdicom/apps/tests/test_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,15 +609,15 @@
             "LT": ("ExtendedCodeMeaning", "Another long string"),
             "PN": ("PatientName", "CITIZEN^Jan^X"),
             "SH": ("CodeValue", "16 character str"),
             "ST": ("InstitutionAddress", "1024 character string"),
             "TM": ("StudyTime", "120000.123456"),
             "UC": ("LongCodeValue", "So many characters in this one"),
             "UI": ("SOPClassUID", "1.2.3.4.5.6"),
-            "UR": ("CodingSchemeURL", "http://github.com/pydicom/pynetdicom"),
+            "UR": ("CodingSchemeURL", "https://github.com/pydicom/pynetdicom"),
             "UT": ("StrainAdditionalInformation", "Wheeeeeeeeee"),
         }
         for vr, (kw, val) in keywords.items():
             epath = "{}={}".format(kw, val)
             ds = ElementPath(epath).update(Dataset())
             if vr in ["DS", "IS"]:
                 assert getattr(ds, kw).original_string == val
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/tests/test_echoscp.py` & `pynetdicom-2.1.0/pynetdicom/apps/tests/test_echoscp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Unit tests for echoscp.py"""
 
 import logging
 import os
+from pathlib import Path
 import subprocess
 import sys
 import time
 
 import pytest
 
 from pydicom import dcmread
@@ -19,18 +20,18 @@
 from pynetdicom import AE, evt, debug_logger, DEFAULT_TRANSFER_SYNTAXES
 from pynetdicom.sop_class import Verification, CTImageStorage
 
 
 # debug_logger()
 
 
-APP_DIR = os.path.join(os.path.dirname(__file__), "../")
-APP_FILE = os.path.join(APP_DIR, "echoscp", "echoscp.py")
-DATA_DIR = os.path.join(APP_DIR, "../", "tests", "dicom_files")
-DATASET_FILE = os.path.join(DATA_DIR, "CTImageStorage.dcm")
+APP_DIR = Path(__file__).parent.parent
+APP_FILE = APP_DIR / "echoscp" / "echoscp.py"
+DATA_DIR = APP_DIR.parent / "tests" / "dicom_files"
+DATASET_FILE = DATA_DIR / "CTImageStorage.dcm"
 
 
 def start_echoscp(args):
     """Start the echoscp.py app and return the process."""
     pargs = [sys.executable, APP_FILE, "11112"] + [*args]
     return subprocess.Popen(pargs)
 
@@ -40,21 +41,21 @@
     pargs = [sys.executable, "-m", "pynetdicom", "echoscp", "11112"] + [*args]
     return subprocess.Popen(pargs)
 
 
 class EchoSCPBase:
     """Tests for echoscp.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.p = None
         self.func = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
         if self.p:
             self.p.kill()
             self.p.wait(timeout=5)
@@ -297,22 +298,22 @@
         cx = assoc.accepted_contexts[0]
         assert cx.transfer_syntax[0] == ImplicitVRLittleEndian
 
 
 class TestEchoSCP(EchoSCPBase):
     """Tests for echoscp.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.p = None
         self.func = start_echoscp
 
 
 class TestEchoSCPCLI(EchoSCPBase):
     """Tests for echoscp using CLI"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.p = None
         self.func = start_echoscp_cli
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/tests/test_echoscu.py` & `pynetdicom-2.1.0/pynetdicom/apps/tests/test_echoscu.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Unit tests for echoscu.py"""
 
 import logging
 import os
+from pathlib import Path
 import subprocess
 import sys
 import time
 
 import pytest
 
 from pydicom.uid import (
@@ -18,16 +19,16 @@
 from pynetdicom import AE, evt, debug_logger, DEFAULT_TRANSFER_SYNTAXES
 from pynetdicom.sop_class import Verification, CTImageStorage
 
 
 # debug_logger()
 
 
-APP_DIR = os.path.join(os.path.dirname(__file__), "../")
-APP_FILE = os.path.join(APP_DIR, "echoscu", "echoscu.py")
+APP_DIR = Path(__file__).parent.parent
+APP_FILE = APP_DIR / "echoscu" / "echoscu.py"
 
 
 def start_echoscu(args):
     """Start the echoscu.py app and return the process."""
     pargs = [sys.executable, APP_FILE, "localhost", "11112"] + [*args]
     return subprocess.Popen(pargs)
 
@@ -39,20 +40,20 @@
     ]
     return subprocess.Popen(pargs)
 
 
 class EchoSCUBase:
     """Tests for echoscu.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_default(self):
         """Test default settings."""
         events = []
@@ -535,20 +536,20 @@
         assert events[0].event == evt.EVT_C_ECHO
         assert events[1].event == evt.EVT_ABORTED
 
 
 class TestEchoSCU(EchoSCUBase):
     """Tests for echoscu.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = start_echoscu
 
 
 class TestEchoSCUCLI(EchoSCUBase):
     """Tests for echoscu using CLI"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = start_echoscu_cli
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/tests/test_findscu.py` & `pynetdicom-2.1.0/pynetdicom/apps/tests/test_findscu.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,21 +19,23 @@
 from pynetdicom import (
     AE,
     evt,
     debug_logger,
     DEFAULT_TRANSFER_SYNTAXES,
     QueryRetrievePresentationContexts,
     BasicWorklistManagementPresentationContexts,
+    UnifiedProcedurePresentationContexts,
 )
 from pynetdicom.sop_class import (
     Verification,
     PatientRootQueryRetrieveInformationModelFind,
     StudyRootQueryRetrieveInformationModelFind,
     PatientStudyOnlyQueryRetrieveInformationModelFind,
     ModalityWorklistInformationFind,
+    UnifiedProcedureStepPull,
 )
 
 
 # debug_logger()
 
 
 APP_DIR = os.path.join(os.path.dirname(__file__), "../")
@@ -55,20 +57,20 @@
     ]
     return subprocess.Popen(pargs)
 
 
 class FindSCUBase:
     """Tests for findscu.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_default(self):
         """Test default settings."""
         events = []
@@ -85,14 +87,15 @@
         self.ae = ae = AE()
         ae.acse_timeout = 5
         ae.dimse_timeout = 5
         ae.network_timeout = 5
         ae.supported_contexts = (
             QueryRetrievePresentationContexts
             + BasicWorklistManagementPresentationContexts
+            + UnifiedProcedurePresentationContexts
         )
         scp = ae.start_server(("localhost", 11112), block=False, evt_handlers=handlers)
 
         p = self.func(["-k", "PatientName="])
         p.wait()
         assert p.returncode == 0
 
@@ -107,15 +110,15 @@
         assert "ANY-SCP" == requestor.primitive.called_ae_title
         assert [] == requestor.extended_negotiation
         assert (1, 1) == requestor.asynchronous_operations
         assert {} == requestor.sop_class_common_extended
         assert {} == requestor.sop_class_extended
         assert requestor.user_identity == None
         cxs = requestor.primitive.presentation_context_definition_list
-        assert len(cxs) == 13
+        assert len(cxs) == 19
         cxs = {cx.abstract_syntax: cx for cx in cxs}
         assert PatientRootQueryRetrieveInformationModelFind in cxs
         cx = cxs[PatientRootQueryRetrieveInformationModelFind]
         assert cx.transfer_syntax == DEFAULT_TRANSFER_SYNTAXES
 
     def test_no_peer(self, capfd):
         """Test trying to connect to non-existent host."""
@@ -517,14 +520,47 @@
 
         scp.shutdown()
 
         assert events[0].event == evt.EVT_C_FIND
         cx = events[0].context
         assert cx.abstract_syntax == (PatientStudyOnlyQueryRetrieveInformationModelFind)
 
+    def test_flag_ups(self):
+        """Test the -U flag."""
+        events = []
+
+        def handle_find(event):
+            events.append(event)
+            yield 0x0000, None
+
+        handlers = [
+            (evt.EVT_C_FIND, handle_find),
+        ]
+
+        self.ae = ae = AE()
+        ae.acse_timeout = 5
+        ae.dimse_timeout = 5
+        ae.network_timeout = 5
+        ae.supported_contexts = (
+            QueryRetrievePresentationContexts
+            + BasicWorklistManagementPresentationContexts
+            + UnifiedProcedurePresentationContexts
+        )
+        scp = ae.start_server(("localhost", 11112), block=False, evt_handlers=handlers)
+
+        p = self.func(["-U", "-k", "PatientName="])
+        p.wait()
+        assert p.returncode == 0
+
+        scp.shutdown()
+
+        assert events[0].event == evt.EVT_C_FIND
+        cx = events[0].context
+        assert cx.abstract_syntax == UnifiedProcedureStepPull
+
     def test_flag_worklist(self):
         """Test the -W flag."""
         events = []
 
         def handle_find(event):
             events.append(event)
             yield 0x0000, None
@@ -584,20 +620,20 @@
         assert ds.PatientName == ""
         os.remove("rsp000001.dcm")
 
 
 class TestFindSCU(FindSCUBase):
     """Tests for findscu.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = start_findscu
 
 
 class TestFindSCUCLI(FindSCUBase):
     """Tests for findscu.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = start_findscu_scli
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/tests/test_getscu.py` & `pynetdicom-2.1.0/pynetdicom/apps/tests/test_getscu.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,27 +56,27 @@
     ]
     return subprocess.Popen(pargs)
 
 
 class GetSCUBase:
     """Tests for getscu.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = None
 
         self.response = ds = Dataset()
         ds.file_meta = FileMetaDataset()
         ds.file_meta.TransferSyntaxUID = ImplicitVRLittleEndian
         ds.SOPClassUID = CTImageStorage
         ds.SOPInstanceUID = "1.2.3.4"
         ds.PatientName = "Citizen^Jan"
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_default(self):
         """Test default settings."""
         events = []
@@ -565,15 +565,15 @@
 
         assert "CT.1.2.3.4" not in os.listdir()
 
 
 class TestGetSCU(GetSCUBase):
     """Tests for getscu.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = start_getscu
 
         self.response = ds = Dataset()
         ds.file_meta = FileMetaDataset()
         ds.file_meta.TransferSyntaxUID = ImplicitVRLittleEndian
@@ -581,15 +581,15 @@
         ds.SOPInstanceUID = "1.2.3.4"
         ds.PatientName = "Citizen^Jan"
 
 
 class TestGetSCUCLI(GetSCUBase):
     """Tests for getscu using CLI"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = start_getscu_cli
 
         self.response = ds = Dataset()
         ds.file_meta = FileMetaDataset()
         ds.file_meta.TransferSyntaxUID = ImplicitVRLittleEndian
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/tests/test_movescu.py` & `pynetdicom-2.1.0/pynetdicom/apps/tests/test_movescu.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,27 +57,27 @@
     ]
     return subprocess.Popen(pargs)
 
 
 class MoveSCUBase:
     """Tests for movescu.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = None
 
         self.response = ds = Dataset()
         ds.file_meta = FileMetaDataset()
         ds.file_meta.TransferSyntaxUID = ImplicitVRLittleEndian
         ds.SOPClassUID = CTImageStorage
         ds.SOPInstanceUID = "1.2.3.4"
         ds.PatientName = "Citizen^Jan"
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_default(self):
         """Test default settings."""
         events = []
@@ -126,15 +126,15 @@
         assert 0 == len(requestor.extended_negotiation)
         assert (1, 1) == requestor.asynchronous_operations
         assert {} == requestor.sop_class_common_extended
         assert {} == requestor.sop_class_extended
         assert requestor.role_selection == {}
         assert requestor.user_identity == None
         cxs = requestor.primitive.presentation_context_definition_list
-        assert len(cxs) == 12
+        assert len(cxs) == 13
         cxs = {cx.abstract_syntax: cx for cx in cxs}
         assert PatientRootQueryRetrieveInformationModelMove in cxs
         cx = cxs[PatientRootQueryRetrieveInformationModelMove]
         assert cx.transfer_syntax == DEFAULT_TRANSFER_SYNTAXES
 
     def test_no_peer(self, capfd):
         """Test trying to connect to non-existent host."""
@@ -752,15 +752,15 @@
 
         assert "CT.1.2.3.4" not in os.listdir()
 
 
 class TestMoveSCU(MoveSCUBase):
     """Tests for movescu.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = start_movescu
 
         self.response = ds = Dataset()
         ds.file_meta = FileMetaDataset()
         ds.file_meta.TransferSyntaxUID = ImplicitVRLittleEndian
@@ -768,15 +768,15 @@
         ds.SOPInstanceUID = "1.2.3.4"
         ds.PatientName = "Citizen^Jan"
 
 
 class TestMoveSCUCLI(MoveSCUBase):
     """Tests for movescu.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = start_movescu_cli
 
         self.response = ds = Dataset()
         ds.file_meta = FileMetaDataset()
         ds.file_meta.TransferSyntaxUID = ImplicitVRLittleEndian
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/tests/test_qrscp_db.py` & `pynetdicom-2.1.0/pynetdicom/apps/tests/test_qrscp_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 """Unit tests for the QRSCP app's database functions."""
 
 import os
+from pathlib import Path
 import sys
 import tempfile
 
 import pytest
 
 try:
     from sqlalchemy import create_engine
     from sqlalchemy.schema import MetaData
-    from sqlalchemy.exc import IntegrityError
+    from sqlalchemy.exc import IntegrityError, SAWarning
     from sqlalchemy.orm import sessionmaker
 
     HAVE_SQLALCHEMY = True
 except ImportError:
     HAVE_SQLALCHEMY = False
 
-from pydicom import dcmread, config as PYD_CONFIG
+from pydicom import dcmread
 import pydicom.config
 from pydicom.dataset import Dataset
 from pydicom.tag import Tag
 
 from pynetdicom.sop_class import (
     PatientRootQueryRetrieveInformationModelFind,
     StudyRootQueryRetrieveInformationModelFind,
 )
 
 if HAVE_SQLALCHEMY:
     from pynetdicom.apps.qrscp import db
 
 
-if hasattr(PYD_CONFIG, "settings"):
-    PYD_CONFIG.settings.reading_validation_mode = 0
-
-
-TEST_DIR = os.path.dirname(__file__)
-DATA_DIR = os.path.join(TEST_DIR, "../", "../", "tests", "dicom_files")
+TEST_DIR = Path(__file__).parent
+DATA_DIR = TEST_DIR.parent.parent / "tests" / "dicom_files"
 DATASETS = {
     "CTImageStorage.dcm": {
         "patient_id": "1CT1",
         "patient_name": "CompressedSamples^CT1",
         "study_instance_uid": "1.3.6.1.4.1.5962.1.2.1.20040119072730.12322",
         "study_date": "20040119",
         "study_time": "072730",
@@ -116,26 +113,33 @@
         "instance_number": None,
         "transfer_syntax_uid": "1.2.840.10008.1.2.1.99",
         "sop_class_uid": "1.2.840.10008.5.1.4.1.1.7",
     },
 }
 
 
+try:
+    pydicom.config.settings.writing_validation_mode = 0
+    pydicom.config.settings.reading_validation_mode = 0
+except AttributeError:
+    pass
+
+
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestConnect:
     """Tests for db.connect()."""
 
     def test_create_new(self):
         """Test connecting to the instance database if it doesn't exist."""
         db_file = tempfile.NamedTemporaryFile()
         db_location = f"sqlite:///{db_file.name}"
         engine = db.create(db_location)
 
         # Check exists with tables
-        meta = MetaData(bind=engine)
+        meta = MetaData()
         meta.reflect(bind=engine)
         assert "patient" in meta.tables
         assert "study" in meta.tables
         assert "series" in meta.tables
         assert "image" in meta.tables
         assert "instance" in meta.tables
 
@@ -143,28 +147,28 @@
         """Test connecting to the instance database if it exists."""
         db_file = tempfile.NamedTemporaryFile()
         db_location = "sqlite:///{}".format(db_file.name)
         db.create(db_location)
         # Test creating if already exists
         engine = db.create(db_location)
 
-        meta = MetaData(bind=engine)
+        meta = MetaData()
         meta.reflect(bind=engine)
         assert "patient" in meta.tables
         assert "study" in meta.tables
         assert "series" in meta.tables
         assert "image" in meta.tables
         assert "instance" in meta.tables
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestAddInstance:
     """Tests for db.add_instance()."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         engine = db.create("sqlite:///:memory:")
 
         pydicom.config.use_none_as_empty_text_VR_value = True
 
         ds = Dataset()
         ds.PatientID = "1234"
@@ -173,28 +177,26 @@
         ds.SOPInstanceUID = "1.2.3.4"
         self.minimal = ds
 
         self.session = sessionmaker(bind=engine)()
 
     def test_add_instance(self):
         """Test adding to the instance database."""
-        fpath = os.path.join(DATA_DIR, "CTImageStorage.dcm")
-        ds = dcmread(fpath)
+        ds = dcmread(os.fspath(DATA_DIR / "CTImageStorage.dcm"))
         db.add_instance(ds, self.session)
 
         obj = self.session.query(db.Instance).all()
         assert 1 == len(obj)
         for kk, vv in DATASETS["CTImageStorage.dcm"].items():
             assert vv == getattr(obj[0], kk)
 
     def test_add_multiple_instances(self):
         """Test adding multiple data to the instance database."""
         for fname in DATASETS:
-            fpath = os.path.join(DATA_DIR, fname)
-            ds = dcmread(fpath)
+            ds = dcmread(os.fspath(DATA_DIR / fname))
             db.add_instance(ds, self.session)
 
         obj = self.session.query(db.Instance).all()
         assert 5 == len(obj)
         obj = self.session.query(db.Instance, db.Instance.patient_name).all()
         names = [val[1] for val in obj]
         assert "CompressedSamples^CT1" in names
@@ -225,16 +227,16 @@
         ]
         for attr in rest:
             assert getattr(obj[0], attr) is None
 
     def test_bad_instance(self):
         """Test that instances with bad data aren't added."""
         keywords = [
-            ("PatientID", 16),
-            ("PatientName", 64),
+            ("PatientID", 64),
+            ("PatientName", 400),
             ("StudyInstanceUID", 64),
             ("StudyDate", 8),
             ("StudyTime", 14),
             ("AccessionNumber", 16),
             ("StudyID", 16),
             ("SeriesInstanceUID", 64),
             ("Modality", 16),
@@ -249,15 +251,15 @@
                 db.add_instance(ds, self.session)
 
         assert not self.session.query(db.Instance).all()
 
     def test_bad_instance_none(self):
         """Test that instances with bad data aren't added."""
         keywords = [
-            ("PatientID", 16),
+            ("PatientID", 64),
             ("PatientName", 64),
             ("StudyInstanceUID", 64),
             ("StudyDate", 8),
             ("StudyTime", 14),
             ("AccessionNumber", 16),
             ("StudyID", 16),
             ("SeriesInstanceUID", 64),
@@ -268,15 +270,17 @@
         ]
         ds = Dataset()
         ds.PatientID = None
         ds.StudyInstanceUID = None
         ds.SeriesInstanceUID = None
         ds.SOPInstanceUID = None
         with pytest.raises(IntegrityError):
-            db.add_instance(ds, self.session)
+            msg = r"Column 'instance.sop_instance_uid' is marked as a"
+            with pytest.warns(SAWarning, match=msg):
+                db.add_instance(ds, self.session)
 
         self.session.rollback()
 
         assert not self.session.query(db.Instance).all()
 
     def test_instance_exists(self):
         """Test that adding already existing instance updates it."""
@@ -294,15 +298,15 @@
         assert "CT" == result[0].modality
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestRemoveInstance:
     """Tests for db.remove_instance()."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         engine = db.create("sqlite:///:memory:")
 
         pydicom.config.use_none_as_empty_text_VR_value = True
 
         self.session = sessionmaker(bind=engine)()
         ds = Dataset()
@@ -341,48 +345,46 @@
         assert self.session.query(db.Instance).all()
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestClear:
     """Tests for db.clear()."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         engine = db.create("sqlite:///:memory:")
 
         pydicom.config.use_none_as_empty_text_VR_value = True
 
         self.session = sessionmaker(bind=engine)()
         for fname in DATASETS:
-            fpath = os.path.join(DATA_DIR, fname)
-            ds = dcmread(fpath)
+            ds = dcmread(os.fspath(DATA_DIR / fname))
             db.add_instance(ds, self.session)
 
     def test_clear(self):
         """Test removing if exists in database."""
         assert 5 == len(self.session.query(db.Instance).all())
 
         db.clear(self.session)
         assert not self.session.query(db.Instance).all()
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestSearch:
     """Tests for db.search()."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         engine = db.create("sqlite:///:memory:")
         pydicom.config.use_none_as_empty_text_VR_value = True
 
         self.session = sessionmaker(bind=engine)()
 
         for fname in DATASETS:
-            fpath = os.path.join(DATA_DIR, fname)
-            ds = dcmread(fpath)
+            ds = dcmread(os.fspath(DATA_DIR / fname))
             db.add_instance(ds, self.session)
 
     def test_search(self):
         """Test simple search."""
         pass
 
     def test_search_range_both(self):
@@ -662,23 +664,22 @@
 ]
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestSearchFind:
     """Tests for running C-FIND queries against the database."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         engine = db.create("sqlite:///:memory:")
         pydicom.config.use_none_as_empty_text_VR_value = True
 
         self.session = sessionmaker(bind=engine)()
         for fname in DATASETS:
-            fpath = os.path.join(DATA_DIR, fname)
-            ds = dcmread(fpath)
+            ds = dcmread(DATA_DIR / fname)
             db.add_instance(ds, self.session)
 
     def test_no_attributes(self):
         """Test searching with no attributes."""
         query = Dataset()
         query.QueryRetrieveLevel = "PATIENT"
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/tests/test_qrscp_echo.py` & `pynetdicom-2.1.0/pynetdicom/apps/tests/test_qrscp_echo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Unit tests for qrscp.py verification service."""
 
 import logging
 import os
+from pathlib import Path
 import subprocess
 import sys
 import tempfile
 import time
 
 import pytest
 
@@ -27,46 +28,46 @@
 from pynetdicom import AE, evt, debug_logger, DEFAULT_TRANSFER_SYNTAXES
 from pynetdicom.sop_class import Verification, CTImageStorage
 
 
 # debug_logger()
 
 
-APP_DIR = os.path.join(os.path.dirname(__file__), "../")
-APP_FILE = os.path.join(APP_DIR, "qrscp", "qrscp.py")
-DATA_DIR = os.path.join(APP_DIR, "../", "tests", "dicom_files")
-DATASET_FILE = os.path.join(DATA_DIR, "CTImageStorage.dcm")
+APP_DIR = Path(__file__).parent.parent
+APP_FILE = APP_DIR / "qrscp" / "qrscp.py"
 
 
 def start_qrscp(args):
     """Start the qrscp.py app and return the process."""
-    pargs = [sys.executable, APP_FILE] + [*args]
+    pargs = [sys.executable, os.fspath(APP_FILE)] + [*args]
     return subprocess.Popen(pargs)
 
 
 def start_qrscp_cli(args):
     """Start the qrscp app using CLI and return the process."""
     pargs = [sys.executable, "-m", "pynetdicom", "qrscp"] + [*args]
     return subprocess.Popen(pargs)
 
 
 class EchoSCPBase:
     """Tests for echoscp.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.p = None
         self.func = None
 
         self.tfile = tempfile.NamedTemporaryFile()
         self.db_location = self.tfile.name
         self.instance_location = tempfile.TemporaryDirectory()
 
-    def teardown(self):
+        self.startup = 1.0
+
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
         if self.p:
             self.p.kill()
             self.p.wait(timeout=5)
@@ -83,15 +84,15 @@
             [
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
             ]
         )
-        time.sleep(1)
+        time.sleep(self.startup)
 
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
         assoc.release()
 
         p.terminate()
         p.wait()
@@ -133,15 +134,15 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-q",
             ]
         )
-        time.sleep(0.5)
+        time.sleep(self.startup)
 
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
         status = assoc.send_c_echo()
         assert status.Status == 0x0000
         assoc.release()
 
@@ -166,15 +167,15 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-v",
             ]
         )
-        time.sleep(0.5)
+        time.sleep(self.startup)
 
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
         status = assoc.send_c_echo()
         assert status.Status == 0x0000
         assoc.release()
 
@@ -199,15 +200,15 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(0.5)
+        time.sleep(self.startup)
 
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
         status = assoc.send_c_echo()
         assert status.Status == 0x0000
         assoc.release()
 
@@ -235,23 +236,23 @@
         assert p.returncode != 0
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestEchoSCP(EchoSCPBase):
     """Tests for echoscp.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
-        super().setup()
+        super().setup_method()
 
         self.func = start_qrscp
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestEchoSCPCLI(EchoSCPBase):
     """Tests for echoscp using CLI"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
-        super().setup()
+        super().setup_method()
 
         self.func = start_qrscp_cli
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/tests/test_qrscp_find.py` & `pynetdicom-2.1.0/pynetdicom/apps/tests/test_qrscp_find.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     ]
     subprocess.Popen(pargs)
 
 
 class FindSCPBase:
     """Tests for qrscp.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.p = None
         self.func = None
 
         self.tfile = tempfile.NamedTemporaryFile()
         self.db_location = self.tfile.name
@@ -96,15 +96,17 @@
         self.q_image = ds = Dataset()
         ds.QueryRetrieveLevel = "IMAGE"
         ds.PatientID = None
         ds.StudyInstanceUID = None
         ds.SeriesInstanceUID = None
         ds.SOPInstanceUID = None
 
-    def teardown(self):
+        self.startup = 1.0
+
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
         if self.p:
             self.p.kill()
             self.p.wait(timeout=5)
@@ -116,17 +118,17 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(1)
+        time.sleep(self.startup)
         _send_datasets()
-        time.sleep(1)
+        time.sleep(self.startup)
 
         self.ae = ae = AE()
         ae.acse_timeout = 5
         ae.dimse_timeout = 5
         ae.network_timeout = 5
         model = PatientRootQueryRetrieveInformationModelFind
         ae.add_requested_context(model)
@@ -165,17 +167,17 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(0.5)
+        time.sleep(self.startup)
         _send_datasets()
-        time.sleep(1)
+        time.sleep(self.startup)
 
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
         self.q_patient.StudyInstanceUID = None
         responses = assoc.send_c_find(self.q_patient, model)
         status, ds = next(responses)
         assert status.Status == 0xA900
@@ -201,17 +203,17 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(0.5)
+        time.sleep(self.startup)
         _send_datasets()
-        time.sleep(1)
+        time.sleep(self.startup)
 
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
         self.q_patient.PatientName = None
         responses = assoc.send_c_find(self.q_patient, model)
         for ii in range(5):
             status, ds = next(responses)
@@ -246,17 +248,17 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(0.5)
+        time.sleep(self.startup)
         _send_datasets()
-        time.sleep(1)
+        time.sleep(self.startup)
 
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
         responses = assoc.send_c_find(self.q_study, model)
         for ii in range(5):
             status, ds = next(responses)
             assert status.Status == 0xFF00
@@ -290,17 +292,17 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(0.5)
+        time.sleep(self.startup)
         _send_datasets()
-        time.sleep(1)
+        time.sleep(self.startup)
 
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
         self.q_study.StudyDate = None
         responses = assoc.send_c_find(self.q_study, model)
         for ii in range(5):
             status, ds = next(responses)
@@ -336,17 +338,17 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(0.5)
+        time.sleep(self.startup)
         _send_datasets()
-        time.sleep(1)
+        time.sleep(self.startup)
 
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
         responses = assoc.send_c_find(self.q_series, model)
         for ii in range(5):
             status, ds = next(responses)
             assert status.Status == 0xFF00
@@ -381,17 +383,17 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(0.5)
+        time.sleep(self.startup)
         _send_datasets()
-        time.sleep(1)
+        time.sleep(self.startup)
 
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
         self.q_series.Modality = None
         responses = assoc.send_c_find(self.q_series, model)
         for ii in range(5):
             status, ds = next(responses)
@@ -428,17 +430,17 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(0.5)
+        time.sleep(self.startup)
         _send_datasets()
-        time.sleep(1)
+        time.sleep(self.startup)
 
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
         responses = assoc.send_c_find(self.q_image, model)
         for ii in range(5):
             status, ds = next(responses)
             assert status.Status == 0xFF00
@@ -474,17 +476,17 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(0.5)
+        time.sleep(self.startup)
         _send_datasets()
-        time.sleep(1)
+        time.sleep(self.startup)
 
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
         self.q_image.InstanceNumber = None
         responses = assoc.send_c_find(self.q_image, model)
         for ii in range(5):
             status, ds = next(responses)
@@ -522,17 +524,17 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(0.5)
+        time.sleep(self.startup)
         _send_datasets()
-        time.sleep(1)
+        time.sleep(self.startup)
 
         ds = Dataset()
         ds.QueryRetrieveLevel = "PATIENT"
         ds.PatientID = "4MR1"
 
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
@@ -569,17 +571,17 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(0.5)
+        time.sleep(self.startup)
         _send_datasets()
-        time.sleep(1)
+        time.sleep(self.startup)
 
         ds = Dataset()
         ds.QueryRetrieveLevel = "STUDY"
         ds.PatientID = "4MR1"
 
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
@@ -603,25 +605,25 @@
         p.wait()
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestFindSCP(FindSCPBase):
     """Tests for qrscp.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
-        super().setup()
+        super().setup_method()
         self.ae = None
         self.p = None
         self.func = start_qrscp
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestFindSCPCLI(FindSCPBase):
     """Tests for qrscp using CLI"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
-        super().setup()
+        super().setup_method()
         self.ae = None
         self.p = None
         self.func = start_qrscp_cli
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/tests/test_qrscp_get.py` & `pynetdicom-2.1.0/pynetdicom/apps/tests/test_qrscp_get.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,25 +64,27 @@
     ]
     subprocess.Popen(pargs)
 
 
 class GetSCPBase:
     """Tests for qrscp.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.p = None
         self.func = None
 
         self.tfile = tempfile.NamedTemporaryFile()
         self.db_location = self.tfile.name
         self.instance_location = tempfile.TemporaryDirectory()
 
-    def teardown(self):
+        self.startup = 1.0
+
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
         if self.p:
             self.p.kill()
             self.p.wait(timeout=5)
@@ -94,17 +96,17 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(1)
+        time.sleep(self.startup)
         _send_datasets()
-        time.sleep(1)
+        time.sleep(self.startup)
 
         query = Dataset()
         query.QueryRetrieveLevel = "PATIENT"
         query.PatientID = "1CT1"
 
         datasets = []
 
@@ -147,25 +149,25 @@
         assert "CompressedSamples^CT1" == datasets[0].PatientName
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestGetSCP(GetSCPBase):
     """Tests for qrscp.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
-        super().setup()
+        super().setup_method()
         self.ae = None
         self.p = None
         self.func = start_qrscp
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestGetSCPCLI(GetSCPBase):
     """Tests for qrscp using CLI"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
-        super().setup()
+        super().setup_method()
         self.ae = None
         self.p = None
         self.func = start_qrscp_cli
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/tests/test_qrscp_move.py` & `pynetdicom-2.1.0/pynetdicom/apps/tests/test_qrscp_move.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,25 +64,27 @@
     ]
     subprocess.Popen(pargs)
 
 
 class MoveSCPBase:
     """Tests for qrscp.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.p = None
         self.func = None
 
         self.tfile = tempfile.NamedTemporaryFile()
         self.db_location = self.tfile.name
         self.instance_location = tempfile.TemporaryDirectory()
 
-    def teardown(self):
+        self.startup = 1.0
+
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
         if self.p:
             self.p.kill()
             self.p.wait(timeout=5)
@@ -94,17 +96,17 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(1)
+        time.sleep(self.startup)
         _send_datasets()
-        time.sleep(1)
+        time.sleep(self.startup)
 
         query = Dataset()
         query.QueryRetrieveLevel = "PATIENT"
         query.PatientID = "1CT1"
 
         datasets = []
 
@@ -149,25 +151,25 @@
         assert "CompressedSamples^CT1" == datasets[0].PatientName
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestMoveSCP(MoveSCPBase):
     """Tests for qrscp.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
-        super().setup()
+        super().setup_method()
         self.ae = None
         self.p = None
         self.func = start_qrscp
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestMoveSCPCLI(MoveSCPBase):
     """Tests for qrscp using CLI"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
-        super().setup()
+        super().setup_method()
         self.ae = None
         self.p = None
         self.func = start_qrscp_cli
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/tests/test_qrscp_store.py` & `pynetdicom-2.1.0/pynetdicom/apps/tests/test_qrscp_store.py`

 * *Files 13% similar despite different names*

```diff
@@ -61,25 +61,27 @@
     ]
     subprocess.Popen(pargs)
 
 
 class StoreSCPBase:
     """Tests for qrscp.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.p = None
         self.func = None
 
         self.tfile = tempfile.NamedTemporaryFile()
         self.db_location = self.tfile.name
         self.instance_location = tempfile.TemporaryDirectory()
 
-    def teardown(self):
+        self.startup = 1.0
+
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
         if self.p:
             self.p.kill()
             self.p.wait(timeout=5)
@@ -91,36 +93,36 @@
                 "--database-location",
                 self.db_location,
                 "--instance-location",
                 self.instance_location.name,
                 "-d",
             ]
         )
-        time.sleep(1)
+        time.sleep(self.startup)
         _send_datasets()
-        time.sleep(1)
+        time.sleep(self.startup)
 
         assert 5 == len(os.listdir(self.instance_location.name))
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestStoreSCP(StoreSCPBase):
     """Tests for qrscp.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
-        super().setup()
+        super().setup_method()
         self.ae = None
         self.p = None
         self.func = start_qrscp
 
 
 @pytest.mark.skipif(not HAVE_SQLALCHEMY, reason="Requires sqlalchemy")
 class TestStoreSCPCLI(StoreSCPBase):
     """Tests for qrscp using CLI"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
-        super().setup()
+        super().setup_method()
         self.ae = None
         self.p = None
         self.func = start_qrscp_cli
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/tests/test_storescp.py` & `pynetdicom-2.1.0/pynetdicom/apps/tests/test_storescp.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,21 +48,21 @@
     pargs = [sys.executable, "-m", "pynetdicom", "storescp", "11112"] + [*args]
     return subprocess.Popen(pargs)
 
 
 class StoreSCPBase:
     """Tests for storescp.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.p = None
         self.func = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if TEST_DIR.exists():
             shutil.rmtree(os.fspath(TEST_DIR))
 
         if self.ae:
             self.ae.shutdown()
 
@@ -390,22 +390,22 @@
         shutil.rmtree(os.fspath(TEST_DIR))
         assert not TEST_DIR.exists()
 
 
 class TestStoreSCP(StoreSCPBase):
     """Tests for storescp.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.p = None
         self.func = start_storescp
 
 
 class TestStoreSCPCLI(StoreSCPBase):
     """Tests for storescp using CLI"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.p = None
         self.func = start_storescp_cli
```

### Comparing `pynetdicom-2.0.2/pynetdicom/apps/tests/test_storescu.py` & `pynetdicom-2.1.0/pynetdicom/apps/tests/test_storescu.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,20 +51,20 @@
     ]
     return subprocess.Popen(pargs)
 
 
 class StoreSCUBase:
     """Tests for storescu.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_default(self):
         """Test default settings."""
         events = []
@@ -115,15 +115,14 @@
         ]
 
     def test_no_peer(self, capfd):
         """Test trying to connect to non-existent host."""
         p = self.func([DATASET_FILE])
         p.wait()
         assert p.returncode == 1
-
         out, err = capfd.readouterr()
         assert "Association request failed: unable to connect to remote" in err
         assert "TCP Initialisation Error" in err
 
     def test_flag_version(self, capfd):
         """Test --version flag."""
         p = self.func([DATASET_FILE, "--version"])
@@ -562,32 +561,32 @@
         ae.acse_timeout = 5
         ae.dimse_timeout = 5
         ae.network_timeout = 5
         for cx in AllStoragePresentationContexts:
             ae.add_supported_context(cx.abstract_syntax, ALL_TRANSFER_SYNTAXES)
         scp = ae.start_server(("localhost", 11112), block=False, evt_handlers=handlers)
 
-        p = self.func([LIB_DIR, "--recurse", "-cx"])
+        p = self.func([DATA_DIR, "--recurse", "-cx"])
         p.wait()
         assert p.returncode == 0
 
         scp.shutdown()
 
         assert len(events) == 6
 
 
 class TestStoreSCU(StoreSCUBase):
     """Tests for storescu.py"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = start_storescu
 
 
 class TestStoreSCUCLI(StoreSCUBase):
     """Tests for storescu using CLI"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
         self.func = start_storescu_cli
```

### Comparing `pynetdicom-2.0.2/pynetdicom/association.py` & `pynetdicom-2.1.0/pynetdicom/association.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,31 +3,26 @@
 from io import BytesIO
 import logging
 import os
 from pathlib import Path
 import threading
 import time
 from typing import (
-    Union,
-    Optional,
-    List,
     Callable,
     Any,
-    Dict,
     Iterator,
-    Tuple,
     TYPE_CHECKING,
     cast,
 )
 import warnings
 
 from pydicom import dcmread
 from pydicom.dataset import Dataset
 from pydicom.tag import BaseTag
-from pydicom.uid import UID
+from pydicom.uid import UID, ImplicitVRLittleEndian, ExplicitVRBigEndian
 
 # pylint: disable=no-name-in-module
 from pynetdicom.acse import ACSE
 from pynetdicom import _config, evt
 from pynetdicom.dimse import DIMSEServiceProvider
 from pynetdicom.dimse_primitives import (
     C_ECHO,
@@ -73,32 +68,37 @@
     SCP_SCU_RoleSelectionNegotiation,
     A_ASSOCIATE,
     _UI,
     _UITypes,
 )
 from pynetdicom.presentation import PresentationContext
 from pynetdicom.sop_class import (  # type: ignore
+    RepositoryQuery,
     uid_to_service_class,
-    Verification,
     UnifiedProcedureStepPull,
     UnifiedProcedureStepPush,
-    UnifiedProcedureStepWatch,
     UnifiedProcedureStepEvent,
     UnifiedProcedureStepQuery,
+    UnifiedProcedureStepWatch,
+    Verification,
 )
 from pynetdicom.status import code_to_category, STORAGE_SERVICE_CLASS_STATUS
 from pynetdicom.utils import make_target, set_timer_resolution, set_ae, decode_bytes
 
 if TYPE_CHECKING:  # pragma: no cover
     from pynetdicom.ae import ApplicationEntity
     from pynetdicom.transport import AssociationServer, AssociationSocket
 
 
 # pylint: enable=no-name-in-module
-LOGGER = logging.getLogger("pynetdicom.assoc")
+LOGGER = logging.getLogger(__name__)
+HandlerType = dict[
+    evt.EventType,
+    (list[tuple[Callable, None | list[Any]]] | tuple[Callable, None | list[Any]]),
+]
 
 
 class Association(threading.Thread):
     """Manage an Association with a peer AE.
 
     Attributes
     ----------
@@ -141,15 +141,15 @@
             Must be ``'requestor'`` or ``'acceptor'``.
         """
         self._ae: "ApplicationEntity" = ae
         self.mode: str = mode
 
         # If acceptor this is the parent AssociationServer, used to identify
         #   the thread when updating bound event-handlers
-        self._server: Optional["AssociationServer"] = None
+        self._server: None | "AssociationServer" = None
 
         # Represents the association requestor and acceptor users
         self.requestor: ServiceUser = ServiceUser(self, MODE_REQUESTOR)
         self.acceptor: ServiceUser = ServiceUser(self, MODE_ACCEPTOR)
 
         # Status attributes
         self.is_established: bool = False
@@ -157,39 +157,33 @@
         self.is_aborted: bool = False
         self.is_released: bool = False
 
         # Track whether we've sent an abort or not for the abort() method
         self._sent_abort: bool = False
 
         # Accepted and rejected presentation contexts
-        self._accepted_cx: Dict[int, PresentationContext] = {}
-        self._rejected_cx: List[PresentationContext] = []
+        self._accepted_cx: dict[int, PresentationContext] = {}
+        self._rejected_cx: list[PresentationContext] = []
 
         # Service providers
         self.acse: ACSE = ACSE(self)
         self.dul: DULServiceProvider = DULServiceProvider(self)
         self.dimse: DIMSEServiceProvider = DIMSEServiceProvider(self)
 
         # Timeouts (in seconds), needs to be set after DUL init
-        self.acse_timeout: Optional[float] = self.ae.acse_timeout
-        self.connection_timeout: Optional[float] = self.ae.connection_timeout
-        self.dimse_timeout: Optional[float] = self.ae.dimse_timeout
-        self.network_timeout: Optional[float] = self.ae.network_timeout
+        self.acse_timeout: float | None = self.ae.acse_timeout
+        self.connection_timeout: float | None = self.ae.connection_timeout
+        self.dimse_timeout: float | None = self.ae.dimse_timeout
+        self.network_timeout: float | None = self.ae.network_timeout
 
         # Allow customising the response to a network timeout
         self.network_timeout_response = "A-ABORT"
 
         # Event handlers
-        self._handlers: Dict[
-            evt.EventType,
-            Union[
-                List[Tuple[Callable, Optional[List[Any]]]],
-                Tuple[Callable, Optional[List[Any]]],
-            ],
-        ] = {}
+        self._handlers: HandlerType = {}
         self._bind_defaults()
 
         # Kills the thread loop in run()
         self._kill: bool = False
         # Flag for whether or not the DUL thread has been started
         self._started_dul: bool = False
         # Used to pause the association reactor until the DUL is ready
@@ -197,15 +191,15 @@
         # Used to pause the association reactor while a service is being used
         self._reactor_checkpoint: threading.Event = threading.Event()
         self._reactor_checkpoint.set()
         # Used to ensure the reactor is paused before DIMSE messaging
         self._is_paused: bool = False
 
         # Windows timer resolution
-        self._timer_resolution: Optional[float] = _config.WINDOWS_TIMER_RESOLUTION
+        self._timer_resolution: float | None = _config.WINDOWS_TIMER_RESOLUTION
 
         # Thread setup
         threading.Thread.__init__(self, target=make_target(self.run_reactor))
         self.daemon: bool = True
 
     def abort(self) -> None:
         """Abort the :class:`Association` by sending an A-ABORT to the remote
@@ -227,39 +221,39 @@
             evt.trigger(self, evt.EVT_ABORTED, {})
             self.kill()
 
         # Add short delay to ensure everything shuts down
         time.sleep(0.1)
 
     @property
-    def accepted_contexts(self) -> List[PresentationContext]:
+    def accepted_contexts(self) -> list[PresentationContext]:
         """Return a :class:`list` of accepted
         :class:`~pynetdicom.presentation.PresentationContext` items."""
         # Accepted contexts are stored internally as {context ID : context}
         return sorted(self._accepted_cx.values(), key=lambda x: cast(int, x.context_id))
 
     @property
-    def acse_timeout(self) -> Optional[float]:
+    def acse_timeout(self) -> float | None:
         """The ACSE timeout (in seconds)."""
         return self._acse_timeout
 
     @acse_timeout.setter
-    def acse_timeout(self, value: Optional[float]) -> None:
+    def acse_timeout(self, value: float | None) -> None:
         """Set the ACSE timeout using numeric or ``None``."""
         with self.lock:
             self.dul.artim_timer.timeout = value
             self._acse_timeout = value
 
     @property
     def ae(self) -> "ApplicationEntity":
         """Return the parent :class:`~pynetdicom.ae.ApplicationEntity`."""
         return self._ae
 
     def bind(
-        self, event: evt.EventType, handler: Callable, args: Optional[List[Any]] = None
+        self, event: evt.EventType, handler: Callable, args: None | list[Any] = None
     ) -> None:
         """Bind a callable `handler` to an `event`.
 
         .. versionadded:: 1.3
 
         .. versionchanged:: 1.5
 
@@ -325,25 +319,25 @@
         else:
             LOGGER.error(f"Received an invalid {msg_type} response from the peer")
             self.abort()
 
         return status
 
     @property
-    def dimse_timeout(self) -> Union[int, float, None]:
+    def dimse_timeout(self) -> int | float | None:
         """The DIMSE timeout (in seconds)."""
         return self._dimse_timeout
 
     @dimse_timeout.setter
-    def dimse_timeout(self, value: Union[int, float, None]) -> None:
+    def dimse_timeout(self, value: int | float | None) -> None:
         """Set the DIMSE timeout using numeric or ``None``."""
         with self.lock:
             self._dimse_timeout = value
 
-    def get_events(self) -> List[evt.EventType]:
+    def get_events(self) -> list[evt.EventType]:
         """Return a :class:`list` of currently bound events.
 
         .. versionadded:: 1.3
         """
         return sorted(self._handlers.keys(), key=lambda x: x.name)
 
     def get_handlers(self, event: evt.EventType) -> evt.HandlerArgType:
@@ -373,18 +367,18 @@
         if event not in self._handlers:
             return []
 
         return self._handlers[event]
 
     def _get_valid_context(
         self,
-        ab_syntax: Union[str, UID],
-        tr_syntax: Union[str, UID],
-        role: Optional[str] = None,
-        context_id: Optional[int] = None,
+        ab_syntax: str | UID,
+        tr_syntax: str | UID,
+        role: str | None = None,
+        context_id: int | None = None,
         allow_conversion: bool = True,
     ) -> PresentationContext:
         """Return a valid presentation context matching the parameters.
 
         .. versionchanged:: 1.5
 
             Changed to prefer an exact matching context over a convertible one
@@ -525,15 +519,15 @@
         self._kill = True
         self.is_established = False
         self._is_paused = True
         while self.dul.is_alive() and not self.dul.stop_dul():
             time.sleep(0.01)
 
     @property
-    def local(self) -> Dict[str, Any]:
+    def local(self) -> dict[str, Any]:
         """Return a :class:`dict` with information about the local AE."""
         if self.is_acceptor:
             return self.acceptor.info
 
         return self.requestor.info
 
     @property
@@ -567,27 +561,27 @@
                 "or 'acceptor'"
             )
 
         # pylint: disable=attribute-defined-outside-init
         self._mode = mode
 
     @property
-    def network_timeout(self) -> Union[int, float, None]:
+    def network_timeout(self) -> int | float | None:
         """The network timeout (in seconds)."""
         return self._network_timeout
 
     @network_timeout.setter
-    def network_timeout(self, value: Union[int, float, None]) -> None:
+    def network_timeout(self, value: int | float | None) -> None:
         """Set the network timeout using numeric or ``None``."""
         with self.lock:
             self.dul._idle_timer.timeout = value
             self._network_timeout = value
 
     @property
-    def rejected_contexts(self) -> List[PresentationContext]:
+    def rejected_contexts(self) -> list[PresentationContext]:
         """Return a :class:`list` of rejected
         :class:`~pynetdicom.presentation.PresentationContext`.
         """
         return self._rejected_cx
 
     def release(self) -> None:
         """Initiate association release by send an A-RELEASE request."""
@@ -599,15 +593,15 @@
                 time.sleep(0.0001)
             LOGGER.info("Releasing Association")
             self.acse.negotiate_release()
             # Restart reactor
             self._reactor_checkpoint.set()
 
     @property
-    def remote(self) -> Dict[str, Any]:
+    def remote(self) -> dict[str, Any]:
         """Return a :class:`dict` with information about the peer AE."""
         if self.is_acceptor:
             return self.requestor.info
 
         return self.acceptor.info
 
     def request(self) -> None:
@@ -891,16 +885,16 @@
 
         # Send C-STORE confirmation back to peer
         self.dimse.send_msg(rsp, cast(int, context.context_id))
 
     def send_c_cancel(
         self,
         msg_id: int,
-        context_id: Optional[int] = None,
-        query_model: Optional[Union[str, UID]] = None,
+        context_id: int | None = None,
+        query_model: str | UID | None = None,
     ) -> None:
         """Send a C-CANCEL request to the peer AE.
 
         .. versionchanged:: 2.0
 
             Added `query_model` and made `context_id` optional
 
@@ -1044,26 +1038,30 @@
         status = self._check_received_status(rsp)
 
         return status
 
     def send_c_find(
         self,
         dataset: Dataset,
-        query_model: Union[str, UID],
+        query_model: str | UID,
         msg_id: int = 1,
         priority: int = 2,
-    ) -> Iterator[Tuple[Dataset, Optional[Dataset]]]:
+    ) -> Iterator[tuple[Dataset, Dataset | None]]:
         """Send a C-FIND request to the peer AE.
 
         Yields (*status*, *identifier*) pairs for each response from the peer.
 
         .. versionchanged:: 1.5
 
             `query_model` now only accepts a UID string
 
+        .. versionchanged:: 2.1
+
+            Added support for *Repository Query*
+
         Parameters
         ----------
         dataset : pydicom.dataset.Dataset
             The C-FIND request's *Identifier* dataset. The exact requirements
             for the *Identifier* dataset are Service Class specific (see the
             DICOM Standard, :dcm:`Part 4<part04/PS3.4.html>`).
         query_model : pydicom.uid.UID or str
@@ -1110,32 +1108,42 @@
             Failure
               | ``0x0122`` - SOP class not supported
 
             *Query/Retrieve Service, Basic Worklist Management Service,
             Hanging Protocol Query/Retrieve Service, Defined Procedure Protocol
             Query/Retrieve Service, Substance Administration Query Service,
             Color Palette Query/Retrieve Service*, *Implant Template
-            Query/Retrieve Service*, *Protocol Approval Query/Retrieve
-            Service* and *Unified Protocol Step Service* specific
-            (DICOM Standard, Part 4, Annexes C.4.1, K.4.1.1.4, U.4.1, HH,
-            V.4.1.1.4, X, BB, II and CC):
+            Query/Retrieve Service*, *Inventory Query/Retrieve Service*,
+            *Protocol Approval Query/Retrieve Service* and *Unified Protocol
+            Step Service* specific (DICOM Standard, Part 4, Annexes C.4.1,
+            K.4.1.1.4, U.4.1, HH, V.4.1.1.4, X, BB, II, JJ and CC):
 
             Failure
               | ``0xA700`` - Out of resources
               | ``0xA900`` - Identifier does not match SOP Class
               | ``0xC000`` to ``0xCFFF`` - Unable to process
 
             Pending
               | ``0xFF00`` - Matches are continuing: current match is supplied
                 and any Optional Keys were supported in the same manner as
                 Required Keys
               | ``0xFF01`` - Matches are continuing: warning that one or more
                 Optional Keys were not supported for existence and/or matching
                 for this Identifier)
 
+            *Query/Retrieve Service - Repository Query* specific (DICOM Standard,
+            Part 5, Annex C.6.4):
+
+            Warning
+              | ``0xB001`` - Matching reached response limit, subsequent
+                request may return additional matches
+
+            Failure
+              | ``0xA710`` - Invalid prior record key
+
             *Relevant Patient Information Query Service* specific (DICOM
             Standard Part 4, Annex Q.2.1.1.4):
 
             Failure
               | ``0xA700`` - Out of resources
               | ``0xA900`` - Identifier does not match SOP Class
               | ``0xC000`` - Unable to process
@@ -1167,14 +1175,15 @@
 
         :class:`~pynetdicom.dimse_primitives.C_FIND`
         :class:`~pynetdicom.service_class.BasicWorklistManagementServiceClass`
         :class:`~pynetdicom.service_class.ColorPaletteQueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.DefinedProcedureProtocolQueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.HangingProtocolQueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.ImplantTemplateQueryRetrieveServiceClass`
+        :class:`~pynetdicom.service_class.InventoryQueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.ProtocolApprovalQueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.QueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.RelevantPatientInformationQueryServiceClass`
         :class:`~pynetdicom.service_class.SubstanceAdministrationQueryServiceClass`
         :class:`~pynetdicom.service_class_n.UnifiedProcedureStepServiceClass`
 
         References
@@ -1186,14 +1195,15 @@
         * DICOM Standard, Part 4, :dcm:`Annex U<part04/chapter_U.html>`
         * DICOM Standard, Part 4, :dcm:`Annex V<part04/chapter_V.html>`
         * DICOM Standard, Part 4, :dcm:`Annex X<part04/chapter_X.html>`
         * DICOM Standard, Part 4, :dcm:`Annex BB<part04/chapter_BB.html>`
         * DICOM Standard, Part 4, :dcm:`Annex CC<part04/chapter_CC.html>`
         * DICOM Standard, Part 4, :dcm:`Annex HH<part04/chapter_HH.html>`
         * DICOM Standard, Part 4, :dcm:`Annex II<part04/chapter_II.html>`
+        * DICOM Standard, Part 4, :dcm:`Annex JJ<part04/chapter_JJ.html>`
         * DICOM Standard, Part 7, Sections
           :dcm:`9.1.2<part07/chapter_9.html#sect_9.1.2>`,
           :dcm:`9.3.2<part07/sect_9.3.2.html>` and
           :dcm:`Annex C<part07/chapter_C.html>`
         """
         # Can't send a C-FIND without an Association
         if not self.is_established:
@@ -1208,22 +1218,24 @@
         if context.abstract_syntax != query_model:
             LOGGER.info("Using Presentation Context:")
             LOGGER.info(f"  Context ID:        {context.context_id}")
             LOGGER.info(
                 "  Abstract Syntax:   =" f"{cast(UID, context.abstract_syntax).name}"
             )
 
+        query_model = UID(query_model)
+
         # Build C-FIND request primitive
         #   (M) Message ID
         #   (M) Affected SOP Class UID
         #   (M) Priority
         #   (M) Identifier
         req = C_FIND()
         req.MessageID = msg_id
-        req.AffectedSOPClassUID = UID(query_model)
+        req.AffectedSOPClassUID = query_model
         req.Priority = priority
 
         # Encode the Identifier `dataset` using the agreed transfer syntax
         #   Will return None if failed to encode
         transfer_syntax = context.transfer_syntax[0]
         bytestream = encode(
             dataset,
@@ -1236,40 +1248,42 @@
             req.Identifier = BytesIO(bytestream)
         else:
             LOGGER.error("Failed to encode the supplied Dataset")
             raise ValueError("Failed to encode the supplied Dataset")
 
         LOGGER.info(f"Sending Find Request: MsgID {msg_id}")
         LOGGER.info("")
-        LOGGER.info("# Request Identifier")
-        for line in pretty_dataset(dataset):
-            LOGGER.info(line)
-        LOGGER.info("")
+        if _config.LOG_REQUEST_IDENTIFIERS:
+            LOGGER.info("# Request Identifier")
+            for line in pretty_dataset(dataset):
+                LOGGER.info(line)
+
+            LOGGER.info("")
 
         # Pause the reactor to prevent a race condition
         self._reactor_checkpoint.clear()
         while not self._is_paused:
             time.sleep(0.0001)
 
         # Send C-FIND request to the peer via DIMSE
         self.dimse.send_msg(req, cast(int, context.context_id))
 
         # Get the responses from the peer
         # Wrap the generator so the C-FIND-RQ is sent immediately on
         #   executing this function, otherwise sending C-CANCEL requests
         #   may end up being sent first unless next() is called
-        return self._wrap_find_responses(transfer_syntax)
+        return self._wrap_find_responses(transfer_syntax, query_model)
 
     def send_c_get(
         self,
         dataset: Dataset,
-        query_model: Union[str, UID],
+        query_model: str | UID,
         msg_id: int = 1,
         priority: int = 2,
-    ) -> Iterator[Tuple[Dataset, Optional[Dataset]]]:
+    ) -> Iterator[tuple[Dataset, Dataset | None]]:
         """Send a C-GET request to the peer AE.
 
         Yields (*status*, *identifier*) pairs for each response from the peer.
 
         A :meth:`C-STORE handler<pynetdicom._handlers.doc_handle_store>`
         should be implemented and bound to ``evt.EVT_C_STORE``
         prior to calling :meth:`send_c_get` as the peer will return any matches
@@ -1330,17 +1344,17 @@
               | ``0x0210`` - Duplicate invocation
               | ``0x0211`` - Unrecognised operation
               | ``0x0212`` - Mistyped argument
 
             *Query/Retrieve Service, Hanging Protocol Query/Retrieve Service,
             Defined Procedure Protocol Query/Retrieve Service, Color Palette
             Query/Retrieve Service*, *Implant Template Query/Retrieve
-            Service* and *Protocol Approval Query/Retrieve Service* specific
-            (DICOM Standard, Part 4, Annexes C.4.3,
-            Y.C.4.2.1.4, Z.4.2.1.4, U.4.3, X, BB, HH and II):
+            Service*, *Inventory Query/Retrieve Service* and *Protocol Approval
+            Query/Retrieve Service* specific (DICOM Standard, Part 4, Annexes
+            C.4.3, Y.C.4.2.1.4, Z.4.2.1.4, U.4.3, X, BB, HH, II and JJ):
 
             Pending
               | ``0xFF00`` - Sub-operations are continuing
 
             Cancel
               | ``0xFE00`` - Sub-operations terminated due to Cancel indication
 
@@ -1383,27 +1397,29 @@
 
         :class:`~pynetdicom.dimse_primitives.C_GET`
         :class:`~pynetdicom.service_class.QueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.HangingProtocolQueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.DefinedProcedureProtocolQueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.ColorPaletteQueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.ImplantTemplateQueryRetrieveServiceClass`
+        :class:`~pynetdicom.service_class.InventoryQueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.ProtocolApprovalQueryRetrieveServiceClass`
 
         References
         ----------
 
         * DICOM Standard, Part 4, :dcm:`Annex C<part04/chapter_C.html>`
         * DICOM Standard, Part 4, :dcm:`Annex U<part04/chapter_U.html>`
         * DICOM Standard, Part 4, :dcm:`Annex X<part04/chapter_X.html>`
         * DICOM Standard, Part 4, :dcm:`Annex Y<part04/chapter_Y.html>`
         * DICOM Standard, Part 4, :dcm:`Annex Z<part04/chapter_Z.html>`
         * DICOM Standard, Part 4, :dcm:`Annex BB<part04/chapter_BB.html>`
         * DICOM Standard, Part 4, :dcm:`Annex HH<part04/chapter_HH.html>`
         * DICOM Standard, Part 4, :dcm:`Annex II<part04/chapter_II.html>`
+        * DICOM Standard, Part 4, :dcm:`Annex JJ<part04/chapter_JJ.html>`
         * DICOM Standard, Part 7, Sections
           :dcm:`9.1.3<part07/chapter_9.html#sect_9.1.3>`,
           :dcm:`9.3.3<part07/sect_9.3.3.html>` and
           :dcm:`Annex C<part07/chapter_C.html>`
         """
         # Can't send a C-GET without an Association
         if not self.is_established:
@@ -1440,18 +1456,20 @@
             req.Identifier = BytesIO(bytestream)
         else:
             LOGGER.error("Failed to encode the supplied Identifier dataset")
             raise ValueError("Failed to encode the supplied Identifier dataset")
 
         LOGGER.info(f"Sending Get Request: MsgID {msg_id}")
         LOGGER.info("")
-        LOGGER.info("# Request Identifier")
-        for line in pretty_dataset(dataset):
-            LOGGER.info(line)
-        LOGGER.info("")
+        if _config.LOG_REQUEST_IDENTIFIERS:
+            LOGGER.info("# Request Identifier")
+            for line in pretty_dataset(dataset):
+                LOGGER.info(line)
+
+            LOGGER.info("")
 
         # Pause the reactor to prevent a race condition
         self._reactor_checkpoint.clear()
         while not self._is_paused:
             time.sleep(0.0001)
 
         # Send C-GET request to the peer via DIMSE
@@ -1463,18 +1481,18 @@
         #   may end up being sent first unless next() is called
         return self._wrap_get_move_responses(transfer_syntax)
 
     def send_c_move(
         self,
         dataset: Dataset,
         move_aet: str,
-        query_model: Union[str, UID],
+        query_model: str | UID,
         msg_id: int = 1,
         priority: int = 2,
-    ) -> Iterator[Tuple[Dataset, Optional[Dataset]]]:
+    ) -> Iterator[tuple[Dataset, Dataset | None]]:
         """Send a C-MOVE request to the peer AE.
 
         Yields (*status*, *identifier*) pairs for each response from the peer.
 
         The peer will attempt to start a new association with an Storage SCP
         with AE title `move_aet` and hence the Storage SCP must be known to
         the Move SCP. Once the association has been established, the peer will
@@ -1541,16 +1559,17 @@
 
             Failure
               | ``0x0122`` - SOP class not supported
 
             *Query/Retrieve Service, Hanging Protocol Query/Retrieve Service,
             Defined Procedure Protocol Query/Retrieve Service, Color Palette
             Query/Retrieve Service* , *Implant Template Query/Retrieve
-            Service* and *Protocol Approval Query/Retrieve Service*
-            specific (DICOM Standard, Part 4, Annexes C, U, Y, X, BB and HH):
+            Service*, *Inventory Query/Retrieve Service* and *Protocol Approval
+            Query/Retrieve Service* specific (DICOM Standard, Part 4, Annexes
+            C, U, Y, X, BB, HH and JJ):
 
             Failure
               | ``0xA701`` - Out of resources: unable to calculate number of
                 matches
               | ``0xA702`` - Out of resources: unable to perform sub-operations
               | ``0xA801`` - Move destination unknown
               | ``0xA900`` - Identifier does not match SOP Class
@@ -1589,26 +1608,28 @@
         --------
 
         :class:`~pynetdicom.dimse_primitives.C_MOVE`
         :class:`~pynetdicom.service_class.QueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.HangingProtocolQueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.ColorPaletteQueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.ImplantTemplateQueryRetrieveServiceClass`
+        :class:`~pynetdicom.service_class.InventoryQueryRetrieveServiceClass`
         :class:`~pynetdicom.service_class.ProtocolApprovalQueryRetrieveServiceClass`
 
         References
         ----------
 
         * DICOM Standard, Part 4, :dcm:`Annex C<part04/chapter_C.html>`
         * DICOM Standard, Part 4, :dcm:`Annex U<part04/chapter_U.html>`
         * DICOM Standard, Part 4, :dcm:`Annex X<part04/chapter_X.html>`
         * DICOM Standard, Part 4, :dcm:`Annex Y<part04/chapter_Y.html>`
         * DICOM Standard, Part 4, :dcm:`Annex BB<part04/chapter_BB.html>`
         * DICOM Standard, Part 4, :dcm:`Annex HH<part04/chapter_HH.html>`
         * DICOM Standard, Part 4, :dcm:`Annex II<part04/chapter_II.html>`
+        * DICOM Standard, Part 4, :dcm:`Annex JJ<part04/chapter_JJ.html>`
         * DICOM Standard, Part 7, Sections
           :dcm:`9.1.4<part07/chapter_9.html#sect_9.1.4>`,
           :dcm:`9.3.4<part07/sect_9.3.4.html>` and
           :dcm:`Annex C<part07/chapter_C.html>`
         """
         # Can't send a C-MOVE without an Association
         if not self.is_established:
@@ -1647,18 +1668,20 @@
             req.Identifier = BytesIO(bytestream)
         else:
             LOGGER.error("Failed to encode the supplied Identifier dataset")
             raise ValueError("Failed to encode the supplied Identifier dataset")
 
         LOGGER.info(f"Sending Move Request: MsgID {msg_id}")
         LOGGER.info("")
-        LOGGER.info("# Request Identifier")
-        for line in pretty_dataset(dataset):
-            LOGGER.info(line)
-        LOGGER.info("")
+        if _config.LOG_REQUEST_IDENTIFIERS:
+            LOGGER.info("# Request Identifier")
+            for line in pretty_dataset(dataset):
+                LOGGER.info(line)
+
+            LOGGER.info("")
 
         # Pause the reactor to prevent a race condition
         self._reactor_checkpoint.clear()
         while not self._is_paused:
             time.sleep(0.0001)
 
         # Send C-MOVE request to the peer via DIMSE and wait for the response
@@ -1668,19 +1691,19 @@
         # Wrap the generator so the C-MOVE-RQ is sent immediately on
         #   executing this function, otherwise sending C-CANCEL requests
         #   may end up being sent first unless next() is called
         return self._wrap_get_move_responses(transfer_syntax)
 
     def send_c_store(
         self,
-        dataset: Union[str, Path, Dataset],
+        dataset: str | Path | Dataset,
         msg_id: int = 1,
         priority: int = 2,
-        originator_aet: Optional[str] = None,
-        originator_id: Optional[int] = None,
+        originator_aet: str | None = None,
+        originator_id: int | None = None,
     ) -> Dataset:
         """Send a C-STORE request to the peer AE.
 
         .. versionchanged:: 2.0
 
             * Changed `dataset` parameter to either be a dataset or the path to
               a dataset.
@@ -1860,14 +1883,42 @@
             except (AssertionError, AttributeError):
                 raise AttributeError(
                     "Unable to determine the presentation context to use with "
                     "`dataset` as it contains no '(0002,0010) Transfer Syntax "
                     "UID' file meta information element"
                 )
 
+            ts_encoding: tuple[bool, bool] = (
+                tsyntax.is_implicit_VR,
+                tsyntax.is_little_endian,
+            )
+            # `dataset` might also be created from scratch
+            ds_encoding = getattr(
+                dataset,
+                "original_encoding",
+                (dataset.is_implicit_VR, dataset.is_little_endian),
+            )
+            if None not in ds_encoding and ts_encoding != ds_encoding:
+                s = ("explicit VR", "implicit VR")[cast(bool, ds_encoding[0])]
+                s += (" big endian", " little endian")[cast(bool, ds_encoding[1])]
+                msg = (
+                    f"'dataset' is encoded as {s} but the file meta has a "
+                    f"(0002,0010) Transfer Syntax UID of '{tsyntax.name}'"
+                )
+                if ds_encoding == (True, True):
+                    LOGGER.warning(f"{msg} - using 'Implicit VR Little Endian' instead")
+                    tsyntax = ImplicitVRLittleEndian
+                elif ds_encoding == (False, False):
+                    LOGGER.warning(f"{msg} - using 'Explicit VR Big Endian' instead")
+                    tsyntax = ExplicitVRBigEndian
+                else:
+                    raise AttributeError(
+                        f"{msg} - please set an appropriate Transfer Syntax"
+                    )
+
         # Get a Presentation Context to use for sending the message
         context = self._get_valid_context(
             sop_class, tsyntax, "scu", allow_conversion=allow_conversion
         )
         transfer_syntax = context.transfer_syntax[0]
 
         req.AffectedSOPClassUID = sop_class
@@ -1908,28 +1959,34 @@
 
         # Determine validity of the response and get the status
         status = self._check_received_status(rsp)
 
         return status
 
     def _wrap_find_responses(
-        self, transfer_syntax: UID
-    ) -> Iterator[Tuple[Dataset, Optional[Dataset]]]:
+        self,
+        transfer_syntax: UID,
+        query_model: UID,
+    ) -> Iterator[tuple[Dataset, None | Dataset]]:
         """Wrapper for the C-FIND response generator.
 
         Wrapping the response generators allows us to immediately send the
         service request on calling the ``send_c_find()`` function. This is
         important when it comes to reliably sending C-CANCEL requests
         because otherwise the C-CANCEL may end up being sent prior to the
         C-FIND request.
 
         Parameters
         ----------
         transfer_syntax : pydicom.uid.UID
             The transfer syntax UID used to encode the responses.
+        query_model : pydicom.uid.UID
+            The value to use for the C-FIND request's (0000,0002) *Affected
+            SOP Class UID* parameter, which usually corresponds to the
+            Information Model that is to be used.
 
         Yields
         ------
         See ``send_c_find()``.
         """
         operation_no = 1
         while True:
@@ -1971,26 +2028,37 @@
             # If the Status is 'Pending' then the processing of
             #   matches and sub-operations is initiated or continuing
             # If the Status is 'Cancel', 'Failure', 'Warning' or 'Success'
             #   then we are finished
             category = code_to_category(cast(int, status.Status))
 
             LOGGER.debug("")
+            if query_model == RepositoryQuery and status.Status == 0xB001:
+                # PS3.4, Annex C.6.4.4
+                # 0xB001 conveys end of Pending responses
+                LOGGER.info(
+                    f"Find SCP Response: {operation_no} - "
+                    "0xB001 (Warning - Matching reached response limit, "
+                    "subsequent request may return additional matches)"
+                )
+                yield status, None
+                continue
+
             if category == STATUS_PENDING:
                 LOGGER.info(
                     f"Find SCP Response: {operation_no} - "
                     f"0x{status.Status:04X} (Pending)"
                 )
             else:
                 LOGGER.info(f"Find SCP Result: 0x{status.Status:04X} ({category})")
 
             # 'Success', 'Warning', 'Failure', 'Cancel' are final yields,
             #   'Pending' means more to come
             identifier = None
-            if category in [STATUS_PENDING]:
+            if category == STATUS_PENDING:
                 operation_no += 1
 
                 with self.lock:
                     try:
                         identifier = decode(
                             cast(BytesIO, rsp.Identifier),
                             transfer_syntax.is_implicit_VR,
@@ -2018,15 +2086,15 @@
             break
 
         # Unpause the reactor
         self._reactor_checkpoint.set()
 
     def _wrap_get_move_responses(
         self, transfer_syntax: UID
-    ) -> Iterator[Tuple[Dataset, Optional[Dataset]]]:
+    ) -> Iterator[tuple[Dataset, Dataset | None]]:
         """Wrapper for the C-GET/C-MOVE response generators.
 
         Wrapping the response generators allows us to immediately send the
         service request on calling the respective ``send_c_*()`` function.
         This is important when it comes to reliably sending C-CANCEL requests
         because otherwise the C-CANCEL may end up being sent prior to the
         C-GET/MOVE request.
@@ -2161,19 +2229,19 @@
         self._reactor_checkpoint.set()
 
     # DIMSE-N services provided by the Association
     def send_n_action(
         self,
         dataset: Dataset,
         action_type: int,
-        class_uid: Union[str, UID],
-        instance_uid: Union[str, UID],
+        class_uid: str | UID,
+        instance_uid: str | UID,
         msg_id: int = 1,
-        meta_uid: Optional[Union[str, UID]] = None,
-    ) -> Tuple[Dataset, Optional[Dataset]]:
+        meta_uid: str | UID | None = None,
+    ) -> tuple[Dataset, Dataset | None]:
         """Send an N-ACTION request to the peer AE.
 
         .. versionchanged:: 1.4
 
             Added `meta_uid` keyword parameter
 
         Parameters
@@ -2231,14 +2299,21 @@
               | ``0x0123`` - No such action
               | ``0x0124`` - Not authorised
               | ``0x0210`` - Duplicate invocation
               | ``0x0211`` - Unrecognised operation
               | ``0x0212`` - Mistyped argument
               | ``0x0213`` - Resource limitation
 
+            *Storage Management Service* specific (DICOM
+            Standard Part 4, Annex KK.2.2.3):
+
+            Warning
+              | ``0xB010`` - Attribute list error - One or more of Key
+                Attributes are not supported for matching
+
         action_reply : pydicom.dataset.Dataset or None
             If the status category is 'Success' or 'Warning' then a
             :class:`~pydicom.dataset.Dataset` containing attributes
             corresponding to those supplied in the *Action Reply*. Because
             *Action Reply* is optional the returned
             :class:`~pydicom.dataset.Dataset` may be empty.
 
@@ -2250,25 +2325,27 @@
 
         :class:`~pynetdicom.dimse_primitives.N_ACTION`
         :class:`~pynetdicom.service_class_n.ApplicationEventLoggingServiceClass`
         :class:`~pynetdicom.service_class_n.MediaCreationManagementServiceClass`
         :class:`~pynetdicom.service_class_n.PrintManagementServiceClass`
         :class:`~pynetdicom.service_class_n.RTMachineVerificationServiceClass`
         :class:`~pynetdicom.service_class_n.StorageCommitmentServiceClass`
+        :class:`~pynetdicom.service_class_n.StorageManagementServiceClass`
         :class:`~pynetdicom.service_class_n.UnifiedProcedureStepServiceClass`
 
         References
         ----------
 
         * DICOM Standard, Part 4, :dcm:`Annex H<part04/chapter_H.html>`
         * DICOM Standard, Part 4, :dcm:`Annex J<part04/chapter_J.html>`
         * DICOM Standard, Part 4, :dcm:`Annex P<part04/chapter_P.html>`
         * DICOM Standard, Part 4, :dcm:`Annex S<part04/chapter_S.html>`
         * DICOM Standard, Part 4, :dcm:`Annex CC<part04/chapter_CC.html>`
         * DICOM Standard, Part 4, :dcm:`Annex DD<part04/chapter_DD.html>`
+        * DICOM Standard, Part 4, :dcm:`Annex KK<part04/chapter_KK.html>`
         * DICOM Standard, Part 7, Sections
           :dcm:`10.1.4<part07/chapter_10.html#sect_10.1.4>`,
           :dcm:`10.3.4<part07/sect_10.3.4.html>` and
           :dcm:`Annex C<part07/chapter_C.html>`
         """
         # Can't send an N-ACTION without an Association
         if not self.is_established:
@@ -2368,19 +2445,19 @@
                 action_reply = Dataset()
 
         return status, action_reply
 
     def send_n_create(
         self,
         dataset: Dataset,
-        class_uid: Union[str, UID],
-        instance_uid: Optional[Union[str, UID]] = None,
+        class_uid: str | UID,
+        instance_uid: str | UID | None = None,
         msg_id: int = 1,
-        meta_uid: Optional[Union[str, UID]] = None,
-    ) -> Tuple[Dataset, Optional[Dataset]]:
+        meta_uid: str | UID | None = None,
+    ) -> tuple[Dataset, Dataset | None]:
         """Send an N-CREATE request to the peer AE.
 
         .. versionchanged:: 1.4
 
             Added `meta_uid` keyword parameter
 
         Parameters
@@ -2612,18 +2689,18 @@
             else:
                 attribute_list = Dataset()
 
         return status, attribute_list
 
     def send_n_delete(
         self,
-        class_uid: Union[str, UID],
-        instance_uid: Union[str, UID],
+        class_uid: str | UID,
+        instance_uid: str | UID,
         msg_id: int = 1,
-        meta_uid: Optional[Union[str, UID]] = None,
+        meta_uid: str | UID | None = None,
     ) -> Dataset:
         """Send an N-DELETE request to the peer AE.
 
         .. versionchanged:: 1.4
 
             Added `meta_uid` keyword parameter
 
@@ -2738,19 +2815,19 @@
 
         return status
 
     def send_n_event_report(
         self,
         dataset: Dataset,
         event_type: int,
-        class_uid: Union[str, UID],
-        instance_uid: Union[str, UID],
+        class_uid: str | UID,
+        instance_uid: str | UID,
         msg_id: int = 1,
-        meta_uid: Optional[Union[str, UID]] = None,
-    ) -> Tuple[Dataset, Optional[Dataset]]:
+        meta_uid: str | UID | None = None,
+    ) -> tuple[Dataset, Dataset | None]:
         """Send an N-EVENT-REPORT request to the peer AE.
 
         .. versionchanged:: 1.4
 
             Added `meta_uid` keyword parameter
 
         Parameters
@@ -2826,24 +2903,26 @@
         --------
 
         :class:`~pynetdicom.dimse_primitives.N_EVENT_REPORT`
         :class:`~pynetdicom.service_class_n.PrintManagementServiceClass`
         :class:`~pynetdicom.service_class_n.ProcedureStepServiceClass`
         :class:`~pynetdicom.service_class_n.RTMachineVerificationServiceClass`
         :class:`~pynetdicom.service_class_n.StorageCommitmentServiceClass`
+        :class:`~pynetdicom.service_class_n.StorageManagementServiceClass`
         :class:`~pynetdicom.service_class_n.UnifiedProcedureStepServiceClass`
 
         References
         ----------
 
         * DICOM Standard, Part 4, :dcm:`Annex F <part04/chapter_F.html>`
         * DICOM Standard, Part 4, :dcm:`Annex H <part04/chapter_H.html>`
         * DICOM Standard, Part 4, :dcm:`Annex J <part04/chapter_J.html>`
         * DICOM Standard, Part 4, :dcm:`Annex CC <part04/chapter_CC.html>`
         * DICOM Standard, Part 4, :dcm:`Annex DD <part04/chapter_DD.html>`
+        * DICOM Standard, Part 4, :dcm:`Annex KK <part04/chapter_KK.html>`
         * DICOM Standard, Part 7, Sections
           :dcm:`10.1.1 <part07/chapter_10.html#sect_10.1.1>`,
           :dcm:`10.3.1 <part07/sect_10.3.html#sect_10.3.1>`
           and :dcm:`Annex C <part07/chapter_C.html>`
         """
         # Can't send an N-EVENT-REPORT without an Association
         if not self.is_established:
@@ -2947,20 +3026,20 @@
             else:
                 event_reply = Dataset()
 
         return status, event_reply
 
     def send_n_get(
         self,
-        identifier_list: List[BaseTag],
-        class_uid: Union[str, UID],
-        instance_uid: Union[str, UID],
+        identifier_list: list[BaseTag],
+        class_uid: str | UID,
+        instance_uid: str | UID,
         msg_id: int = 1,
-        meta_uid: Optional[Union[str, UID]] = None,
-    ) -> Tuple[Dataset, Optional[Dataset]]:
+        meta_uid: str | UID | None = None,
+    ) -> tuple[Dataset, Dataset | None]:
         """Send an N-GET request to the peer AE.
 
         .. versionchanged:: 1.4
 
             Added `meta_uid` keyword parameter
 
         Parameters
@@ -3162,19 +3241,19 @@
                 attribute_list = Dataset()
 
         return status, attribute_list
 
     def send_n_set(
         self,
         dataset: Dataset,
-        class_uid: Union[str, UID],
-        instance_uid: Union[str, UID],
+        class_uid: str | UID,
+        instance_uid: str | UID,
         msg_id: int = 1,
-        meta_uid: Optional[Union[str, UID]] = None,
-    ) -> Tuple[Dataset, Optional[Dataset]]:
+        meta_uid: str | UID | None = None,
+    ) -> tuple[Dataset, Dataset | None]:
         """Send an N-SET request to the peer AE.
 
         .. versionchanged:: 1.4
 
             Added `meta_uid` keyword parameter
 
         Parameters
@@ -3432,15 +3511,15 @@
         # No message or not a service request
         if not msg.is_valid_request:
             LOGGER.warning(f"Received unexpected {msg.msg_type} service message")
             return
 
         # Use the Message's Affected SOP Class UID or Requested SOP
         #   Class UID to determine which service to use
-        class_uid: Union[str, UID] = ""
+        class_uid: str | UID = ""
         if getattr(msg, "AffectedSOPClassUID", None) is not None:
             # DIMSE-C, N-EVENT-REPORT, N-CREATE use AffectedSOPClassUID
             class_uid = cast(UID, msg.AffectedSOPClassUID)
         elif getattr(msg, "RequestedSOPClassUID", None) is not None:
             # N-GET, N-SET, N-ACTION, N-DELETE use RequestedSOPClassUID
             class_uid = msg.RequestedSOPClassUID  # type: ignore
 
@@ -3556,38 +3635,38 @@
         mode = mode.lower()
         if mode not in [MODE_REQUESTOR, MODE_ACCEPTOR]:
             raise ValueError("The 'mode' must be either 'requestor' or 'acceptor'")
 
         self.assoc: Association = assoc
         self._mode: str = mode
         self._ae_title: str = ""
-        self.primitive: Optional[A_ASSOCIATE] = None
-        self.port: Optional[int] = None
-        self.address: Optional[str] = ""
+        self.primitive: A_ASSOCIATE | None = None
+        self.port: int | None = None
+        self.address: str | None = ""
 
         # If Requestor this is the requested contexts, otherwise this is
         #   the supported contexts
-        self._contexts: List[PresentationContext] = []
+        self._contexts: list[PresentationContext] = []
 
         # User Information items
-        self._user_info: List[_UI] = []
+        self._user_info: list[_UI] = []
         # Must always be set
         self.maximum_length: int = DEFAULT_MAX_LENGTH
         self.implementation_class_uid: UID = assoc.ae.implementation_class_uid
 
         # These are the proposed extended negotiation items,
-        self._ext_neg: Dict[_UITypes, List[_UI]] = {}
+        self._ext_neg: dict[_UITypes, list[_UI]] = {}
         self.reset_negotiation_items()
 
         # If Acceptor then this the accepted SOP Class Common Extended
         #   negotiation items
-        self._common_ext: Dict[UID, SOPClassCommonExtendedNegotiation] = {}
+        self._common_ext: dict[UID, SOPClassCommonExtendedNegotiation] = {}
 
     @property
-    def accepted_common_extended(self) -> Dict[UID, Tuple[UID, List[UID]]]:
+    def accepted_common_extended(self) -> dict[UID, tuple[UID, list[UID]]]:
         """Return a :class:`dict` of the accepted SOP Class Common Extended
         Negotiation.
 
         Returns
         -------
         dict of 2-tuple
             The ``{'SOP Class UID' : (Service Class UID, Related General SOP
@@ -3676,15 +3755,15 @@
                 DeprecationWarning,
             )
             value = decode_bytes(value)
 
         self._ae_title = cast(str, set_ae(value, "ae_title", False, False))
 
     @property
-    def asynchronous_operations(self) -> Tuple[int, int]:
+    def asynchronous_operations(self) -> tuple[int, int]:
         """Return the Asynchronous Operations Window operations numbers.
 
         Returns
         -------
         2-tuple of int
             The (*Maximum Number of Operations Invoked*, *Maximum Number of
             Operations Performed*) or ``(1, 1)`` if no Asynchronous Operations
@@ -3704,15 +3783,15 @@
                     item.maximum_number_operations_invoked,
                     item.maximum_number_operations_performed,
                 )
 
         return (1, 1)
 
     @property
-    def extended_negotiation(self) -> List[_UI]:
+    def extended_negotiation(self) -> list[_UI]:
         """Return a :class:`list` of Extended Negotiation items.
 
         Extended Negotiation items are:
 
         * SCP/SCU Role Selection Negotiation (0 or more)
         * Asynchronous Operations Window Negotiation (0 or 1)
         * SOP Class Extended Negotiation (0 or more)
@@ -3737,15 +3816,15 @@
         # pylint: disable=unidiomatic-typecheck
         for item in self.user_information:
             if type(item) in self._ext_neg.keys():
                 items.append(item)
 
         return items
 
-    def get_contexts(self, cx_type: str) -> List[PresentationContext]:
+    def get_contexts(self, cx_type: str) -> list[PresentationContext]:
         """Return a :class:`list` of
         :class:`~pynetdicom.presentation.PresentationContext` items
         corresponding to `cx_type`.
 
         Parameters
         ----------
         cx_type : str
@@ -3782,15 +3861,15 @@
                     "pcdl": self.primitive.presentation_context_definition_list,
                     "pcdrl": (
                         self.primitive.presentation_context_definition_results_list
                     ),
                 }
             )
 
-        possible: Dict[bool, Dict[bool, Dict[bool, List[str]]]] = {
+        possible: dict[bool, dict[bool, dict[bool, list[str]]]] = {
             True: {  # self.assoc.is_requestor
                 True: {  # self.writeable
                     True: ["requested"],  # self.is_requestor
                     False: [],  # self.is_acceptor
                 },
                 False: {  # not self.writeable
                     True: ["requested", "pcdl"],  # self.is_requestor
@@ -3815,15 +3894,15 @@
 
         raise ValueError(
             f"No '{cx_type}' presentation contexts are available for the "
             f"{('requestor', 'acceptor')[self.is_acceptor]} service user"
         )
 
     @property
-    def implementation_class_uid(self) -> Optional[UID]:
+    def implementation_class_uid(self) -> UID | None:
         """The Implementation Class UID as a :class:`~pydicom.uid.UID`.
 
         Returns
         -------
         pydicom.uid.UID or None
             Returns the Implementation Class UID if the requestor or if
             the acceptor and they have accepted the negotiation. Returns
@@ -3863,15 +3942,15 @@
                 break
         else:
             item = ImplementationClassUIDNotification()
             item.implementation_class_uid = value
             self._user_info.append(item)
 
     @property
-    def implementation_version_name(self) -> Optional[str]:
+    def implementation_version_name(self) -> str | None:
         """Get or set the *Implementation Version Name*.
 
         Parameters
         ----------
         value : str or None
             The value to use for the *Implementation Version Name*, or ``None``
             if no Implementation Version Name Notification item is to be
@@ -3896,15 +3975,15 @@
         for item in self._user_info:
             if isinstance(item, ImplementationVersionNameNotification):
                 return item.implementation_version_name
 
         return None
 
     @implementation_version_name.setter
-    def implementation_version_name(self, value: Optional[str]) -> None:
+    def implementation_version_name(self, value: str | None) -> None:
         """Set the Implementation Version Name (only prior to association)."""
         if not self.writeable:
             raise RuntimeError(
                 "Can't set the Implementation Version Name after negotiation "
                 "has started"
             )
 
@@ -3925,15 +4004,15 @@
                 break
         else:
             item = ImplementationVersionNameNotification()
             item.implementation_version_name = value
             self._user_info.append(item)
 
     @property
-    def info(self) -> Dict[str, Any]:
+    def info(self) -> dict[str, Any]:
         """Return a :class:`dict` with information about the
         :class:`ServiceUser`.
         """
         info = {
             "ae_title": self.ae_title,
             "address": self.address,
             "port": self.port,
@@ -3955,15 +4034,15 @@
     def is_requestor(self) -> bool:
         """Return ``True`` if the :class:`ServiceUser` is the association
         requestor.
         """
         return self.mode == MODE_REQUESTOR
 
     @property
-    def maximum_length(self) -> Optional[int]:
+    def maximum_length(self) -> int | None:
         """The maximum PDV size as :class:`int`.
 
         Returns
         -------
         int or None
             Returns the Maximum Received Length if the requestor or if
             the acceptor and they have accepted the negotiation. Returns
@@ -4009,25 +4088,25 @@
     def mode(self) -> str:
         """Return the mode as :class:`str`, either ``'requestor'`` or
         ``'acceptor'``.
         """
         return self._mode
 
     @property
-    def requested_contexts(self) -> List[PresentationContext]:
+    def requested_contexts(self) -> list[PresentationContext]:
         """A :class:`list` of the requestor's requested presentation
         contexts.
         """
         if not self.writeable and self.assoc.is_acceptor:
             return self.get_contexts("pcdl")
 
         return self.get_contexts("requested")
 
     @requested_contexts.setter
-    def requested_contexts(self, value: List[PresentationContext]) -> None:
+    def requested_contexts(self, value: list[PresentationContext]) -> None:
         """Set the requested presentation contexts.
 
         Parameters
         ----------
         value : list of presentation.PresentationContext
             A list of the presentation contexts to propose when acting as the
             association requestor.
@@ -4117,15 +4196,15 @@
             UserIdentityNegotiation: [],
             SOPClassExtendedNegotiation: [],
         }
         if self.is_requestor:
             self._ext_neg[SOPClassCommonExtendedNegotiation] = []
 
     @property
-    def role_selection(self) -> Dict[UID, SCP_SCU_RoleSelectionNegotiation]:
+    def role_selection(self) -> dict[UID, SCP_SCU_RoleSelectionNegotiation]:
         """Return any SCP/SCU Role Selection items.
 
         Returns
         -------
         dict
             The SCP/SCU Role Selection items as ``{'SOP Class UID' :
             SCP_SCU_RoleSelectionNegotiation}``.
@@ -4143,15 +4222,15 @@
                 roles[cast(UID, item.sop_class_uid)] = item
 
         return roles
 
     @property
     def sop_class_common_extended(
         self,
-    ) -> Dict[UID, SOPClassCommonExtendedNegotiation]:
+    ) -> dict[UID, SOPClassCommonExtendedNegotiation]:
         """Return the SOP Class Common Extended items.
 
         If the :class:`ServiceUser` is the association acceptor then no SOP
         Class Common Extended items will be present in the User Information.
 
         Returns
         -------
@@ -4173,15 +4252,15 @@
         for item in self.user_information:
             if isinstance(item, SOPClassCommonExtendedNegotiation):
                 sop_classes[cast(UID, item.sop_class_uid)] = item
 
         return sop_classes
 
     @property
-    def sop_class_extended(self) -> Dict[UID, bytes]:
+    def sop_class_extended(self) -> dict[UID, bytes]:
         """Return any SOP Class Extended items.
 
         Returns
         -------
         dict
             The SOP Class Extended items as ``{'SOP Class UID' : Service Class
             Application Information}``.
@@ -4201,29 +4280,29 @@
                 sop_classes[cast(UID, item.sop_class_uid)] = cast(
                     bytes, item.service_class_application_information
                 )
 
         return sop_classes
 
     @property
-    def supported_contexts(self) -> List[PresentationContext]:
+    def supported_contexts(self) -> list[PresentationContext]:
         """The supported presentation contexts.
 
         Returns
         -------
         list of presentation.PresentationContext
             The supported presentation contexts when acting as an acceptor.
         """
         if not self.writeable and self.assoc.is_requestor:
             return self.get_contexts("pcdrl")
 
         return self.get_contexts("supported")
 
     @supported_contexts.setter
-    def supported_contexts(self, value: List[PresentationContext]) -> None:
+    def supported_contexts(self, value: list[PresentationContext]) -> None:
         """Set the supported presentation contexts.
 
         Parameters
         ----------
         value : list of presentation.PresentationContext
             A list of the presentation contexts to support when acting as the
             association acceptor.
@@ -4245,15 +4324,15 @@
             raise AttributeError(
                 "'supported_contexts' can only be set for the association acceptor"
             )
 
         self._contexts = value
 
     @property
-    def user_identity(self) -> Optional[UserIdentityNegotiation]:
+    def user_identity(self) -> UserIdentityNegotiation | None:
         """Return the User Identity Negotiation Item (if available).
 
         Returns
         -------
         pdu_primitives.UserIdentityNegotiation or None
             Returns the User Identity item if one is available, otherwise
             ``None``.
@@ -4268,15 +4347,15 @@
         for item in self.user_information:
             if isinstance(item, UserIdentityNegotiation):
                 return item
 
         return None
 
     @property
-    def user_information(self) -> List[_UI]:
+    def user_information(self) -> list[_UI]:
         """Returns a :class:`list` of the User Information items."""
         if not self.writeable:
             return cast(A_ASSOCIATE, self.primitive).user_information
 
         return self._user_info + self.extended_negotiation
 
     @property
```

### Comparing `pynetdicom-2.0.2/pynetdicom/benchmarks/bench_c_send.py` & `pynetdicom-2.1.0/pynetdicom/benchmarks/bench_c_send.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,24 +19,24 @@
 
 
 DS_DIR = os.path.join(os.path.dirname(__file__), "../tests", "dicom_files")
 DATASET = dcmread(os.path.join(DS_DIR, "CTImageStorage.dcm"))
 
 
 class TestSendCEcho:
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.scp = DummyVerificationSCP()
         self.scp.start()
 
         ae = AE()
         ae.add_requested_context(Verification)
         self.assoc = ae.associate("localhost", 11112)
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.scp:
             self.scp.abort()
 
         time.sleep(0.1)
 
         for thread in threading.enumerate():
@@ -53,25 +53,25 @@
 
             self.assoc.release()
         else:
             raise RuntimeError("Unable to associate with the echo SCP")
 
 
 class TestSendCStore:
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.scp = DummyStorageSCP()
         self.scp.status = 0x0000
         self.scp.start()
 
         ae = AE()
         ae.add_requested_context(CTImageStorage)
         self.assoc = ae.associate("localhost", 11112)
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.scp:
             self.scp.abort()
 
         time.sleep(0.1)
 
         for thread in threading.enumerate():
```

### Comparing `pynetdicom-2.0.2/pynetdicom/benchmarks/bench_dimse_message.py` & `pynetdicom-2.1.0/pynetdicom/benchmarks/bench_dimse_message.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 TEST_DS_DIR = os.path.join(os.path.dirname(__file__), "../tests", "dicom_files")
 DATASET = dcmread(os.path.join(TEST_DS_DIR, "CTImageStorage.dcm"))
 
 
 class TestDecodeMessage:
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         primitive = C_STORE()
         primitive.MessageID = 7
         primitive.AffectedSOPClassUID = "1.1.1"
         primitive.AffectedSOPInstanceUID = "1.2.1"
         primitive.Priority = 0x02
         primitive.MoveOriginatorApplicationEntityTitle = b"UNITTEST"
@@ -36,15 +36,15 @@
         for ii in range(100):
             msg = DIMSEMessage()
             for fragment in self.fragments:
                 msg.decode_msg(fragment)
 
 
 class TestEncodeMessage:
-    def setup(self):
+    def setup_method(self):
         primitive = C_STORE()
         primitive.MessageID = 7
         primitive.AffectedSOPClassUID = "1.1.1"
         primitive.AffectedSOPInstanceUID = "1.2.1"
         primitive.Priority = 0x02
         primitive.MoveOriginatorApplicationEntityTitle = b"UNITTEST"
         primitive.MoveOriginatorMessageID = 3
```

### Comparing `pynetdicom-2.0.2/pynetdicom/benchmarks/bench_pdu.py` & `pynetdicom-2.1.0/pynetdicom/benchmarks/bench_pdu.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     a_release_rp,
     a_abort,
     p_data_tf,
 )
 
 
 class TimePDUDecode:
-    def setup(self):
+    def setup_method(self):
         """Setup the test"""
         pass
 
     def time_decode_assoc_rq_pdu(self):
         """Time decoding an A-ASSOCIATE-RQ PDU."""
         pdu = PDU_TYPES[0x01]()
         for ii in range(1000):
@@ -61,15 +61,15 @@
         """Time decoding an A-ABORT-RQ PDU."""
         pdu = PDU_TYPES[0x07]()
         for ii in range(1000):
             pdu.decode(a_abort)
 
 
 class TimePDUEncode:
-    def setup(self):
+    def setup_method(self):
         """Setup the test"""
         self.assoc_rq = PDU_TYPES[0x01]()
         self.assoc_rq.decode(a_associate_rq_user_id_ext_neg)
 
         self.assoc_ac = PDU_TYPES[0x02]()
         self.assoc_ac.decode(a_associate_ac)
```

### Comparing `pynetdicom-2.0.2/pynetdicom/benchmarks/bench_presentation.py` & `pynetdicom-2.1.0/pynetdicom/benchmarks/bench_presentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     PresentationContext,
     negotiate_as_acceptor,
     negotiate_as_requestor,
 )
 
 
 class TimePresentationContext:
-    def setup(self):
+    def setup_method(self):
         self.contexts = []
         for x in range(500):
             cx = PresentationContext()
             cx.context_id = 1
             cx.abstract_syntax = "1.2.840.10008.5.1.4.1.1.2"
             cx.transfer_syntax = [
                 "1.2.840.10008.1.2",
@@ -71,15 +71,15 @@
 
 
 class TimePresentationAcceptorRoleNegotiation:
     """Time presentation context negotiation as acceptor with SCP/SCU Role
     Selection
     """
 
-    def setup(self):
+    def setup_method(self):
         # Requestor presentation contexts - max 126
         self.requestor_contexts = []
         for ii, cx in enumerate(StoragePresentationContexts):
             cx.context_id = ii * 2 + 1
             cx.scp_role = True
             cx.scu_role = True
             self.requestor_contexts.append(cx)
@@ -107,15 +107,15 @@
 
 
 class TimePresentationRequestorRoleNegotiation:
     """Time presentation context negotiation as requestor with SCP/SCU Role
     Selection
     """
 
-    def setup(self):
+    def setup_method(self):
         # Requestor presentation contexts - max 126
         self.requestor_contexts = []
         for ii, cx in enumerate(StoragePresentationContexts):
             cx.context_id = ii * 2 + 1
             cx.SCP = True
             cx.SCU = True
             self.requestor_contexts.append(cx)
@@ -137,15 +137,15 @@
         for ii in range(100):
             negotiate_as_requestor(self.requestor_contexts, self.acceptor_contexts)
 
 
 class TimePresentationAcceptor:
     """Time presentation context negotiation as acceptor"""
 
-    def setup(self):
+    def setup_method(self):
         # Requestor presentation contexts - max 128
         self.requestor_contexts = []
 
         for ii, cx in enumerate(StoragePresentationContexts):
             cx.context_id = ii * 2 + 1
             self.requestor_contexts.append(cx)
 
@@ -167,15 +167,15 @@
         for ii in range(100):
             negotiate_as_acceptor(self.requestor_contexts, self.acceptor_contexts)
 
 
 class TimePresentationRequestor:
     """Time presentation context negotiation as requestor"""
 
-    def setup(self):
+    def setup_method(self):
         # Requestor presentation contexts - max 126
         self.requestor_contexts = []
         for ii, cx in enumerate(StoragePresentationContexts):
             cx.context_id = ii * 2 + 1
             self.requestor_contexts.append(cx)
 
         # Acceptor presentation contexts - no max
```

### Comparing `pynetdicom-2.0.2/pynetdicom/dimse.py` & `pynetdicom-2.1.0/pynetdicom/dimse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Implementation of the DIMSE service provider.
 """
+
 from io import BytesIO
 import logging
 import queue
 import threading
 from typing import TYPE_CHECKING, Tuple, Optional, Dict, Union, cast
 
 from pynetdicom import evt
@@ -58,15 +59,15 @@
 
 if TYPE_CHECKING:  # pragma: no cover
     from pynetdicom.association import Association
     from pynetdicom.dul import DULServiceProvider
     from pynetdicom.pdu_primitives import P_DATA
 
 
-LOGGER = logging.getLogger("pynetdicom.dimse")
+LOGGER = logging.getLogger(__name__)
 
 _RQ_TO_MESSAGE = {
     C_ECHO: C_ECHO_RQ,
     C_STORE: C_STORE_RQ,
     C_FIND: C_FIND_RQ,
     C_MOVE: C_MOVE_RQ,
     C_GET: C_GET_RQ,
@@ -320,14 +321,16 @@
             else:
                 self.msg_queue.put((context_id, cast(DimseServiceType, d_primitive)))
 
             # Fix for memory leak, Issue #41
             #   Reset the DIMSE message, ready for the next one
             self.message.encoded_command_set = BytesIO()
             self.message.data_set = BytesIO()
+            self.message._data_set_file = None
+            self.message._data_set_path = None
             self.message = None
 
     def send_msg(self, primitive: DimsePrimitiveType, context_id: int) -> None:
         """Encode and send a DIMSE-C or DIMSE-N message to the peer AE.
 
         Parameters
         ----------
```

### Comparing `pynetdicom-2.0.2/pynetdicom/dimse_messages.py` & `pynetdicom-2.1.0/pynetdicom/dimse_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from pynetdicom.pdu_primitives import P_DATA
 
 if TYPE_CHECKING:  # pragma: no cover
     from pynetdicom.association import Association
     from pynetdicom.dimse_primitives import NTF
 
 
-LOGGER = logging.getLogger("pynetdicom.dimse")
+LOGGER = logging.getLogger(__name__)
 
 
 # PS3.7 Section 9.3
 _COMMAND_SET_KEYWORDS = {
     "C-ECHO-RQ": (
         "CommandGroupLength",
         "AffectedSOPClassUID",
@@ -402,29 +402,25 @@
 
         * DICOM Standard, Part 8, :dcm:`Annex E<part08/chapter_E.html>`
         """
         # Make sure this is a P-DATA primitive
         if primitive.__class__ != P_DATA or primitive is None:
             return False
 
-        for (context_id, data) in primitive.presentation_data_value_list:
-
+        for context_id, data in primitive.presentation_data_value_list:
             # The first byte of the P-DATA is the Message Control Header
             #   See Part 8, Annex E.2
             # The standard says that only the significant bits (ie the last
             #   two) should be checked
             # xxxxxx00 - Message Dataset information, not the last fragment
             # xxxxxx01 - Command information, not the last fragment
             # xxxxxx10 - Message Dataset information, the last fragment
             # xxxxxx11 - Command information, the last fragment
             control_header_byte = data[0]
 
-            # LOGGER.debug('Control header byte %s', control_header_byte)
-            # print(f'Control header byte {control_header_byte}')
-
             # COMMAND SET
             # P-DATA fragment contains Command Set information
             #   (control_header_byte is xxxxxx01 or xxxxxx11)
             if control_header_byte & 1:
                 # The command set may be spread out over a number
                 #   of fragments and P-DATA primitives and we need to remember
                 #   the elements from previous fragments, hence the
```

### Comparing `pynetdicom-2.0.2/pynetdicom/dimse_primitives.py` & `pynetdicom-2.1.0/pynetdicom/dimse_primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,22 +25,20 @@
     from typing import Protocol  # Python 3.8+
 
     class NTF(Protocol):
         # Protocol for a NamedTemporaryFile
         name: str
         file: BufferedWriter
 
-        def write(self, data: bytes) -> bytes:
-            ...
+        def write(self, data: bytes) -> bytes: ...
 
-        def close(self) -> None:
-            ...
+        def close(self) -> None: ...
 
 
-LOGGER = logging.getLogger("pynetdicom.dimse_primitives")
+LOGGER = logging.getLogger(__name__)
 
 
 DimseServiceType = Union[
     "C_ECHO",
     "C_FIND",
     "C_GET",
     "C_MOVE",
@@ -471,14 +469,15 @@
     OffendingElement : list of int or None
         An optional status related field containing a list of the
         elements in which an error was detected.
     ErrorComment : str or None
         An optional status related field containing a text description
         of the error detected. 64 characters maximum.
     """
+
     STATUS_OPTIONAL_KEYWORDS = (
         "OffendingElement",
         "ErrorComment",
     )
     REQUEST_KEYWORDS = (
         "MessageID",
         "AffectedSOPClassUID",
@@ -677,14 +676,15 @@
     OffendingElement : list of int or None
         An optional status related field containing a list of the
         elements in which an error was detected.
     ErrorComment : str or None
         An optional status related field containing a text
         description of the error detected. 64 characters maximum.
     """
+
     STATUS_OPTIONAL_KEYWORDS = (
         "OffendingElement",
         "ErrorComment",
     )
     REQUEST_KEYWORDS = ("MessageID", "AffectedSOPClassUID", "Priority", "Identifier")
 
     def __init__(self) -> None:
@@ -802,14 +802,15 @@
     OffendingElement : list of int or None
         An optional status related field containing a list of the
         elements in which an error was detected.
     ErrorComment : str or None
         An optional status related field containing a text
         description of the error detected. 64 characters maximum.
     """
+
     STATUS_OPTIONAL_KEYWORDS = (
         "ErrorComment",
         "OffendingElement",
         "NumberOfRemainingSuboperations",
         "NumberOfCompletedSuboperations",
         "NumberOfFailedSuboperations",
         "NumberOfWarningSuboperations",
@@ -987,14 +988,15 @@
     OffendingElement : list of int or None
         An optional status related field containing a list of the
         elements in which an error was detected.
     ErrorComment : str or None
         An optional status related field containing a text
         description of the error detected. 64 characters maximum.
     """
+
     STATUS_OPTIONAL_KEYWORDS = (
         "ErrorComment",
         "OffendingElement",
         "NumberOfRemainingSuboperations",
         "NumberOfCompletedSuboperations",
         "NumberOfFailedSuboperations",
         "NumberOfWarningSuboperations",
@@ -1181,14 +1183,15 @@
         to the value in the request/indication
     Status : int or None
         The error or success notification of the operation.
     ErrorComment : str or None
         An optional status related field containing a text description
         of the error detected. 64 characters maximum.
     """
+
     STATUS_OPTIONAL_KEYWORDS = ("ErrorComment",)
     REQUEST_KEYWORDS = ("MessageID", "AffectedSOPClassUID")
 
     def __init__(self) -> None:
         # Variable names need to match the corresponding DICOM Element keywords
         #   in order for the DIMSE Message classes to be built correctly.
         # Changes to the variable names can be made provided the DIMSEMessage()
@@ -1311,14 +1314,15 @@
     AffectedSOPClassUID : pydicom.uid.UID, bytes or str
         For the request/indication this specifies the SOP Class for
         storage. If included in the response/confirmation, it shall be equal
         to the value in the request/indication
     Status : int
         The error or success notification of the operation.
     """
+
     # Optional status element keywords other than 'Status'
     STATUS_OPTIONAL_KEYWORDS = (
         "AffectedSOPClassUID",
         "AffectedSOPInstanceUID",
         "EventTypeID",
         "ErrorComment",
         "ErrorID",  # EventInformation
@@ -1459,14 +1463,15 @@
         response/confirmation applies.
     AffectedSOPClassUID : pydicom.uid.UID, bytes or str
         The SOP Class UID of the SOP Instance for which the attributes were
         retrieved.
     Status : int
         The error or success notification of the operation.
     """
+
     STATUS_OPTIONAL_KEYWORDS = (
         "AttributeIdentifierList",
         "ErrorComment",
         "ErrorID",
     )
     REQUEST_KEYWORDS = ("MessageID", "RequestedSOPClassUID", "RequestedSOPInstanceUID")
 
@@ -1508,34 +1513,37 @@
         """Get or set the *Attribute Identifier List* as a :class:`list` of
         :class:`~pydicom.tag.BaseTag`.
 
         Parameters
         ----------
         pydicom.tag.BaseTag or list of pydicom.tag.BaseTag
             The value to use for the *Attribute Identifier List* parameter.
-            A list of pydicom :class:`pydicom.tag.BaseTag` instances or any
-            values acceptable for creating them.
+            A pydicom :class:`pydicom.tag.BaseTag` or list of
+            :class:`pydicom.tag.BaseTag` or any values acceptable for creating
+            them.
         """
         return self._attribute_identifier_list
 
     @AttributeIdentifierList.setter
     def AttributeIdentifierList(
         self, value: Optional[Union[BaseTag, List[BaseTag]]]
     ) -> None:
         """Set the *Attribute Identifier List*."""
+        # Be careful as a tag value of 0x00000000 is possible (though unlikely)
         if value is None:
             self._attribute_identifier_list = None
             return
 
         try:
             if isinstance(value, Sequence):
                 if not value:
                     self._attribute_identifier_list = None
 
                 if len(value) == 1:
+                    # Force to a single value - workaround for pydicom #757
                     self._attribute_identifier_list = Tag(value[0])
                 else:
                     self._attribute_identifier_list = [Tag(tag) for tag in value]
             else:
                 self._attribute_identifier_list = Tag(value)
         except (TypeError, ValueError):
             raise ValueError(
@@ -1638,14 +1646,15 @@
         The Message ID of the operation request/indication to which this
         response/confirmation applies.
     AffectedSOPClassUID : pydicom.uid.UID, bytes or str
         The SOP Class UID of the modified SOP Instance.
     Status : int
         The error or success notification of the operation.
     """
+
     STATUS_OPTIONAL_KEYWORDS = ("ErrorComment", "ErrorID", "AttributeIdentifierList")
     REQUEST_KEYWORDS = (
         "MessageID",
         "RequestedSOPClassUID",
         "RequestedSOPInstanceUID",
         "ModificationList",
     )
@@ -1797,14 +1806,15 @@
     AffectedSOPClassUID : pydicom.uid.UID, bytes or str
         For the request/indication this specifies the SOP Class for
         storage. If included in the response/confirmation, it shall be equal
         to the value in the request/indication
     Status : int
         The error or success notification of the operation.
     """
+
     STATUS_OPTIONAL_KEYWORDS = ("ErrorComment", "ErrorID", "AttributeIdentifierList")
     REQUEST_KEYWORDS = (
         "MessageID",
         "RequestedSOPClassUID",
         "RequestedSOPInstanceUID",
         "ActionTypeID",
     )
@@ -1967,14 +1977,15 @@
         For the request/indication this specifies the SOP Class for
         storage. If included in the response/confirmation, it shall be equal
         to the value in the request/indication
     Status : int
         The error or success notification of the operation. It shall be
         one of the following values:
     """
+
     STATUS_OPTIONAL_KEYWORDS = (
         "ErrorComment",
         "ErrorID",
     )
     REQUEST_KEYWORDS = ("MessageID", "AffectedSOPClassUID")
 
     def __init__(self) -> None:
@@ -2064,14 +2075,15 @@
     AffectedSOPClassUID : pydicom.uid.UID, bytes or str
         For the request/indication this specifies the SOP Class for
         storage. If included in the response/confirmation, it shall be equal
         to the value in the request/indication
     Status : int
         The error or success notification of the operation.
     """
+
     STATUS_OPTIONAL_KEYWORDS = (
         "ErrorComment",
         "ErrorID",
     )
     REQUEST_KEYWORDS = ("MessageID", "RequestedSOPClassUID", "RequestedSOPInstanceUID")
 
     def __init__(self) -> None:
```

### Comparing `pynetdicom-2.0.2/pynetdicom/dsutils.py` & `pynetdicom-2.1.0/pynetdicom/dsutils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """DICOM dataset utility functions."""
 
 from io import BytesIO
 import logging
 from pathlib import Path
-from typing import Optional, List, Tuple
 import zlib
 
 from pydicom import Dataset
 from pydicom.dataset import FileMetaDataset
 from pydicom.dataelem import DataElement
 from pydicom.filebase import DicomBytesIO
 from pydicom.filereader import read_dataset, read_preamble
-from pydicom.filewriter import write_dataset
+from pydicom.filewriter import write_dataset, write_file_meta_info
 from pydicom.tag import BaseTag
 from pydicom.uid import UID
 
 from pynetdicom import PYNETDICOM_IMPLEMENTATION_UID, PYNETDICOM_IMPLEMENTATION_VERSION
 from pynetdicom.utils import pretty_bytes
 
 
-LOGGER = logging.getLogger("pynetdicom.dsutils")
+LOGGER = logging.getLogger(__name__)
 
 
 def create_file_meta(
     *,
     sop_class_uid: UID,
     sop_instance_uid: UID,
     transfer_syntax: UID,
@@ -124,15 +123,15 @@
 
     # Decode the dataset
     return read_dataset(bytestring, is_implicit_vr, is_little_endian)
 
 
 def encode(
     ds: Dataset, is_implicit_vr: bool, is_little_endian: bool, deflated: bool = False
-) -> Optional[bytes]:
+) -> bytes | None:
     """Encode a *pydicom* :class:`~pydicom.dataset.Dataset` `ds`.
 
     .. versionchanged:: 1.5
 
         Added `deflated` keyword parameter
 
     Parameters
@@ -178,15 +177,29 @@
         bytestring = compressor.compress(bytestring)
         bytestring += compressor.flush()
         bytestring += b"\x00" if len(bytestring) % 2 else b""
 
     return bytestring
 
 
-def pretty_dataset(ds: Dataset, indent: int = 0, indent_char: str = "  ") -> List[str]:
+def encode_file_meta(file_meta: FileMetaDataset) -> bytes:
+    """Return the encoded File Meta Information elements in `file_meta`.
+
+    .. versionadded:: 2.1
+
+    """
+
+    buffer = DicomBytesIO()
+    buffer.is_little_endian = True
+    buffer.is_implicit_VR = False
+    write_file_meta_info(buffer, file_meta)
+    return buffer.getvalue()
+
+
+def pretty_dataset(ds: Dataset, indent: int = 0, indent_char: str = "  ") -> list[str]:
     """Return a list of pretty dataset strings.
 
     .. versionadded:: 1.5
 
     Parameters
     ----------
     ds : pydicom.dataset.Dataset
@@ -257,23 +270,24 @@
         elif elem.VR == "SQ":
             # Sequence elements
             if elem.VM == 1:
                 value = f"(Sequence with {len(elem.value)} item)"
             else:
                 value = f"(Sequence with {len(elem.value)} items)"
 
-    except Exception as exc:
+    except Exception:
         value = "(pynetdicom failed to beautify value)"
 
-    return "({:04X},{:04X}) {} {: <40} # {} {}".format(
-        elem.tag.group, elem.tag.element, elem.VR, value, elem.VM, elem.keyword
+    return (
+        f"({elem.tag.group:04X},{elem.tag.element:04X}) {elem.VR} "
+        f"{value: <40} # {elem.VM} {elem.keyword}"
     )
 
 
-def split_dataset(path: Path) -> Tuple[Dataset, int]:
+def split_dataset(path: Path) -> tuple[Dataset, int]:
     """Return the file meta elements and the offset to the start of the dataset
 
     .. versionadded:: 2.0
 
     Parameters
     ----------
     path : pathlib.Path
@@ -283,15 +297,15 @@
     -------
     pydicom.dataset.Dataset, int
         The File Meta elements as a Dataset instance and the byte offset to
         the start of the dataset itself. The File Meta dataset may be empty if
         no File Meta is present.
     """
 
-    def _not_group_0002(tag: BaseTag, VR: Optional[str], length: int) -> bool:
+    def _not_group_0002(tag: BaseTag, VR: str | None, length: int) -> bool:
         """Return True if the tag is not in group 0x0002, False otherwise."""
         return tag.group != 2
 
     with open(path, "rb") as fp:
         read_preamble(fp, False)
         file_meta = read_dataset(
             fp, is_implicit_VR=False, is_little_endian=True, stop_when=_not_group_0002
```

### Comparing `pynetdicom-2.0.2/pynetdicom/dul.py` & `pynetdicom-2.1.0/pynetdicom/dul.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Implements the DICOM Upper Layer service provider.
 """
 
 import logging
 import queue
-import socket
 import struct
 from threading import Thread
 import time
 from typing import TYPE_CHECKING, Optional, Tuple, cast, Dict, Type, Union
 
 from pynetdicom import evt
 from pynetdicom.fsm import StateMachine
@@ -37,15 +36,15 @@
 if TYPE_CHECKING:  # pragma: no cover
     from pynetdicom.association import Association
     from pynetdicom.transport import AssociationSocket
 
     _QueueType = queue.Queue[Union[_PDUPrimitiveType, T_CONNECT]]
 
 
-LOGGER = logging.getLogger("pynetdicom.dul")
+LOGGER = logging.getLogger(__name__)
 
 
 class DULServiceProvider(Thread):
     """The DICOM Upper Layer Service Provider.
 
     Attributes
     ----------
@@ -240,15 +239,15 @@
 
         return True
 
     def _read_pdu_data(self) -> None:
         """Read PDU data sent by the peer from the socket.
 
         Receives the PDU, attempts to decode it, places the corresponding
-        event in the event queue and and converts it a primitive (if possible).
+        event in the event queue and converts it a primitive (if possible).
 
         If the decoding and conversion is successful then `pdu` and `primitive`
         are set to corresponding class instances.
 
         **Events Emitted**
 
         - Evt6: A-ASSOCIATE-RQ PDU received
@@ -263,28 +262,28 @@
         """
         bytestream = bytearray()
         self.socket = cast("AssociationSocket", self.socket)
 
         # Try and read the PDU type and length from the socket
         try:
             bytestream.extend(self.socket.recv(6))
-        except (socket.error, socket.timeout) as exc:
+        except (OSError, TimeoutError) as exc:
             # READ_PDU_EXC_A
             LOGGER.error("Connection closed before the entire PDU was received")
             LOGGER.exception(exc)
             # Evt17: Transport connection closed
             self.event_queue.put("Evt17")
             return
 
         try:
             # Byte 1 is always the PDU type
             # Byte 2 is always reserved
             # Bytes 3-6 are always the PDU length
             pdu_type, _, pdu_length = struct.unpack(">BBL", bytestream)
-        except struct.error as exc:
+        except struct.error:
             # READ_PDU_EXC_B
             # LOGGER.error("Insufficient data received to decode the PDU")
             # Evt17: Transport connection closed
             self.event_queue.put("Evt17")
             return
 
         # If the `pdu_type` is unrecognised
@@ -294,15 +293,15 @@
             # Evt19: Unrecognised or invalid PDU received
             self.event_queue.put("Evt19")
             return
 
         # Try and read the rest of the PDU
         try:
             bytestream += self.socket.recv(pdu_length)
-        except (socket.error, socket.timeout) as exc:
+        except (OSError, TimeoutError) as exc:
             # READ_PDU_EXC_D
             LOGGER.error("Connection closed before the entire PDU was received")
             LOGGER.exception(exc)
             # Evt17: Transport connection closed
             self.event_queue.put("Evt17")
             return
```

### Comparing `pynetdicom-2.0.2/pynetdicom/events.py` & `pynetdicom-2.1.0/pynetdicom/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,82 +1,69 @@
 """Module used to support events and event handling, not to be confused with
 the state machine events.
 """
 
 from datetime import datetime
+from io import BytesIO
 import inspect
 import logging
 from pathlib import Path
 import sys
-from typing import (
-    Union,
-    Callable,
-    Any,
-    Tuple,
-    List,
-    NamedTuple,
-    Optional,
-    TYPE_CHECKING,
-    Dict,
-    cast,
-    Iterator,
-)
+from typing import Callable, Any, NamedTuple, TYPE_CHECKING, cast, Iterator, Union
 
 from pydicom.dataset import Dataset, FileMetaDataset
+from pynetdicom.dimse_primitives import C_STORE
 from pydicom.filereader import dcmread
 from pydicom.tag import BaseTag
 from pydicom.uid import UID
 
-from pynetdicom.dsutils import decode, create_file_meta
+from pynetdicom.dsutils import decode, create_file_meta, encode_file_meta
 
 if TYPE_CHECKING:  # pragma: no cover
     from pynetdicom.association import Association
     from pynetdicom.dimse_messages import DIMSEMessage
     from pynetdicom.dimse_primitives import (
         C_ECHO,
         C_FIND,
         C_GET,
         C_MOVE,
-        C_STORE,
         N_ACTION,
         N_CREATE,
         N_DELETE,
         N_EVENT_REPORT,
         N_GET,
         N_SET,
     )
     from pynetdicom.pdu import _PDUType
     from pynetdicom.pdu_primitives import SOPClassCommonExtendedNegotiation
     from pynetdicom.presentation import PresentationContextTuple
 
-    _RequestType = Union[
-        C_ECHO,
-        C_FIND,
-        C_GET,
-        C_MOVE,
-        C_STORE,
-        N_ACTION,
-        N_CREATE,
-        N_DELETE,
-        N_EVENT_REPORT,
-        N_GET,
-        N_SET,
-    ]
+    _RequestType = (
+        C_ECHO
+        | C_FIND
+        | C_GET
+        | C_MOVE
+        | C_STORE
+        | N_ACTION
+        | N_CREATE
+        | N_DELETE
+        | N_EVENT_REPORT
+        | N_GET
+        | N_SET
+    )
 
 
-LOGGER = logging.getLogger("pynetdicom.events")
+LOGGER = logging.getLogger(__name__)
 
 
 EventType = Union["NotificationEvent", "InterventionEvent"]
-EventHandlerType = Union[
-    Tuple[EventType, Callable], Tuple[EventType, Callable, List[Any]]
-]
-_BasicReturnType = Union[Dataset, int]
-_DatasetReturnType = Tuple[_BasicReturnType, Optional[Dataset]]
-_IteratorType = Iterator[Tuple[_BasicReturnType, Optional[Dataset]]]
+EventHandlerType = tuple[EventType, Callable] | tuple[EventType, Callable, list[Any]]
+_BasicReturnType = Dataset | int
+_DatasetReturnType = tuple[_BasicReturnType, Dataset | None]
+_IteratorType = Iterator[tuple[_BasicReturnType, Dataset | None]]
 
 
 # Notification events
 #   No returns/yields needed, can have multiple handlers per event
 class NotificationEvent(NamedTuple):
     """Representation of a notification event.
 
@@ -218,36 +205,35 @@
     ii[1]
     for ii in inspect.getmembers(
         sys.modules[__name__], lambda x: isinstance(x, NotificationEvent)
     )
 ]
 
 
-_HandlerBase = Tuple[Callable, Optional[List[Any]]]
-_NotificationHandlerAttr = List[_HandlerBase]
+_HandlerBase = tuple[Callable, list[Any] | None]
+_NotificationHandlerAttr = list[_HandlerBase]
 _InterventionHandlerAttr = _HandlerBase
-HandlerArgType = Union[_NotificationHandlerAttr, _InterventionHandlerAttr]
-_HandlerAttr = Dict[EventType, HandlerArgType]
+HandlerArgType = _NotificationHandlerAttr | _InterventionHandlerAttr
+_HandlerAttr = dict[EventType, HandlerArgType]
 
 
 def _add_handler(
     event: EventType, handlers_attr: _HandlerAttr, handler_arg: _HandlerBase
 ) -> None:
     """Add a handler to an object's handler recording attribute.
 
     Parameters
     ----------
     event : NotificationEvent or InterventionEvent
         The event the handler should be bound to.
     handlers_attr : dict
-        The object attribute of {event: Union[
-            [(handler, Optional[args])],
-            (handler, Optional[args])
-        ]} used to record bindings.
-    handler_arg : Tuple[Callable, Optional[List[Any]]]
+        The object attribute of
+        {event: [(handler, None | args)] | (handler, None | args)} used to
+        record bindings.
+    handler_arg : tuple[Callable, None | list[Any]]
         The handler and optional arguments to be bound.
     """
     if isinstance(event, NotificationEvent):
         if event not in handlers_attr:
             handlers_attr[event] = []
 
         if handler_arg not in handlers_attr[event]:
@@ -266,20 +252,16 @@
 
     Parameters
     ----------
     event : NotificationEvent or InterventionEvent
         The event the handler should be unbound from.
     handlers_attr : dict
         The object attribute of
-        {
-            event: Union[
-                List[(handler, Optional[args])],
-                (handler, Optional[args])
-            ]
-        } used to record bindings.
+        {event: list[(handler, None | args)] | (handler, None | args)} used
+        to record bindings.
     handler_arg : Callable
         The handler to be unbound.
     """
     if event not in handlers_attr:
         return
 
     if isinstance(event, NotificationEvent):
@@ -316,16 +298,16 @@
         EVT_N_GET: _n_get_handler,
         EVT_N_SET: _n_set_handler,
     }
     return handlers[event]
 
 
 def trigger(
-    assoc: "Association", event: EventType, attrs: Optional[Dict[str, Any]] = None
-) -> Optional[Any]:
+    assoc: "Association", event: EventType, attrs: dict[str, Any] | None = None
+) -> Any | None:
     """Trigger an `event` and call any bound handler(s).
 
     .. versionadded:: 1.3
 
     Notification events can be bound to multiple handlers, intervention events
     can only be bound to a single handler.
 
@@ -431,15 +413,15 @@
         the actual event that this object represents.
     """
 
     def __init__(
         self,
         assoc: "Association",
         event: EventType,
-        attrs: Optional[Dict[str, Any]] = None,
+        attrs: dict[str, Any] | None = None,
     ) -> None:
         """Create a new Event.
 
         Parameters
         ----------
         assoc : association.Association
             The association in which the event occurred.
@@ -450,16 +432,16 @@
             :class:`Event`'s  attributes.
         """
         self.assoc = assoc
         self._event = event
         self.timestamp = datetime.now()
 
         # Only decode a dataset when necessary
-        self._hash: Optional[int] = None
-        self._decoded: Optional[Dataset] = None
+        self._hash: int | None = None
+        self._decoded: Dataset | None = None
 
         # Define type hints for dynamic attributes
         self.request: "_RequestType"
         self._is_cancelled: Callable[[int], bool]
         self.context: "PresentationContextTuple"
         self.current_state: str
         self.fsm_event: str
@@ -499,15 +481,15 @@
         msg = (
             "The corresponding event is not an N-ACTION request and has no "
             "'Action Information' parameter"
         )
         return self._get_dataset("ActionInformation", msg)
 
     @property
-    def action_type(self) -> Optional[int]:
+    def action_type(self) -> int | None:
         """Return an N-ACTION request's `Action Type ID` as an :class:`int`.
 
         .. versionadded:: 1.4
 
         Returns
         -------
         int or None
@@ -524,15 +506,15 @@
         except AttributeError:
             raise AttributeError(
                 "The corresponding event is not an N-ACTION request and has "
                 "no 'Action Type ID' parameter"
             )
 
     @property
-    def attribute_identifiers(self) -> List[BaseTag]:
+    def attribute_identifiers(self) -> list[BaseTag]:
         """Return an N-GET request's `Attribute Identifier List` as a
         :class:`list` of *pydicom* :class:`~pydicom.tag.BaseTag`.
 
         Returns
         -------
         list of pydicom.tag.BaseTag
             The (0000,1005) *Attribute Identifier List* tags, may be an empty
@@ -640,14 +622,74 @@
                 "The corresponding event is either not a C-STORE request or "
                 "'STORE_RECV_CHUNKED_DATASET' is not True."
             )
             raise AttributeError(msg)
 
         return cast(Path, path)
 
+    def encoded_dataset(self, include_meta: bool = True) -> bytes:
+        """Return the encoded C-STORE dataset sent by the peer without first
+        decoding it.
+
+        .. versionadded:: 2.1
+
+        Examples
+        --------
+        Retrieve the encoded dataset as sent by the peer::
+
+          def handle_store(event: pynetdicom.events.Event) -> int:
+              stream: bytes = event.encoded_dataset(include_meta=False)
+
+              return 0x0000
+
+        Write the encoded dataset to file in the DICOM File Format without
+        having to first decode it::
+
+          def handle_store(event: pynetdicom.events.Event, dst: pathlib.Path) -> int:
+              with dst.open("wb") as f:
+                  f.write(event.encoded_dataset())
+
+              return 0x0000
+
+        Parameters
+        ----------
+        include_meta : bool, optional
+            If ``True`` (default) then include the encoded DICOM preamble,
+            prefix and file meta information with the returned bytestream.
+
+        Returns
+        -------
+        bytes
+            The encoded dataset as sent by the peer, with or without the file
+            meta information.
+
+        Raises
+        ------
+        AttributeError
+            If the corresponding event is not a C-STORE request.
+        """
+        try:
+            request = cast(C_STORE, self.request)
+            stream = cast(BytesIO, request.DataSet).getvalue()
+        except AttributeError:
+            raise AttributeError(
+                "The corresponding event is not a C-STORE request and has no "
+                "'Data Set' parameter"
+            )
+
+        if not include_meta:
+            return stream
+
+        return b"".join((
+            b"\x00" * 128,
+            b"DICM",
+            encode_file_meta(self.file_meta),
+            stream,
+        ))
+
     @property
     def event(self) -> EventType:
         """Return the corresponding event.
 
         .. versionadded:: 1.4
 
         Returns
@@ -682,15 +724,15 @@
         msg = (
             "The corresponding event is not an N-EVENT-REPORT request and has "
             "no 'Event Information' parameter"
         )
         return self._get_dataset("EventInformation", msg)
 
     @property
-    def event_type(self) -> Optional[int]:
+    def event_type(self) -> int | None:
         """Return an N-EVENT-REPORT request's `Event Type ID` as an
         :class:`int`.
 
         .. versionadded:: 1.4
 
         Returns
         -------
@@ -743,15 +785,16 @@
 
             >>> ds = event.dataset
             >>> ds.file_meta = event.file_meta
             >>> ds.save_as('example.dcm', write_like_original=False)
 
         Encode the File Meta Information in a new file and append the encoded
         *Data Set* to it. This skips having to decode/re-encode the *Data Set*
-        as in the previous example.
+        as in the previous example (or alternatively, just use the
+        :meth:`~pynetdicom.events.Event.encoded_dataset` method).
 
         .. code-block:: python
 
            >>> from pydicom.filewriter import write_file_meta_info
            >>> with open('example.dcm', 'wb') as f:
            ...     f.write(b'\x00' * 128)
            ...     f.write(b'DICM')
@@ -833,15 +876,15 @@
             else:
                 # Dataset-like parameter hasn't been used
                 self._decoded = Dataset()
 
             self._hash = hash(bytestream)
             return self._decoded
 
-        except AttributeError as exc:
+        except AttributeError:
             pass
 
         raise AttributeError(exc_msg)
 
     @property
     def identifier(self) -> Dataset:
         """Return a C-FIND, C-GET or C-MOVE request's `Identifier` as a
@@ -941,15 +984,15 @@
         msg = (
             "The corresponding event is not an N-SET request and has no "
             "'Modification List' parameter"
         )
         return self._get_dataset("ModificationList", msg)
 
     @property
-    def move_destination(self) -> Optional[str]:
+    def move_destination(self) -> str | None:
         """Return a C-MOVE request's `Move Destination` as :class:`str`.
 
         .. versionadded:: 1.4
 
         .. versionchanged:: 2.0
 
             Changed to return :class:`str` and trailing spaces removed.
@@ -972,46 +1015,46 @@
             raise AttributeError(
                 "The corresponding event is not a C-MOVE request and has no "
                 "'Move Destination' parameter"
             )
 
 
 # Default extended negotiation event handlers
-def _async_ops_handler(event: Event) -> Tuple[int, int]:
+def _async_ops_handler(event: Event) -> tuple[int, int]:
     """Default handler for when an Asynchronous Operations Window Negotiation
     item is include in the association request.
 
     See _handlers.doc_handle_async for detailed documentation.
     """
     raise NotImplementedError(
         "No handler has been bound to 'evt.EVT_ASYNC_OPS', so no "
         "Asynchronous Operations Window Negotiation response will be "
         "sent"
     )
 
 
-def _sop_common_handler(event: Event) -> Dict[UID, "SOPClassCommonExtendedNegotiation"]:
+def _sop_common_handler(event: Event) -> dict[UID, "SOPClassCommonExtendedNegotiation"]:
     """Default handler for when one or more SOP Class Common Extended
     Negotiation items are included in the association request.
 
     See _handlers.doc_handle_sop_common for detailed documentation.
     """
     return {}
 
 
-def _sop_extended_handler(event: Event) -> Dict[UID, bytes]:
+def _sop_extended_handler(event: Event) -> dict[UID, bytes]:
     """Default handler for when one or more SOP Class Extended Negotiation
     items are included in the association request.
 
     See _handlers.doc_handler_sop_extended for detailed documentation.
     """
     return {}
 
 
-def _user_identity_handler(event: Event) -> Tuple[bool, Optional[bytes]]:
+def _user_identity_handler(event: Event) -> tuple[bool, bytes | None]:
     """Default handler for when a user identity negotiation item is included
     with the association request.
 
     See _handlers.doc_handler_userid for detailed documentation.
     """
     raise NotImplementedError(
         "No handler has been bound to 'evt.EVT_USER_ID', so the User Identity "
```

### Comparing `pynetdicom-2.0.2/pynetdicom/fsm.py` & `pynetdicom-2.1.0/pynetdicom/fsm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 The DUL's finite state machine representation.
 """
+
 import logging
 import queue
 from typing import TYPE_CHECKING, cast
 
 from pynetdicom import evt
 from pynetdicom.pdu import (
     A_ASSOCIATE_RQ,
@@ -20,15 +21,15 @@
 
 if TYPE_CHECKING:  # pragma: no cover
     from pynetdicom.dul import DULServiceProvider
     from pynetdicom.transport import AssociationSocket
     from pynetdicom.pdu_primitives import A_ASSOCIATE, P_DATA, A_RELEASE
 
 
-LOGGER = logging.getLogger("pynetdicom.sm")
+LOGGER = logging.getLogger(__name__)
 
 
 class InvalidEventError(Exception):
     """Exception for use when an invalid event occurs for a given state."""
 
     pass
 
@@ -1091,15 +1092,15 @@
         "Issue A-RELEASE indication (release collision): if "
         "association-requestor, next state is Sta9, if not next "
         "state is Sta10",
         AR_8,
         ("Sta9", "Sta10"),
     ),
     "AR-9": ("Send A-RELEASE-RP PDU", AR_9, "Sta11"),
-    "AR-10": ("Issue A-RELEASE confimation primitive", AR_10, "Sta12"),
+    "AR-10": ("Issue A-RELEASE confirmation primitive", AR_10, "Sta12"),
     # Association abort related actions
     "AA-1": (
         "Send A-ABORT PDU (service-user source) and start (or "
         "restart if already started) ARTIM timer",
         AA_1,
         "Sta13",
     ),
```

### Comparing `pynetdicom-2.0.2/pynetdicom/pdu.py` & `pynetdicom-2.1.0/pynetdicom/pdu.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         P_DATA,
         A_RELEASE,
         A_ABORT,
         A_P_ABORT,
     )
 
 
-LOGGER = logging.getLogger("pynetdicom.pdu")
+LOGGER = logging.getLogger(__name__)
 
 _PDVItem = List[PresentationDataValueItem]
 _AbortType = Union["A_ABORT", "A_P_ABORT"]
 _PDUType = Union[
     "A_ASSOCIATE_RQ",
     "A_ASSOCIATE_AC",
     "A_ASSOCIATE_RJ",
@@ -271,39 +271,38 @@
 
         return bytestream
 
     @staticmethod
     def _wrap_encode_str(value: str, pad: int = 0) -> bytes:
         """Return `value` as ASCII encoded :class:`bytes`.
 
-         Each component of Application Context, Abstract Syntax and Transfer
-         Syntax UIDs should be encoded as a ISO 646:1990-Basic G0 Set Numeric
-         String (characters 0-9), with each component separated by '.' (0x2e)
-        .
-
-         'ascii' is chosen because this is the codec Python uses for ISO 646
-         [3]_.
-
-         Parameters
-         ----------
-         value : str
-             The ASCII string to be encoded.
-         pad : int, optional
-             The amount of trailing padding to be used (default ``0``).
-
-         Returns
-         -------
-         bytes
-             The encoded `value`.
-
-         References
-         ----------
-         * DICOM Standard, Part 8, :dcm:`Annex F <part08/chapter_F.html>`
-         * `Python 3 codecs module
-           <https://docs.python.org/2/library/codecs.html#standard-encodings>`_
+        Each component of Application Context, Abstract Syntax and Transfer
+        Syntax UIDs should be encoded as a ISO 646:1990-Basic G0 Set Numeric
+        String (characters 0-9), with each component separated by '.' (0x2e).
+
+        'ascii' is chosen because this is the `codec Python uses
+        <https://docs.python.org/3/library/codecs.html>`_ for ISO 646.
+
+        Parameters
+        ----------
+        value : str
+            The ASCII string to be encoded.
+        pad : int, optional
+            The maximum amount of trailing padding to be used (default ``0``).
+
+        Returns
+        -------
+        bytes
+            The encoded `value`.
+
+        References
+        ----------
+        * DICOM Standard, Part 8, :dcm:`Annex F <part08/chapter_F.html>`
+        * `Python codecs module
+           <https://docs.python.org/3/library/codecs.html>`_
         """
         return value.ljust(pad).encode("ascii", errors="strict")
 
     def _wrap_generate_items(self, bytestream: bytes) -> List[PDUItem]:
         """Return a list of decoded PDU items generated from `bytestream`."""
         item_list = []
         for item_type, item_bytes in self._generate_items(bytestream):
@@ -892,16 +891,16 @@
         from pynetdicom.pdu_primitives import A_ASSOCIATE
 
         primitive = A_ASSOCIATE()
 
         # The two reserved parameters at byte offsets 11 and 27 shall be set
         #    to called and calling AET byte the value shall not be
         #   tested when received (PS3.8 Table 9-17)
-        primitive.called_ae_title = self.reserved_aet
-        primitive.calling_ae_title = self.reserved_aec
+        primitive._called_ae_title = self.reserved_aet
+        primitive._calling_ae_title = self.reserved_aec
 
         for item in self.variable_items:
             # Add application context
             if isinstance(item, ApplicationContextItem):
                 primitive.application_context_name = item.application_context_name
 
             # Add presentation contexts
@@ -1544,15 +1543,15 @@
             encoded data as bytes.
 
         Notes
         -----
         **Encoding**
         When encoded, a Presentation Data Value Item has the following
         structure, taken from Table 9-23 (offset shown with Python
-        indexing). The item is encoded using Big Endian, but the encoding of
+        indexing). The item is encoded using Big Endian, but the encoding
         of the presentation data message fragments is dependent on the
         negotiated transfer syntax.
 
         +--------+-------------+-------------------------+
         | Offset | Length      | Description             |
         +========+=============+=========================+
         | 0      | 4           | Item length             |
```

### Comparing `pynetdicom-2.0.2/pynetdicom/pdu_items.py` & `pynetdicom-2.1.0/pynetdicom/pdu_items.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         SCP_SCU_RoleSelectionNegotiation,
         UserIdentityNegotiation,
         AsynchronousOperationsWindowNegotiation,
         _UserInformationPrimitiveType,
     )
 
 
-LOGGER = logging.getLogger("pynetdicom.pdu_items")
+LOGGER = logging.getLogger(__name__)
 
 # Predefine some structs to make decoding and encoding faster
 UCHAR = Struct("B")
 UINT2 = Struct(">H")
 UINT4 = Struct(">I")
 
 UNPACK_UCHAR = UCHAR.unpack
@@ -399,15 +399,15 @@
         return unpacker(bytestream)[0]
 
 
 # A-ASSOCIATE-RQ and -AC items
 class ApplicationContextItem(PDUItem):
     """An Application Context Item.
 
-    An Application Context explicitly defines the set of appliation service
+    An Application Context explicitly defines the set of application service
     elements, related options and any other information necessary for the
     inter-working of Application Entities on an association.
 
     Notes
     -----
     An Application Context Item requires the following parameters:
 
@@ -753,20 +753,19 @@
     def transfer_syntax(self) -> List[UID]:
         """Return the *Transfer Syntax(es)*.
 
         Returns
         -------
         list of pydicom.uid.UID
         """
-        syntaxes = []
-        for item in self.abstract_transfer_syntax_sub_items:
-            if isinstance(item, TransferSyntaxSubItem):
-                syntaxes.append(cast(UID, item.transfer_syntax_name))
-
-        return syntaxes
+        return [
+            cast(UID, item.transfer_syntax_name)
+            for item in self.abstract_transfer_syntax_sub_items
+            if isinstance(item, TransferSyntaxSubItem)
+        ]
 
 
 class PresentationContextItemAC(PDUItem):
     """A Presentation Context (AC) Ttem.
 
     Presentation Contexts (AC) Items are used by the association acceptor to
     signal which Abstract Syntaxes and Transfer Syntaxes have been accepted or
@@ -1078,19 +1077,15 @@
             - ImplementationVersionnameNotification
             - AsynchronousOperationsWindowNegotiation
             - SCP_SCU_RoleSelectionNegotiation
             - SOPClassExtendedNegotiation
             - SOPClassCommonExtendedNegotiation
             - UserIdentityNegotiation
         """
-        primitive = []
-        for item in self.user_data:
-            primitive.append(item.to_primitive())
-
-        return primitive
+        return [item.to_primitive() for item in self.user_data]
 
     @property
     def async_ops_window(self) -> Optional["AsynchronousOperationsWindowSubItem"]:
         """Return the *Asynchronous Operations Window Sub-item*, if
         available.
         """
         for item in self.user_data:
@@ -1098,20 +1093,19 @@
                 return item
 
         return None
 
     @property
     def common_ext_neg(self) -> List["SOPClassCommonExtendedNegotiationSubItem"]:
         """Return the *SOP Class Common Extended Negotiation Sub-items*."""
-        items = []
-        for item in self.user_data:
-            if isinstance(item, SOPClassCommonExtendedNegotiationSubItem):
-                items.append(item)
-
-        return items
+        return [
+            item
+            for item in self.user_data
+            if isinstance(item, SOPClassCommonExtendedNegotiationSubItem)
+        ]
 
     @property
     def _decoders(self) -> Any:
         """Return an iterable of tuples that contain field decoders.
 
         Returns
         -------
@@ -1146,20 +1140,19 @@
             ("item_length", PACK_UINT2, []),
             ("user_data", self._wrap_encode_items, []),
         ]
 
     @property
     def ext_neg(self) -> List["SOPClassExtendedNegotiationSubItem"]:
         """Return the *SOP Class Extended Negotiation Sub-items*."""
-        items = []
-        for item in self.user_data:
-            if isinstance(item, SOPClassExtendedNegotiationSubItem):
-                items.append(item)
-
-        return items
+        return [
+            item
+            for item in self.user_data
+            if isinstance(item, SOPClassExtendedNegotiationSubItem)
+        ]
 
     @property
     def implementation_class_uid(self) -> Optional[UID]:
         """Return the item's *Implementation Class UID* field value, if
         available.
         """
         for item in self.user_data:
@@ -2932,19 +2925,15 @@
 
         s.append("")
 
         return "\n".join(s)
 
     def _wrap_generate_items(self, b: bytes) -> List[UID]:  # type: ignore
         """Return a list of UID items generated from `bytestream`."""
-        item_list = []
-        for uid in self._generate_items(b):
-            item_list.append(uid)
-
-        return item_list
+        return [uid for uid in self._generate_items(b)]
 
     def _wrap_list(self, uid_list: List[UID]) -> bytes:
         """Return `uid_list` encoded as bytes.
 
         Parameters
         ----------
         uid_list : list of pydicom.uid.UID
```

### Comparing `pynetdicom-2.0.2/pynetdicom/pdu_primitives.py` & `pynetdicom-2.1.0/pynetdicom/pdu_primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Implementation of the service parameter primitives.
 """
+
 import logging
 from typing import Optional, List, Any, Union, Tuple, cast, Type
 
 from pydicom.uid import UID
 
 from pynetdicom._globals import OptionalUIDType
 from pynetdicom.pdu_items import (
@@ -18,15 +19,15 @@
     UserIdentitySubItemRQ,
     UserIdentitySubItemAC,
 )
 from pynetdicom.presentation import PresentationContext
 from pynetdicom.utils import validate_uid, decode_bytes, set_ae, set_uid
 from pynetdicom._globals import DEFAULT_MAX_LENGTH
 
-LOGGER = logging.getLogger("pynetdicom.pdu_primitives")
+LOGGER = logging.getLogger(__name__)
 
 _PDUPrimitiveType = Union["A_ASSOCIATE", "A_RELEASE", "A_ABORT", "A_P_ABORT", "P_DATA"]
 _UserInformationPrimitiveType = List[
     Union[
         "MaximumLengthNotification",
         "ImplementationClassUIDNotification",
         "ImplementationVersionNameNotification",
```

### Comparing `pynetdicom-2.0.2/pynetdicom/service_class.py` & `pynetdicom-2.1.0/pynetdicom/service_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,20 @@
 import logging
 import os
 import sys
 import traceback
 from types import TracebackType
 from typing import (
     TYPE_CHECKING,
-    Optional,
     Type,
     cast,
-    Union,
-    Tuple,
     Any,
     TypeVar,
     Iterator,
     Sequence,
-    Dict,
 )
 
 from pydicom.dataset import Dataset
 from pydicom.tag import Tag
 
 from pynetdicom import evt, _config
 from pynetdicom.dsutils import decode, encode, pretty_dataset
@@ -63,28 +59,28 @@
 if TYPE_CHECKING:  # pragma: no cover
     from pynetdicom.ae import ApplicationEntity
     from pynetdicom.association import Association
     from pynetdicom.dimse import DIMSEServiceProvider
     from pynetdicom.presentation import PresentationContext
     from pynetdicom.transport import AssociationSocket
 
-    _QR = Union[C_FIND, C_MOVE, C_GET]
+    _QR = C_FIND | C_MOVE | C_GET
 
 
-StatusType = Union[int, Dataset]
-DatasetType = Optional[Dataset]
-UserReturnType = Tuple[StatusType, DatasetType]
+StatusType = int | Dataset
+DatasetType = Dataset | None
+UserReturnType = tuple[StatusType, DatasetType]
 _T = TypeVar("_T", bound=DIMSEPrimitive)
-_ExcInfoType = Union[
-    Tuple[None, None, None], Tuple[Type[BaseException], BaseException, TracebackType]
-]
-DestinationType = Union[Tuple[str, int], Tuple[str, int, Dict[str, Any]]]
+_ExcInfoType = (
+    tuple[None, None, None] | tuple[Type[BaseException], BaseException, TracebackType]
+)
+DestinationType = tuple[str, int] | tuple[str, int, dict[str, Any]]
 
 
-LOGGER = logging.getLogger("pynetdicom.service-c")
+LOGGER = logging.getLogger(__name__)
 
 
 class attempt:
     """Context manager for sending replies when an exception is raised.
 
     The code within the context is executed, and if an exception is raised
     then it's logged and a DIMSE message is sent to the peer using the
@@ -104,18 +100,18 @@
         self._cx_id = cx_id
 
     def __enter__(self) -> "attempt":
         return self
 
     def __exit__(
         self,
-        exc_type: Optional[Type[BaseException]],
-        exc_val: Optional[BaseException],
-        exc_tb: Optional[TracebackType],
-    ) -> Optional[bool]:
+        exc_type: Type[BaseException] | None,
+        exc_val: BaseException | None,
+        exc_tb: TracebackType | None,
+    ) -> bool | None:
         if exc_type is None:
             # No exceptions raised
             return None
 
         # Exception raised within the context
         LOGGER.error(self.error_msg)
         LOGGER.exception(exc_val)
@@ -194,20 +190,25 @@
         Success
           | ``0x0000`` Success
 
         Pending
           | ``0xFF00`` Matches are continuing, current match supplied
           | ``0xFF01`` Matches are continuing, warning
 
+        Warning
+          | ``0xB001`` Matching reached response limit, subsequent request may
+            return additional matches
+
         Cancel
           | ``0xFE00`` Cancel
 
         Failure
           | ``0x0122`` SOP class not supported
           | ``0xA700`` Out of resources
+          | ``0xA710`` Invalid prior record key
           | ``0xA900`` Identifier does not match SOP class
           | ``0xC000`` to ``0xCFFF`` Unable to process
 
         References
         ----------
 
         * DICOM Standard, Part 4, :dcm:`Annex C<part04/chapter_C.html>`
@@ -276,24 +277,24 @@
             generator = iter([(0x0000, None)])
 
         ii = -1  # So if there are no results, log below doesn't break
         # Iterate through the results
         for ii, (result, exc) in enumerate(self._wrap_handler(generator)):
             # Reset the response Identifier
             rsp.Identifier = None
-            dataset: Optional[Dataset]
+            dataset: Dataset | None
             rsp_status: StatusType
 
             # Exception raised by user's generator
             if exc:
                 LOGGER.error("Exception in handler bound to 'evt.EVT_C_FIND'")
                 LOGGER.error(
                     "\nTraceback (most recent call last):\n"
                     + "".join(traceback.format_tb(exc[2]))
-                    + f"{exc[0].__name__}: {str(exc[1])}"  # type: ignore
+                    + f"{exc[0].__name__}: {exc[1]}"  # type: ignore
                 )
                 rsp_status = 0xC311
                 dataset = None
             else:
                 (rsp_status, dataset) = cast(UserReturnType, result)
 
             # Event handler has aborted or released
@@ -312,29 +313,40 @@
 
             if status[0] == STATUS_CANCEL:
                 # If cancel, then dataset is None
                 LOGGER.info("Received C-CANCEL-FIND RQ from peer")
                 LOGGER.info(f"Find SCP Response {ii + 1}: 0x{rsp.Status:04X} (Cancel)")
                 self.dimse.send_msg(rsp, cx_id)
                 return
-            elif status[0] == STATUS_FAILURE:
+
+            if status[0] == STATUS_FAILURE:
                 # If failed, then dataset is None
                 LOGGER.info(
                     f"Find SCP Response {ii + 1}: 0x{rsp.Status:04X} "
                     f"(Failure - {status[1]})"
                 )
                 self.dimse.send_msg(rsp, cx_id)
                 return
-            elif status[0] == STATUS_SUCCESS:
+
+            if status[0] == STATUS_SUCCESS:
                 # User isn't supposed to send these, but handle anyway
                 # If success, then dataset is None
                 LOGGER.info(f"Find SCP Response {ii + 1}: 0x0000 (Success)")
                 self.dimse.send_msg(rsp, cx_id)
                 return
-            elif status[0] == STATUS_PENDING:
+
+            if status[0] == STATUS_WARNING:
+                LOGGER.info(
+                    f"Find SCP Response {ii + 1}: 0x{rsp.Status:04X} "
+                    f"(Warning - {status[1]})"
+                )
+                self.dimse.send_msg(rsp, cx_id)
+                continue
+
+            if status[0] == STATUS_PENDING:
                 # If pending, `dataset` is the Identifier
                 dataset = cast(Dataset, dataset)
                 enc = encode(
                     dataset,
                     transfer_syntax.is_implicit_VR,
                     transfer_syntax.is_little_endian,
                     transfer_syntax.is_deflated,
@@ -1299,15 +1311,15 @@
         """
         msg = (
             f"No service class has been implemented for the "
             f"SOP Class UID '{context.abstract_syntax}'"
         )
         raise NotImplementedError(msg)
 
-    def validate_status(self, status: Union[int, Dataset], rsp: _T) -> _T:
+    def validate_status(self, status: int | Dataset, rsp: _T) -> _T:
         """Validate `status` and set `rsp.Status` accordingly.
 
         Parameters
         ----------
         status : pydicom.dataset.Dataset or int
             A Dataset containing a Status element or an int.
         rsp : dimse_primitive
@@ -1348,22 +1360,22 @@
             #   a valid status type
             rsp.Status = 0xC002
 
         if not self.is_valid_status(cast(int, rsp.Status)):
             # Failure: Cannot Understand - Unknown status returned by the
             #   callback
             LOGGER.warning(
-                f"Unknown status value returned by callback - " f"0x{rsp.Status:04X}"
+                f"Unknown status value returned by callback - 0x{rsp.Status:04X}"
             )
 
         return rsp
 
     def _wrap_handler(
         self, handler: Iterator
-    ) -> Iterator[Union[Tuple[None, _ExcInfoType], Tuple[UserReturnType, None]]]:
+    ) -> Iterator[tuple[None, _ExcInfoType] | tuple[UserReturnType, None]]:
         """Wrap a generator handler to catch exceptions.
 
         Parameters
         ----------
         handler : generator
             A generator returned by a user's handler.
 
@@ -1383,15 +1395,15 @@
                 ):
                     LOGGER.debug(
                         "A-ABORT or A-RELEASE-RQ received during Q/R sub-operations"
                     )
                     return
 
                 yield (result, None)
-        except Exception as exc:
+        except Exception:
             yield (None, sys.exc_info())
 
 
 # Service Class implementations
 class VerificationServiceClass(ServiceClass):
     """Implementation of the Verification Service Class."""
 
@@ -1534,72 +1546,86 @@
         "PixelData",
         "FloatPixelData",
         "DoubleFloatPixelData",
         "PixelDataProviderURL",
         "SpectroscopyData",
         "EncapsulatedDocument",
     ]
-
-    def SCP(self, req: "_QR", context: "PresentationContext") -> None:
-        """The SCP implementation for the Query/Retrieve Service Class.
-
-        Parameters
-        ----------
-        req : dimse_primitives.C_FIND or C_GET or C_MOVE
-            The request primitive received from the peer.
-        context : presentation.PresentationContext
-            The presentation context that the SCP is operating under.
-        """
-        _find_uids = [
+    _SUPPORTED_UIDS = {
+        "C-FIND": [
             "1.2.840.10008.5.1.4.1.2.1.1",
             "1.2.840.10008.5.1.4.1.2.2.1",
             "1.2.840.10008.5.1.4.1.2.3.1",
             "1.2.840.10008.5.1.4.20.1",
             "1.2.840.10008.5.1.4.38.2",
             "1.2.840.10008.5.1.4.39.2",
             "1.2.840.10008.5.1.4.43.2",
             "1.2.840.10008.5.1.4.44.2",
             "1.2.840.10008.5.1.4.45.2",
             "1.2.840.10008.5.1.4.1.1.200.4",
-        ]
-        _get_uids = [
+            "1.2.840.10008.5.1.4.1.1.201.2",
+            "1.2.840.10008.5.1.4.1.1.201.6",
+        ],
+        "C-GET": [
             "1.2.840.10008.5.1.4.1.2.1.3",
             "1.2.840.10008.5.1.4.1.2.2.3",
             "1.2.840.10008.5.1.4.1.2.3.3",
             "1.2.840.10008.5.1.4.1.2.4.3",
             "1.2.840.10008.5.1.4.1.2.5.3",
             "1.2.840.10008.5.1.4.20.3",
             "1.2.840.10008.5.1.4.38.4",
             "1.2.840.10008.5.1.4.39.4",
             "1.2.840.10008.5.1.4.43.4",
             "1.2.840.10008.5.1.4.44.4",
             "1.2.840.10008.5.1.4.45.4",
             "1.2.840.10008.5.1.4.1.1.200.6",
-        ]
-        _move_uids = [
+            "1.2.840.10008.5.1.4.1.1.201.4",
+        ],
+        "C-MOVE": [
             "1.2.840.10008.5.1.4.1.2.1.2",
             "1.2.840.10008.5.1.4.1.2.2.2",
             "1.2.840.10008.5.1.4.1.2.3.2",
             "1.2.840.10008.5.1.4.1.2.4.2",
             "1.2.840.10008.5.1.4.20.2",
             "1.2.840.10008.5.1.4.38.3",
             "1.2.840.10008.5.1.4.39.3",
             "1.2.840.10008.5.1.4.43.3",
             "1.2.840.10008.5.1.4.44.3",
             "1.2.840.10008.5.1.4.45.3",
             "1.2.840.10008.5.1.4.1.1.200.5",
-        ]
+            "1.2.840.10008.5.1.4.1.1.201.3",
+        ],
+    }
+
+    def SCP(self, req: "_QR", context: "PresentationContext") -> None:
+        """The SCP implementation for the Query/Retrieve Service Class.
 
-        if isinstance(req, C_FIND) and context.abstract_syntax in _find_uids:
+        Parameters
+        ----------
+        req : dimse_primitives.C_FIND or C_GET or C_MOVE
+            The request primitive received from the peer.
+        context : presentation.PresentationContext
+            The presentation context that the SCP is operating under.
+        """
+        if (
+            isinstance(req, C_FIND)
+            and context.abstract_syntax in self._SUPPORTED_UIDS["C-FIND"]
+        ):
             self.statuses = QR_FIND_SERVICE_CLASS_STATUS
             self._c_find_scp(req, context)
-        elif isinstance(req, C_GET) and context.abstract_syntax in _get_uids:
+        elif (
+            isinstance(req, C_GET)
+            and context.abstract_syntax in self._SUPPORTED_UIDS["C-GET"]
+        ):
             self.statuses = QR_GET_SERVICE_CLASS_STATUS
             self._get_scp(req, context)
-        elif isinstance(req, C_MOVE) and context.abstract_syntax in _move_uids:
+        elif (
+            isinstance(req, C_MOVE)
+            and context.abstract_syntax in self._SUPPORTED_UIDS["C-MOVE"]
+        ):
             self.statuses = QR_MOVE_SERVICE_CLASS_STATUS
             self._move_scp(req, context)
         else:
             raise ValueError(
                 "The supplied abstract syntax is not valid for use with the "
                 "Query/Retrieve Service Class"
             )
@@ -1703,15 +1729,15 @@
 
             # Exception raised by user's generator
             if exc:
                 LOGGER.error("Exception in handler bound to 'evt.EVT_C_GET'")
                 LOGGER.error(
                     "\nTraceback (most recent call last):\n"
                     + "".join(traceback.format_tb(exc[2]))
-                    + f"{exc[0].__name__}: {str(exc[1])}"  # type: ignore
+                    + f"{exc[0].__name__}: {exc[1]}"  # type: ignore
                 )
                 rsp_status = 0xC411
                 dataset = None
             else:
                 (rsp_status, dataset) = cast(UserReturnType, result)
 
             # Event handler has aborted or released - after any yields
@@ -1867,18 +1893,17 @@
                         for base in repeaters:
                             tag = Tag(base[0] + rpt, base[1])
                             if tag in dataset:
                                 del dataset[tag]
 
                     if _bulk_data:
                         LOGGER.warning(
-                            f"The Query/Retrieve - Composite Instance "
-                            f"Retrieve Without Bulk Data service is "
-                            f"requested but a yielded dataset contains the "
-                            f"following (to be removed) bulk data "
+                            "The Query/Retrieve - Composite Instance Retrieve "
+                            "Without Bulk Data service is requested but a yielded "
+                            "dataset contains the following (to be removed) bulk data "
                             f"elements: {','.join(_bulk_data)}"
                         )
 
                 # Send `dataset` via C-STORE sub-operations over the existing
                 #   association and check that the response's Status exists and
                 #   is a known value
                 try:
@@ -1899,17 +1924,15 @@
 
                 if store_status_int is not None:
                     msg = (
                         f"Get SCP: Received Store SCP response "
                         f"0x{store_status_int:04X} ({store_status[0]})"
                     )
                 else:
-                    msg = (
-                        f"Get SCP: Received Store SCP response " f"({store_status[0]})"
-                    )
+                    msg = f"Get SCP: Received Store SCP response ({store_status[0]})"
                 LOGGER.info(msg)
 
                 # Update the C-STORE sub-operation result tracker
                 if store_status[0] == STATUS_FAILURE:
                     store_results[1] += 1
                     # Part 4, C.4.3.1.3.2
                     _add_failed_instance(dataset)
@@ -2081,16 +2104,16 @@
         with attempt(rsp, self.dimse, cx_id) as ctx:
             ctx.error_msg = (
                 "The handler bound to 'evt.EVT_C_MOVE' yielded an invalid "
                 "destination AE (addr, port) or (addr, port, kwargs) value"
             )
             ctx.error_status = 0xC515
             kwargs = {"ae_title": req.MoveDestination}
-            if len(destination) >= 3 and destination[2]:  # type: ignore
-                kwargs.update(destination[2])  # type: ignore
+            if len(destination) >= 3 and destination[2]:
+                kwargs.update(destination[2])
 
             store_assoc = self.ae.associate(
                 destination[0], destination[1], **kwargs  # type: ignore
             )
 
         if not ctx.success:
             return
@@ -2127,15 +2150,15 @@
 
             # Exception raised by handler
             if exc:
                 LOGGER.error("Exception in handler bound to 'evt.EVT_C_MOVE'")
                 LOGGER.error(
                     "\nTraceback (most recent call last):\n"
                     + "".join(traceback.format_tb(exc[2]))
-                    + f"{exc[0].__name__}: {str(exc[1])}"  # type: ignore
+                    + f"{exc[0].__name__}: {exc[1]}"  # type: ignore
                 )
                 rsp_status = 0xC511
                 dataset = None
             else:
                 (rsp_status, dataset) = cast(UserReturnType, result)
 
             # Event handler has aborted or released - during any status yields
@@ -2299,21 +2322,19 @@
                     LOGGER.warning("C-STORE sub-operation failed.")
                     LOGGER.error(str(exc))
                     store_status_int = None
                     store_status = (STATUS_FAILURE, "Unknown")
 
                 if store_status_int is not None:
                     msg = (
-                        f"Move SCP: Received Store SCP response "
+                        "Move SCP: Received Store SCP response "
                         f"0x{store_status_int:04X} ({store_status[0]})"
                     )
                 else:
-                    msg = (
-                        f"Move SCP: Received Store SCP response " f"({store_status[0]})"
-                    )
+                    msg = f"Move SCP: Received Store SCP response ({store_status[0]})"
 
                 LOGGER.info(msg)
 
                 # Update the C-STORE sub-operation result tracker
                 if store_status[0] == STATUS_FAILURE:
                     store_results[1] += 1
                     # Part 4, C.4.2.1.4.2
@@ -2375,28 +2396,31 @@
         self.dimse.send_msg(rsp, cx_id)
 
 
 class BasicWorklistManagementServiceClass(QueryRetrieveServiceClass):
     """Implementation of the Basic Worklist Management Service Class."""
 
     statuses = QR_FIND_SERVICE_CLASS_STATUS
+    _SUPPORTED_UIDS = {
+        "C-FIND": ["1.2.840.10008.5.1.4.31"],
+    }
 
     def SCP(self, req: "_QR", context: "PresentationContext") -> None:
         """The SCP implementation for Basic Worklist Management.
 
         Parameters
         ----------
         req : dimse_primitives.C_FIND
             The C-FIND request primitive received from the peer.
         context : presentation.PresentationContext
             The presentation context that the SCP is operating under.
         """
         if (
             isinstance(req, C_FIND)
-            and context.abstract_syntax == "1.2.840.10008.5.1.4.31"
+            and context.abstract_syntax in self._SUPPORTED_UIDS["C-FIND"]
         ):
             self._c_find_scp(req, context)
         else:
             raise ValueError(
                 "The supplied abstract syntax is not valid for use with the "
                 "Basic Worklist Management Service Class"
             )
@@ -2422,14 +2446,23 @@
 
 class ImplantTemplateQueryRetrieveServiceClass(QueryRetrieveServiceClass):
     """Implementation of the Implant Template QR Service."""
 
     pass
 
 
+class InventoryQueryRetrieveServiceClass(QueryRetrieveServiceClass):
+    """Implementation of the Inventory QR Service.
+
+    .. versionadded:: 2.1
+    """
+
+    pass
+
+
 class NonPatientObjectStorageServiceClass(StorageServiceClass):
     """Implementation of the Non-Patient Object Storage Service"""
 
     statuses = NON_PATIENT_SERVICE_CLASS_STATUS
 
 
 class ProtocolApprovalQueryRetrieveServiceClass(QueryRetrieveServiceClass):
@@ -2581,27 +2614,32 @@
             self.dimse.send_msg(rsp, cx_id)
 
 
 class SubstanceAdministrationQueryServiceClass(QueryRetrieveServiceClass):
     """Implementation of the Substance Administration Query Service"""
 
     statuses = SUBSTANCE_ADMINISTRATION_SERVICE_CLASS_STATUS
+    _SUPPORTED_UIDS = {
+        "C-FIND": ["1.2.840.10008.5.1.4.41", "1.2.840.10008.5.1.4.42"],
+    }
 
     def SCP(self, req: "_QR", context: "PresentationContext") -> None:
         """The SCP implementation for the Relevant Patient Information Query
         Service Class.
 
         Parameters
         ----------
         req : dimse_primitives.C_FIND
             The C-FIND request primitive sent by the peer.
         context : presentation.PresentationContext
             The presentation context that the SCP is operating under.
         """
-        uids = ["1.2.840.10008.5.1.4.41", "1.2.840.10008.5.1.4.42"]
-        if isinstance(req, C_FIND) and context.abstract_syntax in uids:
+        if (
+            isinstance(req, C_FIND)
+            and context.abstract_syntax in self._SUPPORTED_UIDS["C-FIND"]
+        ):
             self._c_find_scp(req, context)
         else:
             raise ValueError(
                 "The supplied abstract syntax is not valid for use with the "
                 "Substance Administration Query Service Class"
             )
```

### Comparing `pynetdicom-2.0.2/pynetdicom/service_class_n.py` & `pynetdicom-2.1.0/pynetdicom/service_class_n.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Implements the supported Service Classes that make use of DIMSE-N."""
 
 import logging
-from typing import TYPE_CHECKING, Union
+from typing import TYPE_CHECKING
 
 from pynetdicom.dimse_primitives import (
     N_ACTION,
     N_CREATE,
     N_DELETE,
     N_EVENT_REPORT,
     N_GET,
@@ -16,29 +16,31 @@
 from pynetdicom.status import (
     GENERAL_STATUS,
     APPLICATION_EVENT_LOGGING_SERVICE_CLASS_STATUS,
     MEDIA_CREATION_MANAGEMENT_SERVICE_CLASS_STATUS,
     PRINT_JOB_MANAGEMENT_SERVICE_CLASS_STATUS,
     PROCEDURE_STEP_STATUS,
     STORAGE_COMMITMENT_SERVICE_CLASS_STATUS,
+    STORAGE_MANAGEMENT_SERVICE_CLASS_STATUS,
     RT_MACHINE_VERIFICATION_SERVICE_CLASS_STATUS,
     UNIFIED_PROCEDURE_STEP_SERVICE_CLASS_STATUS,
 )
 
 if TYPE_CHECKING:  # pragma: no cover
     from pynetdicom.presentation import PresentationContext
 
-    _MCM = Union[N_CREATE, N_GET, N_ACTION]
-    _PJ = Union[N_CREATE, N_EVENT_REPORT, N_GET, N_SET, N_ACTION, N_DELETE]
-    _PS = Union[N_CREATE, N_EVENT_REPORT, N_GET, N_SET]
-    _SCS = Union[N_EVENT_REPORT, N_ACTION]
-    _UPS = Union[N_CREATE, N_EVENT_REPORT, N_GET, N_SET, N_ACTION, C_FIND]
+    _MCM = N_CREATE | N_GET | N_ACTION
+    _PJ = N_CREATE | N_EVENT_REPORT | N_GET | N_SET | N_ACTION | N_DELETE
+    _PS = N_CREATE | N_EVENT_REPORT | N_GET | N_SET
+    _SCS = N_EVENT_REPORT | N_ACTION
+    _SMS = N_ACTION | N_EVENT_REPORT
+    _UPS = N_CREATE | N_EVENT_REPORT | N_GET | N_SET | N_ACTION | C_FIND
 
 
-LOGGER = logging.getLogger("pynetdicom.service-n")
+LOGGER = logging.getLogger(__name__)
 
 
 class ApplicationEventLoggingServiceClass(ServiceClass):
     """Implementation of the Application Event Logging Service Class
 
     .. versionadded:: 1.4
     """
@@ -285,14 +287,43 @@
         else:
             raise ValueError(
                 f"Invalid DIMSE primitive '{req.__class__.__name__}' used "
                 f"with Storage Commitment"
             )
 
 
+class StorageManagementServiceClass(ServiceClass):
+    """Implementation of the Storage Management Service Class
+
+    .. versionadded:: 2.1
+    """
+
+    statuses = STORAGE_MANAGEMENT_SERVICE_CLASS_STATUS
+
+    def SCP(self, req: "_SMS", context: "PresentationContext") -> None:
+        """The SCP implementation for Storage Management Service Class.
+
+        Parameters
+        ----------
+        req : dimse_primitives.N_EVENT_REPORT or N_ACTION
+            The N-ACTION or N-EVENT-REPORT request primitive sent by the peer.
+        context : presentation.PresentationContext
+            The presentation context that the service is operating under.
+        """
+        if isinstance(req, N_EVENT_REPORT):
+            self._n_event_report_scp(req, context)
+        elif isinstance(req, N_ACTION):
+            self._n_action_scp(req, context)
+        else:
+            raise ValueError(
+                f"Invalid DIMSE primitive '{req.__class__.__name__}' used "
+                f"with Storage Management"
+            )
+
+
 class UnifiedProcedureStepServiceClass(ServiceClass):
     """Implementation of the Unified Procedure Step Service Class
 
     .. versionadded:: 1.4
     """
 
     statuses = UNIFIED_PROCEDURE_STEP_SERVICE_CLASS_STATUS
```

### Comparing `pynetdicom-2.0.2/pynetdicom/sop_class.py` & `pynetdicom-2.1.0/pynetdicom/sop_class.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """Generates the supported SOP Classes and well-known SOP Instances."""
 
 import inspect
+from keyword import iskeyword
 import logging
 import sys
-from typing import Optional, Type, Any, cast, Dict
+from typing import Optional, Type, cast, Dict
 
 from pydicom.uid import UID
 
 from pynetdicom.service_class import (
     BasicWorklistManagementServiceClass,
     ColorPaletteQueryRetrieveServiceClass,
     DefinedProcedureProtocolQueryRetrieveServiceClass,
     HangingProtocolQueryRetrieveServiceClass,
     ImplantTemplateQueryRetrieveServiceClass,
+    InventoryQueryRetrieveServiceClass,
     NonPatientObjectStorageServiceClass,
     ProtocolApprovalQueryRetrieveServiceClass,
     QueryRetrieveServiceClass,
     RelevantPatientInformationQueryServiceClass,
     ServiceClass,
     StorageServiceClass,
     SubstanceAdministrationQueryServiceClass,
@@ -27,19 +29,20 @@
     DisplaySystemManagementServiceClass,
     InstanceAvailabilityNotificationServiceClass,
     MediaCreationManagementServiceClass,
     PrintManagementServiceClass,
     ProcedureStepServiceClass,
     RTMachineVerificationServiceClass,
     StorageCommitmentServiceClass,
+    StorageManagementServiceClass,
     UnifiedProcedureStepServiceClass,
 )
 
 
-LOGGER = logging.getLogger("pynetdicom.sop")
+LOGGER = logging.getLogger(__name__)
 
 
 def uid_to_service_class(uid: str) -> Type[ServiceClass]:
     """Return the :class:`~pynetdicom.service_class.ServiceClass` object
     corresponding to `uid`.
 
     Parameters
@@ -52,80 +55,106 @@
     -------
     subclass of service_class.ServiceClass
         The Service Class corresponding to the SOP Class UID or the base class
         if support for the SOP Class isn't implemented.
     """
     if uid in _VERIFICATION_CLASSES.values():
         return VerificationServiceClass
-    elif uid in _QR_CLASSES.values():
+
+    if uid in _QR_CLASSES.values():
         return QueryRetrieveServiceClass
-    elif uid in _STORAGE_CLASSES.values():
+
+    if uid in _STORAGE_CLASSES.values():
         return StorageServiceClass
-    elif uid in _SERVICE_CLASSES:
+
+    if uid in _SERVICE_CLASSES:
         return _SERVICE_CLASSES[uid]
-    elif uid in _APPLICATION_EVENT_CLASSES.values():
+
+    if uid in _APPLICATION_EVENT_CLASSES.values():
         return ApplicationEventLoggingServiceClass
-    elif uid in _BASIC_WORKLIST_CLASSES.values():
+
+    if uid in _BASIC_WORKLIST_CLASSES.values():
         return BasicWorklistManagementServiceClass
-    elif uid in _COLOR_PALETTE_CLASSES.values():
+
+    if uid in _COLOR_PALETTE_CLASSES.values():
         return ColorPaletteQueryRetrieveServiceClass
-    elif uid in _DEFINED_PROCEDURE_CLASSES.values():
+
+    if uid in _DEFINED_PROCEDURE_CLASSES.values():
         return DefinedProcedureProtocolQueryRetrieveServiceClass
-    elif uid in _DISPLAY_SYSTEM_CLASSES.values():
+
+    if uid in _DISPLAY_SYSTEM_CLASSES.values():
         return DisplaySystemManagementServiceClass
-    elif uid in _HANGING_PROTOCOL_CLASSES.values():
+
+    if uid in _HANGING_PROTOCOL_CLASSES.values():
         return HangingProtocolQueryRetrieveServiceClass
-    elif uid in _IMPLANT_TEMPLATE_CLASSES.values():
+
+    if uid in _IMPLANT_TEMPLATE_CLASSES.values():
         return ImplantTemplateQueryRetrieveServiceClass
-    elif uid in _INSTANCE_AVAILABILITY_CLASSES.values():
+
+    if uid in _INSTANCE_AVAILABILITY_CLASSES.values():
         return InstanceAvailabilityNotificationServiceClass
-    elif uid in _MEDIA_CREATION_CLASSES.values():
+
+    if uid in _INVENTORY_CLASSES.values():
+        return InventoryQueryRetrieveServiceClass
+
+    if uid in _MEDIA_CREATION_CLASSES.values():
         return MediaCreationManagementServiceClass
-    elif uid in _MEDIA_STORAGE_CLASSES.values():
+
+    if uid in _MEDIA_STORAGE_CLASSES.values():
         return ServiceClass  # Not yet implemented
-    elif uid in _NON_PATIENT_OBJECT_CLASSES.values():
+
+    if uid in _NON_PATIENT_OBJECT_CLASSES.values():
         return NonPatientObjectStorageServiceClass
-    elif uid in _PRINT_MANAGEMENT_CLASSES.values():
+
+    if uid in _PRINT_MANAGEMENT_CLASSES.values():
         return PrintManagementServiceClass
-    elif uid in _PROCEDURE_STEP_CLASSES.values():
+
+    if uid in _PROCEDURE_STEP_CLASSES.values():
         return ProcedureStepServiceClass
-    elif uid in _PROTOCOL_APPROVAL_CLASSES.values():
+
+    if uid in _PROTOCOL_APPROVAL_CLASSES.values():
         return ProtocolApprovalQueryRetrieveServiceClass
-    elif uid in _RELEVANT_PATIENT_QUERY_CLASSES.values():
+
+    if uid in _RELEVANT_PATIENT_QUERY_CLASSES.values():
         return RelevantPatientInformationQueryServiceClass
-    elif uid in _RT_MACHINE_VERIFICATION_CLASSES.values():
+
+    if uid in _RT_MACHINE_VERIFICATION_CLASSES.values():
         return RTMachineVerificationServiceClass
-    elif uid in _STORAGE_COMMITMENT_CLASSES.values():
+
+    if uid in _STORAGE_COMMITMENT_CLASSES.values():
         return StorageCommitmentServiceClass
-    elif uid in _SUBSTANCE_ADMINISTRATION_CLASSES.values():
+
+    if uid in _STORAGE_MANAGEMENT_CLASSES.values():
+        return StorageManagementServiceClass
+
+    if uid in _SUBSTANCE_ADMINISTRATION_CLASSES.values():
         return SubstanceAdministrationQueryServiceClass
-    elif uid in _UNIFIED_PROCEDURE_STEP_CLASSES.values():
+
+    if uid in _UNIFIED_PROCEDURE_STEP_CLASSES.values():
         return UnifiedProcedureStepServiceClass
 
     # No SCP implemented
     return ServiceClass
 
 
 class SOPClass(UID):
     """Extend :class:`~pydicom.uid.UID` to include the corresponding Service
     Class.
 
     """
 
     _service_class: Optional[Type[ServiceClass]] = None
+    _name: str = ""
 
     def __new__(cls: Type["SOPClass"], val: str) -> "SOPClass":
         if isinstance(val, SOPClass):
             return val
 
         return cast("SOPClass", super().__new__(cls, val))
 
-    def __getattribute__(self, name: str) -> Any:
-        return super(SOPClass, self).__getattribute__(name)
-
     @property
     def service_class(self) -> ServiceClass:
         """Return the corresponding Service Class implementation."""
         return cast(ServiceClass, self._service_class)
 
 
 def _generate_sop_classes(sop_class_dict: Dict[str, str]) -> None:
@@ -185,14 +214,19 @@
     "ImplantTemplateGroupInformationModelFind": "1.2.840.10008.5.1.4.45.2",
     "ImplantTemplateGroupInformationModelMove": "1.2.840.10008.5.1.4.45.3",
     "ImplantTemplateGroupInformationModelGet": "1.2.840.10008.5.1.4.45.4",
 }
 _INSTANCE_AVAILABILITY_CLASSES = {
     "InstanceAvailabilityNotification": "1.2.840.10008.5.1.4.33",
 }
+_INVENTORY_CLASSES = {
+    "InventoryFind": "1.2.840.10008.5.1.4.1.1.201.2",
+    "InventoryMove": "1.2.840.10008.5.1.4.1.1.201.3",
+    "InventoryGet": "1.2.840.10008.5.1.4.1.1.201.4",
+}
 _MEDIA_CREATION_CLASSES = {
     "MediaCreationManagement": "1.2.840.10008.5.1.1.33",
 }
 _MEDIA_STORAGE_CLASSES = {
     "MediaStorageDirectoryStorage": "1.2.840.10008.1.3.10",
 }
 _NON_PATIENT_OBJECT_CLASSES = {
@@ -200,14 +234,15 @@
     "ColorPaletteStorage": "1.2.840.10008.5.1.4.39.1",
     "GenericImplantTemplateStorage": "1.2.840.10008.5.1.4.43.1",
     "ImplantAssemblyTemplateStorage": "1.2.840.10008.5.1.4.44.1",
     "ImplantTemplateGroupStorage": "1.2.840.10008.5.1.4.45.1",
     "CTDefinedProcedureProtocolStorage": "1.2.840.10008.5.1.4.1.1.200.1",
     "ProtocolApprovalStorage": "1.2.840.10008.5.1.4.1.1.200.3",
     "XADefinedProcedureProtocolStorage": "1.2.840.10008.5.1.4.1.1.200.7",
+    "InventoryStorage": "1.2.840.10008.5.1.4.1.1.201.1",
 }
 _PRINT_MANAGEMENT_CLASSES = {
     "BasicFilmSession": "1.2.840.10008.5.1.1.1",
     "BasicFilmBox": "1.2.840.10008.5.1.1.2",
     "BasicGrayscaleImageBox": "1.2.840.10008.5.1.1.4",
     "BasicColorImageBox": "1.2.840.10008.5.1.1.4.1",
     "PrintJob": "1.2.840.10008.5.1.1.14",
@@ -240,14 +275,15 @@
     "StudyRootQueryRetrieveInformationModelGet": "1.2.840.10008.5.1.4.1.2.2.3",
     "PatientStudyOnlyQueryRetrieveInformationModelFind": "1.2.840.10008.5.1.4.1.2.3.1",
     "PatientStudyOnlyQueryRetrieveInformationModelMove": "1.2.840.10008.5.1.4.1.2.3.2",
     "PatientStudyOnlyQueryRetrieveInformationModelGet": "1.2.840.10008.5.1.4.1.2.3.3",
     "CompositeInstanceRootRetrieveMove": "1.2.840.10008.5.1.4.1.2.4.2",
     "CompositeInstanceRootRetrieveGet": "1.2.840.10008.5.1.4.1.2.4.3",
     "CompositeInstanceRetrieveWithoutBulkDataGet": "1.2.840.10008.5.1.4.1.2.5.3",
+    "RepositoryQuery": "1.2.840.10008.5.1.4.1.1.201.6",
 }
 _RELEVANT_PATIENT_QUERY_CLASSES = {
     "GeneralRelevantPatientInformationQuery": "1.2.840.10008.5.1.4.37.1",
     "BreastImagingRelevantPatientInformationQuery": "1.2.840.10008.5.1.4.37.2",
     "CardiacRelevantPatientInformationQuery": "1.2.840.10008.5.1.4.37.3",
 }
 _RT_MACHINE_VERIFICATION_CLASSES = {
@@ -269,22 +305,24 @@
     "MRImageStorage": "1.2.840.10008.5.1.4.1.1.4",  # A.4
     "EnhancedMRImageStorage": "1.2.840.10008.5.1.4.1.1.4.1",  # A.36.2
     "MRSpectroscopyStorage": "1.2.840.10008.5.1.4.1.1.4.2",  # A.36.3
     "EnhancedMRColorImageStorage": "1.2.840.10008.5.1.4.1.1.4.3",  # A.36.4
     "LegacyConvertedEnhancedMRImageStorage": "1.2.840.10008.5.1.4.1.1.4.4",  # A.71
     "UltrasoundImageStorage": "1.2.840.10008.5.1.4.1.1.6.1",  # A.6
     "EnhancedUSVolumeStorage": "1.2.840.10008.5.1.4.1.1.6.2",  # A.59
+    "PhotoacousticImageStorage": "1.2.840.10008.5.1.4.1.1.6.3",
     "SecondaryCaptureImageStorage": "1.2.840.10008.5.1.4.1.1.7",  # A.8.1
     "MultiFrameSingleBitSecondaryCaptureImageStorage": "1.2.840.10008.5.1.4.1.1.7.1",  # A.8.2
     "MultiFrameGrayscaleByteSecondaryCaptureImageStorage": "1.2.840.10008.5.1.4.1.1.7.2",  # A.8.3
     "MultiFrameGrayscaleWordSecondaryCaptureImageStorage": "1.2.840.10008.5.1.4.1.1.7.3",  # A.8.4
     "MultiFrameTrueColorSecondaryCaptureImageStorage": "1.2.840.10008.5.1.4.1.1.7.4",  # A.8.5
     "TwelveLeadECGWaveformStorage": "1.2.840.10008.5.1.4.1.1.9.1.1",  # A.34.3
     "GeneralECGWaveformStorage": "1.2.840.10008.5.1.4.1.1.9.1.2",  # A.34.4
     "AmbulatoryECGWaveformStorage": "1.2.840.10008.5.1.4.1.1.9.1.3",  # A.34.5
+    "General32bitECGWaveformStorage": "1.2.840.10008.5.1.4.1.1.9.1.4",
     "HemodynamicWaveformStorage": "1.2.840.10008.5.1.4.1.1.9.2.1",  # A.34.6
     "CardiacElectrophysiologyWaveformStorage": "1.2.840.10008.5.1.4.1.1.9.3.1",  # A.34.7
     "BasicVoiceAudioWaveformStorage": "1.2.840.10008.5.1.4.1.1.9.4.1",  # A.34.2
     "GeneralAudioWaveformStorage": "1.2.840.10008.5.1.4.1.1.9.4.2",  # A.34.10
     "ArterialPulseWaveformStorage": "1.2.840.10008.5.1.4.1.1.9.5.1",  # A.34.8
     "RespiratoryWaveformStorage": "1.2.840.10008.5.1.4.1.1.9.6.1",  # A.34.9
     "MultichannelRespiratoryWaveformStorage": "1.2.840.10008.5.1.4.1.1.9.6.2",  # A.34.16
@@ -300,14 +338,15 @@
     "XAXRFGrayscaleSoftcopyPresentationStateStorage": "1.2.840.10008.5.1.4.1.1.11.5",  # A.33.6
     "GrayscalePlanarMPRVolumetricPresentationStateStorage": "1.2.840.10008.5.1.4.1.1.11.6",  # A.80.1
     "CompositingPlanarMPRVolumetricPresentationStateStorage": "1.2.840.10008.5.1.4.1.1.11.7",  # A.80.1
     "AdvancedBlendingPresentationStateStorage": "1.2.840.10008.5.1.4.1.1.11.8",  # A.33.7
     "VolumeRenderingVolumetricPresentationStateStorage": "1.2.840.10008.5.1.4.1.1.11.9",  # A.80.2
     "SegmentedVolumeRenderingVolumetricPresentationStateStorage": "1.2.840.10008.5.1.4.1.1.11.10",  # A.80.2
     "MultipleVolumeRenderingVolumetricPresentationStateStorage": "1.2.840.10008.5.1.4.1.1.11.11",  # A.80.2
+    "VariableModalityLUTSoftcopyPresentationStageStorage": "1.2.840.10008.5.1.4.1.1.11.12",
     "XRayAngiographicImageStorage": "1.2.840.10008.5.1.4.1.1.12.1",  # A.14
     "EnhancedXAImageStorage": "1.2.840.10008.5.1.4.1.1.12.1.1",  # A.47
     "XRayRadiofluoroscopicImageStorage": "1.2.840.10008.5.1.4.1.1.12.2",  # A.16
     "EnhancedXRFImageStorage": "1.2.840.10008.5.1.4.1.1.12.2.1",  # A.48
     "XRay3DAngiographicImageStorage": "1.2.840.10008.5.1.4.1.1.13.1.1",  # A.53
     "XRay3DCraniofacialImageStorage": "1.2.840.10008.5.1.4.1.1.13.1.2",  # A.54
     "BreastTomosynthesisImageStorage": "1.2.840.10008.5.1.4.1.1.13.1.3",  # A.55
@@ -340,14 +379,16 @@
     "OphthalmicTomographyImageStorage": "1.2.840.10008.5.1.4.1.1.77.1.5.4",  # A.52
     "WideFieldOphthalmicPhotographyStereographicProjectionImageStorage": "1.2.840.10008.5.1.4.1.1.77.1.5.5",  # A.76
     "WideFieldOphthalmicPhotography3DCoordinatesImageStorage": "1.2.840.10008.5.1.4.1.1.77.1.5.6",  # A.77
     "OphthalmicOpticalCoherenceTomographyEnFaceImageStorage": "1.2.840.10008.5.1.4.1.1.77.1.5.7",  # A.83
     "OphthlamicOpticalCoherenceTomographyBscanVolumeAnalysisStorage": "1.2.840.10008.5.1.4.1.1.77.1.5.8",  # A.84
     "VLWholeSlideMicroscopyImageStorage": "1.2.840.10008.5.1.4.1.1.77.1.6",  # A.32.8
     "DermoscopicPhotographyImageStorage": "1.2.840.10008.5.1.4.1.1.77.1.7",  # A.32.11
+    "ConfocalMicroscopyImageStorage": "1.2.840.10008.5.1.4.1.1.77.1.8",
+    "ConfocalMicroscopyTiledPyramidalImageStorage": "1.2.840.10008.5.1.4.1.1.77.1.9",
     "LensometryMeasurementsStorage": "1.2.840.10008.5.1.4.1.1.78.1",  # A.60.1
     "AutorefractionMeasurementsStorage": "1.2.840.10008.5.1.4.1.1.78.2",  # A.60.2
     "KeratometryMeasurementsStorage": "1.2.840.10008.5.1.4.1.1.78.3",  # A.60.3
     "SubjectiveRefractionMeasurementsStorage": "1.2.840.10008.5.1.4.1.1.78.4",  # A.60.4
     "VisualAcuityMeasurementsStorage": "1.2.840.10008.5.1.4.1.1.78.5",  # A.60.5
     "SpectaclePrescriptionReportStorage": "1.2.840.10008.5.1.4.1.1.78.6",  # A.35.9
     "OphthalmicAxialMeasurementsStorage": "1.2.840.10008.5.1.4.1.1.78.7",  # A.60.6
@@ -379,15 +420,14 @@
     "MicroscopyBulkSimpleAnnotationsStorage": "1.2.840.10008.5.1.4.1.1.91.1",
     "EncapsulatedPDFStorage": "1.2.840.10008.5.1.4.1.1.104.1",  # A.45.1
     "EncapsulatedCDAStorage": "1.2.840.10008.5.1.4.1.1.104.2",  # A.45.2
     "EncapsulatedSTLStorage": "1.2.840.10008.5.1.4.1.1.104.3",  # A.85.1
     "EncapsulatedOBJStorage": "1.2.840.10008.5.1.4.1.1.104.4",  # A.85.2
     "EncapsulatedMTLStorage": "1.2.840.10008.5.1.4.1.1.104.5",  # A.85.3
     "PositronEmissionTomographyImageStorage": "1.2.840.10008.5.1.4.1.1.128",  # A.21
-    # 128 presentation context limit here
     "LegacyConvertedEnhancedPETImageStorage": "1.2.840.10008.5.1.4.1.1.128.1",  # A.72
     "EnhancedPETImageStorage": "1.2.840.10008.5.1.4.1.1.130",  # A.56
     "BasicStructuredDisplayStorage": "1.2.840.10008.5.1.4.1.1.131",  # A.33.5
     "CTPerformedProcedureProtocolStorage": "1.2.840.10008.5.1.4.1.1.200.2",  # A.82.1
     "XAPerformedProcedureProtocolStorage": "1.2.840.10008.5.1.4.1.1.200.8",
     "RTImageStorage": "1.2.840.10008.5.1.4.1.1.481.1",  # A.17
     "RTDoseStorage": "1.2.840.10008.5.1.4.1.1.481.2",  # A.18
@@ -407,20 +447,26 @@
     "RTRadiationRecordSetStorage": "1.2.840.10008.5.1.4.1.1.481.16",  # A.86.1.8
     "RTRadiationSalvageRecordStorage": "1.2.840.10008.5.1.4.1.1.481.17",  # A.86.1.9
     "TomotherapeuticRadiationRecordStorage": "1.2.840.10008.5.1.4.1.1.481.18",  # A.86.1.10
     "CArmPhotonElectronRadiationRecordStorage": "1.2.840.10008.5.1.4.1.1.481.19",  # A.86.1.11
     "RoboticArmRadiationRecordStorage": "1.2.840.10008.5.1.4.1.1.481.20",  # A.86.1.12
     "RTRadiationSetDeliveryInstructionStorage": "1.2.840.10008.5.1.4.1.1.481.21",
     "RTTreatmentPreparationStorage": "1.2.840.10008.5.1.4.1.1.481.22",
+    "EnhancedRTImageStorage": "1.2.840.10008.5.1.4.1.1.481.23",
+    "EnhancedContinuousRTImageStorage": "1.2.840.10008.5.1.4.1.1.481.24",
+    "RTPatientPositionAcquisitionInstructionStorage": "1.2.840.10008.5.1.4.1.1.481.25",
     "RTBeamsDeliveryInstructionStorage": "1.2.840.10008.5.1.4.34.7",  # A.64
     "RTBrachyApplicationSetupDeliveryInstructionsStorage": "1.2.840.10008.5.1.4.34.10",  # A.79
 }
 _STORAGE_COMMITMENT_CLASSES = {
     "StorageCommitmentPushModel": "1.2.840.10008.1.20.1",
 }
+_STORAGE_MANAGEMENT_CLASSES = {
+    "InventoryCreation": "1.2.840.10008.5.1.4.1.1.201.5",
+}
 _SUBSTANCE_ADMINISTRATION_CLASSES = {
     "ProductCharacteristicsQuery": "1.2.840.10008.5.1.4.41",
     "SubstanceApprovalQuery": "1.2.840.10008.5.1.4.42",
 }
 _UNIFIED_PROCEDURE_STEP_CLASSES = {
     "UnifiedProcedureStepPush": "1.2.840.10008.5.1.4.34.6.1",
     "UnifiedProcedureStepWatch": "1.2.840.10008.5.1.4.34.6.2",
@@ -428,34 +474,62 @@
     "UnifiedProcedureStepEvent": "1.2.840.10008.5.1.4.34.6.4",
     "UnifiedProcedureStepQuery": "1.2.840.10008.5.1.4.34.6.5",
 }
 _VERIFICATION_CLASSES = {
     "Verification": "1.2.840.10008.1.1",
 }
 
+
+_SERVICE_TO_UID_GROUP = {
+    VerificationServiceClass: _VERIFICATION_CLASSES,
+    QueryRetrieveServiceClass: _QR_CLASSES,
+    StorageServiceClass: _STORAGE_CLASSES,
+    ApplicationEventLoggingServiceClass: _APPLICATION_EVENT_CLASSES,
+    BasicWorklistManagementServiceClass: _BASIC_WORKLIST_CLASSES,
+    ColorPaletteQueryRetrieveServiceClass: _COLOR_PALETTE_CLASSES,
+    DefinedProcedureProtocolQueryRetrieveServiceClass: _DEFINED_PROCEDURE_CLASSES,
+    DisplaySystemManagementServiceClass: _DISPLAY_SYSTEM_CLASSES,
+    HangingProtocolQueryRetrieveServiceClass: _HANGING_PROTOCOL_CLASSES,
+    ImplantTemplateQueryRetrieveServiceClass: _IMPLANT_TEMPLATE_CLASSES,
+    InstanceAvailabilityNotificationServiceClass: _INSTANCE_AVAILABILITY_CLASSES,
+    MediaCreationManagementServiceClass: _MEDIA_CREATION_CLASSES,
+    NonPatientObjectStorageServiceClass: _NON_PATIENT_OBJECT_CLASSES,
+    PrintManagementServiceClass: _PRINT_MANAGEMENT_CLASSES,
+    ProcedureStepServiceClass: _PROCEDURE_STEP_CLASSES,
+    ProtocolApprovalQueryRetrieveServiceClass: _PROTOCOL_APPROVAL_CLASSES,
+    RelevantPatientInformationQueryServiceClass: _RELEVANT_PATIENT_QUERY_CLASSES,
+    RTMachineVerificationServiceClass: _RT_MACHINE_VERIFICATION_CLASSES,
+    StorageCommitmentServiceClass: _STORAGE_COMMITMENT_CLASSES,
+    SubstanceAdministrationQueryServiceClass: _SUBSTANCE_ADMINISTRATION_CLASSES,
+    UnifiedProcedureStepServiceClass: _UNIFIED_PROCEDURE_STEP_CLASSES,
+}
+
+
 # pylint: enable=line-too-long
 _generate_sop_classes(_APPLICATION_EVENT_CLASSES)
 _generate_sop_classes(_BASIC_WORKLIST_CLASSES)
 _generate_sop_classes(_COLOR_PALETTE_CLASSES)
 _generate_sop_classes(_DEFINED_PROCEDURE_CLASSES)
 _generate_sop_classes(_DISPLAY_SYSTEM_CLASSES)
 _generate_sop_classes(_HANGING_PROTOCOL_CLASSES)
 _generate_sop_classes(_IMPLANT_TEMPLATE_CLASSES)
 _generate_sop_classes(_INSTANCE_AVAILABILITY_CLASSES)
+_generate_sop_classes(_INVENTORY_CLASSES)
 _generate_sop_classes(_MEDIA_CREATION_CLASSES)
 _generate_sop_classes(_MEDIA_STORAGE_CLASSES)
 _generate_sop_classes(_NON_PATIENT_OBJECT_CLASSES)
 _generate_sop_classes(_PRINT_MANAGEMENT_CLASSES)
 _generate_sop_classes(_PROCEDURE_STEP_CLASSES)
 _generate_sop_classes(_PROTOCOL_APPROVAL_CLASSES)
 _generate_sop_classes(_QR_CLASSES)
 _generate_sop_classes(_RELEVANT_PATIENT_QUERY_CLASSES)
 _generate_sop_classes(_RT_MACHINE_VERIFICATION_CLASSES)
 _generate_sop_classes(_STORAGE_CLASSES)
 _generate_sop_classes(_STORAGE_COMMITMENT_CLASSES)
+_generate_sop_classes(_STORAGE_MANAGEMENT_CLASSES)
 _generate_sop_classes(_SUBSTANCE_ADMINISTRATION_CLASSES)
 _generate_sop_classes(_UNIFIED_PROCEDURE_STEP_CLASSES)
 _generate_sop_classes(_VERIFICATION_CLASSES)
 
 
 def uid_to_sop_class(uid: str) -> SOPClass:
     """Return the :class:`SOPClass` object corresponding to `uid`.
@@ -487,14 +561,95 @@
 
     sop_class = SOPClass(uid)
     sop_class._service_class = ServiceClass
 
     return sop_class
 
 
+def register_uid(
+    uid: str,
+    keyword: str,
+    service_class: Type[ServiceClass],
+    dimse_msg_type: str = "",
+) -> None:
+    """Register a private or public SOP Class UID `uid` with the
+    :mod:`~pynetdicom.sop_class` module.
+
+    Examples
+    --------
+
+    Register the UID ``1.2.246.352.70.1.70`` with the
+    :class:`~pynetdicom.service_class.StorageServiceClass`::
+
+        >>> from pynetdicom import register_uid
+        >>> from pynetdicom.service_class import StorageServiceClass
+        >>> register_uid(
+        ...     "1.2.246.352.70.1.70",
+        ...     "FooStorage",
+        ...     StorageServiceClass,
+        ... )
+
+    Using a UID after registration::
+
+        >>> from pynetdicom import AE
+        >>> from pynetdicom.sop_class import FooStorage
+        >>> ae = AE()
+        >>> ae.add_supported_context(FooStorage)
+
+    Parameters
+    ----------
+    uid : str
+        The UID to be registered.
+    keyword : str
+        The keyword to use for the UID, must be a valid Python identifier and
+        may not be a Python keyword.
+    service_class : pynetdicom.service_class.ServiceClass
+        The service that the `uid` will be registered with, such as
+        :class:`~pynetdicom.service_class.StorageServiceClass`. Note that this
+        must be the class object itself and not a class instance.
+    dimse_msg_type : str, optional
+        If `service_class` is
+        :class:`~pynetdicom.service_class.QueryRetrieveServiceClass` then this
+        should be the DIMSE service message type that the `uid` is being
+        registered to. One of (``"C-FIND"``, ``"C-GET"``, ``"C-MOVE"``).
+    """
+    if not keyword.isidentifier() or iskeyword(keyword):
+        raise ValueError(
+            f"The keyword '{keyword}' is not a valid Python identifier or is "
+            "a Python keyword"
+        )
+
+    if not inspect.isclass(service_class):
+        raise TypeError("'service_class' must be a class object not a class instance")
+
+    if not issubclass(service_class, ServiceClass):
+        raise TypeError(
+            "'service_class' must be a ServiceClass subclass object "
+            "such as 'StorageServiceClass'"
+        )
+
+    group = _SERVICE_TO_UID_GROUP[service_class]
+    group[keyword] = uid
+
+    sop_class = SOPClass(uid)
+    sop_class._service_class = uid_to_service_class(uid)
+    globals()[keyword] = sop_class
+
+    if issubclass(service_class, QueryRetrieveServiceClass):
+        if service_class is QueryRetrieveServiceClass:
+            if dimse_msg_type not in ("C-FIND", "C-GET", "C-MOVE"):
+                raise ValueError(
+                    "'dimse_msg_type' must be 'C-FIND', 'C-GET' or 'C-MOVE' "
+                    "when registering a UID with QueryRetrieveServiceClass"
+                )
+            service_class._SUPPORTED_UIDS[dimse_msg_type].append(uid)
+        else:
+            service_class._SUPPORTED_UIDS["C-FIND"].append(uid)
+
+
 # Well-known SOP Instance UIDs for the supported Service Classes
 DisplaySystemInstance = UID("1.2.840.10008.5.1.1.40.1")
 """``1.2.840.10008.5.1.1.40.1``
 
 .. versionadded:: 1.5
 """
 PrinterConfigurationRetrievalInstance = UID("1.2.840.10008.5.1.1.17.376")
@@ -513,14 +668,19 @@
 .. versionadded:: 1.5
 """
 StorageCommitmentPushModelInstance = UID("1.2.840.10008.1.20.1.1")
 """``1.2.840.10008.1.20.1.1``
 
 .. versionadded:: 1.5
 """
+StorageManagementInstance = UID("1.2.840.10008.5.1.4.1.1.201.1.1")
+"""``1.2.840.10008.5.1.4.1.1.201.1.1``
+
+.. versionadded:: 2.1
+"""
 SubstanceAdministrationLoggingInstance = UID("1.2.840.10008.1.42.1")
 """``1.2.840.10008.1.42.1``
 
 .. versionadded:: 1.5
 """
 UPSFilteredGlobalSubscriptionInstance = UID("1.2.840.10008.5.1.4.34.5.1")
 """``1.2.840.10008.5.1.4.34.5.1``
```

### Comparing `pynetdicom-2.0.2/pynetdicom/status.py` & `pynetdicom-2.1.0/pynetdicom/status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 """Implementation of the DIMSE Status values."""
 
 from enum import IntEnum
-from typing import Dict, Tuple
 
 from pydicom.dataset import Dataset
 
 from pynetdicom._globals import (
     STATUS_SUCCESS,
     STATUS_FAILURE,
     STATUS_WARNING,
     STATUS_CANCEL,
     STATUS_PENDING,
     STATUS_UNKNOWN,
 )
 
 
-StatusDictType = Dict[int, Tuple[str, str]]
+StatusDictType = dict[int, tuple[str, str]]
 
 
 # Non-Service Class specific statuses - PS3.7 Annex C
 GENERAL_STATUS: StatusDictType = {
     0x0000: (STATUS_SUCCESS, ""),
     0x0105: (STATUS_FAILURE, "No Such Attribute"),
     0x0106: (STATUS_FAILURE, "Invalid Attribute Value"),
@@ -71,26 +70,31 @@
     STORAGE_SERVICE_CLASS_STATUS[_code] = (STATUS_FAILURE, "Cannot Understand")
 
 # Add the General status code values - PS3.7 9.1.1.1.9 and Annex C
 STORAGE_SERVICE_CLASS_STATUS.update(GENERAL_STATUS)
 
 
 # Query Retrieve - FIND specific status code values
-#   PS3.4 Annex C.4.1.1.4
+#   PS3.4 Annex C.4.1.1.4 and Annex C.6.4.3
 # Hanging Protocol - FIND specific status code values
 #   PS3.4 Annex U.4.1
 # Color Palette - FIND specific status code values
 #   PS3.4 Annex X
 # Implant Template - FIND specific status code values
 #   PS3.4 Annex BB
 # Defined Procedure Protocol - FIND specific status code values
 #   PS3.4 Annex HH
 QR_FIND_SERVICE_CLASS_STATUS: StatusDictType = {
     0xA700: (STATUS_FAILURE, "Refused: Out of Resources"),
+    0xA710: (STATUS_FAILURE, "Invalid Prior Record Key"),
     0xA900: (STATUS_FAILURE, "Identifier Does Not Match SOP Class"),
+    0xB001: (
+        STATUS_WARNING,
+        "Matching reached response limit, subsequent request may return additional matches",
+    ),
     0xFF00: (STATUS_PENDING, "Matches are continuing, current match supplied"),
     0xFF01: (STATUS_PENDING, "Matches are continuing, warning"),
 }
 
 # Ranged values
 for _code in range(0xC000, 0xCFFF + 1):
     QR_FIND_SERVICE_CLASS_STATUS[_code] = (STATUS_FAILURE, "Unable to Process")
@@ -345,14 +349,27 @@
 PRINT_JOB_MANAGEMENT_SERVICE_CLASS_STATUS.update(GENERAL_STATUS)
 
 
 # Storage Commitment Service Class specific status code values
 STORAGE_COMMITMENT_SERVICE_CLASS_STATUS = GENERAL_STATUS
 
 
+# Storage Management Service Class specific status code values
+STORAGE_MANAGEMENT_SERVICE_CLASS_STATUS: StatusDictType = {
+    0xB010: (
+        STATUS_WARNING,
+        (
+            "Attribute list error - One or more of Key Attributes are not "
+            "supported for matching"
+        ),
+    ),
+}
+STORAGE_MANAGEMENT_SERVICE_CLASS_STATUS.update(GENERAL_STATUS)
+
+
 # Application Event Logging Service Class specific status code values
 APPLICATION_EVENT_LOGGING_SERVICE_CLASS_STATUS: StatusDictType = {
     0xB101: (
         STATUS_WARNING,
         "Specified Synchronisation Frame of Reference UID doesn't "
         "match SCP Synchronization Frame of Reference",
     ),
@@ -511,31 +528,34 @@
     """Return a :class:`~pydicom.dataset.Dataset` with a *Status* element
     value of `code`.
     """
     if isinstance(code, int) and code >= 0:
         ds = Dataset()
         ds.Status = code
         return ds
-    else:
-        raise ValueError("'code' must be a positive integer.")
+
+    raise ValueError("'code' must be a positive integer.")
 
 
 def code_to_category(code: int) -> str:
     """Return a *Status* category as :class:`str` or ``'Unknown'`` if not
     recognised.
     """
     # pylint: disable=too-many-return-statements
     if isinstance(code, int) and code >= 0:
         if code == 0x0000:
             return STATUS_SUCCESS
-        elif code in [0xFF00, 0xFF01]:
+
+        if code in [0xFF00, 0xFF01]:
             return STATUS_PENDING
-        elif code == 0xFE00:
+
+        if code == 0xFE00:
             return STATUS_CANCEL
-        elif code in [
+
+        if code in [
             0x0105,
             0x0106,
             0x0110,
             0x0111,
             0x0112,
             0x0113,
             0x0114,
@@ -550,28 +570,33 @@
             0x0124,
             0x0210,
             0x0211,
             0x0212,
             0x0213,
         ]:
             return STATUS_FAILURE
-        elif code in range(0xA000, 0xB000):
+
+        if code in range(0xA000, 0xB000):
             return STATUS_FAILURE
-        elif code in range(0xC000, 0xD000):
+
+        if code in range(0xC000, 0xD000):
             return STATUS_FAILURE
-        elif code in [0x0107, 0x0116]:
+
+        if code in [0x0107, 0x0116]:
             return STATUS_WARNING
-        elif code in range(0xB000, 0xC000):
+
+        if code in range(0xB000, 0xC000):
             return STATUS_WARNING
-        elif code == 0x0001:
+
+        if code == 0x0001:
             return STATUS_WARNING
 
         return STATUS_UNKNOWN
-    else:
-        raise ValueError("'code' must be a positive integer.")
+
+    raise ValueError("'code' must be a positive integer.")
 
 
 class Status(IntEnum):
     """Constants for common status codes.
 
     .. versionadded:: 1.5
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/benchmark_script.py` & `pynetdicom-2.1.0/pynetdicom/tests/benchmark_script.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,48 +77,53 @@
 
 def which(program):
     # Determine if a given program is installed on PATH
     def is_exe(fpath):
         return os.path.isfile(fpath) and os.access(fpath, os.X_OK)
 
     fpath, fname = os.path.split(program)
-    if fpath:
-        if is_exe(program):
-            return program
-    else:
-        for path in os.environ["PATH"].split(os.pathsep):
-            exe_file = os.path.join(path, program)
-            if is_exe(exe_file):
-                return exe_file
+    if fpath and is_exe(program):
+        return program
+
+    # for path in os.environ["PATH"].split(os.pathsep):
+    for path in sorted(os.environ["PATH"].split(os.pathsep), reverse=True):
+        exe_file = os.path.join(path, program)
+        if is_exe(exe_file):
+            return exe_file
 
 
 def start_storescp():
     """Start DCMTK's storescp in a background process.
 
     Returns
     -------
     subprocess.Popen
         The running process.
     """
     args = [which("storescp"), "--ignore", "11112"]
     return subprocess.Popen(args)
 
 
+def start_pynetdicom_storescp():
+    args = ["python", "-m", "pynetdicom", "storescp", "11112", "--ignore"]
+    return subprocess.Popen(args)
+
+
 def start_storescu(test_ds, ds_per_assoc):
     """Run DCMTK's storescu in a background process.
 
     Parameters
     ----------
     test_ds : pydicom.dataset.Dataset
         The test dataset to use
     ds_per_assoc : int
         The number of datasets to send using `storescu`.
     """
     fpath = test_ds.filename
-    args = [which("storescu"), "localhost", "11112"] + [fpath] * ds_per_assoc
+    args = [which("storescu"), "localhost", "11112", "--repeat", f"{ds_per_assoc}", fpath]
     return subprocess.Popen(args)
 
 
 def receive_store(test_ds, nr_assoc, ds_per_assoc, write_ds=0, use_yappi=False):
     """Run a Storage SCP and transfer datasets with sequential storescu's.
 
     Parameters
@@ -213,66 +218,45 @@
         ``3`` to write raw bytes with unlimited PDU size.
     use_yappi : bool, optional
         True to use the yappi profiler, False otherwise (default).
     """
     if use_yappi:
         init_yappi()
 
-    def handle(event):
-        if write_ds == 1:
-            with tempfile.TemporaryFile("w+b") as tfile:
-                ds = event.dataset
-                ds.file_meta = event.file_meta
-                ds.save_as(tfile)
-        elif write_ds in (2, 3):
-            with tempfile.TemporaryFile("w+b") as tfile:
-                tfile.write(b"\x00" * 128)
-                tfile.write(b"DICM")
-                write_file_meta_info(tfile, event.file_meta)
-                tfile.write(event.request.DataSet.getvalue())
-
-        return 0x0000
+    server = start_pynetdicom_storescp()
 
     ae = AE()
     ae.acse_timeout = 5
     ae.dimse_timeout = 5
     ae.network_timeout = 5
-    if write_ds == 3:
-        ae.maximum_pdu_size = 0
-    ae.add_supported_context(test_ds.SOPClassUID, ImplicitVRLittleEndian)
     ae.add_requested_context(test_ds.SOPClassUID, ImplicitVRLittleEndian)
 
-    server = ae.start_server(
-        ("localhost", 11112), block=False, evt_handlers=[(evt.EVT_C_STORE, handle)]
-    )
-
     time.sleep(0.5)
     start_time = time.time()
     is_successful = True
 
     for ii in range(nr_assoc):
         assoc = ae.associate("127.0.0.1", 11112)
         if assoc.is_established:
             for jj in range(ds_per_assoc):
                 assoc.send_c_store(test_ds)
 
             assoc.release()
 
     if is_successful:
-        write_msg = ["", " (write)", " (write fast)", " (write fastest)"][write_ds]
         print(
             f"C-STORE SCU/SCP transferred {nr_assoc * ds_per_assoc} total "
             f"{os.path.basename(test_ds.filename)} datasets over "
-            f"{nr_assoc} association{'' if nr_assoc == 1 else 's'}{write_msg} "
+            f"{nr_assoc} association{'' if nr_assoc == 1 else 's'} "
             f"in {time.time() - start_time:.2f} s"
         )
     else:
         print("C-STORE SCU/SCP benchmark failed")
 
-    server.shutdown()
+    server.terminate()
 
 
 def receive_store_dcmtk(test_ds, nr_assoc, ds_per_assoc, use_yappi=False):
     """Run a Storage SCP and transfer datasets with sequential storescu's.
 
     Parameters
     ----------
@@ -429,51 +413,52 @@
             assoc.release()
             if is_successful:
                 run_times.append(time.time() - start_time)
         else:
             is_successful = False
             break
 
+    end_time = time.time()
     if is_successful:
         print(
             f"C-STORE SCU transferred {nr_assoc * ds_per_assoc} total "
             f"{os.path.basename(test_ds.filename)} datasets over "
             f"{nr_assoc} association{'' if nr_assoc == 1 else 's'} "
-            f"in {time.time() - start_time:.2f} s"
+            f"in {end_time - start_time:.2f} s"
         )
     else:
         print("C-STORE SCU benchmark failed")
 
     server.terminate()
     time.sleep(0.5)
 
 
 if __name__ == "__main__":
-    print("Use yappi? (y/n:)")
+    print("Use yappi? (y/n): ", end="")
     use_yappi = input()
     if use_yappi in ["y", "Y"]:
         use_yappi = True
     else:
         use_yappi = False
 
-    print("Use large dataset? (y/n:)")
+    print("Use large dataset? (y/n): ", end="")
     use_large_dcm = input()
     if use_large_dcm in ["y", "Y"]:
         use_large_dcm = True
     else:
         use_large_dcm = False
 
     if use_large_dcm:
         ds_name = "RTImageStorage.dcm"  # 2.1 MB
         default_nr_ds = 100
     else:
         ds_name = "CTImageStorage.dcm"  # 39 kB
         default_nr_ds = 1000
 
-    print(f"number of datasets? (default = {default_nr_ds})")
+    print(f"number of datasets? (default = {default_nr_ds}): ", end="")
     try:
         nr_ds = int(input())
     except ValueError:
         nr_ds = default_nr_ds
 
     test_ds = dcmread(os.path.join(TEST_DS_DIR, ds_name))
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/cert_files/client.crt` & `pynetdicom-2.1.0/pynetdicom/tests/cert_files/client.crt`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/cert_files/client.key` & `pynetdicom-2.1.0/pynetdicom/tests/cert_files/client.key`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/cert_files/server.crt` & `pynetdicom-2.1.0/pynetdicom/tests/cert_files/server.crt`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/cert_files/server.key` & `pynetdicom-2.1.0/pynetdicom/tests/cert_files/server.key`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/dicom_files/CTImageStorage.dcm` & `pynetdicom-2.1.0/pynetdicom/tests/dicom_files/CTImageStorage.dcm`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/dicom_files/CTImageStorage_bad_meta.dcm` & `pynetdicom-2.1.0/pynetdicom/tests/dicom_files/CTImageStorage_bad_meta.dcm`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/dicom_files/MRImageStorage_ExplicitVRBigEndian.dcm` & `pynetdicom-2.1.0/pynetdicom/tests/dicom_files/MRImageStorage_ExplicitVRBigEndian.dcm`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/dicom_files/MRImageStorage_JPG2000_Lossless.dcm` & `pynetdicom-2.1.0/pynetdicom/tests/dicom_files/MRImageStorage_JPG2000_Lossless.dcm`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/dicom_files/RTImageStorage.dcm` & `pynetdicom-2.1.0/pynetdicom/tests/dicom_files/RTImageStorage.dcm`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/dicom_files/SCImageStorage_Deflated.dcm` & `pynetdicom-2.1.0/pynetdicom/tests/dicom_files/SCImageStorage_Deflated.dcm`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/encoded_dimse_msg.py` & `pynetdicom-2.1.0/pynetdicom/tests/encoded_dimse_msg.py`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/encoded_dimse_n_msg.py` & `pynetdicom-2.1.0/pynetdicom/tests/encoded_dimse_n_msg.py`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/encoded_pdu_items.py` & `pynetdicom-2.1.0/pynetdicom/tests/encoded_pdu_items.py`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/hide_modules.py` & `pynetdicom-2.1.0/pynetdicom/tests/hide_modules.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,25 +22,18 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-try:
-    import importlib.abc
+from importlib.abc import MetaPathFinder
 
-    # py>=3.3 has MetaPathFinder
-    _ModuleHiderBase = getattr(importlib.abc, "MetaPathFinder", importlib.abc.Finder)
-except ImportError:
-    # py2
-    _ModuleHiderBase = object
 
-
-class ModuleHider(_ModuleHiderBase):
+class ModuleHider(MetaPathFinder):
     """Import finder hook to hide specified modules
     ModuleHider(hidden_modules) -> instance
     hidden_modules is a list of strings naming modules to hide.
     """
 
     def __init__(self, hidden):
         self.hidden = hidden
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/parrot.py` & `pynetdicom-2.1.0/pynetdicom/tests/parrot.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from struct import pack, unpack
 import threading
 import time
 
 from pynetdicom.transport import AssociationServer
 
 
-LOGGER = logging.getLogger("pynetdicom")
+LOGGER = logging.getLogger(__name__)
 
 
 class ParrotRequest(BaseRequestHandler):
     @property
     def commands(self):
         """Return a list of command tuples."""
         # commands: recv, send, exit
@@ -30,15 +30,15 @@
     def handle(self):
         # self.server: ThreadedParrot
         # self.client_address: remote's (host, port)
         # self.request: socket
         self.event.clear()
         self.received = []
         self.sent = []
-        for (cmd, data) in self.commands:
+        for cmd, data in self.commands:
             if cmd == "recv":
                 self.kill_read = False
                 while not self.kill_read:
                     if self.ready:
                         self.received.append(bytes(self.read_data))
                         self.kill_read = True
             elif cmd == "send":
@@ -57,40 +57,40 @@
         -------
         bool
             True if the socket has data ready to be read, False otherwise.
         """
         try:
             # Use a timeout of 0 so we get an "instant" result
             ready, _, _ = select.select([self.socket], [], [], 0.5)
-        except (socket.error, socket.timeout, ValueError):
+        except (OSError, TimeoutError, ValueError):
             return False
 
         return bool(ready)
 
     @property
     def read_data(self):
         bytestream = bytearray()
 
         # Try and read the PDU type and length from the socket
         try:
             bytestream.extend(self.recv(6))
-        except (socket.error, socket.timeout):
+        except (OSError, TimeoutError):
             pass
         try:
             # Byte 1 is always the PDU type
             # Byte 2 is always reserved
             # Bytes 3-6 are always the PDU length
             pdu_type, _, pdu_length = unpack(">BBL", bytestream)
         except struct.error:
             pass
 
         # Try and read the rest of the PDU
         try:
             bytestream += self.recv(pdu_length)
-        except (socket.error, socket.timeout):
+        except (OSError, TimeoutError):
             pass
 
         return bytestream
 
     def recv(self, nr_bytes):
         """Read `nr_bytes` from the socket.
 
@@ -150,15 +150,15 @@
         total_sent = 0
         length_data = len(bytestream)
         try:
             while total_sent < length_data:
                 # Returns the number of bytes sent
                 nr_sent = self.socket.send(bytestream)
                 total_sent += nr_sent
-        except (socket.error, socket.timeout):
+        except (OSError, TimeoutError):
             # Evt17: Transport connection closed
             return False
 
         return True
 
     @property
     def socket(self):
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_acse.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_acse.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 
         return self._handlers[event]
 
 
 class TestACSE:
     """Tests for initialising the ACSE class"""
 
-    def setup(self):
+    def setup_method(self):
         self.assoc = DummyAssociation()
         self.assoc.requestor.requested_contexts = [build_context("1.2.840.10008.1.1")]
 
     def test_default(self):
         """Test default initialisation"""
         acse = ACSE(self.assoc)
         assert hasattr(acse, "acse_timeout") is True
@@ -185,22 +185,22 @@
             self.assoc.dul.queue.get(block=False)
         assert acse.is_release_requested() is False
 
 
 class TestNegotiationRequestor:
     """Test ACSE negotiation as requestor."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
         self.assoc = DummyAssociation()
         self.assoc.requestor.requested_contexts = [build_context("1.2.840.10008.1.1")]
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_no_requested_cx(self, caplog):
         """Test error logged if no requested contexts."""
         ae = AE()
@@ -336,18 +336,18 @@
 
         scp.shutdown()
 
 
 class TestNegotiationAcceptor:
     """Test ACSE negotiation as acceptor."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
     def test_response_has_rejected(self):
         """Test that the A-ASSOCIATE-AC contains rejected contexts."""
         self.ae = ae = AE()
         ae.acse_timeout = 5
@@ -381,15 +381,15 @@
     (0x02, 0x03, (0x01, 0x02)),
 ]
 
 
 class TestPrimitiveConstruction:
     """Test the primitive builders"""
 
-    def setup(self):
+    def setup_method(self):
         self.assoc = DummyAssociation()
         self.assoc.requestor.requested_contexts = [build_context("1.2.840.10008.1.1")]
 
     def test_send_request(self):
         """Test A-ASSOCIATE (rq) construction and sending"""
         acse = ACSE(self.assoc)
         role = SCP_SCU_RoleSelectionNegotiation()
@@ -582,19 +582,19 @@
     ((5, b"\x00\x05", b"invalid", True), (True, b"\x01\x05")),
 ]
 
 
 class TestUserIdentityNegotiation:
     """Tests for User Identity Negotiation."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     @pytest.mark.parametrize("req, rsp", REFERENCE_USER_IDENTITY_REQUEST)
     def test_check_usrid_not_implemented(self, req, rsp):
         """Check _check_user_identity if user hasn't implemented."""
@@ -1061,19 +1061,19 @@
             assoc.release()
         scp.shutdown()
 
 
 class TestSOPClassExtendedNegotiation:
     """Tests for SOP Class Extended Negotiation."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_check_ext_no_req(self):
         """Test the an empty SOP Extended request"""
         self.ae = ae = AE()
@@ -1475,19 +1475,19 @@
 
         scp.shutdown()
 
 
 class TestSOPClassCommonExtendedNegotiation:
     """Tests for SOP Class Extended Negotiation."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_check_ext_no_req(self):
         """Test the default handler for evt.EVT_SOP_COMMON"""
         self.ae = ae = AE()
@@ -1755,19 +1755,19 @@
 
         scp.shutdown()
 
 
 class TestAsyncOpsNegotiation:
     """Tests for Asynchronous Operations Window Negotiation."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_check_async_no_req(self):
         """Test the default evt.EVT_ASYNC_OPS handler"""
         self.ae = ae = AE()
@@ -1932,19 +1932,19 @@
 
         scp.shutdown()
 
 
 class TestNegotiateRelease:
     """Tests for ACSE.negotiate_release."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.scp = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.scp:
             self.scp.shutdown()
 
     def create_assoc(self):
         ae = AE()
         ae.add_requested_context(Verification)
@@ -2194,19 +2194,19 @@
         assert scp.received[1] == a_release_rq
         assert scp.received[2] == a_release_rp
 
 
 class TestEventHandlingAcceptor:
     """Test the transport events and handling as acceptor."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
         _config.LOG_HANDLER_LEVEL = "none"
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
         _config.LOG_HANDLER_LEVEL = "standard"
 
     def test_no_handlers(self):
         """Test with no transport event handlers bound."""
@@ -2569,19 +2569,19 @@
             assert msg in caplog.text
             assert "Exception description" in caplog.text
 
 
 class TestEventHandlingRequestor:
     """Test the transport events and handling as requestor."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
         _config.LOG_HANDLER_LEVEL = "none"
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
         _config.LOG_HANDLER_LEVEL = "standard"
 
     def test_no_handlers(self):
         """Test with no transport event handlers bound."""
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_ae.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_ae.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import signal
 import threading
 import time
 
 import pytest
 
-from pydicom import read_file, config as PYD_CONFIG
+from pydicom import dcmread, config as PYD_CONFIG
 from pydicom.dataset import Dataset
 from pydicom.uid import UID, ImplicitVRLittleEndian
 
 from pynetdicom import (
     AE,
     build_context,
     _config,
@@ -33,18 +33,16 @@
     PYD_CONFIG.settings.reading_validation_mode = 0
 
 
 # debug_logger()
 
 
 TEST_DS_DIR = os.path.join(os.path.dirname(__file__), "dicom_files")
-DATASET = read_file(os.path.join(TEST_DS_DIR, "RTImageStorage.dcm"))
-COMP_DATASET = read_file(
-    os.path.join(TEST_DS_DIR, "MRImageStorage_JPG2000_Lossless.dcm")
-)
+DATASET = dcmread(os.path.join(TEST_DS_DIR, "RTImageStorage.dcm"))
+COMP_DATASET = dcmread(os.path.join(TEST_DS_DIR, "MRImageStorage_JPG2000_Lossless.dcm"))
 
 
 def test_blocking_handler():
     """Test binding events to the blocking AssociationServer."""
     ae = AE()
     ae.add_supported_context("1.2.840.10008.1.1")
 
@@ -65,19 +63,19 @@
 
     ae.shutdown()
 
 
 class TestMakeServer:
     """Tests for AE.make_server()"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_default_arguments(self):
         self.ae = ae = AE()
         ae.add_supported_context(Verification)
@@ -111,19 +109,19 @@
             assert server.ae_title == "BADAE2"
             server.shutdown()
 
 
 class TestStartServer:
     """Tests for AE.start_server()"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_ae_title(self):
         """Test the `ae_title` keyword parameter."""
         self.ae = ae = AE()
@@ -172,19 +170,19 @@
 
         server.shutdown()
 
 
 class TestAEVerificationSCP:
     """Check verification SCP"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     @pytest.mark.skipif(os.name == "nt", reason="Kills pytest on windows")
     def test_start_server_keyboard_interrupt(self):
         """Test stopping the SCP with keyboard"""
@@ -226,19 +224,19 @@
         ae = AE()
         ae.__str__()
 
 
 class TestAEPresentationSCU:
     """Tests for AE presentation contexts when running as an SCU"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_associate_context(self):
         """Test that AE.associate doesn't modify the supplied contexts"""
         # Test AE.requested_contexts
@@ -421,19 +419,19 @@
 
         assoc.release()
 
         scp.shutdown()
 
 
 class TestAEGoodAssociation:
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_associate_establish_release(self):
         """Check SCU Association with SCP"""
         self.ae = ae = AE()
@@ -606,14 +604,15 @@
                 bind_address=("", 0),
             )
             assert not assoc.is_established
             assert assoc.is_aborted
             msgs = [
                 "TCP Initialisation Error: timed out",
                 "TCP Initialisation Error: [Errno -2] Name or service not known",
+                # "TCP Initialisation Error: [Errno 113] No route to host",
             ]
             assert len([m for m in msgs if m in caplog.text]) == 1
 
     def test_select_timeout_okay(self):
         """Test that using start works OK with timeout."""
         # Multiple release/association in a sort time causes an OSError as
         # the port is still in use due to the use of select.select() with
@@ -704,18 +703,18 @@
 
         msg = r"'ae_title' must be str, not 'int'"
         with pytest.raises(TypeError, match=msg):
             ae.associate("localhost", 11112, ae_title=12345)
 
 
 class TestAEGoodMiscSetters:
-    def setup(self):
+    def setup_method(self):
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
     def test_ae_title_good(self):
         """Check AE title change produces good value"""
         ae = AE()
         ae.ae_title = "     TEST     "
@@ -987,19 +986,19 @@
 
         msg = r"'ae_title' must be str, not 'NoneType'"
         with pytest.raises(TypeError, match=msg):
             AE(ae_title=None)
 
 
 class TestAE_GoodExit:
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_ae_release_assoc(self):
         """Association releases OK"""
         self.ae = ae = AE()
@@ -1046,15 +1045,15 @@
 
         scp.shutdown()
 
 
 class TestAESupportedPresentationContexts:
     """Tests for AE's presentation contexts when acting as an SCP"""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = AE()
 
     def test_add_supported_context_str(self):
         """Tests for AE.add_supported_context using str."""
         self.ae.add_supported_context("1.2.840.10008.1.1")
 
         context = self.ae.supported_contexts[0]
@@ -1469,15 +1468,15 @@
 
         assert self.ae.supported_contexts == []
 
 
 class TestAERequestedPresentationContexts:
     """Tests for AE's presentation contexts when acting as an SCU"""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = AE()
 
     def test_add_requested_context_str(self):
         """Tests for AE.add_requested_context using str."""
         self.ae.add_requested_context("1.2.840.10008.1.1")
 
         context = self.ae.requested_contexts[0]
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_assoc.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_assoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     PatientRootQueryRetrieveInformationModelGet,
     PatientRootQueryRetrieveInformationModelMove,
     PatientStudyOnlyQueryRetrieveInformationModelMove,
     StudyRootQueryRetrieveInformationModelMove,
     SecondaryCaptureImageStorage,
     UnifiedProcedureStepPull,
     UnifiedProcedureStepPush,
+    RepositoryQuery,
 )
 
 from .hide_modules import hide_modules
 
 
 # debug_logger()
 
@@ -88,14 +89,22 @@
 @pytest.fixture()
 def enable_unrestricted():
     _config.UNRESTRICTED_STORAGE_SERVICE = True
     yield
     _config.UNRESTRICTED_STORAGE_SERVICE = False
 
 
+@pytest.fixture
+def disable_identifer_logging():
+    original = _config.LOG_REQUEST_IDENTIFIERS
+    _config.LOG_REQUEST_IDENTIFIERS = False
+    yield
+    _config.LOG_REQUEST_IDENTIFIERS = original
+
+
 class DummyDIMSE:
     def __init__(self):
         self.status = None
         self.msg_queue = queue.Queue()
 
     def send_msg(self, rsp, context_id):
         self.status = rsp.Status
@@ -104,19 +113,19 @@
     def get_msg(self, block=False):
         return None, None
 
 
 class TestAssociation:
     """Run tests on Associtation."""
 
-    def setup(self):
+    def setup_method(self):
         """This function runs prior to all test methods"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """This function runs after all test methods"""
         if self.ae:
             self.ae.shutdown()
 
     def test_bad_connection(self, caplog):
         """Test connect to non-AE"""
         ae = AE()
@@ -610,18 +619,18 @@
         scp.shutdown()
 
 
 class TestCStoreSCP:
     """Tests for Association._c_store_scp()."""
 
     # Used with C-GET (always) and C-MOVE (over the same association)
-    def setup(self):
+    def setup_method(self):
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
     def test_no_context(self):
         """Test correct response if no valid presentation context."""
 
         def handle(event):
@@ -862,19 +871,19 @@
 
         scp.shutdown()
 
 
 class TestAssociationSendCEcho:
     """Run tests on Association evt.EVT_C_ECHO handler."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_must_be_associated(self):
         """Test can't send without association."""
         # Test raise if assoc not established
@@ -1251,27 +1260,28 @@
             assert "Network timeout reached" in caplog.text
             assert "Association Released" in caplog.text
 
 
 class TestAssociationSendCStore:
     """Run tests on Association send_c_store."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
         _config.STORE_SEND_CHUNKED_DATASET = False
 
     def test_must_be_associated(self):
         """Test SCU can't send without association."""
+
         # Test raise if assoc not established
         def handle_store(event):
             return 0x0000
 
         handlers = [(evt.EVT_C_STORE, handle_store)]
 
         self.ae = ae = AE()
@@ -1840,14 +1850,77 @@
             assoc.send_c_store(BAD_DATASET_PATH)
 
         assoc.release()
         assert assoc.is_released
 
         scp.shutdown()
 
+    def test_dataset_encoding_mismatch(self, caplog):
+        """Tests for when transfer syntax doesn't match dataset encoding."""
+
+        def handle_store(event):
+            return 0x0000
+
+        handlers = [(evt.EVT_C_STORE, handle_store)]
+
+        self.ae = ae = AE()
+        ae.acse_timeout = 5
+        ae.dimse_timeout = 5
+        ae.network_timeout = 5
+        ae.add_supported_context(
+            CTImageStorage,
+            [ExplicitVRBigEndian, ImplicitVRLittleEndian],
+        )
+        scp = ae.start_server(("localhost", 11112), block=False, evt_handlers=handlers)
+
+        ae.add_requested_context(CTImageStorage, ImplicitVRLittleEndian)
+        ae.add_requested_context(CTImageStorage, ExplicitVRBigEndian)
+        assoc = ae.associate("localhost", 11112)
+
+        assert assoc.is_established
+        ds = dcmread(DATASET_PATH)
+        assert ds.is_little_endian
+        assert not ds.is_implicit_VR
+        assert ds.file_meta.TransferSyntaxUID == ExplicitVRLittleEndian
+        ds.is_implicit_VR = True
+        with caplog.at_level(logging.WARNING, logger="pynetdicom"):
+            status = assoc.send_c_store(ds)
+            assert status.Status == 0x0000
+
+            ds.is_implicit_VR = False
+            ds.is_little_endian = False
+            status = assoc.send_c_store(ds)
+            assert status.Status == 0x0000
+
+        ds.is_implicit_VR = False
+        ds.is_little_endian = True
+        ds.file_meta.TransferSyntaxUID = ImplicitVRLittleEndian
+        msg = (
+            "'dataset' is encoded as explicit VR little endian but the file "
+            r"meta has a \(0002,0010\) Transfer Syntax UID of 'Implicit VR "
+            "Little Endian' - please set an appropriate Transfer Syntax"
+        )
+        with pytest.raises(AttributeError, match=msg):
+            status = assoc.send_c_store(ds)
+
+        assoc.release()
+        assert assoc.is_released
+        scp.shutdown()
+
+        assert (
+            "'dataset' is encoded as implicit VR little endian but the file "
+            "meta has a (0002,0010) Transfer Syntax UID of 'Explicit VR "
+            "Little Endian' - using 'Implicit VR Little Endian' instead"
+        ) in caplog.text
+        assert (
+            "'dataset' is encoded as explicit VR big endian but the file "
+            "meta has a (0002,0010) Transfer Syntax UID of 'Explicit VR "
+            "Little Endian' - using 'Explicit VR Big Endian' instead"
+        ) in caplog.text
+
     # Regression tests
     def test_no_send_mismatch(self):
         """Test sending a dataset with mismatched transfer syntax (206)."""
 
         def handle_store(event):
             return 0x0000
 
@@ -1919,23 +1992,23 @@
 
         assert "^^^^" == recv_ds[0].PatientName
 
 
 class TestAssociationSendCFind:
     """Run tests on Association send_c_find."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ds = Dataset()
         self.ds.PatientName = "*"
         self.ds.QueryRetrieveLevel = "PATIENT"
 
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_must_be_associated(self):
         """Test can't send without association."""
         # Test raise if assoc not established
@@ -2046,15 +2119,15 @@
             ("localhost", 11112), block=False, evt_handlers=[(evt.EVT_C_FIND, handle)]
         )
 
         ae.add_requested_context(PatientRootQueryRetrieveInformationModelFind)
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
 
-        for (status, ds) in assoc.send_c_find(
+        for status, ds in assoc.send_c_find(
             self.ds, PatientRootQueryRetrieveInformationModelFind
         ):
             assert status.Status == 0xA700
             assert ds is None
         assoc.release()
         assert assoc.is_released
 
@@ -2108,26 +2181,27 @@
             ("localhost", 11112), block=False, evt_handlers=[(evt.EVT_C_FIND, handle)]
         )
 
         ae.add_requested_context(PatientRootQueryRetrieveInformationModelFind)
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
 
-        for (status, ds) in assoc.send_c_find(
+        for status, ds in assoc.send_c_find(
             self.ds, PatientRootQueryRetrieveInformationModelFind
         ):
             assert status.Status == 0x0000
             assert ds is None
         assoc.release()
         assert assoc.is_released
 
         scp.shutdown()
 
     def test_rsp_empty(self):
         """Test receiving a success response from the peer"""
+
         # No matches
         def handle(event):
             pass
 
         self.ae = ae = AE()
         ae.acse_timeout = 5
         ae.dimse_timeout = 5
@@ -2137,15 +2211,15 @@
             ("localhost", 11112), block=False, evt_handlers=[(evt.EVT_C_FIND, handle)]
         )
 
         ae.add_requested_context(PatientRootQueryRetrieveInformationModelFind)
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
 
-        for (status, ds) in assoc.send_c_find(
+        for status, ds in assoc.send_c_find(
             self.ds, PatientRootQueryRetrieveInformationModelFind
         ):
             assert status.Status == 0x0000
             assert ds is None
         assoc.release()
         assert assoc.is_released
 
@@ -2166,15 +2240,15 @@
             ("localhost", 11112), block=False, evt_handlers=[(evt.EVT_C_FIND, handle)]
         )
 
         ae.add_requested_context(PatientRootQueryRetrieveInformationModelFind)
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
 
-        for (status, ds) in assoc.send_c_find(
+        for status, ds in assoc.send_c_find(
             self.ds, PatientRootQueryRetrieveInformationModelFind
         ):
             assert status.Status == 0xFE00
             assert ds is None
         assoc.release()
         assert assoc.is_released
 
@@ -2203,15 +2277,15 @@
                 return DummyResponse(), None
 
         assoc._reactor_checkpoint.clear()
         while not assoc._is_paused:
             time.sleep(0.01)
         assoc.dimse = DummyDIMSE()
         assert assoc.is_established
-        for (_, _) in assoc.send_c_find(
+        for _, _ in assoc.send_c_find(
             self.ds, PatientRootQueryRetrieveInformationModelFind
         ):
             pass
 
         assert assoc.is_aborted
 
         scp.shutdown()
@@ -2231,15 +2305,15 @@
             ("localhost", 11112), block=False, evt_handlers=[(evt.EVT_C_FIND, handle)]
         )
 
         ae.add_requested_context(PatientRootQueryRetrieveInformationModelFind)
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
 
-        for (status, ds) in assoc.send_c_find(
+        for status, ds in assoc.send_c_find(
             self.ds, PatientRootQueryRetrieveInformationModelFind
         ):
             assert status.Status == 0xFFF0
         assoc.release()
         assert assoc.is_released
 
         scp.shutdown()
@@ -2264,15 +2338,15 @@
             ("localhost", 11112), block=False, evt_handlers=[(evt.EVT_C_FIND, handle)]
         )
 
         model = PatientRootQueryRetrieveInformationModelFind
         ae.add_requested_context(model, ExplicitVRLittleEndian)
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
-        for (status, ds) in assoc.send_c_find(self.ds, model):
+        for status, ds in assoc.send_c_find(self.ds, model):
             assert status.Status in range(0xC000, 0xD000)
 
         assoc.release()
         assert assoc.is_released
 
         scp.shutdown()
 
@@ -2451,15 +2525,15 @@
         ae.add_requested_context(PatientRootQueryRetrieveInformationModelFind)
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
 
         responses = assoc.send_c_find(
             self.ds, PatientRootQueryRetrieveInformationModelFind
         )
-        for (status, ds) in responses:
+        for status, ds in responses:
             assert status.Status == 0x0000
             assert ds is None
         assoc.release()
         assert assoc.is_released
 
         scp.shutdown()
 
@@ -2491,23 +2565,96 @@
 
             msg = (
                 "No supported service class available for the SOP Class "
                 "UID '1.2.3.4'"
             )
             assert msg in caplog.text
 
+    def test_repository_query(self, caplog):
+        """Test receiving a success response from the peer"""
+
+        def handle(event):
+            yield 0xB001, None
+            yield 0x0000, None
+
+        self.ae = ae = AE()
+        ae.acse_timeout = 5
+        ae.dimse_timeout = 5
+        ae.network_timeout = 5
+        ae.add_supported_context(RepositoryQuery)
+        scp = ae.start_server(
+            ("localhost", 11112), block=False, evt_handlers=[(evt.EVT_C_FIND, handle)]
+        )
+
+        ae.add_requested_context(RepositoryQuery)
+        assoc = ae.associate("localhost", 11112)
+        assert assoc.is_established
+
+        with caplog.at_level(logging.INFO, logger="pynetdicom"):
+            responses = assoc.send_c_find(self.ds, RepositoryQuery)
+            status, ds = next(responses)
+            assert status.Status == 0xB001
+            assert ds is None
+            status, ds = next(responses)
+            assert status.Status == 0x0000
+            assert ds is None
+
+        assoc.release()
+        assert assoc.is_released
+
+        scp.shutdown()
+
+        msg = (
+            f"Find SCP Response: 1 - 0xB001 (Warning - Matching reached "
+            "response limit, subsequent request may return additional matches)"
+        )
+        assert msg in caplog.text
+
+    def test_identifier_logging(self, caplog, disable_identifer_logging):
+        """Test identifiers not logged if config option set"""
+
+        def handle(event):
+            yield 0x0000, None
+
+        self.ae = ae = AE()
+        ae.acse_timeout = 5
+        ae.dimse_timeout = 5
+        ae.network_timeout = 5
+        ae.add_supported_context(PatientRootQueryRetrieveInformationModelFind)
+        scp = ae.start_server(
+            ("localhost", 11112), block=False, evt_handlers=[(evt.EVT_C_FIND, handle)]
+        )
+
+        ae.add_requested_context(PatientRootQueryRetrieveInformationModelFind)
+        assoc = ae.associate("localhost", 11112)
+        assert assoc.is_established
+
+        with caplog.at_level(logging.INFO, logger="pynetdicom"):
+            for status, ds in assoc.send_c_find(
+                self.ds, PatientRootQueryRetrieveInformationModelFind
+            ):
+                assert status.Status == 0x0000
+                assert ds is None
+
+        assoc.release()
+        assert assoc.is_released
+
+        scp.shutdown()
+
+        assert "(0010,0010) PN" not in caplog.text
+
 
 class TestAssociationSendCCancel:
     """Run tests on Association send_c_cancel."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_must_be_associated(self):
         """Test can't send without association."""
         # Test raise if assoc not established
@@ -2598,30 +2745,30 @@
 
         scp.shutdown()
 
 
 class TestAssociationSendCGet:
     """Run tests on Association send_c_get."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ds = Dataset()
         self.ds.PatientName = "*"
         self.ds.QueryRetrieveLevel = "PATIENT"
 
         self.good = Dataset()
         self.good.file_meta = FileMetaDataset()
         self.good.file_meta.TransferSyntaxUID = ImplicitVRLittleEndian
         self.good.SOPClassUID = CTImageStorage
         self.good.SOPInstanceUID = "1.1.1"
         self.good.PatientName = "Test"
 
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_must_be_associated(self):
         """Test can't send without association."""
         self.ae = ae = AE()
@@ -2793,15 +2940,15 @@
             "localhost",
             11112,
             ext_neg=[role],
             evt_handlers=[(evt.EVT_C_STORE, handle_store)],
         )
         assert assoc.is_established
 
-        for (status, ds) in assoc.send_c_get(
+        for status, ds in assoc.send_c_get(
             self.ds, PatientRootQueryRetrieveInformationModelGet
         ):
             assert status.Status == 0xA701
         assoc.release()
         assert assoc.is_released
 
         scp.shutdown()
@@ -3060,15 +3207,15 @@
             "localhost",
             11112,
             ext_neg=[role],
             evt_handlers=[(evt.EVT_C_STORE, handle_store)],
         )
         assert assoc.is_established
 
-        for (status, ds) in assoc.send_c_get(
+        for status, ds in assoc.send_c_get(
             self.ds, PatientRootQueryRetrieveInformationModelGet
         ):
             assert status.Status == 0xFE00
         assoc.release()
         assert assoc.is_released
 
         scp.shutdown()
@@ -3160,15 +3307,15 @@
             "localhost",
             11112,
             ext_neg=[role],
             evt_handlers=[(evt.EVT_C_STORE, handle_store)],
         )
         assert assoc.is_established
 
-        for (status, ds) in assoc.send_c_get(
+        for status, ds in assoc.send_c_get(
             self.ds, PatientRootQueryRetrieveInformationModelGet
         ):
             assert status.Status == 0xFFF0
         assoc.release()
         assert assoc.is_released
 
         scp.shutdown()
@@ -3372,15 +3519,15 @@
         ae.add_requested_context(PatientRootQueryRetrieveInformationModelGet)
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
 
         responses = assoc.send_c_get(
             self.ds, PatientRootQueryRetrieveInformationModelGet
         )
-        for (status, ds) in responses:
+        for status, ds in responses:
             assert status.Status == 0x0000
             assert ds is None
         assoc.release()
         assert assoc.is_released
 
         scp.shutdown()
 
@@ -3555,34 +3702,91 @@
         assoc.release()
         assert assoc.is_released
 
         assert store_pname == ["Unknown^Public"]
 
         scp.shutdown()
 
+    def test_identifier_logging(self, caplog, disable_identifer_logging):
+        """Test identifiers not logged if config option set"""
+
+        def handle_get(event):
+            yield 2
+            yield 0xFF00, self.good
+            yield 0xFF00, self.good
+
+        def handle_store(event):
+            return 0x0000
+
+        scu_handler = [(evt.EVT_C_STORE, handle_store)]
+        scp_handler = [(evt.EVT_C_GET, handle_get)]
+
+        self.ae = ae = AE()
+        ae.acse_timeout = 5
+        ae.dimse_timeout = 5
+        ae.network_timeout = 5
+        ae.add_supported_context(PatientRootQueryRetrieveInformationModelGet)
+        ae.add_supported_context(CTImageStorage, scu_role=True, scp_role=True)
+
+        scp = ae.start_server(
+            ("localhost", 11112), block=False, evt_handlers=scp_handler
+        )
+
+        ae.add_requested_context(PatientRootQueryRetrieveInformationModelGet)
+        ae.add_requested_context(CTImageStorage)
+
+        role = build_role(CTImageStorage, scp_role=True, scu_role=True)
+
+        assoc = ae.associate(
+            "localhost", 11112, evt_handlers=scu_handler, ext_neg=[role]
+        )
+
+        assert assoc.is_established
+
+        with caplog.at_level(logging.INFO, logger="pynetdicom"):
+            result = assoc.send_c_get(
+                self.ds, PatientRootQueryRetrieveInformationModelGet
+            )
+            (status, ds) = next(result)
+            assert status.Status == 0xFF00
+            assert ds is None
+            (status, ds) = next(result)
+            assert status.Status == 0xFF00
+            assert ds is None
+            (status, ds) = next(result)
+            assert status.Status == 0x0000
+            assert ds is None
+
+        assoc.release()
+        assert assoc.is_released
+
+        scp.shutdown()
+
+        assert "(0010,0010) PN" not in caplog.text
+
 
 class TestAssociationSendCMove:
     """Run tests on Association send_c_move."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ds = Dataset()
         self.ds.PatientName = "*"
         self.ds.QueryRetrieveLevel = "PATIENT"
 
         self.good = Dataset()
         self.good.file_meta = FileMetaDataset()
         self.good.file_meta.TransferSyntaxUID = ImplicitVRLittleEndian
         self.good.SOPClassUID = CTImageStorage
         self.good.SOPInstanceUID = "1.1.1"
         self.good.PatientName = "Test"
 
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_must_be_associated(self):
         """Test can't send without association."""
         # Test raise if assoc not established
@@ -3679,14 +3883,15 @@
         assert assoc.is_released
         del DATASET.PerimeterValue  # Fix up our changes
 
         scp.shutdown()
 
     def test_move_destination_no_assoc(self):
         """Test move destination failed to assoc"""
+
         # Move SCP
         def handle_move(event):
             yield "localhost", 11113
             yield 2
             yield 0xFF00, self.good
 
         self.ae = ae = AE()
@@ -3699,15 +3904,15 @@
             block=False,
             evt_handlers=[(evt.EVT_C_MOVE, handle_move)],
         )
 
         ae.add_requested_context(PatientRootQueryRetrieveInformationModelMove)
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
-        for (status, ds) in assoc.send_c_move(
+        for status, ds in assoc.send_c_move(
             self.ds, "TESTMOVE", PatientRootQueryRetrieveInformationModelMove
         ):
             assert status.Status == 0xA801
         assoc.release()
         assert assoc.is_released
 
         move_scp.shutdown()
@@ -3731,15 +3936,15 @@
             evt_handlers=[(evt.EVT_C_MOVE, handle_move)],
         )
 
         ae.add_requested_context(PatientRootQueryRetrieveInformationModelMove)
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
 
-        for (status, ds) in assoc.send_c_move(
+        for status, ds in assoc.send_c_move(
             self.ds, "UNKNOWN", PatientRootQueryRetrieveInformationModelMove
         ):
             assert status.Status == 0xA801
         assoc.release()
         assert assoc.is_released
 
         move_scp.shutdown()
@@ -4089,15 +4294,15 @@
             evt_handlers=[(evt.EVT_C_STORE, handle_store)],
         )
 
         ae.add_requested_context(PatientRootQueryRetrieveInformationModelMove)
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
 
-        for (status, ds) in assoc.send_c_move(
+        for status, ds in assoc.send_c_move(
             self.ds, "TESTMOVE", PatientRootQueryRetrieveInformationModelMove
         ):
             assert status.Status == 0xFFF0
         assoc.release()
         assert assoc.is_released
 
         store_scp.shutdown()
@@ -4443,23 +4648,87 @@
 
             msg = (
                 "No supported service class available for the SOP Class "
                 "UID '1.2.3.4'"
             )
             assert msg in caplog.text
 
+    def test_identifier_logging(self, caplog, disable_identifer_logging):
+        """Test identifiers not logged if config option set"""
+
+        def handle_store(event):
+            return 0x0000
+
+        self.ae = ae = AE()
+        ae.acse_timeout = 5
+        ae.dimse_timeout = 5
+        ae.network_timeout = 5
+
+        # Storage SCP
+        ae.add_supported_context(CTImageStorage)
+        store_scp = ae.start_server(
+            ("localhost", 11112),
+            block=False,
+            evt_handlers=[(evt.EVT_C_STORE, handle_store)],
+        )
+
+        # Move SCP
+        def handle_move(event):
+            yield "localhost", 11112
+            yield 2
+            yield 0xFF00, self.good
+
+        ae.add_requested_context(CTImageStorage)
+        ae.add_supported_context(PatientRootQueryRetrieveInformationModelMove)
+        ae.add_supported_context(StudyRootQueryRetrieveInformationModelMove)
+        ae.add_supported_context(PatientStudyOnlyQueryRetrieveInformationModelMove)
+        move_scp = ae.start_server(
+            ("localhost", 11113),
+            block=False,
+            evt_handlers=[(evt.EVT_C_MOVE, handle_move)],
+        )
+
+        # Move SCU
+        ae.add_requested_context(PatientRootQueryRetrieveInformationModelMove)
+        ae.add_requested_context(StudyRootQueryRetrieveInformationModelMove)
+        ae.add_requested_context(PatientStudyOnlyQueryRetrieveInformationModelMove)
+
+        assoc = ae.associate("localhost", 11113)
+        assert assoc.is_established
+
+        with caplog.at_level(logging.INFO, logger="pynetdicom"):
+            result = assoc.send_c_move(
+                self.ds, "TESTMOVE", PatientRootQueryRetrieveInformationModelMove
+            )
+            (status, ds) = next(result)
+            assert status.Status == 0xFF00
+            assert ds is None
+            (status, ds) = next(result)
+            assert status.Status == 0x0000
+            assert ds is None
+            with pytest.raises(StopIteration):
+                next(result)
+
+        assoc.release()
+        assert assoc.is_released
+
+        store_scp.shutdown()
+        move_scp.shutdown()
+
+        assert "(0010,0010) PN" not in caplog.text
+
 
 class TestGetValidContext:
     """Tests for Association._get_valid_context."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_id_no_abstract_syntax_match(self):
         """Test exception raised if with ID no abstract syntax match"""
         self.ae = ae = AE()
@@ -5169,19 +5438,19 @@
         assoc.release()
         scp.shutdown()
 
 
 class TestEventHandlingAcceptor:
     """Test the transport events and handling as acceptor."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
         _config.LOG_HANDLER_LEVEL = "none"
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
         _config.LOG_HANDLER_LEVEL = "standard"
 
     def test_no_handlers(self):
         """Test with no association event handlers bound."""
@@ -6473,19 +6742,19 @@
         assert len(arguments) == 1
         assert args == list(arguments[0])
 
 
 class TestEventHandlingRequestor:
     """Test the transport events and handling as acceptor."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
         _config.LOG_HANDLER_LEVEL = "none"
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
         _config.LOG_HANDLER_LEVEL = "standard"
 
     def test_no_handlers(self):
         """Test with no association event handlers bound."""
@@ -7242,19 +7511,19 @@
         assert args == list(arguments[0])
 
 
 @pytest.mark.skipif(not ON_WINDOWS, reason="Not running on Windows")
 class TestAssociationWindows:
     """Windows specific association tests."""
 
-    def setup(self):
+    def setup_method(self):
         """This function runs prior to all test methods"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """This function runs after all test methods"""
         if self.ae:
             self.ae.shutdown()
 
         import importlib
 
         importlib.reload(pynetdicom.utils)
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_assoc_n.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_assoc_n.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,18 +39,18 @@
     def get_msg(self, block=False):
         return None, None
 
 
 class TestAssociationSendNEventReport:
     """Run tests on Association send_n_event_report."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_must_be_associated(self):
         """Test can't send without association."""
 
@@ -664,19 +664,19 @@
 
         scp.shutdown()
 
 
 class TestAssociationSendNGet:
     """Run tests on Association send_n_get."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_must_be_associated(self):
         """Test can't send without association."""
 
@@ -1219,18 +1219,18 @@
 
         scp.shutdown()
 
 
 class TestAssociationSendNSet:
     """Run tests on Association send_n_set."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_must_be_associated(self):
         """Test can't send without association."""
 
@@ -1798,18 +1798,18 @@
 
         scp.shutdown()
 
 
 class TestAssociationSendNAction:
     """Run tests on Association send_n_action."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_must_be_associated(self):
         """Test can't send without association."""
 
@@ -2332,18 +2332,18 @@
 
         scp.shutdown()
 
 
 class TestAssociationSendNCreate:
     """Run tests on Association send_n_create."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_must_be_associated(self):
         """Test can't send without association."""
 
@@ -2892,18 +2892,18 @@
 
         scp.shutdown()
 
 
 class TestAssociationSendNDelete:
     """Run tests on Association send_n_delete."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_must_be_associated(self):
         """Test can't send without association."""
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_assoc_user.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_assoc_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 # debug_logger()
 
 
 class TestServiceUserAcceptor:
     """Tests for ServiceUser as acceptor."""
 
-    def setup(self):
+    def setup_method(self):
         self.assoc = Association(AE(), mode="requestor")
 
         primitive = A_ASSOCIATE()
         primitive.application_context_name = "1.2.840.10008.3.1.1.1"
         primitive.calling_ae_title = "LOCAL_AE_TITLE  "
         primitive.called_ae_title = "REMOTE_AE_TITLE "
         primitive.result = 0x00
@@ -160,15 +160,15 @@
         assert user._contexts == [1]
         assert user.maximum_length == 16383
 
     def test_mode_assignment_raises(self):
         """Test that assigning mode after init raises exception."""
         user = ServiceUser(self.assoc, mode="acceptor")
         assert user.mode == "acceptor"
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             user.mode = "requestor"
 
         assert user.mode == "acceptor"
 
     def test_minimal_ac(self):
         """Test access with a minimal allowed A-ASSOCIATE (ac) primitive."""
         user = ServiceUser(self.assoc, mode="acceptor")
@@ -254,15 +254,15 @@
         assert user.sop_class_common_extended == {}
 
         item = user.user_identity
         assert item.user_identity_type == 0x01
         assert item.primary_field == b"username"
 
     def test_info(self):
-        """Test the .info propoerty"""
+        """Test the .info property"""
         user = ServiceUser(self.assoc, mode="acceptor")
         info = user.info
 
         assert info["port"] is None
         assert info["mode"] == "acceptor"
         assert info["address"] == ""
         assert info["ae_title"] == ""
@@ -293,30 +293,30 @@
         msg = (
             r"Can't set the Implementation Version Name after negotiation "
             r"has started"
         )
         with pytest.raises(RuntimeError, match=msg):
             user.implementation_version_name = "1.2.3"
 
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             user.asynchronous_operations = (1, 1)
 
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             user.role_selection = {}
 
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             user.sop_class_common_extended = {}
 
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             user.sop_class_extended = {}
 
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             user.user_identity = "test"
 
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             user.extended_negotiation = []
 
     def test_add_neg_pre(self):
         """Test adding negotiation items."""
         user = ServiceUser(self.assoc, mode="acceptor")
         assert len(user.extended_negotiation) == 0
         assert len(user.user_information) == 2
@@ -1378,15 +1378,15 @@
             user.ae_title = b"BADAE2"
             assert user.ae_title == "BADAE2"
 
 
 class TestServiceUserRequestor:
     """Tests for ServiceUser as requestor."""
 
-    def setup(self):
+    def setup_method(self):
         self.assoc = Association(AE(), mode="requestor")
 
         primitive = A_ASSOCIATE()
         primitive.application_context_name = "1.2.840.10008.3.1.1.1"
         primitive.calling_ae_title = "LOCAL_AE_TITLE  "
         primitive.called_ae_title = "REMOTE_AE_TITLE "
         primitive.calling_presentation_address = ("127.0.0.1", 11112)
@@ -1473,15 +1473,15 @@
         assert user._contexts == [1]
         assert user.maximum_length == 16383
 
     def test_mode_assignment_raises(self):
         """Test that assigning mode after init raises exception."""
         user = ServiceUser(self.assoc, mode="requestor")
         assert user.mode == "requestor"
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             user.mode = "acceptor"
 
         assert user.mode == "requestor"
 
     def test_minimal(self):
         """Test access with a minimal allowed A-ASSOCIATE primitive."""
         user = ServiceUser(self.assoc, mode="requestor")
@@ -1558,15 +1558,15 @@
         assert classes["1.2.3"].related_general_sop_class_identification == ["1.3.4"]
 
         item = user.user_identity
         assert item.user_identity_type == 0x01
         assert item.primary_field == b"username"
 
     def test_info(self):
-        """Test the .info propoerty"""
+        """Test the .info property"""
         user = ServiceUser(self.assoc, mode="requestor")
         info = user.info
 
         assert info["port"] is None
         assert info["mode"] == "requestor"
         assert info["address"] == ""
         assert info["ae_title"] == ""
@@ -1597,30 +1597,30 @@
         msg = (
             r"Can't set the Implementation Version Name after negotiation "
             r"has started"
         )
         with pytest.raises(RuntimeError, match=msg):
             user.implementation_version_name = "1.2.3"
 
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             user.asynchronous_operations = (1, 1)
 
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             user.role_selection = {}
 
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             user.sop_class_common_extended = {}
 
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             user.sop_class_extended = {}
 
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             user.user_identity = "test"
 
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             user.extended_negotiation = []
 
     def test_accepted_common_raises(self):
         """Test trying to get the accepted common ext items raises."""
         user = ServiceUser(self.assoc, mode="requestor")
 
         msg = r"'accepted_common_extended' is only available for the " r"'acceptor'"
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_cli.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Tests for the command-line interface."""
 
 import subprocess
+import sys
 
 import pytest
 
 from pynetdicom import __version__
 
 
 def test_version():
     """Test --version."""
-    command = ["python", "-m", "pynetdicom", "--version"]
+    command = [sys.executable, "-m", "pynetdicom", "--version"]
     out = subprocess.check_output(command)
     assert __version__ == out.decode("utf-8").strip()
 
 
 def test_echoscu():
     """Test echoscu."""
-    command = ["python", "-m", "pynetdicom", "echoscu", "localhost", "11112"]
+    command = [sys.executable, "-m", "pynetdicom", "echoscu", "localhost", "11112"]
     p = subprocess.Popen(command, stderr=subprocess.PIPE)
     p.wait()
     assert p.returncode == 1
     out, err = p.communicate()
     assert "unable to connect to remote" in err.decode("utf-8")
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_dimse_c.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_dimse_c.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     c_move_rq_cmd,
     c_move_rq_ds,
     c_move_rsp_cmd,
     c_move_rsp_ds,
 )
 
 
-LOGGER = logging.getLogger("pynetdicom")
+LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.CRITICAL)
 
 
 @pytest.fixture()
 def use_long_aet():
     _config.USE_SHORT_DIMSE_AET = False
     yield
@@ -71,19 +71,19 @@
         with pytest.raises(TypeError):
             primitive.MessageIDBeingRespondedTo = "test"
 
 
 class TestPrimitive_C_STORE:
     """Test DIMSE C-STORE operations."""
 
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
         self.default_aet_length = _config.USE_SHORT_DIMSE_AET
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
         _config.USE_SHORT_DIMSE_AET = self.default_aet_length
 
     def test_assignment(self):
         """Check assignment works correctly"""
         primitive = C_STORE()
 
@@ -393,18 +393,18 @@
 
         assert primitive.MoveOriginatorApplicationEntityTitle == "TEST"
 
 
 class TestPrimitive_C_FIND:
     """Test DIMSE C-FIND operations."""
 
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_assignment(self):
         """Check assignment works correctly"""
         primitive = C_FIND()
 
         primitive.MessageID = 11
@@ -606,18 +606,18 @@
         primitive.Status = 0x0000
         assert primitive.is_valid_response
 
 
 class TestPrimitive_C_GET:
     """Test DIMSE C-GET operations."""
 
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_assignment(self):
         """Check assignment works correctly"""
         primitive = C_GET()
 
         primitive.MessageID = 11
@@ -862,19 +862,19 @@
         primitive.Status = 0x0000
         assert primitive.is_valid_response
 
 
 class TestPrimitive_C_MOVE:
     """Test DIMSE C-MOVE operations."""
 
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
         self.default_aet_length = _config.USE_SHORT_DIMSE_AET
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
         _config.USE_SHORT_DIMSE_AET = self.default_aet_length
 
     def test_assignment(self):
         """Check assignment works correctly"""
         primitive = C_MOVE()
 
@@ -1175,18 +1175,18 @@
 
         assert primitive.MoveDestination == "TEST"
 
 
 class TestPrimitive_C_ECHO:
     """Test DIMSE C-ECHO operations."""
 
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_assignment(self):
         """Check assignment works correctly"""
         primitive = C_ECHO()
 
         primitive.MessageID = 11
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_dimse_msg.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_dimse_msg.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     n_set_rq_ds,
     n_set_rsp_cmd,
     n_set_rsp_ds,
     n_create_rq_cmd_empty,
     n_set_rq_cmd_empty,
 )
 
-LOGGER = logging.getLogger("pynetdicom")
+LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.CRITICAL)
 
 
 def print_nice_bytes(bytestream):
     """Nice output for bytestream."""
     str_list = pretty_bytes(
         bytestream, prefix="b'\\x", delimiter="\\x", items_per_line=10, suffix="' \\"
@@ -747,15 +747,15 @@
         assert primitive.MessageID == 7
         assert primitive.RequestedSOPInstanceUID is None
 
 
 class TestThreadSafety:
     """Tests for the thread safety of DIMSEMessage classes."""
 
-    def setup(self):
+    def setup_method(self):
         ds = Dataset()
         ds.SOPClassUID = "1.2.840.10008.5.1.4.1.1"
         ds.SOPInstanceUID = "1.2.3.4"
         ds.PatientName = "Test^Testing"
         self.ds = ds
 
     def test_msg_init(self):
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_dimse_n.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_dimse_n.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,25 +65,25 @@
 )
 
 
 if hasattr(PYD_CONFIG, "settings"):
     PYD_CONFIG.settings.reading_validation_mode = 0
 
 
-LOGGER = logging.getLogger("pynetdicom")
+LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.CRITICAL)
 
 
 class TestPrimitive_N_EVENT:
     """Test DIMSE N-EVENT-REPORT operations."""
 
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_assignment(self):
         """Check assignment works correctly"""
         primitive = N_EVENT_REPORT()
 
         # AffectedSOPClassUID
@@ -326,18 +326,18 @@
         primitive.Status = 0x0000
         assert primitive.is_valid_response
 
 
 class TestPrimitive_N_GET:
     """Test DIMSE N-GET operations."""
 
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_assignment(self):
         """Check assignment works correctly"""
         primitive = N_GET()
 
         # AffectedSOPClassUID
@@ -381,15 +381,15 @@
             Tag(0x7FE0, 0x0010),
         ] == primitive.AttributeIdentifierList
         primitive.AttributeIdentifierList = [(0x7FE0, 0x0010)]
         assert Tag(0x7FE0, 0x0010) == primitive.AttributeIdentifierList
         primitive.AttributeIdentifierList = (0x7FE0, 0x0010)
         assert Tag(0x7FE0, 0x0010) == primitive.AttributeIdentifierList
 
-        elem = DataElement((0x0000, 0x0005), "AT", [Tag(0x0000, 0x1000)])
+        elem = DataElement((0x0000, 0x0005), "AT", Tag(0x0000, 0x1000))
         assert isinstance(elem.value, BaseTag)
         primitive.AttributeIdentifierList = elem.value
         assert Tag(0x0000, 0x1000) == primitive.AttributeIdentifierList
 
         # MessageID
         primitive.MessageID = 11
         assert 11 == primitive.MessageID
@@ -628,18 +628,18 @@
         primitive.Status = 0x0000
         assert primitive.is_valid_response
 
 
 class TestPrimitive_N_SET:
     """Test DIMSE N-SET operations."""
 
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_assignment(self):
         """Check assignment works correctly"""
         primitive = N_SET()
 
         # AffectedSOPClassUID
@@ -928,18 +928,18 @@
         primitive.Status = 0x0000
         assert primitive.is_valid_response
 
 
 class TestPrimitive_N_ACTION:
     """Test DIMSE N-ACTION operations."""
 
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_assignment(self):
         """Check assignment works correctly"""
         primitive = N_ACTION()
 
         # Action Type ID
@@ -1234,18 +1234,18 @@
         primitive.Status = 0x0000
         assert primitive.is_valid_response
 
 
 class TestPrimitive_N_CREATE:
     """Test DIMSE N-CREATE operations."""
 
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_assignment(self):
         """Check assignment works correctly"""
         primitive = N_CREATE()
 
         # AffectedSOPClassUID
@@ -1453,18 +1453,18 @@
         primitive.Status = 0x0000
         assert primitive.is_valid_response
 
 
 class TestPrimitive_N_DELETE:
     """Test DIMSE N-DELETE operations."""
 
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_assignment(self):
         """Check assignment works correctly"""
         primitive = N_DELETE()
 
         # AffectedSOPClassUID
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_dimse_provider.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_dimse_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,15 @@
     (N_DELETE(), ("N_DELETE_RQ", "N_DELETE_RSP")),
 ]
 
 
 class TestDIMSEProvider:
     """Test DIMSE service provider operations."""
 
-    def setup(self):
+    def setup_method(self):
         """Set up"""
         self.dimse = DIMSEServiceProvider(DummyAssociation())
 
     def test_receive_not_pdata(self):
         """Test we get back None if not a P_DATA"""
         assert self.dimse.get_msg(True) == (None, None)
 
@@ -226,19 +226,19 @@
         dimse.receive_primitive(pdata)
         assert dimse.assoc.dul.event_queue.get() == "Evt19"
 
 
 class TestEventHandlingAcceptor:
     """Test the transport events and handling as acceptor."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
         _config.LOG_HANDLER_LEVEL = "none"
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
         _config.LOG_HANDLER_LEVEL = "standard"
 
     def test_no_handlers(self):
         """Test with no transport event handlers bound."""
@@ -597,19 +597,19 @@
             assert msg in caplog.text
             assert "Exception description" in caplog.text
 
 
 class TestEventHandlingRequestor:
     """Test the transport events and handling as requestor."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
         _config.LOG_HANDLER_LEVEL = "none"
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
         _config.LOG_HANDLER_LEVEL = "standard"
 
     def test_no_handlers(self):
         """Test with no transport event handlers bound."""
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_dsutils.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_dsutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         with pytest.raises(AttributeError):
             print(decode(dummy, False, True))
 
 
 class TestPrettyElement:
     """Tests for pretty_element()."""
 
-    def teardown(self):
+    def teardown_method(self):
         config.DS_decimal(False)
         config.datetime_conversion = False
 
     def test_bytes_empty(self):
         """Test empty byte VRs"""
         ds = Dataset()
         ds.PixelData = b""
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_dul.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_dul.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,19 +74,19 @@
     READ_PDU_EXC_B - test_assoc.py::TestAssociation::test_unknown_abort_source
     READ_PDU_EXC_C - test_assoc.py::TestAssociation::test_bad_connection
     READ_PDU_EXC_D - test_dul.py::TestDUL::test_recv_short_aborts
     READ_PDU_EXC_E - test_dul.py::TestDUL::test_recv_missing_data
     READ_PDU_EXC_F - test_dul.py::TestDUL::test_recv_bad_pdu_aborts
     """
 
-    def setup(self):
+    def setup_method(self):
         self.scp = None
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         if self.scp:
             self.scp.commands = [("exit", None)]
             self.scp.step
             self.scp.commands = []
             self.scp.shutdown()
 
         if self.ae:
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_environment.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
     def test_python_version(self):
         """Test that the python version is correct."""
         version = get_envar("PYTHON_VERSION")
         if not version:
             raise RuntimeError("No 'PYTHON_VERSION' envar has been set")
 
+        # remove any pre-release suffix
+        version = version.split("-")[0]
         version = tuple([int(vv) for vv in version.split(".")])
         assert version[:2] == sys.version_info[:2]
 
 
 # Tests for the pynetdicom version
 def test_is_canonical():
     """Test is_canonical"""
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_events.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,28 +90,28 @@
     assert evt.EVT_C_ECHO not in evt._NOTIFICATION_EVENTS
     assert evt.EVT_DATA_RECV in evt._NOTIFICATION_EVENTS
 
 
 class TestEvent:
     """Tests for event.Event."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
         _config.LOG_HANDLER_LEVEL = "none"
 
         # Implicit VR Little Endian
         self.bytestream = BytesIO(
             #  (0010,0010) PatientName
             # | tag           | length        | value
             b"\x10\x00\x10\x00\x09\x00\x00\x00"
             b"\x54\x45\x53\x54\x5E\x54\x65\x73\x74"
         )
         self.context = build_context("1.2.840.10008.1.1", ImplicitVRLittleEndian)
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
         _config.LOG_HANDLER_LEVEL = "standard"
 
     def test_init(self):
         """Test initialisation of event.Event."""
@@ -146,14 +146,21 @@
             r"The corresponding event is not a C-STORE "
             r"request and has no 'Data Set' parameter"
         )
         with pytest.raises(AttributeError, match=msg):
             event.dataset
 
         msg = (
+            r"The corresponding event is not a C-STORE request "
+            r"and has no 'Data Set' parameter"
+        )
+        with pytest.raises(AttributeError, match=msg):
+            event.encoded_dataset()
+
+        msg = (
             r"The corresponding event is not a C-FIND, C-GET or C-MOVE request "
             r"and has no 'Identifier' parameter"
         )
         with pytest.raises(AttributeError, match=msg):
             event.identifier
 
         msg = (
@@ -479,14 +486,15 @@
         assert isinstance(tags[1], BaseTag)
         assert tags[1] == 0x00100020
 
         request.AttributeIdentifierList = 0x00100010
         event = Event(
             None, evt.EVT_N_GET, {"request": request, "context": self.context.as_tuple}
         )
+
         tags = event.attribute_identifiers
         assert tags == [0x00100010]
 
     def test_action_type(self):
         """Test with action_type."""
         request = N_ACTION()
         request.ActionTypeID = 2
@@ -506,14 +514,48 @@
             None,
             evt.EVT_N_EVENT_REPORT,
             {"request": request, "context": self.context.as_tuple},
         )
 
         assert event.event_type == 2
 
+    def test_encode_dataset(self):
+        """Test Event.encode_dataset()"""
+        request = C_STORE()
+        request.AffectedSOPClassUID = "1.2"
+        request.AffectedSOPInstanceUID = "1.3"
+        request.DataSet = BytesIO(b"\x00\x01")
+
+        event = Event(
+            None,
+            evt.EVT_C_STORE,
+            {"request": request, "context": self.context.as_tuple},
+        )
+        bs = event.encoded_dataset()
+
+        from pynetdicom.utils import pretty_bytes
+
+        assert bs[:128] == b"\x00" * 128
+        assert bs[128:132] == b"DICM"
+        assert bs[132:144] == b"\x02\x00\x00\x00\x55\x4c\x04\x00\x7e\x00\x00\x00"
+        assert bs[144:144 + 64] == (
+            b"\x02\x00\x01\x00\x4f\x42\x00\x00\x02\x00\x00\x00\x00\x01"
+            b"\x02\x00\x02\x00\x55\x49\x04\x00\x31\x2e\x32\x00"
+            b"\x02\x00\x03\x00\x55\x49\x04\x00\x31\x2e\x33\x00"
+            b"\x02\x00\x10\x00\x55\x49\x12\x00\x31\x2e\x32\x2e\x38\x34"
+            b"\x30\x2e\x31\x30\x30\x30\x38\x2e\x31\x2e\x32\x00"
+        )
+
+        # Note: may not be 126 if Implementation Class and Version change
+        assert 128 + 4 + 12 + 126 + 2== len(bs)
+
+        # Test without file_meta
+        bs = event.encoded_dataset(include_meta=False)
+        assert bs == b"\x00\x01"
+
 
 # TODO: Should be able to remove in v1.4
 INTERVENTION_HANDLERS = [
     _async_ops_handler,
     _sop_common_handler,
     _sop_extended_handler,
     _user_identity_handler,
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_fsm.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_fsm.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,15 +189,15 @@
             assert fsm.dul.is_killed is True
             assert fsm.current_state == state
 
 
 class TestStateBase:
     """Base class for State tests."""
 
-    def setup(self):
+    def setup_method(self):
         ae = AE()
         ae.add_requested_context(Verification)
         ae.acse_timeout = 5
         ae.dimse_timeout = 5
 
         assoc = Association(ae, mode="requestor")
 
@@ -220,15 +220,15 @@
         cx.context_id = 1
         assoc.requestor.requested_contexts = [cx]
 
         self.assoc = assoc
         self.fsm = self.monkey_patch(assoc.dul.state_machine)
         self.scp = None
 
-    def teardown(self):
+    def teardown_method(self):
         if self.scp:
             for commands in self.scp.commands:
                 self.scp.step()
             # self.scp.commands = [('exit', None)]
             # self.scp.step()
             self.scp.shutdown()
 
@@ -397,15 +397,15 @@
         cx = build_context(Verification)
         cx.context_id = 1
         assoc.acceptor.supported_contexts = [cx]
 
         fsm = self.monkey_patch(assoc.dul.state_machine)
         return assoc, fsm
 
-    def wait_on_state(self, fsm, state, timeout=2):
+    def wait_on_state(self, fsm, state, timeout=5):
         start = 0
         while (
             fsm.current_state != state
             and fsm.current_state not in state
             and start < timeout
         ):
             time.sleep(0.0001)
@@ -1842,15 +1842,15 @@
             """Override the socket's connect so no event gets added."""
             if assoc.dul.socket.socket is None:
                 assoc.dul.socket.socket = assoc.dul.socket._create_socket()
 
             try:
                 assoc.dul.socket.socket.connect(address)
                 assoc.dul.socket._is_connected = True
-            except (socket.error, socket.timeout) as exc:
+            except (OSError, TimeoutError) as exc:
                 assoc.dul.socket.close()
 
         assoc.dul.socket.connect = connect
 
         assoc.start()
         self.wait_on_state(assoc.dul.state_machine, "Sta4")
 
@@ -2301,26 +2301,30 @@
         pass
 
     def test_evt03(self):
         """Test Sta5 + Evt3."""
         # Sta5 + Evt3 -> AE-3 -> Sta6
         # Evt3: Receive A-ASSOCIATE-AC PDU from <remote>
         # AE-3: Issue A-ASSOCIATE (ac) primitive
-        commands = [("recv", None), ("send", a_associate_ac), ("exit", None)]
+        commands = [
+            ("recv", None),
+            ("send", a_associate_ac),
+            ("exit", None),
+        ]
         self.scp = scp = self.start_server(commands)
         self.move_to_state(self.assoc, scp)
 
         scp.step()
         scp.step()
         scp.shutdown()
 
         assert self.fsm._changes[:3] == [
             ("Sta1", "Evt1", "AE-1"),
             ("Sta4", "Evt2", "AE-2"),
-            ("Sta5", "Evt3", "AE-3"),
+            ("Sta5", "Evt3", "AE-3"),  # Sometimes not making it to Sta5...
         ]
         assert self.fsm._transitions[:3] == ["Sta4", "Sta5", "Sta6"]
         assert self.fsm._events[:3] == ["Evt1", "Evt2", "Evt3"]
 
     def test_evt04(self):
         """Test Sta5 + Evt4."""
         # Sta5 + Evt4 -> AE-4 -> Sta1
@@ -3853,21 +3857,23 @@
         # Evt3: Receive A-ASSOCIATE-AC PDU from <remote>
         # AA-8: Send A-ABORT PDU, issue A-P-ABORT primitive, start ARTIM
         commands = [
             ("recv", None),
             ("send", a_associate_ac),
             ("send", a_release_rq),
             ("send", a_associate_ac),
+            ("recv", None),
             ("exit", None),
         ]
         self.scp = scp = self.start_server(commands)
         self.move_to_state(self.assoc, scp)
 
         scp.step()
         scp.step()
+        scp.step()
         scp.shutdown()
 
         assert self.fsm._changes[:5] == [
             ("Sta1", "Evt1", "AE-1"),
             ("Sta4", "Evt2", "AE-2"),
             ("Sta5", "Evt3", "AE-3"),
             ("Sta6", "Evt12", "AR-2"),
@@ -3882,21 +3888,23 @@
         # Evt4: Receive A-ASSOCIATE-RJ PDU from <remote>
         # AA-8: Send A-ABORT PDU, issue A-P-ABORT primitive, start ARTIM
         commands = [
             ("recv", None),
             ("send", a_associate_ac),
             ("send", a_release_rq),
             ("send", a_associate_rj),
+            ("recv", None),
             ("exit", None),
         ]
         self.scp = scp = self.start_server(commands)
         self.move_to_state(self.assoc, scp)
 
         scp.step()
         scp.step()
+        scp.step()
         scp.shutdown()
 
         assert self.fsm._changes[:5] == [
             ("Sta1", "Evt1", "AE-1"),
             ("Sta4", "Evt2", "AE-2"),
             ("Sta5", "Evt3", "AE-3"),
             ("Sta6", "Evt12", "AR-2"),
@@ -3918,21 +3926,23 @@
         # Evt6: Receive A-ASSOCIATE-RQ PDU from <remote>
         # AA-8: Send A-ABORT PDU, issue A-P-ABORT primitive, start ARTIM
         commands = [
             ("recv", None),
             ("send", a_associate_ac),
             ("send", a_release_rq),
             ("send", a_associate_rq),
+            ("recv", None),
             ("exit", None),
         ]
         self.scp = scp = self.start_server(commands)
         self.move_to_state(self.assoc, scp)
 
         scp.step()
         scp.step()
+        scp.step()
         scp.shutdown()
 
         assert self.fsm._changes[:5] == [
             ("Sta1", "Evt1", "AE-1"),
             ("Sta4", "Evt2", "AE-2"),
             ("Sta5", "Evt3", "AE-3"),
             ("Sta6", "Evt12", "AR-2"),
@@ -4008,22 +4018,24 @@
         # Sta8 + Evt9 -> AR-7 -> Sta8
         # Evt9: Receive P-DATA primitive from <local user>
         # AR-7: Send P-DATA-TF PDU to <remote>
         commands = [
             ("recv", None),
             ("send", a_associate_ac),
             ("send", a_release_rq),
+            ("recv", None),
             ("exit", None),
         ]
         self.scp = scp = self.start_server(commands)
         self.move_to_state(self.assoc, scp)
 
         self.assoc.dul.send_pdu(self.get_pdata())
 
         scp.step()
+        scp.step()
         scp.shutdown()
 
         assert self.fsm._changes[:4] == [
             ("Sta1", "Evt1", "AE-1"),
             ("Sta4", "Evt2", "AE-2"),
             ("Sta5", "Evt3", "AE-3"),
             ("Sta6", "Evt12", "AR-2"),
@@ -4037,21 +4049,23 @@
         # Evt10: Receive P-DATA-TF PDU from <remote>
         # AA-8: Send A-ABORT PDU, issue A-P-ABORT primitive, start ARTIM
         commands = [
             ("recv", None),
             ("send", a_associate_ac),
             ("send", a_release_rq),
             ("send", p_data_tf),
+            ("recv", None),
             ("exit", None),
         ]
         self.scp = scp = self.start_server(commands)
         self.move_to_state(self.assoc, scp)
 
         scp.step()
         scp.step()
+        scp.step()
         scp.shutdown()
 
         assert self.fsm._changes[:5] == [
             ("Sta1", "Evt1", "AE-1"),
             ("Sta4", "Evt2", "AE-2"),
             ("Sta5", "Evt3", "AE-3"),
             ("Sta6", "Evt12", "AR-2"),
@@ -4097,21 +4111,23 @@
         # Evt12: Receive A-RELEASE-RQ PDU from <remote>
         # AA-8: Send A-ABORT PDU, issue A-P-ABORT primitive, start ARTIM
         commands = [
             ("recv", None),  # get a_assoc_rq
             ("send", a_associate_ac),
             ("send", a_release_rq),
             ("send", a_release_rq),
+            ("recv", None),
             ("exit", None),
         ]
         self.scp = scp = self.start_server(commands)
         self.move_to_state(self.assoc, scp)
 
         scp.step()
         scp.step()
+        scp.step()
         scp.shutdown()
 
         assert self.fsm._changes[:5] == [
             ("Sta1", "Evt1", "AE-1"),
             ("Sta4", "Evt2", "AE-2"),
             ("Sta5", "Evt3", "AE-3"),
             ("Sta6", "Evt12", "AR-2"),
@@ -4126,21 +4142,23 @@
         # Evt13: Receive A-RELEASE-RP PDU from <remote>
         # AA-8: Send A-ABORT PDU, issue A-P-ABORT primitive, start ARTIM
         commands = [
             ("recv", None),
             ("send", a_associate_ac),
             ("send", a_release_rq),
             ("send", a_release_rp),
+            ("recv", None),
             ("exit", None),
         ]
         self.scp = scp = self.start_server(commands)
         self.move_to_state(self.assoc, scp)
 
         scp.step()
         scp.step()
+        scp.step()
         scp.shutdown()
 
         assert self.fsm._changes[:5] == [
             ("Sta1", "Evt1", "AE-1"),
             ("Sta4", "Evt2", "AE-2"),
             ("Sta5", "Evt3", "AE-3"),
             ("Sta6", "Evt12", "AR-2"),
@@ -4154,22 +4172,24 @@
         # Sta8 + Evt14 -> AR-4 -> Sta13
         # Evt14: Receive A-RELEASE (rsp) primitive from <local user>
         # AR-4: Send A-RELEASE-RP PDU and start ARTIM
         commands = [
             ("recv", None),
             ("send", a_associate_ac),
             ("send", a_release_rq),
+            ("recv", None),
             ("exit", None),
         ]
         self.scp = scp = self.start_server(commands)
         self.move_to_state(self.assoc, scp)
 
         self.assoc.dul.send_pdu(self.get_release(True))
 
         scp.step()
+        scp.step()
         scp.shutdown()
 
         assert self.fsm._changes[:4] == [
             ("Sta1", "Evt1", "AE-1"),
             ("Sta4", "Evt2", "AE-2"),
             ("Sta5", "Evt3", "AE-3"),
             ("Sta6", "Evt12", "AR-2"),
@@ -4304,21 +4324,23 @@
         # Evt19: Received unrecognised or invalid PDU from <remote>
         # AA-8: Send A-ABORT PDU, issue A-P-ABORT primitive, start ARTIM
         commands = [
             ("recv", None),
             ("send", a_associate_ac),
             ("send", a_release_rq),
             ("send", b"\x08\x00\x00\x00\x00\x00"),
+            ("recv", None),
             ("exit", None),
         ]
         self.scp = scp = self.start_server(commands)
         self.move_to_state(self.assoc, scp)
 
         scp.step()
         scp.step()
+        scp.step()
         scp.shutdown()
 
         assert self.fsm._changes[:5] == [
             ("Sta1", "Evt1", "AE-1"),
             ("Sta4", "Evt2", "AE-2"),
             ("Sta5", "Evt3", "AE-3"),
             ("Sta6", "Evt12", "AR-2"),
@@ -8191,15 +8213,15 @@
             ("Sta13", "Evt17", "AR-5"),
         ] == fsm._changes[:30]
 
 
 class TestStateMachineFunctionalRequestor:
     """Functional tests for StateMachine as association requestor."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
         ae = AE()
         ae.add_requested_context(Verification)
         ae.acse_timeout = 5
         ae.dimse_timeout = 5
@@ -8226,15 +8248,15 @@
 
         self.assoc = assoc
         self.fsm = self.monkey_patch(assoc.dul.state_machine)
 
         self.orig_ar2 = FINITE_STATE.ACTIONS["AR-2"]
         self.orig_ar4 = FINITE_STATE.ACTIONS["AR-4"]
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
         FINITE_STATE.ACTIONS["AR-4"] = self.orig_ar4
         FINITE_STATE.ACTIONS["AR-2"] = self.orig_ar2
 
@@ -8576,14 +8598,15 @@
 
         assert self.fsm.current_state == "Sta1"
 
         scp.shutdown()
 
     def test_release_AR6(self):
         """Test receive P-DATA-TF while waiting for A-RELEASE-RP."""
+
         # Requestor sends A-RELEASE-RQ, acceptor sends P-DATA-TF then
         #   A-RELEASE-RP
         # Patch AR-4 to also send a P-DATA-TF
         def AR_4(dul):
             # Send C-ECHO-RQ
             dul.socket.send(p_data_tf)
 
@@ -8716,15 +8739,15 @@
 
         scp.shutdown()
 
 
 class TestStateMachineFunctionalAcceptor:
     """Functional tests for StateMachine as association acceptor."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
         ae = AE()
         ae.add_requested_context(Verification)
         ae.acse_timeout = 5
         ae.dimse_timeout = 5
@@ -8750,15 +8773,15 @@
         assoc.requestor.requested_contexts = [cx]
 
         self.assoc = assoc
         self.fsm = self.monkey_patch(assoc.dul.state_machine)
 
         self.orig_entry = FINITE_STATE.ACTIONS["AE-2"]
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
         FINITE_STATE.ACTIONS["AE-2"] = self.orig_entry
 
     def monkey_patch(self, fsm):
@@ -8834,18 +8857,18 @@
 
         scp.shutdown()
 
 
 class TestEventHandling:
     """Test the FSM event handlers."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
     def test_no_handlers(self):
         """Test with no handlers bound."""
         self.ae = ae = AE()
         ae.add_supported_context("1.2.840.10008.1.1")
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_logging.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_logging.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,19 +194,19 @@
 
     @pytest.mark.parametrize("handler", DOC_HANDLERS)
     def test_doc_handlers(self, handler):
         handler(None)
 
 
 class TestStandardDIMSE:
-    def setup(self):
+    def setup_method(self):
         """Setup each test."""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Cleanup after each test"""
         if self.ae:
             self.ae.shutdown()
 
     def test_send_n_delete_rsp(self):
         """Test the handler for N-DELETE rsp"""
         self.ae = ae = AE()
@@ -295,15 +295,15 @@
         assoc.release()
         scp.shutdown()
 
 
 class TestStandardLogging:
     """Tests for standard logging handlers."""
 
-    def setup(self):
+    def setup_method(self):
         """Setup each test."""
         self.ae = None
 
         # A-ASSOCIATE (request)
         primitive = A_ASSOCIATE()
         primitive.application_context_name = APPLICATION_CONTEXT_NAME
         # Calling AE Title is the source DICOM AE title
@@ -366,15 +366,15 @@
 
         item = ImplementationClassUIDNotification()
         item.implementation_class_uid = generate_uid(entropy_srcs=["lorem"])
         primitive.user_information.append(item)
 
         self.associate_ac = primitive
 
-    def teardown(self):
+    def teardown_method(self):
         """Cleanup after each test"""
         if self.ae:
             self.ae.shutdown()
 
     def add_impl_name(self, primitive, name=b"A               "):
         """Add an Implementation Version Name to the A-ASSOCIATE primitive."""
         assert len(name) == 16
@@ -1284,19 +1284,19 @@
             assoc.release()
             scp.shutdown()
 
 
 class TestDebuggingLogging:
     """Tests for debugging handlers."""
 
-    def setup(self):
+    def setup_method(self):
         """Setup each test."""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Cleanup after each test"""
         if self.ae:
             self.ae.shutdown()
 
     def test_debug_fsm(self, caplog):
         """Test debug_fsm."""
         self.ae = ae = AE()
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_pdu.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_pdu.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     a_associate_ac_no_ts,
     a_associate_rq_called,
     a_associate_rq_calling,
 )
 from pynetdicom.sop_class import Verification
 from pynetdicom.utils import pretty_bytes
 
-LOGGER = logging.getLogger("pynetdicom")
+LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.CRITICAL)
 
 
 class TestPDU:
     """Test the PDU equality/inequality operators."""
 
     def test_decode_raises(self):
@@ -730,14 +730,32 @@
         assert primitive.responding_presentation_address == (
             primitive.called_presentation_address
         )
         assert primitive.presentation_context_definition_list == []
         assert primitive.presentation_requirements == "Presentation Kernel"
         assert primitive.session_requirements == ""
 
+    def test_to_primitive_bad_reserved_aet(self):
+        """Test conversion with a non-conformant reserved ae title."""
+        pdu = A_ASSOCIATE_AC()
+        pdu.decode(a_associate_ac)
+        aec = (
+            b"\x4c\x57\x50\x41\x43\x53" b"\x00\x00\x00\x00\x00\x00\x0f\x00\x00\x00\x00"
+        )
+        pdu.reserved_aec = aec.decode("ascii")
+        pdu.reserved_aet = aec.decode("ascii")
+
+        primitive = pdu.to_primitive()
+        assert primitive.calling_ae_title == (
+            "LWPACS\x00\x00\x00\x00\x00\x00\x0f\x00\x00\x00\x00"
+        )
+        assert primitive.called_ae_title == (
+            "LWPACS\x00\x00\x00\x00\x00\x00\x0f\x00\x00\x00\x00"
+        )
+
     def test_from_primitive(self):
         """Check converting PDU to primitive"""
         orig = A_ASSOCIATE_AC()
         orig.decode(a_associate_ac)
 
         primitive = orig.to_primitive()
 
@@ -1489,19 +1507,19 @@
         pdu.source = None
         assert pdu.reason_str == "(no value available)"
 
 
 class TestEventHandlingAcceptor:
     """Test the transport events and handling as acceptor."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
         _config.LOG_HANDLER_LEVEL = "none"
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
         _config.LOG_HANDLER_LEVEL = "standard"
 
     def test_no_handlers(self):
         """Test with no transport event handlers bound."""
@@ -1821,19 +1839,19 @@
             assert msg in caplog.text
             assert "Exception description" in caplog.text
 
 
 class TestEventHandlingRequestor:
     """Test the transport events and handling as requestor."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
         _config.LOG_HANDLER_LEVEL = "none"
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
         _config.LOG_HANDLER_LEVEL = "standard"
 
     def test_no_handlers(self):
         """Test with no transport event handlers bound."""
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_pdu_items.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_pdu_items.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,18 +321,18 @@
         uid = UID("1.2.840.10008.1.10")
         assert len(uid) % 2 == 0
         out = item._wrap_encode_str(uid)
         assert out == b"1.2.840.10008.1.10"
 
 
 class TestApplicationContext:
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_init(self):
         """Test a new ApplicationContextItem"""
         item = ApplicationContextItem()
         assert item.item_type == 0x10
         assert item.item_length == 21
@@ -800,18 +800,18 @@
         item = item.transfer_syntax_sub_item[0]
         assert item.item_length == 0
         assert item._skip_validation is True
         assert item.transfer_syntax_name is None
 
 
 class TestAbstractSyntax:
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_init(self):
         """Test a new AbstractSyntaxSubItem."""
         item = AbstractSyntaxSubItem()
         assert item.item_type == 0x30
         assert item.item_length == 0
@@ -941,18 +941,18 @@
         assert item.abstract_syntax_name == "1.2.3"
         assert len(item.abstract_syntax_name) % 2 > 0
         assert len(item) == 9
         assert item.encode() == b"\x30\x00\x00\x05\x31\x2e\x32\x2e\x33"
 
 
 class TestTransferSyntax:
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_init(self):
         """Test a new AbstractSyntaxSubItem."""
         item = TransferSyntaxSubItem()
         assert item.item_type == 0x40
         assert item.item_length == 0
@@ -1390,18 +1390,18 @@
         params = orig_max_length.to_primitive()
         new_max_length = MaximumLengthSubItem()
         new_max_length.from_primitive(params)
         assert orig_max_length == new_max_length
 
 
 class TestUserInformation_ImplementationUID:
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_uid(self):
         """Test the UID conformance with ENFORCE_UID_CONFORMANCE."""
         item = ImplementationClassUIDSubItem()
         item.implementation_class_uid = ""
         assert item.implementation_class_uid == ""
@@ -1842,18 +1842,18 @@
                 break
 
         assert item.max_operations_invoked == 5
         assert item.max_operations_performed == 5
 
 
 class TestUserInformation_RoleSelection:
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_uid_conformance(self):
         """Test the UID conformance with ENFORCE_UID_CONFORMANCE."""
         _config.ENFORCE_UID_CONFORMANCE = False
 
         item = SCP_SCU_RoleSelectionSubItem()
@@ -2363,18 +2363,18 @@
         pdu = A_ASSOCIATE_AC()
         pdu.decode(a_associate_ac_user)
         item = pdu.user_information.user_identity
         assert item.response == b"Accepted"
 
 
 class TestUserInformation_ExtendedNegotiation:
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_uid_conformance(self):
         """Test the UID conformance with ENFORCE_UID_CONFORMANCE."""
         _config.ENFORCE_UID_CONFORMANCE = False
 
         item = SOPClassExtendedNegotiationSubItem()
@@ -2572,18 +2572,18 @@
         assert len(item.sop_class_uid) % 2 > 0
         assert len(item) == 12
         assert item.service_class_application_information == b"\xFF"
         assert item.encode() == (b"\x56\x00\x00\x08\x00\x05\x31\x2e\x32\x2e\x33\xFF")
 
 
 class TestUserInformation_CommonExtendedNegotiation:
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_uid_conformance(self):
         """Test the UID conformance with ENFORCE_UID_CONFORMANCE."""
         _config.ENFORCE_UID_CONFORMANCE = False
 
         item = SOPClassCommonExtendedNegotiationSubItem()
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_presentation.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_presentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,18 +66,18 @@
     """Good init values."""
     return request.param
 
 
 class TestPresentationContext:
     """Test the PresentationContext class"""
 
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_setter(self, good_init):
         """Test the presentation context class init"""
         (context_id, abs_syn, tran_syn) = good_init
         pc = PresentationContext()
         pc.context_id = context_id
@@ -293,14 +293,15 @@
         msg = "Invalid 'abstract_syntax' value '1.4.1.' - UID is non-conformant"
         with pytest.raises(ValueError, match=msg):
             pc.abstract_syntax = UID("1.4.1.")
         assert pc.abstract_syntax is None
 
         _config.ENFORCE_UID_CONFORMANCE = False
         pc.abstract_syntax = UID("1.4.1.")
+
         assert pc.abstract_syntax == UID("1.4.1.")
         assert isinstance(pc.abstract_syntax, UID)
 
         assert msg in caplog.text
 
     def test_transfer_syntax(self):
         """Test transfer syntax setter"""
@@ -331,14 +332,15 @@
 
     def test_transfer_syntax_nonconformant(self, caplog):
         """Test setting non-conformant transfer syntaxes"""
         caplog.set_level(logging.DEBUG, logger="pynetdicom.presentation")
         pc = PresentationContext()
         pc.context_id = 1
         pc.transfer_syntax = ["1.4.1.", "1.2.840.10008.1.2"]
+
         assert pc.transfer_syntax == ["1.4.1.", "1.2.840.10008.1.2"]
         assert "A non-conformant UID has been added to 'transfer_syntax'" in caplog.text
 
     def test_status(self):
         """Test presentation context status"""
         pc = PresentationContext()
         pc.context_id = 1
@@ -370,28 +372,28 @@
         assert out.transfer_syntax == "1.2.840.10008.1.2"
 
     def test_as_scp(self):
         """Test the Presentation.as_scp property."""
         context = build_context("1.2.3")
         assert context.as_scp is None
 
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             context.as_scp = True
 
         context._as_scp = True
         assert context.as_scp
         context._as_scp = False
         assert not context.as_scp
 
     def test_as_scu(self):
         """Test the Presentation.as_scu property."""
         context = build_context("1.2.3")
         assert context.as_scu is None
 
-        with pytest.raises(AttributeError, match=r"can't set attribute"):
+        with pytest.raises(AttributeError, match=r"can't set attribute|has no setter"):
             context.as_scu = True
 
         context._as_scu = True
         assert context.as_scu
         context._as_scu = False
         assert not context.as_scu
 
@@ -429,15 +431,15 @@
         cx = build_context("1.2.840.10008.1.1")
         assert "Verification SOP Class" == repr(cx)
 
 
 class TestNegotiateAsAcceptor:
     """Tests negotiation_as_acceptor."""
 
-    def setup(self):
+    def setup_method(self):
         self.test_func = negotiate_as_acceptor
 
     def test_no_req_no_acc(self):
         """Test negotiation with no contexts."""
         result = self.test_func([], [], [])
         assert result == ([], [])
 
@@ -648,19 +650,25 @@
         assert roles == []
         context = result[0]
         assert context.context_id == 1
         assert context.abstract_syntax == "1.2.3.4"
         assert context.result == 0x00
         assert context.transfer_syntax == ["1.2.840.10008.1.2.1"]
 
-    @pytest.mark.skipif(PYDICOM_VERSION < ["2", "2"], reason="Old data dict")
     def test_typical(self):
         """Test a typical set of presentation context negotiations."""
         req_contexts = []
         for ii, context in enumerate(StoragePresentationContexts):
+            # Old pydicom UID dict
+            if context.abstract_syntax in (
+                "1.2.840.10008.5.1.4.1.1.6.3",
+                "1.2.840.10008.5.1.4.1.1.9.1.4",
+            ):
+                continue
+
             pc = PresentationContext()
             pc.context_id = ii * 2 + 1
             pc.abstract_syntax = context.abstract_syntax
             pc.transfer_syntax = [
                 "1.2.840.10008.1.2",
                 "1.2.840.10008.1.2.1",
                 "1.2.840.10008.1.2.2",
@@ -1321,15 +1329,15 @@
 
         scp.shutdown()
 
 
 class TestNegotiateAsRequestor:
     """Tests negotiate_as_requestor."""
 
-    def setup(self):
+    def setup_method(self):
         self.test_acc = negotiate_as_acceptor
         self.test_func = negotiate_as_requestor
 
     def test_no_req_no_acc_raise(self):
         """Test negotiation with no contexts."""
         with pytest.raises(ValueError):
             result = self.test_func([], [])
@@ -1590,19 +1598,25 @@
         assert len(result) == 1
         context = result[0]
         assert context.context_id == 1
         assert context.abstract_syntax == "1.2.3.4"
         assert context.result == 0x00
         assert context.transfer_syntax == ["1.2.840.10008.1.2.1"]
 
-    @pytest.mark.skipif(PYDICOM_VERSION < ["2", "2"], reason="Old data dict")
     def test_typical(self):
         """Test a typical set of presentation context negotiations."""
         req_contexts = []
         for ii, context in enumerate(StoragePresentationContexts):
+            # Old pydicom UID dict
+            if context.abstract_syntax in (
+                "1.2.840.10008.5.1.4.1.1.6.3",
+                "1.2.840.10008.5.1.4.1.1.9.1.4",
+            ):
+                continue
+
             pc = PresentationContext()
             pc.context_id = ii * 2 + 1
             pc.abstract_syntax = context.abstract_syntax
             pc.transfer_syntax = [
                 "1.2.840.10008.1.2",
                 "1.2.840.10008.1.2.1",
                 "1.2.840.10008.1.2.2",
@@ -1677,15 +1691,15 @@
         assert context.abstract_syntax == "1.2.840.10008.5.1.4.1.1.2.1"
         assert context.result == 0x01
 
 
 class TestNegotiateUnrestricted:
     """Tests for presentation.negotiate_unrestricted()"""
 
-    def setup(self):
+    def setup_method(self):
         self.test_func = negotiate_unrestricted
 
     def test_no_contexts(self):
         """Test negotiation with no contexts."""
         assert self.test_func([], [], []) == ([], [])
 
     def test_non_storage_no_acc(self):
@@ -2031,28 +2045,29 @@
             assert context.context_id is None
 
         assert contexts[0].abstract_syntax == "1.2.840.10008.1.3.10"
 
     def test_non_patient(self):
         """Tests with non patient object presentation contexts"""
         contexts = NonPatientObjectPresentationContexts
-        assert len(contexts) == 8
+        assert len(contexts) == 9
 
         for context in contexts:
             assert context.transfer_syntax == DEFAULT_TRANSFER_SYNTAXES
             assert context.context_id is None
 
         assert contexts[0].abstract_syntax == "1.2.840.10008.5.1.4.1.1.200.1"
         assert contexts[1].abstract_syntax == "1.2.840.10008.5.1.4.1.1.200.3"
         assert contexts[2].abstract_syntax == "1.2.840.10008.5.1.4.1.1.200.7"
-        assert contexts[3].abstract_syntax == "1.2.840.10008.5.1.4.38.1"
-        assert contexts[4].abstract_syntax == "1.2.840.10008.5.1.4.39.1"
-        assert contexts[5].abstract_syntax == "1.2.840.10008.5.1.4.43.1"
-        assert contexts[6].abstract_syntax == "1.2.840.10008.5.1.4.44.1"
-        assert contexts[7].abstract_syntax == "1.2.840.10008.5.1.4.45.1"
+        assert contexts[3].abstract_syntax == "1.2.840.10008.5.1.4.1.1.201.1"
+        assert contexts[4].abstract_syntax == "1.2.840.10008.5.1.4.38.1"
+        assert contexts[5].abstract_syntax == "1.2.840.10008.5.1.4.39.1"
+        assert contexts[6].abstract_syntax == "1.2.840.10008.5.1.4.43.1"
+        assert contexts[7].abstract_syntax == "1.2.840.10008.5.1.4.44.1"
+        assert contexts[8].abstract_syntax == "1.2.840.10008.5.1.4.45.1"
 
     def test_print_management(self):
         """Tests with print management presentation contexts"""
         contexts = PrintManagementPresentationContexts
         assert len(contexts) == 11
 
         for context in contexts:
@@ -2096,22 +2111,22 @@
         assert contexts[0].abstract_syntax == "1.2.840.10008.5.1.4.1.1.200.4"
         assert contexts[1].abstract_syntax == "1.2.840.10008.5.1.4.1.1.200.5"
         assert contexts[2].abstract_syntax == "1.2.840.10008.5.1.4.1.1.200.6"
 
     def test_qr(self):
         """Test the query/retrieve service presentation contexts."""
         contexts = QueryRetrievePresentationContexts
-        assert len(contexts) == 12
+        assert len(contexts) == 13
 
         for context in contexts:
             assert context.transfer_syntax == DEFAULT_TRANSFER_SYNTAXES
             assert context.context_id is None
 
-        assert contexts[0].abstract_syntax == "1.2.840.10008.5.1.4.1.2.1.1"
-        assert contexts[4].abstract_syntax == "1.2.840.10008.5.1.4.1.2.2.2"
+        assert contexts[0].abstract_syntax == "1.2.840.10008.5.1.4.1.1.201.6"
+        assert contexts[4].abstract_syntax == "1.2.840.10008.5.1.4.1.2.2.1"
         assert contexts[-1].abstract_syntax == "1.2.840.10008.5.1.4.1.2.5.3"
 
     def test_relevant_patient(self):
         """Tests with relevant patient info presentation contexts"""
         contexts = RelevantPatientInformationPresentationContexts
         assert len(contexts) == 3
 
@@ -2141,16 +2156,16 @@
         assert len(contexts) == 128
 
         for context in contexts:
             assert context.transfer_syntax == DEFAULT_TRANSFER_SYNTAXES
             assert context.context_id is None
 
         assert contexts[0].abstract_syntax == "1.2.840.10008.5.1.4.1.1.1"
-        assert contexts[80].abstract_syntax == "1.2.840.10008.5.1.4.1.1.66.5"
-        assert contexts[-1].abstract_syntax == "1.2.840.10008.5.1.4.1.1.88.65"
+        assert contexts[80].abstract_syntax == "1.2.840.10008.5.1.4.1.1.77.1.6"
+        assert contexts[-1].abstract_syntax == "1.2.840.10008.5.1.4.34.7"
 
     def test_storage_commitement(self):
         """Tests with storage commitment presentation contexts"""
         contexts = StorageCommitmentPresentationContexts
         assert len(contexts) == 1
 
         for context in contexts:
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_primitives.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_primitives.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from pynetdicom.utils import pretty_bytes
 
 
 if hasattr(PYD_CONFIG, "settings"):
     PYD_CONFIG.settings.reading_validation_mode = 0
 
 
-LOGGER = logging.getLogger("pynetdicom")
+LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.CRITICAL)
 
 
 def print_nice_bytes(bytestream):
     """Nice output for bytestream."""
     str_list = pretty_bytes(
         bytestream, prefix="b'\\x", delimiter="\\x", items_per_line=10
@@ -86,18 +86,18 @@
     def test_string(self):
         """Check the string output."""
         primitive = MaximumLengthNotification()
         assert "16382 bytes" in primitive.__str__()
 
 
 class TestPrimitive_ImplementationClassUIDNotification:
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_uid_conformance_false(self):
         """Test UID conformance with ENFORCE_UID_CONFORMANCE = False"""
         _config.ENFORCE_UID_CONFORMANCE = False
         primitive = ImplementationClassUIDNotification()
 
@@ -285,18 +285,18 @@
         primitive.maximum_number_operations_invoked = 10
         primitive.maximum_number_operations_performed = 0
         assert "invoked: 10" in primitive.__str__()
         assert "performed: 0" in primitive.__str__()
 
 
 class TestPrimitive_SCP_SCU_RoleSelectionNegotiation:
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_uid_conformance_false(self):
         """Test UID conformance with ENFORCE_UID_CONFORMANCE = False"""
         _config.ENFORCE_UID_CONFORMANCE = False
         primitive = SCP_SCU_RoleSelectionNegotiation()
 
@@ -404,18 +404,18 @@
         primitive.scp_role = False
         primitive.scu_role = False
         with pytest.raises(ValueError):
             primitive.from_primitive()
 
 
 class TestPrimitive_SOPClassExtendedNegotiation:
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_uid_conformance_false(self):
         """Test UID conformance with ENFORCE_UID_CONFORMANCE = False"""
         _config.ENFORCE_UID_CONFORMANCE = False
         primitive = SOPClassExtendedNegotiation()
 
@@ -495,18 +495,18 @@
             b"\x56\x00\x00\x21\x00\x19\x31\x2e\x32\x2e\x38\x34\x30\x2e\x31\x30"
             b"\x30\x30\x38\x2e\x35\x2e\x31\x2e\x34\x2e\x31\x2e\x31\x2e\x32"
             b"\x02\x00\x03\x00\x01\x00"
         )
 
 
 class TestPrimitive_SOPClassCommonExtendedNegotiation:
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_uid_conformance_false(self):
         """Test UID conformance with ENFORCE_UID_CONFORMANCE = False"""
         _config.ENFORCE_UID_CONFORMANCE = False
         primitive = SOPClassCommonExtendedNegotiation()
 
@@ -728,18 +728,18 @@
         primitive = UserIdentityNegotiation()
         primitive.server_response = b"Test"
         item = primitive.from_primitive()
         assert item.encode() == b"\x59\x00\x00\x06\x00\x04\x54\x65\x73\x74"
 
 
 class TestPrimitive_A_ASSOCIATE:
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     def test_uid_conformance_false(self):
         """Test UID conformance with ENFORCE_UID_CONFORMANCE = False"""
         _config.ENFORCE_UID_CONFORMANCE = False
         primitive = A_ASSOCIATE()
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_service_class.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_service_class.py`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_service_n.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_service_n.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     ModalityPerformedProcedureStepRetrieve,  # N-GET
     ModalityPerformedProcedureStepNotification,  # N-EVENT-REPORT
     # Print Management - N-ACTION, N-CREATE, N-DELETE, N-SET
     BasicFilmSession,
     PrintJob,  # N-EVENT-REPORT, N-GET
     # Storage Commitment - N-ACTION, N-EVENT-REPORT
     StorageCommitmentPushModel,
+    # Storage Management - N-ACTION, N-EVENT-REPORT
+    InventoryCreation,
     # Application Event Logging - N-ACTION
     ProceduralEventLogging,
     # Instance Availability - N-CREATE
     InstanceAvailabilityNotification,
     # Media Creation - N-ACTION, N-CREATE, N-GET
     MediaCreationManagement,
     # Unified Procedure Step - N-ACTION, N-CREATE, N-GET
@@ -58,14 +60,16 @@
     (BasicFilmSession, "N-CREATE", 0xB600, 0xC616),
     (BasicFilmSession, "N-DELETE", None, None),
     (BasicFilmSession, "N-SET", 0xB600, 0xC616),
     (PrintJob, "N-EVENT-REPORT", None, None),
     (PrintJob, "N-GET", None, None),
     (StorageCommitmentPushModel, "N-ACTION", None, None),
     (StorageCommitmentPushModel, "N-EVENT-REPORT", None, None),
+    (InventoryCreation, "N-ACTION", 0xB010, None),
+    (InventoryCreation, "N-EVENT-REPORT", None, None),
     (ProceduralEventLogging, "N-ACTION", 0xB101, 0xC101),
     (InstanceAvailabilityNotification, "N-CREATE", None, None),
     (MediaCreationManagement, "N-ACTION", None, 0xC201),
     (MediaCreationManagement, "N-CREATE", None, 0xA510),
     (MediaCreationManagement, "N-GET", 0x0001, None),
     (UnifiedProcedureStepPush, "N-ACTION", 0xB301, 0xC300),
     (UnifiedProcedureStepPush, "N-CREATE", 0xB300, 0xC309),
@@ -81,27 +85,27 @@
     (RTConventionalMachineVerification, "N-SET", None, 0xC224),
 ]
 
 
 class TestNServiceClass:
     """Generic tests for the DIMSE-N Service Classes"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
         ds = Dataset()
         ds.PatientName = "Test"
         ds.SOPClassUID = DisplaySystem
         ds.SOPInstanceUID = "1.2.3.4"
         self.ds = ds
 
         self.event = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def abort_dual(self, status, ds):
         """Return a callable function that aborts then returns two values.
 
@@ -1204,23 +1208,23 @@
         assert assoc.is_aborted
         scp.shutdown()
 
 
 class TestUPSFindServiceClass:
     """Test the Unified Proecedure Step (Find) Service Class"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.query = Dataset()
         self.query.QueryRetrieveLevel = "PATIENT"
         self.query.PatientName = "*"
 
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_bad_req_identifier(self):
         """Test SCP handles a bad request identifier"""
 
@@ -2129,19 +2133,19 @@
         assert assoc.is_aborted
         scp.shutdown()
 
 
 class TestNEventReport:
     """Functional tests for N-EVENT-REPORT services."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_same_assoc(self):
         """Test SCP sending over the same association."""
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_service_non_patient.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_service_non_patient.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,25 +25,26 @@
 
 class TestNonPatientObjectStorageServiceClass:
     """Test the NonPatientObjectStorageServiceClass.
 
     Subclass of StorageServiceClass with its own set of statuses.
     """
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_scp_failed_ds_decode(self):
         """Test failure to decode the dataset"""
+
         # Hard to test directly as decode errors won't show up until the
         #   dataset is actually used
         def handle(event):
             try:
                 for elem in event.dataset.iterall():
                     pass
             except:
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_service_qr.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_service_qr.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,28 +22,33 @@
 from pynetdicom import (
     AE,
     build_context,
     StoragePresentationContexts,
     evt,
     build_role,
     debug_logger,
+    sop_class,
+    register_uid,
 )
 from pynetdicom.dimse_primitives import C_FIND, C_GET, C_MOVE, C_STORE
 from pynetdicom.presentation import PresentationContext
 from pynetdicom.service_class import (
     QueryRetrieveServiceClass,
     BasicWorklistManagementServiceClass,
 )
 from pynetdicom.sop_class import (
     CTImageStorage,
     ModalityWorklistInformationFind,
     PatientRootQueryRetrieveInformationModelFind,
     PatientRootQueryRetrieveInformationModelGet,
     PatientRootQueryRetrieveInformationModelMove,
     CompositeInstanceRetrieveWithoutBulkDataGet,
+    RepositoryQuery,
+    _QR_CLASSES,
+    _BASIC_WORKLIST_CLASSES,
 )
 
 
 # debug_logger()
 
 
 TEST_DS_DIR = os.path.join(os.path.dirname(__file__), "dicom_files")
@@ -56,26 +61,40 @@
     context = PresentationContext()
     context.abstract_syntax = "1.2.3.4"
     context.add_transfer_syntax("1.2")
     with pytest.raises(ValueError):
         service.SCP(None, context)
 
 
+@pytest.fixture()
+def register_new_uid_find():
+    register_uid(
+        "1.2.3.4",
+        "NewFind",
+        QueryRetrieveServiceClass,
+        "C-FIND",
+    )
+    yield
+    del _QR_CLASSES["NewFind"]
+    delattr(sop_class, "NewFind")
+    QueryRetrieveServiceClass._SUPPORTED_UIDS["C-FIND"].remove("1.2.3.4")
+
+
 class TestQRFindServiceClass:
     """Test the QueryRetrieveFindServiceClass"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.query = Dataset()
         self.query.QueryRetrieveLevel = "PATIENT"
         self.query.PatientName = "*"
 
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_bad_req_identifier(self):
         """Test SCP handles a bad request identifier"""
 
@@ -1077,14 +1096,15 @@
         assoc.release()
         time.sleep(0.1)
         assert assoc.is_released
         scp.shutdown()
 
     def test_success_no_identifier(self):
         """Test success response has no identifier dataset"""
+
         # Regression test for #571
         def handle(event):
             status = Dataset()
             status.Status = 0xFF00
             yield status, self.query
 
         handlers = [(evt.EVT_C_FIND, handle)]
@@ -1170,17 +1190,102 @@
         assert identifier is None
         with pytest.raises(StopIteration):
             next(result)
 
         assert assoc.is_aborted
         scp.shutdown()
 
+    def test_register(self, register_new_uid_find):
+        """Test registering a new UID"""
+        from pynetdicom.sop_class import NewFind
+
+        def handle(event):
+            yield 0xFF01, self.query
+            yield 0x0000, None
+            yield 0xA700, None
+
+        handlers = [(evt.EVT_C_FIND, handle)]
+
+        self.ae = ae = AE()
+        ae.add_supported_context(NewFind)
+        ae.add_requested_context(NewFind, ExplicitVRLittleEndian)
+        scp = ae.start_server(("localhost", 11112), block=False, evt_handlers=handlers)
+
+        ae.acse_timeout = 5
+        ae.dimse_timeout = 5
+        assoc = ae.associate("localhost", 11112)
+        assert assoc.is_established
+        result = assoc.send_c_find(self.query, NewFind)
+        status, identifier = next(result)
+        assert status.Status == 0xFF01
+        assert identifier == self.query
+        status, identifier = next(result)
+        assert status.Status == 0x0000
+        assert identifier is None
+        with pytest.raises(StopIteration):
+            next(result)
+
+        assoc.release()
+        assert assoc.is_released
+        scp.shutdown()
+
+    def test_repository_query(self):
+        """Test handler yielding pending then success status"""
+
+        def handle(event):
+            yield 0xFF01, self.query
+            yield 0xB001, None
+            yield 0x0000, None
+
+        handlers = [(evt.EVT_C_FIND, handle)]
+
+        self.ae = ae = AE()
+        ae.add_supported_context(RepositoryQuery)
+        ae.add_requested_context(RepositoryQuery, ExplicitVRLittleEndian)
+        scp = ae.start_server(("localhost", 11112), block=False, evt_handlers=handlers)
+
+        ae.acse_timeout = 5
+        ae.dimse_timeout = 5
+        assoc = ae.associate("localhost", 11112)
+        assert assoc.is_established
+        result = assoc.send_c_find(self.query, RepositoryQuery)
+
+        status, identifier = next(result)
+        assert status.Status == 0xFF01
+        assert identifier == self.query
+        status, identifier = next(result)
+        assert status.Status == 0xB001
+        assert identifier == None
+        status, identifier = next(result)
+        assert status.Status == 0x0000
+        assert identifier is None
+        with pytest.raises(StopIteration):
+            next(result)
+
+        assoc.release()
+        assert assoc.is_released
+        scp.shutdown()
+
+
+@pytest.fixture()
+def register_new_uid_get():
+    register_uid(
+        "1.2.3.4",
+        "NewGet",
+        QueryRetrieveServiceClass,
+        "C-GET",
+    )
+    yield
+    del _QR_CLASSES["NewGet"]
+    delattr(sop_class, "NewGet")
+    QueryRetrieveServiceClass._SUPPORTED_UIDS["C-GET"].remove("1.2.3.4")
+
 
 class TestQRGetServiceClass:
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.query = Dataset()
         self.query.PatientName = "*"
         self.query.QueryRetrieveLevel = "PATIENT"
 
         self.ds = Dataset()
         self.ds.file_meta = FileMetaDataset()
@@ -1190,15 +1295,15 @@
         self.ds.PatientName = "Test"
 
         self.fail = Dataset()
         self.fail.FailedSOPInstanceUIDList = ["1.2.3"]
 
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_bad_req_identifier(self):
         """Test SCP handles a bad request identifier"""
 
@@ -2514,15 +2619,14 @@
             attrs["request"] = event.request
             attrs["identifier"] = event.identifier
             attrs["assoc"] = event.assoc
             yield 1
             yield 0xFF00, self.ds
 
         def handle_store(event):
-
             return 0x0000
 
         handlers = [(evt.EVT_C_GET, handle)]
 
         self.ae = ae = AE()
         ae.add_supported_context(PatientRootQueryRetrieveInformationModelGet)
         ae.add_supported_context(CTImageStorage, scu_role=False, scp_role=True)
@@ -3392,14 +3496,15 @@
 
         time.sleep(0.1)
         assert assoc.is_aborted
         scp.shutdown()
 
     def test_success_no_identifier(self):
         """Test pending and success responses have no identifier dataset"""
+
         # Regression test for #571
         def handle(event):
             yield 1
             status = Dataset()
             status.Status = 0xFF00
             yield status, self.ds
 
@@ -3496,17 +3601,74 @@
         assert identifier.FailedSOPInstanceUIDList == "1.1.1"
         pytest.raises(StopIteration, next, result)
 
         assoc.release()
         assert assoc.is_released
         scp.shutdown()
 
+    def test_register(self, register_new_uid_get):
+        """Test registering a new UID"""
+        from pynetdicom.sop_class import NewGet
+
+        def handle(event):
+            yield 1
+            yield 0xFF00, self.ds
+
+        def handle_store(event):
+            return 0x0000
+
+        handlers = [(evt.EVT_C_GET, handle)]
+
+        self.ae = ae = AE()
+        ae.add_supported_context(NewGet)
+        ae.add_supported_context(CTImageStorage, scu_role=False, scp_role=True)
+        ae.add_requested_context(NewGet)
+        ae.add_requested_context(CTImageStorage)
+        scp = ae.start_server(("localhost", 11112), block=False, evt_handlers=handlers)
+
+        role = build_role(CTImageStorage, scp_role=True)
+        handlers = [(evt.EVT_C_STORE, handle_store)]
+
+        ae.acse_timeout = 5
+        ae.dimse_timeout = 5
+        assoc = ae.associate("localhost", 11112, ext_neg=[role], evt_handlers=handlers)
+        assert assoc.is_established
+        result = assoc.send_c_get(self.query, NewGet)
+        status, identifier = next(result)
+        assert status.Status == 0xFF00
+        assert identifier is None
+        status, identifier = next(result)
+        assert status.Status == 0x0000
+        assert status.NumberOfFailedSuboperations == 0
+        assert status.NumberOfWarningSuboperations == 0
+        assert status.NumberOfCompletedSuboperations == 1
+        assert identifier is None
+        pytest.raises(StopIteration, next, result)
+
+        assoc.release()
+        assert assoc.is_released
+        scp.shutdown()
+
+
+@pytest.fixture()
+def register_new_uid_move():
+    register_uid(
+        "1.2.3.4",
+        "NewMove",
+        QueryRetrieveServiceClass,
+        "C-MOVE",
+    )
+    yield
+    del _QR_CLASSES["NewMove"]
+    delattr(sop_class, "NewMove")
+    QueryRetrieveServiceClass._SUPPORTED_UIDS["C-MOVE"].remove("1.2.3.4")
+
 
 class TestQRMoveServiceClass:
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.query = Dataset()
         self.query.PatientName = "*"
         self.query.QueryRetrieveLevel = "PATIENT"
 
         self.ds = Dataset()
         self.ds.file_meta = FileMetaDataset()
@@ -3518,15 +3680,15 @@
         self.fail = Dataset()
         self.fail.FailedSOPInstanceUIDList = ["1.2.3"]
 
         self.destination = ("localhost", 11112)
 
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_bad_req_identifier(self):
         """Test SCP handles a bad request identifier"""
 
@@ -3576,14 +3738,15 @@
 
         assoc.release()
         assert assoc.is_released
         scp.shutdown()
 
     def test_move_handler_bad_yield_destination(self):
         """Test correct status returned if handler doesn't yield dest."""
+
         # Testing what happens if the handler doesn't yield
         def handle(event):
             return
 
         handlers = [(evt.EVT_C_MOVE, handle)]
 
         self.ae = ae = AE()
@@ -5960,19 +6123,59 @@
         assert status.NumberOfCompletedSuboperations == 0
         assert identifier.FailedSOPInstanceUIDList == "1.1.1"
         pytest.raises(StopIteration, next, result)
 
         assoc.release()
         scp.shutdown()
 
+    def test_register(self, register_new_uid_move):
+        """Test registering a new UID"""
+        from pynetdicom.sop_class import NewMove
+
+        def handle(event):
+            yield self.destination
+            yield 1
+            yield 0xFF00, self.ds
+
+        def handle_store(event):
+            return 0x0000
+
+        handlers = [(evt.EVT_C_MOVE, handle), (evt.EVT_C_STORE, handle_store)]
+
+        self.ae = ae = AE()
+        ae.add_supported_context(NewMove)
+        ae.add_supported_context(CTImageStorage, scu_role=False, scp_role=True)
+        ae.add_requested_context(NewMove)
+        ae.add_requested_context(CTImageStorage)
+        scp = ae.start_server(("localhost", 11112), block=False, evt_handlers=handlers)
+
+        ae.acse_timeout = 5
+        ae.dimse_timeout = 5
+        assoc = ae.associate("localhost", 11112)
+        assert assoc.is_established
+        result = assoc.send_c_move(self.query, "TESTMOVE", NewMove)
+        status, identifier = next(result)
+        assert status.Status == 0xFF00
+        assert identifier is None
+        status, identifier = next(result)
+        assert status.Status == 0x0000
+        assert status.NumberOfFailedSuboperations == 0
+        assert status.NumberOfWarningSuboperations == 0
+        assert status.NumberOfCompletedSuboperations == 1
+        assert identifier is None
+        pytest.raises(StopIteration, next, result)
+
+        assoc.release()
+        scp.shutdown()
+
 
 class TestQRCompositeInstanceWithoutBulk:
     """Tests for QR + Composite Instance Without Bulk Data"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.query = Dataset()
         self.query.PatientName = "*"
         self.query.QueryRetrieveLevel = "PATIENT"
 
         self.ds = Dataset()
         self.ds.file_meta = FileMetaDataset()
@@ -5984,15 +6187,15 @@
         self.fail = Dataset()
         self.fail.FailedSOPInstanceUIDList = ["1.2.3"]
 
         self.destination = ("localhost", 11112)
 
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_pixel_data(self):
         """Test pixel data is removed"""
         assert "PixelData" in DATASET
@@ -6168,58 +6371,73 @@
         assert has_repeaters[1] is False
         assert has_repeaters[2] is False
 
         assoc.release()
         scp.shutdown()
 
 
+@pytest.fixture()
+def register_new_uid_bwm():
+    register_uid(
+        "1.2.3.4",
+        "NewFind",
+        BasicWorklistManagementServiceClass,
+        "C-FIND",
+    )
+    yield
+    del _BASIC_WORKLIST_CLASSES["NewFind"]
+    delattr(sop_class, "NewFind")
+    BasicWorklistManagementServiceClass._SUPPORTED_UIDS["C-FIND"].remove("1.2.3.4")
+
+
 class TestBasicWorklistServiceClass:
     """Tests for BasicWorklistManagementServiceClass."""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.query = Dataset()
         self.query.QueryRetrieveLevel = "PATIENT"
         self.query.PatientName = "*"
 
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_bad_abstract_syntax_raises(self):
         """Test calling the BWM SCP with an unknown UID raises exception."""
         msg = r"The supplied abstract syntax is not valid"
         with pytest.raises(ValueError, match=msg):
             bwm = BasicWorklistManagementServiceClass(None)
             context = build_context("1.2.3.4")
             bwm.SCP(None, context)
 
-    def test_pending_success(self):
-        """Test handler yielding pending then success status"""
+    def test_register(self, register_new_uid_bwm):
+        """Test registering a new UID"""
+        from pynetdicom.sop_class import NewFind
 
         def handle(event):
             yield 0xFF01, self.query
             yield 0x0000, None
             yield 0xA700, None
 
         handlers = [(evt.EVT_C_FIND, handle)]
 
         self.ae = ae = AE()
-        ae.add_supported_context(ModalityWorklistInformationFind)
-        ae.add_requested_context(ModalityWorklistInformationFind)
+        ae.add_supported_context(NewFind)
+        ae.add_requested_context(NewFind)
         scp = ae.start_server(("localhost", 11112), block=False, evt_handlers=handlers)
 
         ae.acse_timeout = 5
         ae.dimse_timeout = 5
         assoc = ae.associate("localhost", 11112)
         assert assoc.is_established
-        result = assoc.send_c_find(self.query, ModalityWorklistInformationFind)
+        result = assoc.send_c_find(self.query, NewFind)
         status, identifier = next(result)
         assert status.Status == 0xFF01
         assert identifier == self.query
         status, identifier = next(result)
         assert status.Status == 0x0000
         assert identifier is None
         with pytest.raises(StopIteration):
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_service_relevant_patient.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_service_relevant_patient.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,23 +21,23 @@
 
 # debug_logger()
 
 
 class TestRelevantPatientServiceClass:
     """Test the RelevantPatientInformationQueryServiceClass"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.query = Dataset()
         self.query.QueryRetrieveLevel = "PATIENT"
         self.query.PatientName = "*"
 
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_bad_req_identifier(self):
         """Test SCP handles a bad request identifier"""
 
@@ -288,14 +288,15 @@
         pytest.raises(StopIteration, next, result)
 
         assoc.release()
         scp.shutdown()
 
     def test_pending_cancel(self):
         """Test handler yielding pending then cancel status"""
+
         # Note: success should be second, cancel should get ignored
         def handle(event):
             yield 0xFF00, self.query
             yield 0xFE00, None
 
         handlers = [(evt.EVT_C_FIND, handle)]
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_service_storage.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_service_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """Tests for the StorageServiceClass."""
 
+from copy import deepcopy
 from io import BytesIO
 import os
 from pathlib import Path
 import time
 
 import pytest
 
 from pydicom import dcmread
 from pydicom.dataset import Dataset, FileMetaDataset
 from pydicom.uid import ExplicitVRLittleEndian, ImplicitVRLittleEndian
 
-from pynetdicom import AE, _config, evt, debug_logger
+from pynetdicom import AE, _config, evt, debug_logger, register_uid, sop_class
 from pynetdicom.dimse_primitives import C_STORE
 from pynetdicom.pdu_primitives import SOPClassExtendedNegotiation
 from pynetdicom.sop_class import (
     Verification,
     CTImageStorage,
+    _STORAGE_CLASSES,
 )
+from pynetdicom.service_class import StorageServiceClass
 
 try:
     from pynetdicom.status import Status
 
     HAS_STATUS = True
 except ImportError:
     HAS_STATUS = False
@@ -37,29 +40,41 @@
 @pytest.fixture()
 def enable_unrestricted():
     _config.UNRESTRICTED_STORAGE_SERVICE = True
     yield
     _config.UNRESTRICTED_STORAGE_SERVICE = False
 
 
+@pytest.fixture()
+def register_new_uid():
+    register_uid(
+        "1.2.3.4",
+        "NewStorage",
+        StorageServiceClass,
+    )
+    yield
+    del _STORAGE_CLASSES["NewStorage"]
+    delattr(sop_class, "NewStorage")
+
+
 class TestStorageServiceClass:
     """Test the StorageServiceClass"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
         self.ds = Dataset()
         self.ds.file_meta = FileMetaDataset()
         self.ds.file_meta.TransferSyntaxUID = ImplicitVRLittleEndian
         self.ds.SOPClassUID = CTImageStorage
         self.ds.SOPInstanceUID = "1.1.1"
         self.ds.PatientName = "Test"
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
         _config.STORE_RECV_CHUNKED_DATASET = False
 
     @pytest.mark.skipif(not HAS_STATUS, reason="No Status class available")
@@ -795,7 +810,39 @@
 
         assoc.release()
         assert assoc.is_released
 
         assert recv == ["CompressedSamples^CT1", "Private", "Unknown^Public"]
 
         scp.shutdown()
+
+    def test_register(self, register_new_uid):
+        """Test registering a new UID."""
+        from pynetdicom.sop_class import NewStorage
+
+        attrs = {}
+
+        def handle(event):
+            attrs["uid"] = event.dataset.SOPClassUID
+            return 0x0000
+
+        ds = deepcopy(DATASET)
+        ds.SOPClassUID = NewStorage
+
+        handlers = [(evt.EVT_C_STORE, handle)]
+
+        self.ae = ae = AE()
+        ae.add_supported_context(NewStorage)
+        ae.add_requested_context(NewStorage)
+        scp = ae.start_server(("localhost", 11112), block=False, evt_handlers=handlers)
+
+        assoc = ae.associate("localhost", 11112)
+        assert assoc.is_established
+        rsp = assoc.send_c_store(ds)
+        assert rsp.Status == 0x0000
+        assert "ErrorComment" not in rsp
+        assoc.release()
+        assert assoc.is_released
+
+        assert attrs["uid"] == NewStorage
+
+        scp.shutdown()
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_service_substance_admin.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_service_substance_admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 import time
 
 import pytest
 
 from pydicom.dataset import Dataset
 from pydicom.uid import ExplicitVRLittleEndian
 
-from pynetdicom import AE, evt, debug_logger
+from pynetdicom import AE, evt, debug_logger, register_uid, sop_class
 from pynetdicom.dimse_primitives import C_FIND
 from pynetdicom.presentation import PresentationContext
 from pynetdicom.service_class import (
     SubstanceAdministrationQueryServiceClass,
 )
 from pynetdicom.sop_class import (
     ProductCharacteristicsQuery,
+    _SUBSTANCE_ADMINISTRATION_CLASSES,
 )
 
 
 # debug_logger()
 
 
 def test_unknown_sop_class():
@@ -32,29 +33,43 @@
         r"The supplied abstract syntax is not valid for use with the "
         r"Substance Administration Query Service Class"
     )
     with pytest.raises(ValueError, match=msg):
         service.SCP(C_FIND(), context)
 
 
+@pytest.fixture()
+def register_new_uid():
+    register_uid(
+        "1.2.3.4",
+        "NewFind",
+        SubstanceAdministrationQueryServiceClass,
+        "C-FIND",
+    )
+    yield
+    del _SUBSTANCE_ADMINISTRATION_CLASSES["NewFind"]
+    delattr(sop_class, "NewFind")
+    SubstanceAdministrationQueryServiceClass._SUPPORTED_UIDS["C-FIND"].remove("1.2.3.4")
+
+
 class TestSubstanceAdministrationQueryServiceClass:
     """Test the SubstanceAdministrationQueryServiceClass.
 
     Subclass of QR Find Service class with its own statuses.
     """
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.query = Dataset()
         self.query.QueryRetrieveLevel = "PATIENT"
         self.query.PatientName = "*"
 
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_handler_status_dataset(self):
         """Test handler yielding a Dataset status"""
 
@@ -226,7 +241,39 @@
         assert status.Status == 0xC002
         with pytest.raises(StopIteration):
             next(result)
 
         assoc.release()
         assert assoc.is_released
         scp.shutdown()
+
+    def test_register(self, register_new_uid):
+        """Test handler yielding a Dataset status"""
+        from pynetdicom.sop_class import NewFind
+
+        def handle(event):
+            status = Dataset()
+            status.Status = 0xFF00
+            yield status, self.query
+            yield 0x0000, None
+
+        handlers = [(evt.EVT_C_FIND, handle)]
+
+        self.ae = ae = AE()
+        ae.add_supported_context(NewFind)
+        ae.add_requested_context(NewFind, ExplicitVRLittleEndian)
+        scp = ae.start_server(("localhost", 11112), block=False, evt_handlers=handlers)
+
+        assoc = ae.associate("localhost", 11112)
+        assert assoc.is_established
+        result = assoc.send_c_find(self.query, NewFind)
+        status, identifier = next(result)
+        assert status.Status == 0xFF00
+        status, identifier = next(result)
+        assert status.Status == 0x0000
+        with pytest.raises(StopIteration):
+            next(result)
+
+        assoc.release()
+        assert assoc.is_released
+
+        scp.shutdown()
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_service_verification.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_service_verification.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,19 +15,19 @@
 
 # debug_logger()
 
 
 class TestVerificationServiceClass:
     """Test the VerifictionSOPClass"""
 
-    def setup(self):
+    def setup_method(self):
         """Run prior to each test"""
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         """Clear any active threads"""
         if self.ae:
             self.ae.shutdown()
 
     def test_scp_handler_return_dataset(self):
         """Test handler returning a Dataset status"""
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_sop.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_sop.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Tests for the sop_class module."""
 
 import pytest
 
 from pynetdicom import __version__
 from pydicom._uid_dict import UID_dictionary
 
+from pynetdicom import sop_class
 from pynetdicom.sop_class import (
     uid_to_sop_class,
     uid_to_service_class,
     SOPClass,
     _SERVICE_CLASSES,
     _APPLICATION_EVENT_CLASSES,
     ProceduralEventLogging,
@@ -22,14 +23,16 @@
     DisplaySystem,
     _HANGING_PROTOCOL_CLASSES,
     HangingProtocolInformationModelGet,
     _IMPLANT_TEMPLATE_CLASSES,
     ImplantTemplateGroupInformationModelFind,
     _INSTANCE_AVAILABILITY_CLASSES,
     InstanceAvailabilityNotification,
+    _INVENTORY_CLASSES,
+    InventoryFind,
     _MEDIA_CREATION_CLASSES,
     MediaCreationManagement,
     _MEDIA_STORAGE_CLASSES,
     MediaStorageDirectoryStorage,
     _NON_PATIENT_OBJECT_CLASSES,
     HangingProtocolStorage,
     _PRINT_MANAGEMENT_CLASSES,
@@ -46,36 +49,41 @@
     GeneralRelevantPatientInformationQuery,
     _RT_MACHINE_VERIFICATION_CLASSES,
     RTConventionalMachineVerification,
     _STORAGE_CLASSES,
     CTImageStorage,
     _STORAGE_COMMITMENT_CLASSES,
     StorageCommitmentPushModel,
+    _STORAGE_MANAGEMENT_CLASSES,
+    InventoryCreation,
     _SUBSTANCE_ADMINISTRATION_CLASSES,
     ProductCharacteristicsQuery,
     _UNIFIED_PROCEDURE_STEP_CLASSES,
     UnifiedProcedureStepPull,
     _VERIFICATION_CLASSES,
     Verification,
     DisplaySystemInstance,
     PrinterConfigurationRetrievalInstance,
     PrinterInstance,
     ProceduralEventLoggingInstance,
     StorageCommitmentPushModelInstance,
+    StorageManagementInstance,
     SubstanceAdministrationLoggingInstance,
     UPSFilteredGlobalSubscriptionInstance,
     UPSGlobalSubscriptionInstance,
+    register_uid,
 )
 from pynetdicom.service_class import (
     ServiceClass,
     BasicWorklistManagementServiceClass,
     ColorPaletteQueryRetrieveServiceClass,
     DefinedProcedureProtocolQueryRetrieveServiceClass,
     HangingProtocolQueryRetrieveServiceClass,
     ImplantTemplateQueryRetrieveServiceClass,
+    InventoryQueryRetrieveServiceClass,
     NonPatientObjectStorageServiceClass,
     ProtocolApprovalQueryRetrieveServiceClass,
     QueryRetrieveServiceClass,
     RelevantPatientInformationQueryServiceClass,
     StorageServiceClass,
     SubstanceAdministrationQueryServiceClass,
     VerificationServiceClass,
@@ -85,14 +93,15 @@
     DisplaySystemManagementServiceClass,
     InstanceAvailabilityNotificationServiceClass,
     MediaCreationManagementServiceClass,
     PrintManagementServiceClass,
     ProcedureStepServiceClass,
     RTMachineVerificationServiceClass,
     StorageCommitmentServiceClass,
+    StorageManagementServiceClass,
     UnifiedProcedureStepServiceClass,
 )
 
 
 PYDICOM_VERSION = __version__.split(".")[:2]
 
 
@@ -110,14 +119,16 @@
         assert uid in UID_dictionary
     for uid in _HANGING_PROTOCOL_CLASSES.values():
         assert uid in UID_dictionary
     for uid in _IMPLANT_TEMPLATE_CLASSES.values():
         assert uid in UID_dictionary
     for uid in _INSTANCE_AVAILABILITY_CLASSES.values():
         assert uid in UID_dictionary
+    for uid in _INVENTORY_CLASSES.values():
+        assert uid in UID_dictionary
     for uid in _MEDIA_CREATION_CLASSES.values():
         assert uid in UID_dictionary
     for uid in _MEDIA_STORAGE_CLASSES.values():
         assert uid in UID_dictionary
     for uid in _NON_PATIENT_OBJECT_CLASSES.values():
         assert uid in UID_dictionary
     for uid in _PRINT_MANAGEMENT_CLASSES.values():
@@ -128,19 +139,28 @@
         assert uid in UID_dictionary
     for uid in _QR_CLASSES.values():
         assert uid in UID_dictionary
     for uid in _RELEVANT_PATIENT_QUERY_CLASSES.values():
         assert uid in UID_dictionary
     for uid in _RT_MACHINE_VERIFICATION_CLASSES.values():
         assert uid in UID_dictionary
-    if PYDICOM_VERSION >= ["2", "2"]:
-        for uid in _STORAGE_CLASSES.values():
-            assert uid in UID_dictionary
+    for uid in _STORAGE_CLASSES.values():
+        if uid in (
+            "1.2.840.10008.5.1.4.1.1.6.3",
+            "1.2.840.10008.5.1.4.1.1.9.1.4",
+            "1.2.840.10008.5.1.4.1.1.77.1.8",
+            "1.2.840.10008.5.1.4.1.1.77.1.9",
+        ):
+            continue
+
+        assert uid in UID_dictionary
     for uid in _STORAGE_COMMITMENT_CLASSES.values():
         assert uid in UID_dictionary
+    for uid in _STORAGE_MANAGEMENT_CLASSES.values():
+        assert uid in UID_dictionary
     for uid in _SUBSTANCE_ADMINISTRATION_CLASSES.values():
         assert uid in UID_dictionary
     for uid in _UNIFIED_PROCEDURE_STEP_CLASSES.values():
         assert uid in UID_dictionary
     for uid in _VERIFICATION_CLASSES.values():
         assert uid in UID_dictionary
 
@@ -154,37 +174,38 @@
 def test_all_sop_instances():
     """Test the well-known SOP Instances are correct."""
     assert DisplaySystemInstance in UID_dictionary
     assert PrinterConfigurationRetrievalInstance in UID_dictionary
     assert PrinterInstance in UID_dictionary
     assert ProceduralEventLoggingInstance in UID_dictionary
     assert StorageCommitmentPushModelInstance in UID_dictionary
+    assert StorageManagementInstance in UID_dictionary
     assert SubstanceAdministrationLoggingInstance in UID_dictionary
     assert UPSFilteredGlobalSubscriptionInstance in UID_dictionary
     assert UPSGlobalSubscriptionInstance in UID_dictionary
 
 
 class TestUIDtoSOPlass:
     """Tests for uid_to_sop_class"""
 
-    def test_missing_sop(self):
+    def test_missing_sop_class(self):
         """Test SOP Class if UID not found."""
-        sop_class = uid_to_sop_class("1.2.3.4")
-        assert sop_class == "1.2.3.4"
-        assert sop_class.service_class == ServiceClass
+        sop = uid_to_sop_class("1.2.3.4")
+        assert sop == "1.2.3.4"
+        assert sop.service_class == ServiceClass
 
     def test_verification_uid(self):
         """Test normal function"""
         assert uid_to_sop_class("1.2.840.10008.1.1") == Verification
 
     def test_existing(self):
         """Test that the existing class is returned."""
         original = Verification
-        sop_class = uid_to_sop_class("1.2.840.10008.1.1")
-        assert id(sop_class) == id(original)
+        sop = uid_to_sop_class("1.2.840.10008.1.1")
+        assert id(sop) == id(original)
 
 
 class TestUIDToServiceClass:
     """Tests for sop_class.uid_to_service_class."""
 
     def test_service_class_uid(self):
         uid = "1.2.840.10008.4.2"
@@ -232,14 +253,19 @@
         """Test that the Instance Availability SOP Class UIDs work correctly."""
         for uid in _INSTANCE_AVAILABILITY_CLASSES.values():
             assert (
                 uid_to_service_class(uid)
                 == InstanceAvailabilityNotificationServiceClass
             )
 
+    def test_inventory_uids(self):
+        """Test that the Inventory QR SOP Class UIDs work correctly."""
+        for uid in _INVENTORY_CLASSES.values():
+            assert uid_to_service_class(uid) == InventoryQueryRetrieveServiceClass
+
     def test_media_creation_uids(self):
         """Test that the Media Creation SOP Class UIDs work correctly."""
         for uid in _MEDIA_CREATION_CLASSES.values():
             assert uid_to_service_class(uid) == MediaCreationManagementServiceClass
 
     def test_media_storage_uids(self):
         """Test that the Media Storage SOP Class UIDs work correctly."""
@@ -291,14 +317,19 @@
             assert uid_to_service_class(uid) == StorageServiceClass
 
     def test_storage_commitment_uids(self):
         """Test that the Storage Commitment SOP Class UIDs work correctly."""
         for uid in _STORAGE_COMMITMENT_CLASSES.values():
             assert uid_to_service_class(uid) == StorageCommitmentServiceClass
 
+    def test_storage_management_uids(self):
+        """Test that the Storage Management SOP Class UIDs work correctly."""
+        for uid in _STORAGE_MANAGEMENT_CLASSES.values():
+            assert uid_to_service_class(uid) == StorageManagementServiceClass
+
     def test_substance_admin_uids(self):
         """Test that the Substance Administration SOP Class UIDs work correctly."""
         for uid in _SUBSTANCE_ADMINISTRATION_CLASSES.values():
             assert uid_to_service_class(uid) == SubstanceAdministrationQueryServiceClass
 
     def test_ups_uids(self):
         """Test that the UPS SOP Class UIDs work correctly."""
@@ -314,14 +345,20 @@
         """Test that an unknown UID returns default service class."""
         assert uid_to_service_class("1.2.3") == ServiceClass
 
 
 class TestSOPClass:
     """Tests for sop_class.SOPClass."""
 
+    def test_class_type(self):
+        """Test the class type is correct."""
+        sop = SOPClass("1.2.840.10008.5.1.4.1.1.2")
+        assert isinstance(sop, SOPClass)
+        assert isinstance(SOPClass(sop), SOPClass)
+
     def test_app_logging_sop(self):
         assert ProceduralEventLogging == "1.2.840.10008.1.40"
         assert (
             ProceduralEventLogging.service_class == ApplicationEventLoggingServiceClass
         )
 
     def test_basic_worklist_sop(self):
@@ -373,14 +410,18 @@
     def test_instance_sop(self):
         assert InstanceAvailabilityNotification == "1.2.840.10008.5.1.4.33"
         assert (
             InstanceAvailabilityNotification.service_class
             == InstanceAvailabilityNotificationServiceClass
         )
 
+    def test_instance_sop(self):
+        assert InventoryFind == "1.2.840.10008.5.1.4.1.1.201.2"
+        assert InventoryFind.service_class == InventoryQueryRetrieveServiceClass
+
     def test_media_creation_sop(self):
         assert MediaCreationManagement == "1.2.840.10008.5.1.1.33"
         assert (
             MediaCreationManagement.service_class == MediaCreationManagementServiceClass
         )
 
     def test_media_storage_sop(self):
@@ -440,14 +481,18 @@
         assert CTImageStorage == "1.2.840.10008.5.1.4.1.1.2"
         assert CTImageStorage.service_class == StorageServiceClass
 
     def test_storage_commitment_sop(self):
         assert StorageCommitmentPushModel == "1.2.840.10008.1.20.1"
         assert StorageCommitmentPushModel.service_class == StorageCommitmentServiceClass
 
+    def test_storage_management_sop(self):
+        assert InventoryCreation == "1.2.840.10008.5.1.4.1.1.201.5"
+        assert InventoryCreation.service_class == StorageManagementServiceClass
+
     def test_substance_admin_sop(self):
         """Test s Substance Administration Query Service SOP Class."""
         assert ProductCharacteristicsQuery == "1.2.840.10008.5.1.4.41"
         assert (
             ProductCharacteristicsQuery.service_class
             == SubstanceAdministrationQueryServiceClass
         )
@@ -461,17 +506,162 @@
     def test_verification_sop(self):
         """Test a Verification Service SOP Class."""
         assert Verification == "1.2.840.10008.1.1"
         assert Verification.service_class == VerificationServiceClass
 
     def test_uid_creation(self):
         """Test creating a new UIDSOPClass."""
-        sop_class = SOPClass("1.2.3")
-        sop_class._service_class = ServiceClass
+        sop = SOPClass("1.2.3")
+        sop._service_class = ServiceClass
 
-        assert sop_class == "1.2.3"
-        assert sop_class.service_class == ServiceClass
+        assert sop == "1.2.3"
+        assert sop.service_class == ServiceClass
 
-        sop_class_b = SOPClass(sop_class)
-        assert sop_class == sop_class_b
-        assert sop_class_b == "1.2.3"
-        assert sop_class_b.service_class == ServiceClass
+        sop_b = SOPClass(sop)
+        assert sop == sop_b
+        assert sop_b == "1.2.3"
+        assert sop_b.service_class == ServiceClass
+
+
+class TestRegisterUID:
+    def test_register_storage(self):
+        """Test registering to the storage service."""
+        register_uid(
+            "1.2.3.4",
+            "FooStorage",
+            StorageServiceClass,
+        )
+
+        sop = sop_class.FooStorage
+        assert sop == "1.2.3.4"
+        assert sop.service_class == StorageServiceClass
+
+        del _STORAGE_CLASSES["FooStorage"]
+        delattr(sop_class, "FooStorage")
+
+    def test_register_qr_find(self):
+        """Test registering to the QR service - FIND."""
+        register_uid(
+            "1.2.3.4",
+            "FooFind",
+            QueryRetrieveServiceClass,
+            dimse_msg_type="C-FIND",
+        )
+
+        sop = sop_class.FooFind
+        assert sop == "1.2.3.4"
+        assert sop.service_class == QueryRetrieveServiceClass
+        assert sop in QueryRetrieveServiceClass._SUPPORTED_UIDS["C-FIND"]
+
+        del _QR_CLASSES["FooFind"]
+        QueryRetrieveServiceClass._SUPPORTED_UIDS["C-FIND"].remove(sop)
+        delattr(sop_class, "FooFind")
+
+    def test_register_qr_get(self):
+        """Test registering to the QR service - GET."""
+        register_uid(
+            "1.2.3.4",
+            "FooGet",
+            QueryRetrieveServiceClass,
+            dimse_msg_type="C-GET",
+        )
+
+        sop = sop_class.FooGet
+        assert sop == "1.2.3.4"
+        assert sop.service_class == QueryRetrieveServiceClass
+        assert sop in QueryRetrieveServiceClass._SUPPORTED_UIDS["C-GET"]
+
+        del _QR_CLASSES["FooGet"]
+        QueryRetrieveServiceClass._SUPPORTED_UIDS["C-GET"].remove(sop)
+        delattr(sop_class, "FooGet")
+
+    def test_register_qr_move(self):
+        """Test registering to the QR service - MOVE."""
+        register_uid(
+            "1.2.3.4",
+            "FooMove",
+            QueryRetrieveServiceClass,
+            dimse_msg_type="C-MOVE",
+        )
+
+        sop = sop_class.FooMove
+        assert sop == "1.2.3.4"
+        assert sop.service_class == QueryRetrieveServiceClass
+        assert sop in QueryRetrieveServiceClass._SUPPORTED_UIDS["C-MOVE"]
+
+        del _QR_CLASSES["FooMove"]
+        QueryRetrieveServiceClass._SUPPORTED_UIDS["C-MOVE"].remove(sop)
+        delattr(sop_class, "FooMove")
+
+    def test_register_bwm_find(self):
+        """Test registering to the BWM service."""
+        register_uid(
+            "1.2.3.4",
+            "FooFind",
+            BasicWorklistManagementServiceClass,
+            dimse_msg_type="C-FIND",
+        )
+
+        sop = sop_class.FooFind
+        assert sop == "1.2.3.4"
+        assert sop.service_class == BasicWorklistManagementServiceClass
+        assert sop in BasicWorklistManagementServiceClass._SUPPORTED_UIDS["C-FIND"]
+
+        del _BASIC_WORKLIST_CLASSES["FooFind"]
+        BasicWorklistManagementServiceClass._SUPPORTED_UIDS["C-FIND"].remove(sop)
+        delattr(sop_class, "FooFind")
+
+    def test_register_substance_admin_find(self):
+        """Test registering to the Substance Admin QR service."""
+        register_uid(
+            "1.2.3.4",
+            "FooFind",
+            SubstanceAdministrationQueryServiceClass,
+            dimse_msg_type="C-FIND",
+        )
+
+        sop = sop_class.FooFind
+        assert sop == "1.2.3.4"
+        assert sop.service_class == SubstanceAdministrationQueryServiceClass
+        assert sop in SubstanceAdministrationQueryServiceClass._SUPPORTED_UIDS["C-FIND"]
+
+        del _SUBSTANCE_ADMINISTRATION_CLASSES["FooFind"]
+        SubstanceAdministrationQueryServiceClass._SUPPORTED_UIDS["C-FIND"].remove(sop)
+        delattr(sop_class, "FooFind")
+
+    def test_invalid_keyword_raises(self):
+        """Test invalid keyword raises exceptions."""
+        msg = (
+            "The keyword '2coo' is not a valid Python identifier or is "
+            "a Python keyword"
+        )
+        with pytest.raises(ValueError, match=msg):
+            register_uid("", "2coo", ServiceClass)
+
+        msg = (
+            "The keyword 'def' is not a valid Python identifier or is "
+            "a Python keyword"
+        )
+        with pytest.raises(ValueError, match=msg):
+            register_uid("", "def", ServiceClass)
+
+    def test_invalid_service_class_raises(self):
+        """Test that an invalid service_class raises exceptions."""
+        msg = "'service_class' must be a class object not a class instance"
+        with pytest.raises(TypeError, match=msg):
+            register_uid("", "Foo", "")
+
+        msg = (
+            "'service_class' must be a ServiceClass subclass object "
+            "such as 'StorageServiceClass'"
+        )
+        with pytest.raises(TypeError, match=msg):
+            register_uid("", "Foo", str)
+
+    def test_invalid_dimse_msg_type_raises(self):
+        """Test that an invalid dimse_msg_type raises exceptions."""
+        msg = (
+            "'dimse_msg_type' must be 'C-FIND', 'C-GET' or 'C-MOVE' "
+            "when registering a UID with QueryRetrieveServiceClass"
+        )
+        with pytest.raises(ValueError, match=msg):
+            register_uid("", "Foo", QueryRetrieveServiceClass, "Foo")
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_status.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     from pynetdicom.status import Status
 
     HAS_STATUS = True
 except ImportError:
     HAS_STATUS = False
 
 
-LOGGER = logging.getLogger("pynetdicom")
+LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.CRITICAL)
 
 
 class TestStatus:
     """Test the status.py module"""
 
     def test_code_to_status(self):
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_timer.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 
 import pytest
 
 from pynetdicom.timer import Timer
 from .utils import sleep
 
-LOGGER = logging.getLogger("pynetdicom")
+LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.CRITICAL)
 
 
 class TestTimer:
     """Test the Timer class."""
 
     def test_init(self):
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_transport.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             conn.result = result
             assert conn.result == result
 
 
 class TestAssociationSocket:
     """Tests for the transport.AssociationSocket class."""
 
-    def setup(self):
+    def setup_method(self):
         ae = AE()
         self.assoc = Association(ae, MODE_REQUESTOR)
 
     def get_listen_socket(self):
         sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         sock.setsockopt(socket.SOL_SOCKET, socket.SO_RCVTIMEO, pack("ll", 1, 0))
@@ -168,16 +168,18 @@
         """Test closing and connecting."""
         sock = AssociationSocket(self.assoc)
         sock._is_connected = True
         assert sock.socket is not None
         sock.close()
         assert sock.socket is None
         # Tries to connect, sets to None if fails
+        # Ensure we fail if *something* is listening
+        self.assoc.connection_timeout = 1
         request = A_ASSOCIATE()
-        request.called_presentation_address = ("localhost", 11112)
+        request.called_presentation_address = ("123", 12)
         sock.connect(T_CONNECT(request))
         assert sock.event_queue.get() == "Evt17"
         assert sock.socket is None
 
     def test_ready_error(self):
         """Test AssociationSocket.ready."""
         sock = AssociationSocket(self.assoc, address=("localhost", 0))
@@ -308,37 +310,36 @@
         assert assoc.is_released
 
         server.shutdown()
 
         assert 2 == len(events)
 
 
-@pytest.fixture
-def server_context(request):
-    """Return a good server SSLContext."""
-    # TLS v1.3 is not currently supported :(
-    # The actual available attributes/protocols depend on OS, OpenSSL version
-    #   and Python version, ugh
-    if hasattr(ssl, "TLSVersion"):
-        # This is the current and future, but heavily depends on OpenSSL
-        # Python 3.7+, w/ OpenSSL 1.1.0g+
-        context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
-        context.verify_mode = ssl.CERT_REQUIRED
-        context.load_cert_chain(certfile=SERVER_CERT, keyfile=SERVER_KEY)
-        context.load_verify_locations(cafile=CLIENT_CERT)
-        context.maximum_version = ssl.TLSVersion.TLSv1_2
-
-        return context
-
-    # Should work with older Python and OpenSSL versions
-    # Python 3.6
-    context = ssl.SSLContext(protocol=ssl.PROTOCOL_TLSv1_2)
+def server_context_v1_2():
+    """Return a good TLs v1.2 server SSLContext."""
+    # Python 3.10 and PEP 644, the ssl module requires OpenSSL 1.1.1 or newer
+    context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
+    context.verify_mode = ssl.CERT_REQUIRED
+    context.load_cert_chain(certfile=SERVER_CERT, keyfile=SERVER_KEY)
+    context.load_verify_locations(cafile=CLIENT_CERT)
+    context.minimum_version = ssl.TLSVersion.TLSv1_2
+    context.maximum_version = ssl.TLSVersion.TLSv1_2
+
+    return context
+
+
+def server_context_v1_3():
+    """Return a good TLS v1.3 server SSLContext."""
+    # Python 3.10 and PEP 644, the ssl module requires OpenSSL 1.1.1 or newer
+    context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
     context.verify_mode = ssl.CERT_REQUIRED
     context.load_cert_chain(certfile=SERVER_CERT, keyfile=SERVER_KEY)
     context.load_verify_locations(cafile=CLIENT_CERT)
+    context.minimum_version = ssl.TLSVersion.TLSv1_3
+    context.maximum_version = ssl.TLSVersion.TLSv1_3
 
     return context
 
 
 @pytest.fixture
 def client_context(request):
     """Return a good client SSLContext."""
@@ -346,22 +347,30 @@
     context.verify_mode = ssl.CERT_REQUIRED
     context.load_cert_chain(certfile=CLIENT_CERT, keyfile=CLIENT_KEY)
     context.check_hostname = False
 
     return context
 
 
+TLS_SERVER_CONTEXTS = [(server_context_v1_2, "TLSv1.2")]
+if ssl.OPENSSL_VERSION_INFO >= (1, 1, 1):
+    TLS_SERVER_CONTEXTS = [
+        (server_context_v1_2, "TLSv1.2"),
+        (server_context_v1_3, "TLSv1.3"),
+    ]
+
+
 class TestTLS:
     """Test using TLS to wrap the association."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
         self.has_ssl = transport._HAS_SSL
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
         # Ensure ssl module is available again
         import importlib
 
         importlib.reload(pynetdicom.transport)
@@ -401,60 +410,66 @@
 
         server.shutdown()
 
         time.sleep(0.5)
 
         assert len(server.active_associations) == 0
 
-    def test_tls_yes_server_not_client(self, server_context, caplog):
+    @pytest.mark.parametrize("server_context, tls_version", TLS_SERVER_CONTEXTS)
+    def test_tls_yes_server_not_client(self, server_context, tls_version, caplog):
         """Test wrapping the acceptor socket with TLS (and not client)."""
         with caplog.at_level(logging.ERROR, logger="pynetdicom"):
             self.ae = ae = AE()
             ae.add_supported_context("1.2.840.10008.1.1")
             server = ae.start_server(
                 ("localhost", 11112),
                 block=False,
-                ssl_context=server_context,
+                ssl_context=server_context(),
             )
 
             ae.add_requested_context("1.2.840.10008.1.1")
             assoc = ae.associate("localhost", 11112)
             assert assoc.is_aborted
 
             server.shutdown()
 
             assert len(server.active_associations) == 0
             assert "Connection closed before the entire PDU was received" in caplog.text
 
-    def test_tls_yes_server_yes_client(self, server_context, client_context):
+    @pytest.mark.parametrize("server_context, tls_version", TLS_SERVER_CONTEXTS)
+    def test_tls_yes_server_yes_client(
+        self, server_context, tls_version, client_context
+    ):
         """Test associating with TLS on both ends."""
         self.ae = ae = AE()
         ae.acse_timeout = 5
         ae.dimse_timeout = 5
         ae.network_timeout = 5
         ae.add_supported_context("1.2.840.10008.1.1")
         server = ae.start_server(
             ("localhost", 11112),
             block=False,
-            ssl_context=server_context,
+            ssl_context=server_context(),
         )
 
         wait_for_server_socket(server, 1)
 
         ae.add_requested_context("1.2.840.10008.1.1")
         assoc = ae.associate("localhost", 11112, tls_args=(client_context, None))
+        assert assoc.dul.socket.socket.version() == tls_version
         assert assoc.is_established
         assoc.release()
         assert assoc.is_released
 
         server.shutdown()
 
         assert len(server.active_associations) == 0
 
-    def test_tls_transfer(self, server_context, client_context):
+    @pytest.mark.parametrize("server_context, tls_version", TLS_SERVER_CONTEXTS)
+    def test_tls_transfer(self, server_context, tls_version, client_context):
         """Test transferring data after associating with TLS."""
         ds = []
 
         def handle_store(event):
             ds.append(event.dataset)
             return 0x0000
 
@@ -465,15 +480,15 @@
         ae.dimse_timeout = 5
         ae.network_timeout = 5
         ae.add_supported_context("1.2.840.10008.1.1")
         ae.add_supported_context(RTImageStorage)
         server = ae.start_server(
             ("localhost", 11112),
             block=False,
-            ssl_context=server_context,
+            ssl_context=server_context(),
             evt_handlers=handlers,
         )
 
         ae.add_requested_context("1.2.840.10008.1.1")
         ae.add_requested_context(RTImageStorage)
         assoc = ae.associate("localhost", 11112, tls_args=(client_context, None))
         assert assoc.is_established
@@ -520,15 +535,16 @@
         ae.dimse_timeout = 5
         ae.network_timeout = 5
         ae.add_requested_context("1.2.840.10008.1.1")
         msg = r"Your Python installation lacks support for SSL"
         with pytest.raises(RuntimeError, match=msg):
             ae.associate("localhost", 11112, tls_args=(["random", "object"], None))
 
-    def test_multiple_pdu_req(self, server_context, client_context):
+    @pytest.mark.parametrize("server_context, tls_version", TLS_SERVER_CONTEXTS)
+    def test_multiple_pdu_req(self, server_context, tls_version, client_context):
         """Test what happens if two PDUs are sent before the select call."""
         events = []
 
         def handle_echo(event):
             events.append(event)
             return 0x0000
 
@@ -538,15 +554,15 @@
         ae.network_timeout = 5
         ae.add_supported_context("1.2.840.10008.1.1")
         ae.add_requested_context("1.2.840.10008.1.1")
 
         server = ae.start_server(
             ("localhost", 11112),
             block=False,
-            ssl_context=server_context,
+            ssl_context=server_context(),
         )
 
         assoc = ae.associate(
             "localhost",
             11112,
             tls_args=(client_context, None),
             evt_handlers=[(evt.EVT_C_ECHO, handle_echo)],
@@ -563,15 +579,16 @@
         timeout = 0
         while not assoc.is_released and timeout < 5:
             time.sleep(0.05)
             timeout += 0.05
 
         assert assoc.is_released
 
-    def test_multiple_pdu_acc(self, server_context, client_context):
+    @pytest.mark.parametrize("server_context, tls_version", TLS_SERVER_CONTEXTS)
+    def test_multiple_pdu_acc(self, server_context, tls_version, client_context):
         """Test what happens if two PDUs are sent before the select call."""
         events = []
 
         def handle_echo(event):
             events.append(event)
             return 0x0000
 
@@ -581,15 +598,15 @@
         ae.network_timeout = 5
         ae.add_supported_context("1.2.840.10008.1.1")
         ae.add_requested_context("1.2.840.10008.1.1")
 
         server = ae.start_server(
             ("localhost", 11112),
             block=False,
-            ssl_context=server_context,
+            ssl_context=server_context(),
             evt_handlers=[(evt.EVT_C_ECHO, handle_echo)],
         )
 
         assoc = ae.associate("localhost", 11112, tls_args=(client_context, None))
         assert assoc.is_established
 
         # Send data directly to the requestor
@@ -608,18 +625,18 @@
 
         server.shutdown()
 
         assert 2 == len(events)
 
 
 class TestAssociationServer:
-    def setup(self):
+    def setup_method(self):
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
     @pytest.mark.skip()
     def test_multi_assoc_block(self):
         """Test that multiple requestors can associate when blocking."""
         self.ae = ae = AE()
@@ -774,15 +791,15 @@
         ae.associate("localhost", 11112)
 
         assert server.socket.fileno() != -1
 
         server.shutdown()
 
         if sys.version_info[0] == 2:
-            with pytest.raises(socket.error):
+            with pytest.raises(OSError):
                 server.socket.fileno()
         else:
             assert server.socket.fileno() == -1
 
     def test_blocking_process_request(self):
         """Test AssociationServer.process_request."""
         self.ae = ae = AE()
@@ -873,18 +890,18 @@
 
         server.shutdown()
 
 
 class TestEventHandlingAcceptor:
     """Test the transport events and handling as acceptor."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
     def test_no_handlers(self):
         """Test with no transport event handlers bound."""
         self.ae = ae = AE()
         ae.add_supported_context(Verification)
@@ -1629,18 +1646,18 @@
             assert msg in caplog.text
             assert "Exception description" in caplog.text
 
 
 class TestEventHandlingRequestor:
     """Test the transport events and handling as requestor."""
 
-    def setup(self):
+    def setup_method(self):
         self.ae = None
 
-    def teardown(self):
+    def teardown_method(self):
         if self.ae:
             self.ae.shutdown()
 
     def test_no_handlers(self):
         """Test associations as requestor with no handlers bound."""
         self.ae = ae = AE()
         ae.add_supported_context(Verification)
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_utils.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Unit tests for the pynetdicom.utils module."""
 
+from codecs import BOM_UTF32_LE
 from io import BytesIO
 from threading import Thread
 import logging
 import sys
 
 import pytest
 
@@ -95,18 +96,18 @@
     ("0.1.2.4", (True, True)),
 ]
 
 
 class TestValidateUID:
     """Tests for utils.validate_uid()."""
 
-    def setup(self):
+    def setup_method(self):
         self.default_conformance = _config.ENFORCE_UID_CONFORMANCE
 
-    def teardown(self):
+    def teardown_method(self):
         _config.ENFORCE_UID_CONFORMANCE = self.default_conformance
 
     @pytest.mark.parametrize("uid,is_valid", REFERENCE_UID)
     def test_validate_uid_conformance_true(self, uid, is_valid):
         _config.ENFORCE_UID_CONFORMANCE = True
         assert validate_uid(UID(uid)) == is_valid[0]
 
@@ -226,15 +227,15 @@
         assert isinstance(b, bytes)
         uid = set_uid(b, "foo")
         assert isinstance(uid, UID)
         assert uid == "1.2.3"
 
     def test_bytes_decoding_error(self, caplog):
         """Test invalid bytes raises exception"""
-        b = "1.2.3".encode("utf_32")
+        b = BOM_UTF32_LE + "1.2.3".encode("utf_32_le")
         assert isinstance(b, bytes)
         msg = (
             r"Unable to decode 'FF FE 00 00 31 00 00 00 2E 00 00 00 32 00 00 "
             r"00 2E 00 00 00 33 00 00 00' using the ascii codec\(s\)"
         )
         with caplog.at_level(logging.ERROR, logger="pynetdicom"):
             with pytest.raises(ValueError, match=msg):
@@ -308,28 +309,28 @@
 
 
 class TestDecodeBytes:
     """Tests for utils.decode_bytes"""
 
     def test_decoding_error(self, caplog):
         """Test decoding error raises and logs"""
-        b = "1.2.3".encode("utf_32")
+        b = BOM_UTF32_LE + "1.2.3".encode("utf_32_le")
         with caplog.at_level(logging.ERROR, logger="pynetdicom"):
             msg = (
                 r"Unable to decode 'FF FE 00 00 31 00 00 00 2E 00 00 00 32 "
                 r"00 00 00 2E 00 00 00 33 00 00 00' using the ascii codec\(s\)"
             )
             with pytest.raises(ValueError, match=msg):
                 decode_bytes(b)
 
             assert ("'ascii' codec can't decode byte 0xff in position 0") in caplog.text
 
     def test_decoding_error_fallback(self, caplog, utf8):
         """Test decoding error raises and logs"""
-        b = "1.2.3".encode("utf_32")
+        b = BOM_UTF32_LE + "1.2.3".encode("utf_32_le")
         with caplog.at_level(logging.ERROR, logger="pynetdicom"):
             msg = (
                 r"Unable to decode 'FF FE 00 00 31 00 00 00 2E 00 00 00 32 "
                 r"00 00 00 2E 00 00 00 33 00 00 00' using the ascii, "
                 r"utf8 codec\(s\)"
             )
             with pytest.raises(ValueError, match=msg):
```

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/test_validators.py` & `pynetdicom-2.1.0/pynetdicom/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/tests/utils.py` & `pynetdicom-2.1.0/pynetdicom/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pynetdicom-2.0.2/pynetdicom/timer.py` & `pynetdicom-2.1.0/pynetdicom/timer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 A generic timer class suitable for use as the DICOM UL's ARTIM timer.
 """
+
 import logging
 import time
 from typing import Optional
 
 
-LOGGER = logging.getLogger("pynetdicom.artim")
+LOGGER = logging.getLogger(__name__)
 
 
 class Timer:
     """A generic timer.
 
     Implementation of the DICOM Upper Layer's ARTIM timer. The ARTIM timer is
     used by the state machine to monitor connection and response timeouts.
```

### Comparing `pynetdicom-2.0.2/pynetdicom/transport.py` & `pynetdicom-2.1.0/pynetdicom/transport.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,27 +10,19 @@
 from socketserver import TCPServer, ThreadingMixIn, BaseRequestHandler
 
 try:
     import ssl
 
     _HAS_SSL = True
 except ImportError:
+    # NOTE: Must check `_HAS_SSL` before all use of `ssl` module
+    #   and must use "ssl.SSLContext" in type hints
     _HAS_SSL = False
 import threading
-from typing import (
-    TYPE_CHECKING,
-    Optional,
-    Any,
-    Tuple,
-    cast,
-    List,
-    Dict,
-    Callable,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, cast, Callable, Optional
 
 from pynetdicom import evt, _config
 from pynetdicom._globals import MODE_ACCEPTOR, BIND_ADDRESS
 from pynetdicom._handlers import (
     standard_dimse_recv_handler,
     standard_dimse_sent_handler,
     standard_pdu_recv_handler,
@@ -41,15 +33,15 @@
 
 if TYPE_CHECKING:  # pragma: no cover
     from pynetdicom.ae import ApplicationEntity
     from pynetdicom.association import Association
     from pynetdicom.dul import _QueueType
 
 
-LOGGER = logging.getLogger("pynetdicom.transport")
+LOGGER = logging.getLogger(__name__)
 
 
 class T_CONNECT:
     """A TRANSPORT CONNECTION primitive
 
     .. versionadded:: 2.0
 
@@ -75,17 +67,17 @@
         if not isinstance(request, A_ASSOCIATE):
             raise TypeError(
                 f"'request' must be 'pynetdicom.pdu_primitives.A_ASSOCIATE', not "
                 f"'{request.__class__.__name__}'"
             )
 
     @property
-    def address(self) -> Tuple[str, int]:
+    def address(self) -> tuple[str, int]:
         """Return the peer's ``(str: IP address, int: port)``."""
-        return cast(Tuple[str, int], self.request.called_presentation_address)
+        return cast(tuple[str, int], self.request.called_presentation_address)
 
     @property
     def result(self) -> str:
         """Return the result of the connection attempt as :class:`str`.
 
         Parameters
         ----------
@@ -132,16 +124,16 @@
     socket : socket.socket or None
         The wrapped socket, will be ``None`` if :meth:`close` is called.
     """
 
     def __init__(
         self,
         assoc: "Association",
-        client_socket: Optional[socket.socket] = None,
-        address: Tuple[str, int] = BIND_ADDRESS,
+        client_socket: socket.socket | None = None,
+        address: tuple[str, int] = BIND_ADDRESS,
     ) -> None:
         """Create a new :class:`AssociationSocket`.
 
         Parameters
         ----------
         assoc : association.Association
             The :class:`~pynetdicom.association.Association` instance that will
@@ -159,27 +151,27 @@
         if client_socket is not None and address != BIND_ADDRESS:
             LOGGER.warning(
                 "AssociationSocket instantiated with both a 'client_socket' "
                 "and bind 'address'. The original socket will not be rebound"
             )
 
         self._ready = threading.Event()
-        self.socket: Optional[socket.socket]
+        self.socket: socket.socket | None
 
         if client_socket is None:
             self.socket = self._create_socket(address)
             self._is_connected = False
         else:
             self.socket = client_socket
             self._is_connected = True
             self._ready.set()
             # Evt5: Transport connection indication
             self.event_queue.put("Evt5")
 
-        self._tls_args: Optional[Tuple["ssl.SSLContext", str]] = None
+        self._tls_args: tuple["ssl.SSLContext", str] | None = None
         self.select_timeout = 0.5
 
     @property
     def assoc(self) -> "Association":
         """Return the parent :class:`~pynetdicom.association.Association`
         instance.
         """
@@ -195,25 +187,25 @@
         - Evt17: Transport connection closed
         """
         if self.socket is None or self._is_connected is False:
             return
 
         try:
             self.socket.shutdown(socket.SHUT_RDWR)
-        except socket.error:
+        except OSError:
             pass
 
         self.socket.close()
         self.socket = None
         self._is_connected = False
         # Evt17: Transport connection closed
         self.event_queue.put("Evt17")
 
     def connect(self, primitive: T_CONNECT) -> None:
-        """Try and connect to a remote using connection details from `primitive`.
+        """Try and connect to a remote using connection details from  `primitive`.
 
         .. versionchanged:: 2.0
 
             Changed to take a :class:`~pynetdicom.transport.T_CONNECT` primitive rather
             than an address tuple.
 
         Parameters
@@ -234,30 +226,30 @@
                         server_side=False,
                         server_hostname=server_hostname,
                     ),
                 )
             # Set ae connection timeout
             self.socket.settimeout(self.assoc.connection_timeout)
             # Try and connect to remote at (address, port)
-            #   raises socket.error if connection refused
+            #   raises OSError if connection refused
             self.socket.connect(primitive.address)
             # Clear ae connection timeout
             self.socket.settimeout(None)
             # Trigger event - connection open
             evt.trigger(self.assoc, evt.EVT_CONN_OPEN, {"address": primitive.address})
             self._is_connected = True
             # Evt2: Transport connection confirmation
             primitive.result = "Evt2"
             self.provider_queue.put(primitive)
         except OSError as exc:
             # Log connection failure
             LOGGER.error("Association request failed: unable to connect to remote")
             LOGGER.error(f"TCP Initialisation Error: {exc}")
             # Log exception if TLS issue to help with troubleshooting
-            if isinstance(exc, ssl.SSLError):
+            if _HAS_SSL and isinstance(exc, ssl.SSLError):
                 LOGGER.exception(exc)
 
             # Don't be tempted to replace this with a self.close() call -
             #   it doesn't work because `_is_connected` is False
             if self.socket:
                 try:
                     self.socket.shutdown(socket.SHUT_RDWR)
@@ -267,15 +259,15 @@
                 self.socket = None
 
             primitive.result = "Evt17"
             self.provider_queue.put(primitive)
         finally:
             self._ready.set()
 
-    def _create_socket(self, address: Tuple[str, int] = BIND_ADDRESS) -> socket.socket:
+    def _create_socket(self, address: tuple[str, int] = BIND_ADDRESS) -> socket.socket:
         """Create a new IPv4 TCP socket and set it up for use.
 
         *Socket Options*
 
         - :attr:`socket.SO_REUSEADDR` is 1
         - :meth:`socket.settimeout` sets the Association's
           :attr:`~pynetdicom.association.Associaton.network_timeout` value.
@@ -311,20 +303,20 @@
     @property
     def event_queue(self) -> "queue.Queue[str]":
         """Return the :class:`~pynetdicom.association.Association`'s service event
         queue.
         """
         return self.assoc.dul.event_queue
 
-    def get_local_addr(self, host: Tuple[str, int] = ("10.255.255.255", 1)) -> str:
+    def get_local_addr(self, host: tuple[str, int] = ("10.255.255.255", 1)) -> str:
         """Return an address for the local computer as :class:`str`.
 
         Parameters
         ----------
-        host : Tuple[str, int]
+        host : tuple[str, int]
             The host's ``(addr: str, port: int)`` when trying to determine the local
             address.
         """
         # Solution from https://stackoverflow.com/a/28950776
         with socket.socket(socket.AF_INET, socket.SOCK_DGRAM) as sock:
             try:
                 # We use `host` to allow unit testing
@@ -359,15 +351,15 @@
         """
         if self.socket is None or self._is_connected is False:
             return False
 
         try:
             # Use a timeout of 0 so we get an "instant" result
             ready, _, _ = select.select([self.socket], [], [], 0)
-        except (socket.error, socket.timeout, ValueError):
+        except (OSError, TimeoutError, ValueError):
             # Evt17: Transport connection closed
             self.event_queue.put("Evt17")
             return False
 
         # An SSLSocket may have buffered data available that `select`
         # is unaware of - see #528
         if _HAS_SSL and isinstance(self.socket, ssl.SSLSocket):
@@ -438,44 +430,44 @@
         try:
             while total_sent < length_data:
                 # Returns the number of bytes sent
                 nr_sent = self.socket.send(bytestream[total_sent:])
                 total_sent += nr_sent
 
             evt.trigger(self.assoc, evt.EVT_DATA_SENT, {"data": bytestream})
-        except (socket.error, socket.timeout):
+        except (OSError, TimeoutError):
             # Evt17: Transport connection closed
             self.event_queue.put("Evt17")
 
     def __str__(self) -> str:
         """Return the string output for ``socket``."""
         return self.socket.__str__()
 
     @property
-    def tls_args(self) -> Optional[Tuple["ssl.SSLContext", str]]:
+    def tls_args(self) -> tuple["ssl.SSLContext", str] | None:
         """Get or set the TLS context and hostname.
 
         Parameters
         ----------
-        tls_args : Tuple[ssl.SSLContext, str] or None
+        tls_args : tuple[ssl.SSLContext, str] or None
             If the socket should be wrapped by TLS then this is
             ``(context, hostname)``, where *context* is a
             :class:`ssl.SSLContext` that will be used to wrap the socket and
             *hostname* is the value to use for the *server_hostname* keyword
             argument for :meth:`SSLContext.wrap_socket()
             <ssl.SSLContext.wrap_socket>`.
 
         Returns
         -------
-        Optional[Tuple[ssl.SSLContext, str]]
+        tuple[ssl.SSLContext, str] | None
         """
         return self._tls_args
 
     @tls_args.setter
-    def tls_args(self, tls_args: Optional[Tuple["ssl.SSLContext", str]]) -> None:
+    def tls_args(self, tls_args: tuple["ssl.SSLContext", str] | None) -> None:
         """Set the TLS arguments for the socket."""
         if not _HAS_SSL:
             raise RuntimeError("Your Python installation lacks support for SSL")
 
         self._tls_args = tls_args
 
 
@@ -512,22 +504,22 @@
 
         # Trigger must be after binding the events
         evt.trigger(assoc, evt.EVT_CONN_OPEN, {"address": self.client_address})
 
         assoc.start()
 
     @property
-    def local(self) -> Tuple[str, int]:
+    def local(self) -> tuple[str, int]:
         """Return a 2-tuple of the local server's ``(host, port)`` address."""
         return self.server.server_address
 
     @property
-    def remote(self) -> Tuple[str, int]:
+    def remote(self) -> tuple[str, int]:
         """Return a 2-tuple of the remote client's ``(host, port)`` address."""
-        return cast(Tuple[str, int], self.client_address)
+        return cast(tuple[str, int], self.client_address)
 
     def _create_association(self) -> "Association":
         """Create an :class:`Association` object for the current request.
 
         .. versionadded:: 1.5
         """
         from pynetdicom.association import Association
@@ -555,18 +547,17 @@
         assoc.requestor.address = self.remote[0]
         assoc.requestor.port = self.remote[1]
 
         # Bind events to handlers
         for event in self.server._handlers:
             # Intervention events
             if event.is_intervention and self.server._handlers[event]:
-
                 assoc.bind(event, *self.server._handlers[event])
             elif isinstance(event, evt.NotificationEvent):
-                # List[Tuple[Callable, Optional[List[Any]]]]
+                # list[tuple[Callable, list[Any] | None]]
                 for handler in self.server._handlers[event]:
                     handler = cast(evt._HandlerBase, handler)
                     assoc.bind(event, handler[0], handler[1])
 
         return assoc
 
 
@@ -590,36 +581,36 @@
 
     Attributes
     ----------
     ae : ae.ApplicationEntity
         The parent AE that is running the server.
     request_queue_size : int
         Default ``5``.
-    server_address : Tuple[str, int]
+    server_address : tuple[str, int]
         The ``(host: str, port: int)`` that the server is running on.
     """
 
     def __init__(
         self,
         ae: "ApplicationEntity",
-        address: Tuple[str, int],
+        address: tuple[str, int],
         ae_title: str,
-        contexts: List[PresentationContext],
+        contexts: list[PresentationContext],
         ssl_context: Optional["ssl.SSLContext"] = None,
-        evt_handlers: List[evt.EventHandlerType] = None,
-        request_handler: Optional[Callable[..., BaseRequestHandler]] = None,
+        evt_handlers: list[evt.EventHandlerType] | None = None,
+        request_handler: Callable[..., BaseRequestHandler] | None = None,
     ) -> None:
         """Create a new :class:`AssociationServer`, bind a socket and start
         listening.
 
         Parameters
         ----------
         ae : ae.ApplicationEntity
             The parent AE that's running the server.
-        address : Tuple[str, int]
+        address : tuple[str, int]
             The ``(host: str, port: int)`` that the server should run on.
         ae_title : str
             The AE title of the SCP.
         contexts : list of presentation.PresentationContext
             The SCPs supported presentation contexts.
         ssl_context : ssl.SSLContext, optional
             If TLS is to be used then this should be the
@@ -635,42 +626,39 @@
             :class:`~socketserver.BaseRequestHandler`.
         """
         self.ae = ae
         self.ae_title = ae_title
         self.contexts = contexts
         self.ssl_context = ssl_context
         self.allow_reuse_address = True
-        self.server_address: Tuple[str, int] = address
-        self.socket: Optional[socket.socket] = None  # type: ignore[assignment]
+        self.server_address: tuple[str, int] = address
+        self.socket: socket.socket | None = None  # type: ignore[assignment]
 
         request_handler = request_handler or RequestHandler
 
         super().__init__(address, request_handler, bind_and_activate=True)
 
         self.timeout = 60
 
         # Stores all currently bound event handlers so future
         #   Associations can be bound
-        self._handlers: Dict[
+        self._handlers: dict[
             evt.EventType,
-            Union[
-                List[Tuple[Callable, Optional[List[Any]]]],
-                Tuple[Callable, Optional[List[Any]]],
-            ],
+            list[tuple[Callable, list[Any] | None]] | tuple[Callable, list[Any] | None],
         ] = {}
         self._bind_defaults()
 
         # Bind the functions to their events
         for evt_hh_args in evt_handlers or ():
             self.bind(*evt_hh_args)
 
         self._gc = [0, 59]
 
     def bind(
-        self, event: evt.EventType, handler: Callable, args: Optional[List[Any]] = None
+        self, event: evt.EventType, handler: Callable, args: list[Any] | None = None
     ) -> None:
         """Bind a callable `handler` to an `event`.
 
         .. versionadded:: 1.3
 
         .. versionchanged:: 1.5
 
@@ -703,26 +691,26 @@
         if _config.LOG_HANDLER_LEVEL == "standard":
             self.bind(evt.EVT_DIMSE_RECV, standard_dimse_recv_handler)
             self.bind(evt.EVT_DIMSE_SENT, standard_dimse_sent_handler)
             self.bind(evt.EVT_PDU_RECV, standard_pdu_recv_handler)
             self.bind(evt.EVT_PDU_SENT, standard_pdu_sent_handler)
 
     @property
-    def active_associations(self) -> List["Association"]:
+    def active_associations(self) -> list["Association"]:
         """Return the server's running
         :class:`~pynetdicom.association.Association` acceptor instances
         """
         # Find all AcceptorThreads with `_server` as self
         threads = cast(
-            List["Association"],
+            list["Association"],
             [tt for tt in threading.enumerate() if "AcceptorThread" in tt.name],
         )
         return [tt for tt in threads if tt._server is self]
 
-    def get_events(self) -> List[evt.EventType]:
+    def get_events(self) -> list[evt.EventType]:
         """Return a list of currently bound events.
 
         .. versionadded:: 1.3
         """
         return sorted(self._handlers.keys(), key=lambda x: x.name)
 
     def get_handlers(self, event: evt.EventType) -> evt.HandlerArgType:
@@ -750,15 +738,15 @@
             ``(None, None)`` if no handler has been bound.
         """
         if event not in self._handlers:
             return []
 
         return self._handlers[event]
 
-    def get_request(self) -> Tuple[socket.socket, Tuple[str, int]]:
+    def get_request(self) -> tuple[socket.socket, tuple[str, int]]:
         """Handle a connection request.
 
         If :attr:`~AssociationServer.ssl_context` is set then the client socket
         will be wrapped using
         :meth:`SSLContext.wrap_socket()<ssl.SSLContext.wrap_socket>`.
 
         Returns
@@ -775,16 +763,16 @@
                 client_socket, server_side=True
             )
 
         return client_socket, address
 
     def process_request(
         self,
-        request: Union[socket.socket, Tuple[bytes, socket.socket]],
-        client_address: Union[Tuple[str, int], str],
+        request: socket.socket | tuple[bytes, socket.socket],
+        client_address: tuple[str, int] | str,
     ) -> None:
         """Process a connection request"""
         # Calls request_handler(request, client_address, self)
         self.finish_request(request, client_address)
 
     def server_bind(self) -> None:
         """Bind the socket and set the socket options.
@@ -813,15 +801,15 @@
         self.server_address = self.socket.getsockname()
 
     def server_close(self) -> None:
         """Close the server."""
         self.socket = cast(socket.socket, self.socket)
         try:
             self.socket.shutdown(socket.SHUT_RDWR)
-        except socket.error:
+        except OSError:
             pass
 
         self.socket.close()
 
     def service_actions(self) -> None:
         """Called by the serve_forever() loop"""
         # For whatever reason dead Association threads aren't being garbage
@@ -883,16 +871,16 @@
     """An :class:`AssociationServer` suitable for threading.
 
     .. versionadded:: 1.2
     """
 
     def process_request_thread(
         self,
-        request: Union[socket.socket, Tuple[bytes, socket.socket]],
-        client_address: Union[Tuple[str, int], str],
+        request: socket.socket | tuple[bytes, socket.socket],
+        client_address: tuple[str, int] | str,
     ) -> None:
         """Process a connection request."""
         # pylint: disable=broad-except
         try:
             self.finish_request(request, client_address)
         except Exception:
             self.handle_error(request, client_address)
```

### Comparing `pynetdicom-2.0.2/pynetdicom/utils.py` & `pynetdicom-2.1.0/pynetdicom/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     HAVE_CTYPES = False
 
 from pydicom.uid import UID
 
 from pynetdicom import _config
 
 
-LOGGER = logging.getLogger("pynetdicom.utils")
+LOGGER = logging.getLogger(__name__)
 
 
 def decode_bytes(encoded_value: bytes) -> str:
     """Return the decoded string from `encoded_value`.
 
     .. versionadded:: 2.0
```

