# Comparing `tmp/pih-0.37.3.tar.gz` & `tmp/pih-0.37.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-0.37.3.tar", last modified: Tue May 21 20:33:10 2024, max compression
+gzip compressed data, was "pih-0.37.4.tar", last modified: Tue May 21 23:31:10 2024, max compression
```

## Comparing `pih-0.37.3.tar` & `pih-0.37.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 20:33:10.599142 pih-0.37.3/
--rw-rw-rw-   0        0        0      249 2024-05-21 20:33:10.567832 pih-0.37.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-21 20:33:08.234643 pih-0.37.3/pih/
--rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.37.3/pih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:33:08.580497 pih-0.37.3/pih/collections/
--rw-rw-rw-   0        0        0    30339 2024-05-17 03:55:00.000000 pih-0.37.3/pih/collections/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.37.3/pih/collections/service.py
--rw-rw-rw-   0        0        0   104226 2024-05-20 23:34:54.000000 pih-0.37.3/pih/console_api.py
--rw-rw-rw-   0        0        0     2549 2024-05-19 11:56:07.000000 pih-0.37.3/pih/console_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:33:10.190731 pih-0.37.3/pih/consts/
--rw-rw-rw-   0        0        0    26749 2024-05-21 20:31:26.000000 pih-0.37.3/pih/consts/__init__.py
--rw-rw-rw-   0        0        0     3694 2024-05-18 23:37:39.000000 pih-0.37.3/pih/consts/ad.py
--rw-rw-rw-   0        0        0     1768 2024-05-08 05:34:18.000000 pih-0.37.3/pih/consts/addresses.py
--rw-rw-rw-   0        0        0      974 2024-04-21 23:56:33.000000 pih-0.37.3/pih/consts/date_time.py
--rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.37.3/pih/consts/document.py
--rw-rw-rw-   0        0        0      936 2024-05-20 02:54:33.000000 pih-0.37.3/pih/consts/errors.py
--rw-rw-rw-   0        0        0    30003 2024-04-22 02:31:56.000000 pih-0.37.3/pih/consts/events.py
--rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.37.3/pih/consts/facade.py
--rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.37.3/pih/consts/file.py
--rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.37.3/pih/consts/hosts.py
--rw-rw-rw-   0        0        0      194 2024-04-17 15:27:11.000000 pih-0.37.3/pih/consts/iot.py
--rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.37.3/pih/consts/names.py
--rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.37.3/pih/consts/password.py
--rw-rw-rw-   0        0        0    12272 2024-05-13 03:26:35.000000 pih-0.37.3/pih/consts/paths.py
--rw-rw-rw-   0        0        0    16022 2024-05-21 01:27:45.000000 pih-0.37.3/pih/consts/polibase.py
--rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.37.3/pih/consts/python.py
--rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.37.3/pih/consts/recognize.py
--rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.37.3/pih/consts/rpc.py
--rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.37.3/pih/consts/service.py
--rw-rw-rw-   0        0        0     6540 2024-04-17 04:46:50.000000 pih-0.37.3/pih/consts/service_commands.py
--rw-rw-rw-   0        0        0    12120 2024-05-12 15:14:12.000000 pih-0.37.3/pih/consts/service_roles.py
--rw-rw-rw-   0        0        0    17771 2024-05-20 23:11:31.000000 pih-0.37.3/pih/consts/settings.py
--rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.37.3/pih/consts/ssh_hosts.py
--rw-rw-rw-   0        0        0      233 2024-05-17 04:55:05.000000 pih-0.37.3/pih/consts/style.py
--rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.37.3/pih/consts/zabbix.py
--rw-rw-rw-   0        0        0   572583 2024-05-21 20:30:41.000000 pih-0.37.3/pih/pih.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:33:10.362614 pih-0.37.3/pih/rpc/
--rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.37.3/pih/rpc/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.37.3/pih/rpc/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.37.3/pih/rpc/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.37.3/pih/service_example.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:33:10.474061 pih-0.37.3/pih/tools/
--rw-rw-rw-   0        0        0    59031 2024-05-20 00:30:59.000000 pih-0.37.3/pih/tools/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.37.3/pih/tools/service.py
--rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.37.3/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2024-05-21 20:33:10.536585 pih-0.37.3/pih.egg-info/
--rw-rw-rw-   0        0        0      249 2024-05-21 20:33:07.000000 pih-0.37.3/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      976 2024-05-21 20:33:07.000000 pih-0.37.3/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 20:33:07.000000 pih-0.37.3/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-21 20:33:07.000000 pih-0.37.3/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-21 20:33:07.000000 pih-0.37.3/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 20:33:10.614705 pih-0.37.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 23:31:10.276829 pih-0.37.4/
+-rw-rw-rw-   0        0        0      249 2024-05-21 23:31:10.229955 pih-0.37.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-21 23:31:08.152620 pih-0.37.4/pih/
+-rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.37.4/pih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:31:08.452912 pih-0.37.4/pih/collections/
+-rw-rw-rw-   0        0        0    30339 2024-05-17 03:55:00.000000 pih-0.37.4/pih/collections/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.37.4/pih/collections/service.py
+-rw-rw-rw-   0        0        0   104226 2024-05-20 23:34:54.000000 pih-0.37.4/pih/console_api.py
+-rw-rw-rw-   0        0        0     2549 2024-05-19 11:56:07.000000 pih-0.37.4/pih/console_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:31:09.814561 pih-0.37.4/pih/consts/
+-rw-rw-rw-   0        0        0    26749 2024-05-21 23:29:23.000000 pih-0.37.4/pih/consts/__init__.py
+-rw-rw-rw-   0        0        0     3694 2024-05-18 23:37:39.000000 pih-0.37.4/pih/consts/ad.py
+-rw-rw-rw-   0        0        0     1768 2024-05-08 05:34:18.000000 pih-0.37.4/pih/consts/addresses.py
+-rw-rw-rw-   0        0        0      974 2024-04-21 23:56:33.000000 pih-0.37.4/pih/consts/date_time.py
+-rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.37.4/pih/consts/document.py
+-rw-rw-rw-   0        0        0      936 2024-05-20 02:54:33.000000 pih-0.37.4/pih/consts/errors.py
+-rw-rw-rw-   0        0        0    30003 2024-04-22 02:31:56.000000 pih-0.37.4/pih/consts/events.py
+-rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.37.4/pih/consts/facade.py
+-rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.37.4/pih/consts/file.py
+-rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.37.4/pih/consts/hosts.py
+-rw-rw-rw-   0        0        0      194 2024-04-17 15:27:11.000000 pih-0.37.4/pih/consts/iot.py
+-rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.37.4/pih/consts/names.py
+-rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.37.4/pih/consts/password.py
+-rw-rw-rw-   0        0        0    12272 2024-05-13 03:26:35.000000 pih-0.37.4/pih/consts/paths.py
+-rw-rw-rw-   0        0        0    16022 2024-05-21 01:27:45.000000 pih-0.37.4/pih/consts/polibase.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.37.4/pih/consts/python.py
+-rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.37.4/pih/consts/recognize.py
+-rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.37.4/pih/consts/rpc.py
+-rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.37.4/pih/consts/service.py
+-rw-rw-rw-   0        0        0     6540 2024-04-17 04:46:50.000000 pih-0.37.4/pih/consts/service_commands.py
+-rw-rw-rw-   0        0        0    12120 2024-05-12 15:14:12.000000 pih-0.37.4/pih/consts/service_roles.py
+-rw-rw-rw-   0        0        0    17771 2024-05-20 23:11:31.000000 pih-0.37.4/pih/consts/settings.py
+-rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.37.4/pih/consts/ssh_hosts.py
+-rw-rw-rw-   0        0        0      233 2024-05-17 04:55:05.000000 pih-0.37.4/pih/consts/style.py
+-rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.37.4/pih/consts/zabbix.py
+-rw-rw-rw-   0        0        0   572646 2024-05-21 23:29:12.000000 pih-0.37.4/pih/pih.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:31:10.010165 pih-0.37.4/pih/rpc/
+-rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.37.4/pih/rpc/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.37.4/pih/rpc/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.37.4/pih/rpc/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.37.4/pih/service_example.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:31:10.119539 pih-0.37.4/pih/tools/
+-rw-rw-rw-   0        0        0    59035 2024-05-21 23:18:29.000000 pih-0.37.4/pih/tools/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.37.4/pih/tools/service.py
+-rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.37.4/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:31:10.183060 pih-0.37.4/pih.egg-info/
+-rw-rw-rw-   0        0        0      249 2024-05-21 23:31:07.000000 pih-0.37.4/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      976 2024-05-21 23:31:07.000000 pih-0.37.4/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 23:31:07.000000 pih-0.37.4/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-21 23:31:07.000000 pih-0.37.4/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-21 23:31:07.000000 pih-0.37.4/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 23:31:10.276829 pih-0.37.4/setup.cfg
```

### Comparing `pih-0.37.3/pih/collections/__init__.py` & `pih-0.37.4/pih/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/collections/service.py` & `pih-0.37.4/pih/collections/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/console_api.py` & `pih-0.37.4/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/console_api_wrapper.py` & `pih-0.37.4/pih/console_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/consts/__init__.py` & `pih-0.37.4/pih/consts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     ZabbixResourceDescriptionDelegated,
     IconedOrderedNameCaptionDescription,
 )
 from pih.consts.password import *
 from pih.consts.date_time import *
 from pih.consts.service_commands import *
 
