# Comparing `tmp/federated_learning_framework-0.0.2.tar.gz` & `tmp/federated_learning_framework-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "federated_learning_framework-0.0.2.tar", last modified: Wed May 29 13:34:09 2024, max compression
+gzip compressed data, was "federated_learning_framework-0.0.3.tar", last modified: Fri May 31 05:42:23 2024, max compression
```

## Comparing `federated_learning_framework-0.0.2.tar` & `federated_learning_framework-0.0.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 13:34:09.351036 federated_learning_framework-0.0.2/
--rw-rw-rw-   0        0        0     1646 2024-05-29 06:56:35.000000 federated_learning_framework-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     7384 2024-05-29 13:34:09.349034 federated_learning_framework-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6168 2024-05-29 13:28:36.000000 federated_learning_framework-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-29 13:34:09.314034 federated_learning_framework-0.0.2/federated_learning_framework/
--rw-rw-rw-   0        0        0        0 2024-05-29 06:33:59.000000 federated_learning_framework-0.0.2/federated_learning_framework/__init__.py
--rw-rw-rw-   0        0        0      269 2024-05-29 13:12:13.000000 federated_learning_framework-0.0.2/federated_learning_framework/active_learning.py
--rw-rw-rw-   0        0        0     2439 2024-05-29 12:42:47.000000 federated_learning_framework-0.0.2/federated_learning_framework/central_server.py
--rw-rw-rw-   0        0        0     2240 2024-05-29 12:47:07.000000 federated_learning_framework-0.0.2/federated_learning_framework/client_device.py
--rw-rw-rw-   0        0        0     1730 2024-05-29 06:41:19.000000 federated_learning_framework-0.0.2/federated_learning_framework/connection.py
--rw-rw-rw-   0        0        0      780 2024-05-29 13:33:35.000000 federated_learning_framework-0.0.2/federated_learning_framework/decorators.py
--rw-rw-rw-   0        0        0      840 2024-05-29 06:41:44.000000 federated_learning_framework-0.0.2/federated_learning_framework/encryption.py
--rw-rw-rw-   0        0        0      146 2024-05-29 13:33:41.000000 federated_learning_framework-0.0.2/federated_learning_framework/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:34:09.348037 federated_learning_framework-0.0.2/federated_learning_framework.egg-info/
--rw-rw-rw-   0        0        0     7384 2024-05-29 13:34:09.000000 federated_learning_framework-0.0.2/federated_learning_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      860 2024-05-29 13:34:09.000000 federated_learning_framework-0.0.2/federated_learning_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 13:34:09.000000 federated_learning_framework-0.0.2/federated_learning_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-29 13:17:12.000000 federated_learning_framework-0.0.2/federated_learning_framework.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       43 2024-05-29 13:34:09.000000 federated_learning_framework-0.0.2/federated_learning_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0       35 2024-05-29 13:34:09.000000 federated_learning_framework-0.0.2/federated_learning_framework.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-29 13:34:09.351036 federated_learning_framework-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1444 2024-05-29 13:33:17.000000 federated_learning_framework-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-29 13:34:09.344038 federated_learning_framework-0.0.2/tests/
--rw-rw-rw-   0        0        0        0 2024-05-29 06:36:42.000000 federated_learning_framework-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0      535 2024-05-29 06:46:34.000000 federated_learning_framework-0.0.2/tests/test_active_learning.py
--rw-rw-rw-   0        0        0      621 2024-05-29 13:33:47.000000 federated_learning_framework-0.0.2/tests/test_central_server.py
--rw-rw-rw-   0        0        0      806 2024-05-29 12:25:04.000000 federated_learning_framework-0.0.2/tests/test_client_device.py
--rw-rw-rw-   0        0        0      910 2024-05-29 13:33:50.000000 federated_learning_framework-0.0.2/tests/test_connection.py
--rw-rw-rw-   0        0        0      374 2024-05-29 06:46:00.000000 federated_learning_framework-0.0.2/tests/test_encryption.py
--rw-rw-rw-   0        0        0      272 2024-05-29 06:47:18.000000 federated_learning_framework-0.0.2/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:42:23.919112 federated_learning_framework-0.0.3/
+-rw-rw-rw-   0        0        0     1646 2024-05-29 06:56:35.000000 federated_learning_framework-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     7285 2024-05-31 05:42:23.917107 federated_learning_framework-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6069 2024-05-31 05:28:58.000000 federated_learning_framework-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-31 05:42:23.817109 federated_learning_framework-0.0.3/federated_learning_framework/
+-rw-rw-rw-   0        0        0        0 2024-05-29 06:33:59.000000 federated_learning_framework-0.0.3/federated_learning_framework/__init__.py
+-rw-rw-rw-   0        0        0      269 2024-05-29 13:12:13.000000 federated_learning_framework-0.0.3/federated_learning_framework/active_learning.py
+-rw-rw-rw-   0        0        0     2439 2024-05-29 12:42:47.000000 federated_learning_framework-0.0.3/federated_learning_framework/central_server.py
+-rw-rw-rw-   0        0        0     2240 2024-05-29 12:47:07.000000 federated_learning_framework-0.0.3/federated_learning_framework/client_device.py
+-rw-rw-rw-   0        0        0     1730 2024-05-29 06:41:19.000000 federated_learning_framework-0.0.3/federated_learning_framework/connection.py
+-rw-rw-rw-   0        0        0      780 2024-05-29 13:33:35.000000 federated_learning_framework-0.0.3/federated_learning_framework/decorators.py
+-rw-rw-rw-   0        0        0      840 2024-05-29 06:41:44.000000 federated_learning_framework-0.0.3/federated_learning_framework/encryption.py
+-rw-rw-rw-   0        0        0      146 2024-05-29 13:33:41.000000 federated_learning_framework-0.0.3/federated_learning_framework/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:42:23.915107 federated_learning_framework-0.0.3/federated_learning_framework.egg-info/
+-rw-rw-rw-   0        0        0     7285 2024-05-31 05:42:23.000000 federated_learning_framework-0.0.3/federated_learning_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      860 2024-05-31 05:42:23.000000 federated_learning_framework-0.0.3/federated_learning_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 05:42:23.000000 federated_learning_framework-0.0.3/federated_learning_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-29 13:17:12.000000 federated_learning_framework-0.0.3/federated_learning_framework.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       43 2024-05-31 05:42:23.000000 federated_learning_framework-0.0.3/federated_learning_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2024-05-31 05:42:23.000000 federated_learning_framework-0.0.3/federated_learning_framework.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 05:42:23.919112 federated_learning_framework-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1444 2024-05-31 05:41:54.000000 federated_learning_framework-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 05:42:23.913110 federated_learning_framework-0.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-29 06:36:42.000000 federated_learning_framework-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0      535 2024-05-29 06:46:34.000000 federated_learning_framework-0.0.3/tests/test_active_learning.py
+-rw-rw-rw-   0        0        0      621 2024-05-29 13:33:47.000000 federated_learning_framework-0.0.3/tests/test_central_server.py
+-rw-rw-rw-   0        0        0      806 2024-05-29 12:25:04.000000 federated_learning_framework-0.0.3/tests/test_client_device.py
+-rw-rw-rw-   0        0        0      910 2024-05-29 13:33:50.000000 federated_learning_framework-0.0.3/tests/test_connection.py
+-rw-rw-rw-   0        0        0      374 2024-05-29 06:46:00.000000 federated_learning_framework-0.0.3/tests/test_encryption.py
+-rw-rw-rw-   0        0        0      272 2024-05-29 06:47:18.000000 federated_learning_framework-0.0.3/tests/test_utils.py
```

### Comparing `federated_learning_framework-0.0.2/LICENSE` & `federated_learning_framework-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `federated_learning_framework-0.0.2/PKG-INFO` & `federated_learning_framework-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-learning-framework
-Version: 0.0.2
+Version: 0.0.3
 Summary: A modular and extensible framework for federated learning applications.
 Home-page: https://github.com/mehrdaddjavadi/federated_learning_framework
 Author: Mehrdad Javadi
 Author-email: mehrdaddjavadi@gmail.com
 Keywords: federated learning,machine learning,deep learning,encryption
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -107,42 +107,40 @@
 File: utils.py
 
 Includes utility functions used throughout the framework.
 
 Installation
 Clone the repository:
 
-bash
-Copy code
+
 git clone https://github.com/mehrdaddjavadi/federated_learning_framework.git
 Navigate to the directory:
 
-bash
-Copy code
+
 cd federated_learning_framework
 Install the dependencies:
 
-bash
-Copy code
+
 pip install -r requirements.txt
+
 Usage
+
 Setting Up the Central Server
-python
-Copy code
+
 import asyncio
 from federated_learning_framework.central_server import CentralServer
 
 async def main():
     server = CentralServer()
     await server.run_server()
 
 asyncio.run(main())
 Setting Up a Client Device
-python
-Copy code
+
+
 import asyncio
 import tensorflow as tf
 from federated_learning_framework.client_device import ClientDevice
 from federated_learning_framework.encryption import create_context
 
 # Define your model
 model = tf.keras.Sequential([
@@ -162,17 +160,19 @@
     x_train, y_train = ...  # Load your training data
     await client.federated_learning(uri, x_train, y_train)
     # Optionally receive data from central server
     data = await client.receive_data()
     print(f"Received data: {data}")
 
 asyncio.run(main())
+
 Using Decorators
-python
-Copy code
+
+
+
 import asyncio
 import tensorflow as tf
 from federated_learning_framework.decorators import federated_learning_decorator, encryption_decorator
 from federated_learning_framework.client_device import ClientDevice
 from federated_learning_framework.encryption import create_context
 
 # Create context for encryption
@@ -192,17 +192,16 @@
     x_train, y_train = ...  # Load your training data
     await client.federated_learning('ws://localhost:8089', x_train, y_train)
 
 asyncio.run(main())
 Running Tests
 To run the tests, execute the following command in the root directory:
 
-bash
-Copy code
 python -m unittest discover -s tests
+
 License
 The usage of this library is free for academic work with proper referencing. For business, governmental, and any other types of usage, please contact me directly. All rights are reserved.
 
 Contact: mehrdaddjavadi@gmail.com
 
 Contributing
 Feel free to contribute by submitting a pull request or opening an issue.
```

