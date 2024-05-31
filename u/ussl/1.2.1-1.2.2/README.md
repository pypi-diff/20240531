# Comparing `tmp/ussl-1.2.1.tar.gz` & `tmp/ussl-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ussl-1.2.1.tar", last modified: Thu May 30 08:35:04 2024, max compression
+gzip compressed data, was "dist\ussl-1.2.2.tar", last modified: Fri May 31 09:34:45 2024, max compression
```

## Comparing `ussl-1.2.1.tar` & `ussl-1.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.934725 ussl-1.2.1/
--rw-rw-rw-   0        0        0    12117 2024-05-30 08:35:04.930725 ussl-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0    11465 2024-05-30 08:20:33.000000 ussl-1.2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-30 08:35:04.934725 ussl-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2233 2024-05-30 08:31:46.000000 ussl-1.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.885216 ussl-1.2.1/ussl/
--rw-rw-rw-   0        0        0      133 2024-05-30 08:35:02.000000 ussl-1.2.1/ussl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.903570 ussl-1.2.1/ussl/exceptions/
--rw-rw-rw-   0        0        0      305 2024-05-29 08:59:11.000000 ussl-1.2.1/ussl/exceptions/__init__.py
--rw-rw-rw-   0        0        0     1369 2024-05-22 08:57:11.000000 ussl-1.2.1/ussl/exceptions/main.py
--rw-rw-rw-   0        0        0     1126 2024-05-29 09:16:44.000000 ussl-1.2.1/ussl/exceptions/protocol_exc.py
--rw-rw-rw-   0        0        0     1084 2024-03-01 08:27:08.000000 ussl-1.2.1/ussl/exceptions/validation_exc.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.905596 ussl-1.2.1/ussl/model/
--rw-rw-rw-   0        0        0     4405 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/model/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.909564 ussl-1.2.1/ussl/postprocessing/
--rw-rw-rw-   0        0        0        0 2024-03-01 08:27:08.000000 ussl-1.2.1/ussl/postprocessing/__init__.py
--rw-rw-rw-   0        0        0     7341 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/postprocessing/base.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.923563 ussl-1.2.1/ussl/protocol/
--rw-rw-rw-   0        0        0      798 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/protocol/__init__.py
--rw-rw-rw-   0        0        0      711 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/protocol/base.py
--rw-rw-rw-   0        0        0     1534 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/protocol/ldap.py
--rw-rw-rw-   0        0        0     4610 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/protocol/ssh.py
--rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.2.1/ussl/protocol/winexe.py
--rw-rw-rw-   0        0        0     8202 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/protocol/winrm.py
--rw-rw-rw-   0        0        0      303 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/protocol/wmi.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.925566 ussl-1.2.1/ussl/transport/
--rw-rw-rw-   0        0        0     1508 2024-05-30 08:20:33.000000 ussl-1.2.1/ussl/transport/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.927564 ussl-1.2.1/ussl/utils/
--rw-rw-rw-   0        0        0     6424 2024-03-01 08:27:08.000000 ussl-1.2.1/ussl/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-30 08:35:04.894926 ussl-1.2.1/ussl.egg-info/
--rw-rw-rw-   0        0        0    12117 2024-05-30 08:35:04.000000 ussl-1.2.1/ussl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      584 2024-05-30 08:35:04.000000 ussl-1.2.1/ussl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 08:35:04.000000 ussl-1.2.1/ussl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2024-05-30 08:35:04.000000 ussl-1.2.1/ussl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-30 08:35:04.000000 ussl-1.2.1/ussl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.290774 ussl-1.2.2/
+-rw-rw-rw-   0        0        0    12117 2024-05-31 09:34:45.286154 ussl-1.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0    11465 2024-05-31 09:32:58.000000 ussl-1.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-31 09:34:45.290774 ussl-1.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     2233 2024-05-31 09:34:43.000000 ussl-1.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.239961 ussl-1.2.2/ussl/
+-rw-rw-rw-   0        0        0      133 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.258977 ussl-1.2.2/ussl/exceptions/
+-rw-rw-rw-   0        0        0      305 2024-05-29 08:59:11.000000 ussl-1.2.2/ussl/exceptions/__init__.py
+-rw-rw-rw-   0        0        0     1369 2024-05-22 08:57:11.000000 ussl-1.2.2/ussl/exceptions/main.py
+-rw-rw-rw-   0        0        0     1126 2024-05-29 09:16:44.000000 ussl-1.2.2/ussl/exceptions/protocol_exc.py
+-rw-rw-rw-   0        0        0     1084 2024-03-01 08:27:08.000000 ussl-1.2.2/ussl/exceptions/validation_exc.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.261976 ussl-1.2.2/ussl/model/
+-rw-rw-rw-   0        0        0     4405 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/model/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.266344 ussl-1.2.2/ussl/postprocessing/
+-rw-rw-rw-   0        0        0        0 2024-03-01 08:27:08.000000 ussl-1.2.2/ussl/postprocessing/__init__.py
+-rw-rw-rw-   0        0        0     7341 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/postprocessing/base.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.280865 ussl-1.2.2/ussl/protocol/
+-rw-rw-rw-   0        0        0      798 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/protocol/__init__.py
+-rw-rw-rw-   0        0        0      711 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/protocol/base.py
+-rw-rw-rw-   0        0        0     1534 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/protocol/ldap.py
+-rw-rw-rw-   0        0        0     4617 2024-05-31 09:34:43.000000 ussl-1.2.2/ussl/protocol/ssh.py
+-rw-rw-rw-   0        0        0        0 2024-01-24 09:57:50.000000 ussl-1.2.2/ussl/protocol/winexe.py
+-rw-rw-rw-   0        0        0     8202 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/protocol/winrm.py
+-rw-rw-rw-   0        0        0      303 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/protocol/wmi.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.283139 ussl-1.2.2/ussl/transport/
+-rw-rw-rw-   0        0        0     1508 2024-05-31 09:32:58.000000 ussl-1.2.2/ussl/transport/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.284139 ussl-1.2.2/ussl/utils/
+-rw-rw-rw-   0        0        0     6424 2024-03-01 08:27:08.000000 ussl-1.2.2/ussl/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:34:45.249733 ussl-1.2.2/ussl.egg-info/
+-rw-rw-rw-   0        0        0    12117 2024-05-31 09:34:45.000000 ussl-1.2.2/ussl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      584 2024-05-31 09:34:45.000000 ussl-1.2.2/ussl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 09:34:45.000000 ussl-1.2.2/ussl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2024-05-31 09:34:45.000000 ussl-1.2.2/ussl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-31 09:34:45.000000 ussl-1.2.2/ussl.egg-info/top_level.txt
```

### Comparing `ussl-1.2.1/PKG-INFO` & `ussl-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ussl
-Version: 1.2.1
+Version: 1.2.2
 Summary: Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами
 Author: ussc soc dev team
 Author-email: iushangaraev@ussc.ru, pbikkuzhina@ussc.ru
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `ussl-1.2.1/README.md` & `ussl-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ussl-1.2.1/setup.py` & `ussl-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 setup(
     name='ussl',
     author='ussc soc dev team',
     author_email='iushangaraev@ussc.ru, pbikkuzhina@ussc.ru',
     description='Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.2.1',
+    version='1.2.2',
     python_requires='>=3.8.0',
     packages=[
         'ussl',
         'ussl.model',
         'ussl.postprocessing',
         'ussl.protocol',
         'ussl.transport',
```