-VERSION: str = "0.37.3"
+VERSION: str = "0.37.4"
 
 
 class DATA:
     # deprecated
     class EXTRACTOR:
         USER_NAME_FULL: str = "user_name_full"
         USER_NAME: str = "user_name"
```

### Comparing `pih-0.37.3/pih/consts/ad.py` & `pih-0.37.4/pih/consts/ad.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/consts/addresses.py` & `pih-0.37.4/pih/consts/addresses.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/consts/date_time.py` & `pih-0.37.4/pih/consts/date_time.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/consts/errors.py` & `pih-0.37.4/pih/consts/errors.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/consts/events.py` & `pih-0.37.4/pih/consts/events.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/consts/hosts.py` & `pih-0.37.4/pih/consts/hosts.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/consts/names.py` & `pih-0.37.4/pih/consts/names.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/consts/password.py` & `pih-0.37.4/pih/consts/password.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/consts/paths.py` & `pih-0.37.4/pih/consts/paths.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/consts/polibase.py` & `pih-0.37.4/pih/consts/polibase.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/consts/service.py` & `pih-0.37.4/pih/consts/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/consts/service_commands.py` & `pih-0.37.4/pih/consts/service_commands.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/consts/service_roles.py` & `pih-0.37.4/pih/consts/service_roles.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/consts/settings.py` & `pih-0.37.4/pih/consts/settings.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/pih.py` & `pih-0.37.4/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from subprocess import DEVNULL, STDOUT, CompletedProcess
 from contextlib import contextmanager, redirect_stdout
 from pkg_resources import parse_version, working_set
 from urllib.parse import unquote, quote_plus, quote
 from concurrent.futures import ThreadPoolExecutor
 from requests import ConnectTimeout, Response
 from colorama import Back, Style, Fore, ansi