### Comparing `federated_learning_framework-0.0.2/README.md` & `federated_learning_framework-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -78,42 +78,40 @@
 File: utils.py
 
 Includes utility functions used throughout the framework.
 
 Installation
 Clone the repository:
 
-bash
-Copy code
+
 git clone https://github.com/mehrdaddjavadi/federated_learning_framework.git
 Navigate to the directory:
 
-bash
-Copy code
+
 cd federated_learning_framework
 Install the dependencies:
 
-bash
-Copy code
+
 pip install -r requirements.txt
+
 Usage
+
 Setting Up the Central Server
-python
-Copy code
+
 import asyncio
 from federated_learning_framework.central_server import CentralServer
 
 async def main():
     server = CentralServer()
     await server.run_server()
 
 asyncio.run(main())
 Setting Up a Client Device
-python
-Copy code
+
+
 import asyncio
 import tensorflow as tf
 from federated_learning_framework.client_device import ClientDevice
 from federated_learning_framework.encryption import create_context
 
 # Define your model
 model = tf.keras.Sequential([
@@ -133,17 +131,19 @@
     x_train, y_train = ...  # Load your training data
     await client.federated_learning(uri, x_train, y_train)
     # Optionally receive data from central server
     data = await client.receive_data()
     print(f"Received data: {data}")
 
 asyncio.run(main())
+
 Using Decorators
-python
-Copy code
+
+
+
 import asyncio
 import tensorflow as tf
 from federated_learning_framework.decorators import federated_learning_decorator, encryption_decorator
 from federated_learning_framework.client_device import ClientDevice
 from federated_learning_framework.encryption import create_context
 
 # Create context for encryption
@@ -163,17 +163,16 @@
     x_train, y_train = ...  # Load your training data
     await client.federated_learning('ws://localhost:8089', x_train, y_train)
 
 asyncio.run(main())
 Running Tests
 To run the tests, execute the following command in the root directory:
 
-bash
-Copy code
 python -m unittest discover -s tests
+
 License
 The usage of this library is free for academic work with proper referencing. For business, governmental, and any other types of usage, please contact me directly. All rights are reserved.
 
 Contact: mehrdaddjavadi@gmail.com
 
 Contributing
 Feel free to contribute by submitting a pull request or opening an issue.
```

### Comparing `federated_learning_framework-0.0.2/federated_learning_framework/central_server.py` & `federated_learning_framework-0.0.3/federated_learning_framework/central_server.py`

 * *Files identical despite different names*

### Comparing `federated_learning_framework-0.0.2/federated_learning_framework/client_device.py` & `federated_learning_framework-0.0.3/federated_learning_framework/client_device.py`

 * *Files identical despite different names*

### Comparing `federated_learning_framework-0.0.2/federated_learning_framework/connection.py` & `federated_learning_framework-0.0.3/federated_learning_framework/connection.py`

 * *Files identical despite different names*

### Comparing `federated_learning_framework-0.0.2/federated_learning_framework/decorators.py` & `federated_learning_framework-0.0.3/federated_learning_framework/decorators.py`

 * *Files identical despite different names*

### Comparing `federated_learning_framework-0.0.2/federated_learning_framework/encryption.py` & `federated_learning_framework-0.0.3/federated_learning_framework/encryption.py`

 * *Files identical despite different names*

### Comparing `federated_learning_framework-0.0.2/federated_learning_framework.egg-info/PKG-INFO` & `federated_learning_framework-0.0.3/federated_learning_framework.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: federated-learning-framework
-Version: 0.0.2
+Version: 0.0.3
 Summary: A modular and extensible framework for federated learning applications.
 Home-page: https://github.com/mehrdaddjavadi/federated_learning_framework
 Author: Mehrdad Javadi
 Author-email: mehrdaddjavadi@gmail.com
 Keywords: federated learning,machine learning,deep learning,encryption
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -107,42 +107,40 @@
 File: utils.py
 
 Includes utility functions used throughout the framework.
 
 Installation
 Clone the repository:
 
-bash
-Copy code
+
 git clone https://github.com/mehrdaddjavadi/federated_learning_framework.git
 Navigate to the directory:
 
-bash
-Copy code
+
 cd federated_learning_framework
 Install the dependencies:
 
-bash
-Copy code
+
 pip install -r requirements.txt
+
 Usage
+
 Setting Up the Central Server
-python
-Copy code
+
 import asyncio
 from federated_learning_framework.central_server import CentralServer
 
 async def main():
     server = CentralServer()
     await server.run_server()
 
 asyncio.run(main())
 Setting Up a Client Device
-python
-Copy code
+
+
 import asyncio
 import tensorflow as tf
 from federated_learning_framework.client_device import ClientDevice
 from federated_learning_framework.encryption import create_context
 
 # Define your model
 model = tf.keras.Sequential([
@@ -162,17 +160,19 @@
     x_train, y_train = ...  # Load your training data
     await client.federated_learning(uri, x_train, y_train)
     # Optionally receive data from central server
     data = await client.receive_data()
     print(f"Received data: {data}")
 
 asyncio.run(main())
+
 Using Decorators
-python
-Copy code
+
+
+
 import asyncio
 import tensorflow as tf
 from federated_learning_framework.decorators import federated_learning_decorator, encryption_decorator
 from federated_learning_framework.client_device import ClientDevice
 from federated_learning_framework.encryption import create_context
 
 # Create context for encryption
@@ -192,17 +192,16 @@
     x_train, y_train = ...  # Load your training data
     await client.federated_learning('ws://localhost:8089', x_train, y_train)
 
 asyncio.run(main())
 Running Tests
 To run the tests, execute the following command in the root directory:
 
-bash
-Copy code
 python -m unittest discover -s tests
+
 License
 The usage of this library is free for academic work with proper referencing. For business, governmental, and any other types of usage, please contact me directly. All rights are reserved.
 
 Contact: mehrdaddjavadi@gmail.com
 
 Contributing
 Feel free to contribute by submitting a pull request or opening an issue.
```

### Comparing `federated_learning_framework-0.0.2/federated_learning_framework.egg-info/SOURCES.txt` & `federated_learning_framework-0.0.3/federated_learning_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `federated_learning_framework-0.0.2/setup.py` & `federated_learning_framework-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='federated-learning-framework',
-    version='0.0.2',
+    version='0.0.3',
     description='A modular and extensible framework for federated learning applications.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Mehrdad Javadi',
     author_email='mehrdaddjavadi@gmail.com',
     url='https://github.com/mehrdaddjavadi/federated_learning_framework',
     packages=find_packages(),
```

### Comparing `federated_learning_framework-0.0.2/tests/test_active_learning.py` & `federated_learning_framework-0.0.3/tests/test_active_learning.py`

 * *Files identical despite different names*

### Comparing `federated_learning_framework-0.0.2/tests/test_central_server.py` & `federated_learning_framework-0.0.3/tests/test_central_server.py`

 * *Files identical despite different names*

### Comparing `federated_learning_framework-0.0.2/tests/test_client_device.py` & `federated_learning_framework-0.0.3/tests/test_client_device.py`

 * *Files identical despite different names*

### Comparing `federated_learning_framework-0.0.2/tests/test_connection.py` & `federated_learning_framework-0.0.3/tests/test_connection.py`

 * *Files identical despite different names*

