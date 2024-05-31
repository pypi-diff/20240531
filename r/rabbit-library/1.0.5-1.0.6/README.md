# Comparing `tmp/rabbit_library-1.0.5.tar.gz` & `tmp/rabbit_library-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbit_library-1.0.5.tar", max compression
+gzip compressed data, was "rabbit_library-1.0.6.tar", max compression
```

## Comparing `rabbit_library-1.0.5.tar` & `rabbit_library-1.0.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1130 2024-05-27 20:47:51.000761 rabbit_library-1.0.5/pyproject.toml
--rw-r--r--   0        0        0       26 2023-07-03 17:14:02.867213 rabbit_library-1.0.5/rabbit_library/__init__.py
--rw-r--r--   0        0        0     9395 2024-05-27 20:44:17.968557 rabbit_library-1.0.5/rabbit_library/Rabbit.py
--rw-r--r--   0        0        0     3448 2023-10-26 20:38:03.049544 rabbit_library-1.0.5/README.md
--rw-r--r--   0        0        0     4076 1970-01-01 00:00:00.000000 rabbit_library-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1130 2024-05-31 17:54:14.782531 rabbit_library-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-07-03 17:14:02.867213 rabbit_library-1.0.6/rabbit_library/__init__.py
+-rw-r--r--   0        0        0     9700 2024-05-31 17:56:15.289643 rabbit_library-1.0.6/rabbit_library/Rabbit.py
+-rw-r--r--   0        0        0     3448 2023-10-26 20:38:03.049544 rabbit_library-1.0.6/README.md
+-rw-r--r--   0        0        0     4076 1970-01-01 00:00:00.000000 rabbit_library-1.0.6/PKG-INFO
```

### Comparing `rabbit_library-1.0.5/pyproject.toml` & `rabbit_library-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rabbit-library"
-version = "1.0.5"
+version = "1.0.6"
 description = "Biblioteca para se conectar ao rabbit e possibilitar trabalhar com o serviço de mensageria"
 license = "MIT"
 authors = ["Eliézer Schwartz <eliezer.mail090@gmail.com>"]
 readme = "README.md"
 packages = [{include = "rabbit_library"}]
 classifiers = [    
     "Environment :: Console",
```

### Comparing `rabbit_library-1.0.5/rabbit_library/Rabbit.py` & `rabbit_library-1.0.6/rabbit_library/Rabbit.py`

 * *Files 6% similar despite different names*

```diff
@@ -128,16 +128,18 @@
                 exchange = self.virtualhost
 
             if not self.__is_connected():
                 self.__connect()
             return self.__send_message(queue, exchange, message)
 
         except Exception as e:
+            error_message = str(e).encode('ascii', 'ignore').decode('ascii')
             logging.error(
-                f"Error the send message to rabbit: {str(e)} ", stack_info=True)
+                "Error the send message to rabbit: {} ".format(error_message), stack_info=True)
+            return False
 
     def __is_connected(self) -> bool:
         """
             Returns True if the RabbitMQ connection is established, otherwise False.
         """
         if self.channel and not self.channel.is_closed:
             return True
@@ -168,16 +170,17 @@
             self.channel.queue_bind(
                 queue=queue, exchange=exchange, routing_key=queue)
             self.channel.basic_publish(
                 exchange=exchange, routing_key=queue, body=message)
 
             return True
         except Exception as e:
+            error_message = str(e).encode('ascii', 'ignore').decode('ascii')
             logging.error(
-                f"Error the send message to rabbbit: {str(e)} ", stack_info=True)
+                "Error the send message to rabbbit: {} ".format(error_message), stack_info=True)
             return False
 
     def __receive_message(self, queue: str, exchange: str, message_handler: typing.Callable, limit_get_messages: int) -> None:
         '''
             Connect the rabbit consume messages the queue and return message in the method "process_message"
             Recived: 
                 queue - queue to get messages
@@ -202,9 +205,10 @@
             self.channel.start_consuming()
 
     def close_connection(self):
         try:
             if self.channel and not self.channel.is_closed:
                 self.channel.close()
         except Exception as e:
+            error_message = str(e).encode('ascii', 'ignore').decode('ascii')
             logging.error(
-                f"Error closing connection: {str(e)} ", stack_info=True)
+                "Error closing connection: {} ".format(error_message), stack_info=True)
```

### Comparing `rabbit_library-1.0.5/README.md` & `rabbit_library-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rabbit_library-1.0.5/PKG-INFO` & `rabbit_library-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rabbit-library
-Version: 1.0.5
+Version: 1.0.6
 Summary: Biblioteca para se conectar ao rabbit e possibilitar trabalhar com o serviço de mensageria
 License: MIT
 Author: Eliézer Schwartz
 Author-email: eliezer.mail090@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