+from datetime import datetime, timedelta, date
 from typing import Any, Callable, TypeAlias
-from datetime import datetime, timedelta
 from collections import defaultdict
 from prettytable import PrettyTable
 from colorama.ansi import CSI, OSC
 from transliterate import translit
 from concurrent import futures
 from random import randrange
 from threading import Thread
@@ -9581,24 +9581,26 @@
                         day_end -= timedelta(days=abs(day_start))
                     else:
                         day_end = start_date.replace(day=day_start)
                 return PIH.RESULT.TIME_TRACKING.create(start_date, end_date, tab_number)
 
             @staticmethod
             def create(
-                start_date: datetime | None = None,
-                end_date: datetime | None = None,
+                start: datetime | date | None = None,
+                end_date: datetime | date | None = None,
                 tab_number_list: list[str] | None = None,
             ) -> Result[list[TimeTrackingResultByPerson]]:
                 now: datetime | None = DataTool.check(
-                    e(start_date) or e(end_date),
+                    e(start) or e(end_date),
                     datetime.now(),
                 )
-                start_date = DateTimeTool.begin_date(start_date or now)
-                end_date = DateTimeTool.end_date(end_date or now)
+                if isinstance(start, date):
+                    start = DateTimeTool.begin_date(start or now)
+                if isinstance(end_date, date):
+                    end_date = DateTimeTool.end_date(end_date or now)
 
                 def get_date_or_time(entity: TimeTrackingEntity, date: bool) -> str:
                     return DataTool.check_not_none(
                         entity,
                         lambda: entity.TimeVal.split(DATE_TIME.SPLITTER)[not date],
                     )
 