### Comparing `ussl-1.2.1/ussl/exceptions/main.py` & `ussl-1.2.2/ussl/exceptions/main.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.1/ussl/exceptions/protocol_exc.py` & `ussl-1.2.2/ussl/exceptions/protocol_exc.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.1/ussl/exceptions/validation_exc.py` & `ussl-1.2.2/ussl/exceptions/validation_exc.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.1/ussl/model/__init__.py` & `ussl-1.2.2/ussl/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.1/ussl/postprocessing/base.py` & `ussl-1.2.2/ussl/postprocessing/base.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.1/ussl/protocol/__init__.py` & `ussl-1.2.2/ussl/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.1/ussl/protocol/base.py` & `ussl-1.2.2/ussl/protocol/base.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.1/ussl/protocol/ldap.py` & `ussl-1.2.2/ussl/protocol/ldap.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.1/ussl/protocol/ssh.py` & `ussl-1.2.2/ussl/protocol/ssh.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import io
 import socket
 import time
-from typing import Optional, Self, Union
+from typing import Optional, Union
 
 import paramiko
 from paramiko.rsakey import RSAKey
 from paramiko.ssh_exception import AuthenticationException, SSHException
 
 from ..model import Protocol, Query, Response
 from .base import BaseProtocol
@@ -80,23 +80,23 @@
 
     def close(self):
         """Close SSH connection."""
         if self._connection is not None:
             self._connection.close()
             self._connection = None
 
-    def __enter__(self) -> Self:
-        self.connect()
-        return self
-
-    def __exit__(self, exc_type: Exception, *args):
-        self.close()  ## TODO: fix
-        if exc_type is not None:
-            return False
-        return True
+    # def __enter__(self):
+    #     self.connect()
+    #     return self
+    #
+    # def __exit__(self, exc_type: Exception, *args):
+    #     self.close()  ## TODO: fix
+    #     if exc_type is not None:
+    #         return False
+    #     return True
 
     def execute(self, query: Union[Query, str]) -> Response:
         if isinstance(query, str):
             query = Query(command=query)
         command = query.command
         sudo = query.sudo
         timeout = query.timeout if query.timeout else SSHProtocol.EXEC_COMMAND_TIMEOUT
```

### Comparing `ussl-1.2.1/ussl/protocol/winrm.py` & `ussl-1.2.2/ussl/protocol/winrm.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.1/ussl/transport/__init__.py` & `ussl-1.2.2/ussl/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.1/ussl/utils/__init__.py` & `ussl-1.2.2/ussl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ussl-1.2.1/ussl.egg-info/PKG-INFO` & `ussl-1.2.2/ussl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ussl
-Version: 1.2.1
+Version: 1.2.2
 Summary: Пакет разработчиков USSC-SOC для упрощения взаимодействия с АРМ, серверами и сетевыми устройствами
 Author: ussc soc dev team
 Author-email: iushangaraev@ussc.ru, pbikkuzhina@ussc.ru
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
```

### Comparing `ussl-1.2.1/ussl.egg-info/SOURCES.txt` & `ussl-1.2.2/ussl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