@@ -9606,15 +9608,15 @@
                 full_name_by_tab_number_map: dict = {}
                 result_data = defaultdict(
                     lambda: defaultdict(lambda: defaultdict(list))
                 )
                 data: list[TimeTrackingEntity] = DataTool.to_result(
                     PIH.SERVICE.call_command(
                         ServiceCommands.get_time_tracking,
-                        (start_date, end_date, tab_number_list),
+                        (start, end_date, tab_number_list),
                     ),
                     TimeTrackingEntity,
                 ).data
                 for time_tracking_entity in data:
                     tab_number: str = time_tracking_entity.TabNumber
                     full_name_by_tab_number_map[tab_number] = (
                         time_tracking_entity.FullName
@@ -9639,17 +9641,17 @@
                         full_name: str = full_name_by_tab_number_map[tab_number]
                         result_person_item: TimeTrackingResultByPerson = (
                             TimeTrackingResultByPerson(
                                 tab_number, full_name_by_tab_number_map[tab_number]
                             )
                         )
                         result_division_item.list.append(result_person_item)
-                        for date in result_data[division_name][tab_number]:
+                        for date_item in result_data[division_name][tab_number]:
                             time_tracking_entity_list: list[TimeTrackingEntity] = (
-                                result_data[division_name][tab_number][date]
+                                result_data[division_name][tab_number][date_item]
                             )
                             time_tracking_enter_entity: TimeTrackingEntity = None
                             time_tracking_exit_entity: TimeTrackingEntity = None
                             for (
                                 time_tracking_entity_list_item
                             ) in time_tracking_entity_list:
                                 if time_tracking_entity_list_item.Mode == 1:
@@ -9676,15 +9678,15 @@
                                             60 * 60
                                             if (full_name in has_lunch_break)
                                             else 0
                                         )
                                     result_person_item.duration += duration
                             result_person_item.list.append(
                                 TimeTrackingResultByDate(
-                                    date,
+                                    date_item,
                                     get_date_or_time(time_tracking_enter_entity, False),
                                     get_date_or_time(time_tracking_exit_entity, False),
                                     duration,
                                 )
                             )
                 for division in result:
                     for person in division.list:
@@ -13229,16 +13231,16 @@
                 plain_format: bool = False,
             ) -> bool:
                 return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
                         ServiceCommands.save_time_tracking_report,
                         (
                             path,
-                            DateTimeTool.begin_date(start_date),
-                            DateTimeTool.end_date(end_date),
+                            start_date,
+                            end_date,
                             tab_number_list,
                             plain_format,
                         ),
                     )
                 )
 
         class INVENTORY:
```

### Comparing `pih-0.37.3/pih/rpc/__init__.py` & `pih-0.37.4/pih/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/rpc/rpcCommandCall_pb2.py` & `pih-0.37.4/pih/rpc/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/rpc/rpcCommandCall_pb2_grpc.py` & `pih-0.37.4/pih/rpc/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/tools/__init__.py` & `pih-0.37.4/pih/tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
         if isinstance(value, (list, tuple)):
             value_list = value
         elif isinstance(value, (int, Enum)):
             value_list = [value]
         return BitMask.set(value_list)
 
     @staticmethod
-    def by_index(data: list | None, index: int, default_value: Any = None) -> Any:
+    def by_index(data: list | None, index: int = 0, default_value: Any = None) -> Any:
         if n(data):
             return default_value
         if len(data) <= index:
             return default_value
         return data[index]
 
     @staticmethod
```

### Comparing `pih-0.37.3/pih/tools/service.py` & `pih-0.37.4/pih/tools/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih/widgets.py` & `pih-0.37.4/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-0.37.3/pih.egg-info/SOURCES.txt` & `pih-0.37.4/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

