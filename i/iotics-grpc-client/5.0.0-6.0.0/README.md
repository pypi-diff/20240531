# Comparing `tmp/iotics-grpc-client-5.0.0.tar.gz` & `tmp/iotics-grpc-client-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotics-grpc-client-5.0.0.tar", last modified: Fri Jan 26 11:56:31 2024, max compression
+gzip compressed data, was "iotics-grpc-client-6.0.0.tar", last modified: Fri May 31 09:35:34 2024, max compression
```

## Comparing `iotics-grpc-client-5.0.0.tar` & `iotics-grpc-client-6.0.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 11:56:31.130881 iotics-grpc-client-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-01-26 11:56:31.130881 iotics-grpc-client-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5356 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-01-26 11:56:31.130881 iotics-grpc-client-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 11:56:31.126881 iotics-grpc-client-5.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 11:56:31.126881 iotics-grpc-client-5.0.0/src/iotics/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 11:56:31.126881 iotics-grpc-client-5.0.0/src/iotics/api/
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10196 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/feed_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    13736 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/feed_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/host_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/host_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/input_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     9814 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/input_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/interest_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     6606 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/interest_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/meta_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/meta_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/search_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/search_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/twin_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11375 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/api/twin_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 11:56:31.126881 iotics-grpc-client-5.0.0/src/iotics/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 11:56:31.130881 iotics-grpc-client-5.0.0/src/iotics/lib/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/lib/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/lib/grpc/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/lib/grpc/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/lib/grpc/feeds.py
--rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/lib/grpc/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/lib/grpc/host.py
--rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/lib/grpc/input.py
--rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/lib/grpc/interest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/lib/grpc/iotics_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/lib/grpc/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/lib/grpc/sparql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-01-26 11:56:27.000000 iotics-grpc-client-5.0.0/src/iotics/lib/grpc/twins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 11:56:31.130881 iotics-grpc-client-5.0.0/src/iotics_grpc_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7116 2024-01-26 11:56:30.000000 iotics-grpc-client-5.0.0/src/iotics_grpc_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-01-26 11:56:31.000000 iotics-grpc-client-5.0.0/src/iotics_grpc_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 11:56:30.000000 iotics-grpc-client-5.0.0/src/iotics_grpc_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-01-26 11:56:30.000000 iotics-grpc-client-5.0.0/src/iotics_grpc_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-26 11:56:30.000000 iotics-grpc-client-5.0.0/src/iotics_grpc_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 11:56:30.000000 iotics-grpc-client-5.0.0/src/iotics_grpc_client.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:34.813371 iotics-grpc-client-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-05-31 09:35:34.813371 iotics-grpc-client-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-31 09:35:34.817371 iotics-grpc-client-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:34.809371 iotics-grpc-client-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:34.809371 iotics-grpc-client-6.0.0/src/iotics/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:34.813371 iotics-grpc-client-6.0.0/src/iotics/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10992 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/feed_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15004 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/feed_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/host_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/host_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9781 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/input_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10745 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/input_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/interest_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7202 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/interest_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/meta_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/meta_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7103 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/search_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9341 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/search_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11235 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/twin_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/api/twin_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:34.813371 iotics-grpc-client-6.0.0/src/iotics/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:34.813371 iotics-grpc-client-6.0.0/src/iotics/lib/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/lib/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/lib/grpc/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/lib/grpc/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/lib/grpc/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6576 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/lib/grpc/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/lib/grpc/host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7262 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/lib/grpc/input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7256 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/lib/grpc/interest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/lib/grpc/iotics_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/lib/grpc/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/lib/grpc/sparql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7565 2024-05-31 09:35:29.000000 iotics-grpc-client-6.0.0/src/iotics/lib/grpc/twins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:35:34.813371 iotics-grpc-client-6.0.0/src/iotics_grpc_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6679 2024-05-31 09:35:34.000000 iotics-grpc-client-6.0.0/src/iotics_grpc_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-31 09:35:34.000000 iotics-grpc-client-6.0.0/src/iotics_grpc_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 09:35:34.000000 iotics-grpc-client-6.0.0/src/iotics_grpc_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-31 09:35:34.000000 iotics-grpc-client-6.0.0/src/iotics_grpc_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 09:35:34.000000 iotics-grpc-client-6.0.0/src/iotics_grpc_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 09:35:34.000000 iotics-grpc-client-6.0.0/src/iotics_grpc_client.egg-info/zip-safe
```

### Comparing `iotics-grpc-client-5.0.0/LICENSE` & `iotics-grpc-client-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-5.0.0/PKG-INFO` & `iotics-grpc-client-6.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,129 +1,129 @@
 Metadata-Version: 2.1
 Name: iotics-grpc-client
-Version: 5.0.0
+Version: 6.0.0
 Summary: Iotics gRPC client library
 Home-page: https://github.com/Iotic-Labs/iotics-grpc-client-py
 Author: Iotics
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Iotic-Labs/iotics-grpc-client-py/issues
 Project-URL: Changelog, https://github.com/Iotic-Labs/iotics-grpc-client-py/releases
 Description: # Iotics gRPC Python Client
-        A Python library for interacting with Iotics API.
         
+        A Python library for interacting with Iotics API.
         
-        ## Usage and Version Compatibility with Iotics host:
+        ## Usage and Version Compatibility with Iotics host
         
         | iotics-grpc-client-py | iotics-host |
         |----------------------| ----------- |
+        |      `pip install iotics-grpc-client~=6.0`       | `>= 7`       |
         |      `pip install iotics-grpc-client~=5.0`       | `>= 6`       |
         |      `pip install iotics-grpc-client~=4.0`       | `>= 6`       |
         |      `pip install iotics-grpc-client~=3.0`       | `>= 6`       |
         |      `pip install iotics-grpc-client~=2.0`       | `>= 5`       |
-        |      `pip install iotics-grpc-client~=0.10.0`      | `>= 4`     |
+        |      `pip install iotics-grpc-client~=0.10.0`    | `>= 4`       |
         
+        ## Examples
         
+        ### Configuring identity
         
-        # Examples
-        ## Configuring identity
         To run examples, either set up required environment variables or create an `.env` file with the following values. For
-        more information on the meaning of these values and how to create them, consult https://docs.iotics.com/docs/identity-api-and-credentials
+        more information on the meaning of these values and how to create them, consult [identity-api-and-credentials](https://docs.iotics.com/docs/identity-api-and-credentials)
+        
         * __Required__:
           * `SPACE` - Domain name of the IOTICSpace with which to communicate. The scheme can be omitted, eg. examplecorp.
             iotics.space
           * `USER_DID` - Identity of the user
           * `AGENT_DID` - Identity of the agent authorised to operate on the user's behalf
           * `AGENT_KEY_NAME` - __secret__ value used to (re)create multiple key pairs
           * `AGENT_NAME` - registered identity name that can be used to e.g. identify public keys
           * `AGENT_SECRET` - __secret__ value, the agent's private key
         
         * __Optional__:
-          * `DID_RESOLVER_URL` - Where the database of identity documents is accessible, defaults to the one used by the given 
+          * `DID_RESOLVER_URL` - Where the database of identity documents is accessible, defaults to the one used by the given
             space.
           * `TOKEN_TTL` - How long in seconds auth tokens will last if not specified in the method call, defaults to 30
-        ## Running example scripts
-        Next, create and activate your virtual environment and run any of the scripts in the [examples](https://github.com/Iotic-Labs/iotics-grpc-client-py/tree/main/examples) directory, 
+        
+        ### Running example scripts
+        
+        Next, create and activate your virtual environment and run any of the scripts in the [examples](https://github.com/Iotic-Labs/iotics-grpc-client-py/tree/main/examples) directory,
         e.g.:
-        ```bash
+        
+        ```shell
         make deps-py
         . env/bin/activate
         python examples/search_twin_models.py
         ```
         
+        ## FAQs
         
-        # FAQs
-        
-        ## Installing on Raspberry PI get: Import error GLIBC_2.33 not found
+        ### Installing on Raspberry PI get: Import error GLIBC_2.33 not found
         
         If you see this error running the exmaples on a Rapberry PI, the current workaround is to install Ubuntu for RPi which has a later version of glibc.
         
-        ```bash
+        ```shell
         ImportError: /lib/arm-linux-gnueabihf/libc.so.6: version 'GLIBC_2.33' not found (required by /home/pi/work/starting/iotics-grpc-client-py/env/lib/python3.9/site-packages/grpc/_cython/cygrpc.cpython-39-arm-linux-gnueabihf.so)
         ```
         
+        ## Contributing
         
+        ### Installing dependencies and generating gRPC client
         
-        # Contributing
-        
+        * To satisfy all dependencies, lint proto files and regenerate client files:
         
-        ## Installing dependencies and generating gRPC client
-        * To satisfy all dependencies, lint proto files and regenerate client files (inside a Docker container):
           ```shell
           make build
           ```
-          * To generate gRPC Python files outside a Docker container the following command can be used: `make generate`.
-            Currently, there is no official binary for Python gRPC plugin, but there is one built from the official repository
-            inside the docker (the following will work on Linux machines):
-            ```bash
-            docker run --rm -dit --name iotics-grpc-client-py-builder iotics-grpc-client-py-builder /bin/bash
-            docker cp iotics-grpc-client-py-builder:/bin/protoc-gen-python_grpc env/bin/protoc-gen-python_grpc
-            docker stop iotics-grpc-client-py-builder
-            make generate
-            ```
-        * To update the Iotics API version and regenerate client  
+        
+        * To generate gRPC Python files:
+        
+          ```shell
+          make generate
+          ```
+        
+        * To update the Iotics API version and regenerate client
           (proto files are submoduled in [./iotics-api.git/](./iotics-api.git)
           from [Iotics API](https://github.com/Iotic-Labs/api) repo):
-          ```bash
+        
+          ```shell
           _ver=vX.X.X
           make GIT_TAG=$_ver deps-proto-update build
           # Address usages of the new client in `src`, update "Unreleased" section in CHANGELOG.md, then:
           git add CHANGELOG.md iotics-api.git src
           git commit -m "Update Iotics API to $_ver"
           # Push your branch and create a PR
           ```
+        
         * Other `make` commands:
           * `clean` - remove artifacts created inside the project.
           * `deps-*` - install specific requirements if missing.
           * `deps-*-update` - update specific requirements when applicable.
         
+        ### PRs
         
-        ## PRs
         Should contain a summary of the changes in [CHANGELOG.md](https://github.com/Iotic-Labs/iotics-grpc-client-py/blob/main/CHANGELOG.md) under the "Unreleased" section.
         
-        
-        ## Versioning
+        ### Versioning
         
         This package adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)
         
+        ### Releasing
         
-        ## Releasing
         * Update package version in [setup.cfg](./setup.cfg) for the release:
         * Update [CHANGELOG.md](./CHANGELOG.md) (move notes from unreleased section, ensure right tags are used, etc.)
           and any other files as needed.
         * Commit changes and create a [PR](https://github.com/Iotic-Labs/iotics-grpc-client-py/compare).
         * Once PR is merged manually run the [Create Draft Release GitHub Action](https://github.com/Iotic-Labs/iotics-grpc-client-py/actions/workflows/draft_release.yml), this will create a tag with the version in setup.py and create a draft release in [releases](https://github.com/Iotic-Labs/iotics-grpc-client-py/releases).
         * Update the release's information and press the publish button on the release to publish it.
         * The [Publish GitHub Action](https://github.com/Iotic-Labs/iotics-grpc-client-ts/actions/workflows/publish.yml)
           will create a package and will publish it to [PyPI](https://pypi.org/project/iotics-grpc-client).
         
+        ## License
         
-        # License
-        
-        Copyright © 2022 IOTIC LABS LTD. info@iotics.com. All rights reserved. Licensed under the Apache License, Version 2.0. See [LICENSE](https://github.com/Iotic-Labs/iotics-grpc-client-py/tree/main/LICENSE) in the project root for license information.
-        
+        Copyright © 2024 IOTIC LABS LTD. info@iotics.com. All rights reserved. Licensed under the Apache License, Version 2.0. See [LICENSE](https://github.com/Iotic-Labs/iotics-grpc-client-py/tree/main/LICENSE) in the project root for license information.
         
 Keywords: iotics,grpc,digital twin
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `iotics-grpc-client-5.0.0/README.md` & `iotics-grpc-client-6.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,113 +1,113 @@
 # Iotics gRPC Python Client
-A Python library for interacting with Iotics API.
 
+A Python library for interacting with Iotics API.
 
-## Usage and Version Compatibility with Iotics host:
+## Usage and Version Compatibility with Iotics host
 
 | iotics-grpc-client-py | iotics-host |
 |----------------------| ----------- |
+|      `pip install iotics-grpc-client~=6.0`       | `>= 7`       |
 |      `pip install iotics-grpc-client~=5.0`       | `>= 6`       |
 |      `pip install iotics-grpc-client~=4.0`       | `>= 6`       |
 |      `pip install iotics-grpc-client~=3.0`       | `>= 6`       |
 |      `pip install iotics-grpc-client~=2.0`       | `>= 5`       |
-|      `pip install iotics-grpc-client~=0.10.0`      | `>= 4`     |
+|      `pip install iotics-grpc-client~=0.10.0`    | `>= 4`       |
 
+## Examples
 
+### Configuring identity
 
-# Examples
-## Configuring identity
 To run examples, either set up required environment variables or create an `.env` file with the following values. For
-more information on the meaning of these values and how to create them, consult https://docs.iotics.com/docs/identity-api-and-credentials
+more information on the meaning of these values and how to create them, consult [identity-api-and-credentials](https://docs.iotics.com/docs/identity-api-and-credentials)
+
 * __Required__:
   * `SPACE` - Domain name of the IOTICSpace with which to communicate. The scheme can be omitted, eg. examplecorp.
     iotics.space
   * `USER_DID` - Identity of the user
   * `AGENT_DID` - Identity of the agent authorised to operate on the user's behalf
   * `AGENT_KEY_NAME` - __secret__ value used to (re)create multiple key pairs
   * `AGENT_NAME` - registered identity name that can be used to e.g. identify public keys
   * `AGENT_SECRET` - __secret__ value, the agent's private key
 
 * __Optional__:
-  * `DID_RESOLVER_URL` - Where the database of identity documents is accessible, defaults to the one used by the given 
+  * `DID_RESOLVER_URL` - Where the database of identity documents is accessible, defaults to the one used by the given
     space.
   * `TOKEN_TTL` - How long in seconds auth tokens will last if not specified in the method call, defaults to 30
-## Running example scripts
-Next, create and activate your virtual environment and run any of the scripts in the [examples](https://github.com/Iotic-Labs/iotics-grpc-client-py/tree/main/examples) directory, 
+
+### Running example scripts
+
+Next, create and activate your virtual environment and run any of the scripts in the [examples](https://github.com/Iotic-Labs/iotics-grpc-client-py/tree/main/examples) directory,
 e.g.:
-```bash
+
+```shell
 make deps-py
 . env/bin/activate
 python examples/search_twin_models.py
 ```
 
+## FAQs
 
-# FAQs
-
-## Installing on Raspberry PI get: Import error GLIBC_2.33 not found
+### Installing on Raspberry PI get: Import error GLIBC_2.33 not found
 
 If you see this error running the exmaples on a Rapberry PI, the current workaround is to install Ubuntu for RPi which has a later version of glibc.
 
-```bash
+```shell
 ImportError: /lib/arm-linux-gnueabihf/libc.so.6: version 'GLIBC_2.33' not found (required by /home/pi/work/starting/iotics-grpc-client-py/env/lib/python3.9/site-packages/grpc/_cython/cygrpc.cpython-39-arm-linux-gnueabihf.so)
 ```
 
+## Contributing
 
+### Installing dependencies and generating gRPC client
 
-# Contributing
-
+* To satisfy all dependencies, lint proto files and regenerate client files:
 
-## Installing dependencies and generating gRPC client
-* To satisfy all dependencies, lint proto files and regenerate client files (inside a Docker container):
   ```shell
   make build
   ```
-  * To generate gRPC Python files outside a Docker container the following command can be used: `make generate`.
-    Currently, there is no official binary for Python gRPC plugin, but there is one built from the official repository
-    inside the docker (the following will work on Linux machines):
-    ```bash
-    docker run --rm -dit --name iotics-grpc-client-py-builder iotics-grpc-client-py-builder /bin/bash
-    docker cp iotics-grpc-client-py-builder:/bin/protoc-gen-python_grpc env/bin/protoc-gen-python_grpc
-    docker stop iotics-grpc-client-py-builder
-    make generate
-    ```
-* To update the Iotics API version and regenerate client  
+
+* To generate gRPC Python files:
+
+  ```shell
+  make generate
+  ```
+
+* To update the Iotics API version and regenerate client
   (proto files are submoduled in [./iotics-api.git/](./iotics-api.git)
   from [Iotics API](https://github.com/Iotic-Labs/api) repo):
-  ```bash
+
+  ```shell
   _ver=vX.X.X
   make GIT_TAG=$_ver deps-proto-update build
   # Address usages of the new client in `src`, update "Unreleased" section in CHANGELOG.md, then:
   git add CHANGELOG.md iotics-api.git src
   git commit -m "Update Iotics API to $_ver"
   # Push your branch and create a PR
   ```
+
 * Other `make` commands:
   * `clean` - remove artifacts created inside the project.
   * `deps-*` - install specific requirements if missing.
   * `deps-*-update` - update specific requirements when applicable.
 
+### PRs
 
-## PRs
 Should contain a summary of the changes in [CHANGELOG.md](https://github.com/Iotic-Labs/iotics-grpc-client-py/blob/main/CHANGELOG.md) under the "Unreleased" section.
 
-
-## Versioning
+### Versioning
 
 This package adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)
 
+### Releasing
 
-## Releasing
 * Update package version in [setup.cfg](./setup.cfg) for the release:
 * Update [CHANGELOG.md](./CHANGELOG.md) (move notes from unreleased section, ensure right tags are used, etc.)
   and any other files as needed.
 * Commit changes and create a [PR](https://github.com/Iotic-Labs/iotics-grpc-client-py/compare).
 * Once PR is merged manually run the [Create Draft Release GitHub Action](https://github.com/Iotic-Labs/iotics-grpc-client-py/actions/workflows/draft_release.yml), this will create a tag with the version in setup.py and create a draft release in [releases](https://github.com/Iotic-Labs/iotics-grpc-client-py/releases).
 * Update the release's information and press the publish button on the release to publish it.
 * The [Publish GitHub Action](https://github.com/Iotic-Labs/iotics-grpc-client-ts/actions/workflows/publish.yml)
   will create a package and will publish it to [PyPI](https://pypi.org/project/iotics-grpc-client).
 
+## License
 
-# License
-
-Copyright © 2022 IOTIC LABS LTD. info@iotics.com. All rights reserved. Licensed under the Apache License, Version 2.0. See [LICENSE](https://github.com/Iotic-Labs/iotics-grpc-client-py/tree/main/LICENSE) in the project root for license information.
-
+Copyright © 2024 IOTIC LABS LTD. info@iotics.com. All rights reserved. Licensed under the Apache License, Version 2.0. See [LICENSE](https://github.com/Iotic-Labs/iotics-grpc-client-py/tree/main/LICENSE) in the project root for license information.
```

### Comparing `iotics-grpc-client-5.0.0/setup.cfg` & `iotics-grpc-client-6.0.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iotics-grpc-client
-version = 5.0.0
+version = 6.0.0
 description = Iotics gRPC client library
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Iotics
 platform = any
 url = https://github.com/Iotic-Labs/iotics-grpc-client-py
 keywords = iotics, grpc, digital twin
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/__init__.py` & `iotics-grpc-client-6.0.0/src/iotics/__init__.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-5.0.0/src/iotics/api/common_pb2.py` & `iotics-grpc-client-6.0.0/src/iotics/api/common_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,68 +1,69 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: iotics/api/common.proto
+# Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17iotics/api/common.proto\x12\niotics.api\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x1d\n\x05Limit\x12\x14\n\x05value\x18\x01 \x01(\rR\x05value\"\x1e\n\x06Offset\x12\x14\n\x05value\x18\x01 \x01(\rR\x05value\"\\\n\x05Range\x12\'\n\x05limit\x18\x01 \x01(\x0b\x32\x11.iotics.api.LimitR\x05limit\x12*\n\x06offset\x18\x02 \x01(\x0b\x32\x12.iotics.api.OffsetR\x06offset\"7\n\x0bLangLiteral\x12\x12\n\x04lang\x18\x01 \x01(\tR\x04lang\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"%\n\rStringLiteral\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\";\n\x07Literal\x12\x1a\n\x08\x64\x61taType\x18\x01 \x01(\tR\x08\x64\x61taType\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value\"\x1b\n\x03Uri\x12\x14\n\x05value\x18\x01 \x01(\tR\x05value\"\xa3\x02\n\x08Property\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x39\n\x0cliteralValue\x18\x02 \x01(\x0b\x32\x13.iotics.api.LiteralH\x00R\x0cliteralValue\x12\x45\n\x10langLiteralValue\x18\x03 \x01(\x0b\x32\x17.iotics.api.LangLiteralH\x00R\x10langLiteralValue\x12K\n\x12stringLiteralValue\x18\x04 \x01(\x0b\x32\x19.iotics.api.StringLiteralH\x00R\x12stringLiteralValue\x12-\n\x08uriValue\x18\x05 \x01(\x0b\x32\x0f.iotics.api.UriH\x00R\x08uriValueB\x07\n\x05value\"1\n\x0bGeoLocation\x12\x10\n\x03lat\x18\x01 \x01(\x01R\x03lat\x12\x10\n\x03lon\x18\x02 \x01(\x01R\x03lon\"\\\n\tGeoCircle\x12\x33\n\x08location\x18\x01 \x01(\x0b\x32\x17.iotics.api.GeoLocationR\x08location\x12\x1a\n\x08radiusKm\x18\x02 \x01(\x01R\x08radiusKm\"\xc7\x01\n\x0bRequestInfo\x12\x38\n\tstartTime\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12\x41\n\x08traceCtx\x18\x02 \x03(\x0b\x32%.iotics.api.RequestInfo.TraceCtxEntryR\x08traceCtx\x1a;\n\rTraceCtxEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xb4\x02\n\x07Headers\x12\x1c\n\tclientRef\x18\x01 \x01(\tR\tclientRef\x12 \n\x0b\x63lientAppId\x18\x02 \x01(\tR\x0b\x63lientAppId\x12&\n\x0etransactionRef\x18\x03 \x03(\tR\x0etransactionRef\x12\x42\n\rconsumerGroup\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\rconsumerGroup\x12\x42\n\x0erequestTimeout\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0erequestTimeout\x12\x39\n\x0brequestInfo\x18\x06 \x01(\x0b\x32\x17.iotics.api.RequestInfoR\x0brequestInfo\"\xa3\x01\n\x13SubscriptionHeaders\x12 \n\x0b\x63lientAppId\x18\x01 \x01(\tR\x0b\x63lientAppId\x12&\n\x0etransactionRef\x18\x02 \x03(\tR\x0etransactionRef\x12\x42\n\rconsumerGroup\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValueR\rconsumerGroup\"0\n\x06TwinID\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x16\n\x06hostId\x18\x02 \x01(\tR\x06hostId\"g\n\x05Value\x12\x14\n\x05label\x18\x01 \x01(\tR\x05label\x12\x18\n\x07\x63omment\x18\x02 \x01(\tR\x07\x63omment\x12\x12\n\x04unit\x18\x03 \x01(\tR\x04unit\x12\x1a\n\x08\x64\x61taType\x18\x04 \x01(\tR\x08\x64\x61taType\"Y\n\x06Values\x12\'\n\x05\x61\x64\x64\x65\x64\x18\x01 \x03(\x0b\x32\x11.iotics.api.ValueR\x05\x61\x64\x64\x65\x64\x12&\n\x0e\x64\x65letedByLabel\x18\x02 \x03(\tR\x0e\x64\x65letedByLabel\"n\n\x08\x46\x65\x65\x64\x44\x61ta\x12:\n\noccurredAt\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\noccurredAt\x12\x12\n\x04mime\x18\x03 \x01(\tR\x04mime\x12\x12\n\x04\x64\x61ta\x18\x04 \x01(\x0cR\x04\x64\x61ta\"\xb0\x01\n\x0ePropertyUpdate\x12\x1e\n\nclearedAll\x18\x01 \x01(\x08R\nclearedAll\x12.\n\x07\x64\x65leted\x18\x02 \x03(\x0b\x32\x14.iotics.api.PropertyR\x07\x64\x65leted\x12\"\n\x0c\x64\x65letedByKey\x18\x03 \x03(\tR\x0c\x64\x65letedByKey\x12*\n\x05\x61\x64\x64\x65\x64\x18\x04 \x03(\x0b\x32\x14.iotics.api.PropertyR\x05\x61\x64\x64\x65\x64*\x1e\n\x05Scope\x12\n\n\x06GLOBAL\x10\x00\x12\t\n\x05LOCAL\x10\x01\x42\x7f\n\x0e\x63om.iotics.apiB\x0b\x43ommonProtoP\x01Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\xa2\x02\x03IAX\xaa\x02\nIotics.Api\xca\x02\nIotics\\Apib\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iotics.api.common_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iotics.api.common_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.iotics.apiB\013CommonProtoP\001Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\242\002\003IAX\252\002\nIotics.Api\312\002\nIotics\\Api'
-  _REQUESTINFO_TRACECTXENTRY._options = None
-  _REQUESTINFO_TRACECTXENTRY._serialized_options = b'8\001'
-  _SCOPE._serialized_start=2102
-  _SCOPE._serialized_end=2132
-  _LIMIT._serialized_start=104
-  _LIMIT._serialized_end=133
-  _OFFSET._serialized_start=135
-  _OFFSET._serialized_end=165
-  _RANGE._serialized_start=167
-  _RANGE._serialized_end=259
-  _LANGLITERAL._serialized_start=261
-  _LANGLITERAL._serialized_end=316
-  _STRINGLITERAL._serialized_start=318
-  _STRINGLITERAL._serialized_end=355
-  _LITERAL._serialized_start=357
-  _LITERAL._serialized_end=416
-  _URI._serialized_start=418
-  _URI._serialized_end=445
-  _PROPERTY._serialized_start=448
-  _PROPERTY._serialized_end=739
-  _GEOLOCATION._serialized_start=741
-  _GEOLOCATION._serialized_end=790
-  _GEOCIRCLE._serialized_start=792
-  _GEOCIRCLE._serialized_end=884
-  _REQUESTINFO._serialized_start=887
-  _REQUESTINFO._serialized_end=1086
-  _REQUESTINFO_TRACECTXENTRY._serialized_start=1027
-  _REQUESTINFO_TRACECTXENTRY._serialized_end=1086
-  _HEADERS._serialized_start=1089
-  _HEADERS._serialized_end=1397
-  _SUBSCRIPTIONHEADERS._serialized_start=1400
-  _SUBSCRIPTIONHEADERS._serialized_end=1563
-  _TWINID._serialized_start=1565
-  _TWINID._serialized_end=1613
-  _VALUE._serialized_start=1615
-  _VALUE._serialized_end=1718
-  _VALUES._serialized_start=1720
-  _VALUES._serialized_end=1809
-  _FEEDDATA._serialized_start=1811
-  _FEEDDATA._serialized_end=1921
-  _PROPERTYUPDATE._serialized_start=1924
-  _PROPERTYUPDATE._serialized_end=2100
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\016com.iotics.apiB\013CommonProtoP\001Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\242\002\003IAX\252\002\nIotics.Api\312\002\nIotics\\Api'
+  _globals['_REQUESTINFO_TRACECTXENTRY']._options = None
+  _globals['_REQUESTINFO_TRACECTXENTRY']._serialized_options = b'8\001'
+  _globals['_SCOPE']._serialized_start=2102
+  _globals['_SCOPE']._serialized_end=2132
+  _globals['_LIMIT']._serialized_start=104
+  _globals['_LIMIT']._serialized_end=133
+  _globals['_OFFSET']._serialized_start=135
+  _globals['_OFFSET']._serialized_end=165
+  _globals['_RANGE']._serialized_start=167
+  _globals['_RANGE']._serialized_end=259
+  _globals['_LANGLITERAL']._serialized_start=261
+  _globals['_LANGLITERAL']._serialized_end=316
+  _globals['_STRINGLITERAL']._serialized_start=318
+  _globals['_STRINGLITERAL']._serialized_end=355
+  _globals['_LITERAL']._serialized_start=357
+  _globals['_LITERAL']._serialized_end=416
+  _globals['_URI']._serialized_start=418
+  _globals['_URI']._serialized_end=445
+  _globals['_PROPERTY']._serialized_start=448
+  _globals['_PROPERTY']._serialized_end=739
+  _globals['_GEOLOCATION']._serialized_start=741
+  _globals['_GEOLOCATION']._serialized_end=790
+  _globals['_GEOCIRCLE']._serialized_start=792
+  _globals['_GEOCIRCLE']._serialized_end=884
+  _globals['_REQUESTINFO']._serialized_start=887
+  _globals['_REQUESTINFO']._serialized_end=1086
+  _globals['_REQUESTINFO_TRACECTXENTRY']._serialized_start=1027
+  _globals['_REQUESTINFO_TRACECTXENTRY']._serialized_end=1086
+  _globals['_HEADERS']._serialized_start=1089
+  _globals['_HEADERS']._serialized_end=1397
+  _globals['_SUBSCRIPTIONHEADERS']._serialized_start=1400
+  _globals['_SUBSCRIPTIONHEADERS']._serialized_end=1563
+  _globals['_TWINID']._serialized_start=1565
+  _globals['_TWINID']._serialized_end=1613
+  _globals['_VALUE']._serialized_start=1615
+  _globals['_VALUE']._serialized_end=1718
+  _globals['_VALUES']._serialized_start=1720
+  _globals['_VALUES']._serialized_end=1809
+  _globals['_FEEDDATA']._serialized_start=1811
+  _globals['_FEEDDATA']._serialized_end=1921
+  _globals['_PROPERTYUPDATE']._serialized_start=1924
+  _globals['_PROPERTYUPDATE']._serialized_end=2100
 # @@protoc_insertion_point(module_scope)
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/api/feed_pb2.py` & `iotics-grpc-client-6.0.0/src/iotics/api/feed_pb2.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,87 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: iotics/api/feed.proto
+# Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from iotics.api import common_pb2 as iotics_dot_api_dot_common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15iotics/api/feed.proto\x12\niotics.api\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x17iotics/api/common.proto\"H\n\x06\x46\x65\x65\x64ID\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x16\n\x06twinId\x18\x02 \x01(\tR\x06twinId\x12\x16\n\x06hostId\x18\x03 \x01(\tR\x06hostId\"\x94\x02\n\x11\x43reateFeedRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12;\n\x04\x61rgs\x18\x02 \x01(\x0b\x32\'.iotics.api.CreateFeedRequest.ArgumentsR\x04\x61rgs\x12?\n\x07payload\x18\x03 \x01(\x0b\x32%.iotics.api.CreateFeedRequest.PayloadR\x07payload\x1a\x19\n\x07Payload\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x1a\x37\n\tArguments\x12*\n\x06twinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x06twinId\"\xbc\x01\n\x12\x43reateFeedResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12@\n\x07payload\x18\x02 \x01(\x0b\x32&.iotics.api.CreateFeedResponse.PayloadR\x07payload\x1a\x35\n\x07Payload\x12*\n\x06\x66\x65\x65\x64Id\x18\x01 \x01(\x0b\x32\x12.iotics.api.FeedIDR\x06\x66\x65\x65\x64Id\"\xb8\x01\n\x11\x44\x65leteFeedRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12;\n\x04\x61rgs\x18\x02 \x01(\x0b\x32\'.iotics.api.DeleteFeedRequest.ArgumentsR\x04\x61rgs\x1a\x37\n\tArguments\x12*\n\x06\x66\x65\x65\x64Id\x18\x01 \x01(\x0b\x32\x12.iotics.api.FeedIDR\x06\x66\x65\x65\x64Id\"\xbc\x01\n\x12\x44\x65leteFeedResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12@\n\x07payload\x18\x02 \x01(\x0b\x32&.iotics.api.DeleteFeedResponse.PayloadR\x07payload\x1a\x35\n\x07Payload\x12*\n\x06\x66\x65\x65\x64Id\x18\x01 \x01(\x0b\x32\x12.iotics.api.FeedIDR\x06\x66\x65\x65\x64Id\"\xa7\x03\n\x11UpdateFeedRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12;\n\x04\x61rgs\x18\x02 \x01(\x0b\x32\'.iotics.api.UpdateFeedRequest.ArgumentsR\x04\x61rgs\x12?\n\x07payload\x18\x03 \x01(\x0b\x32%.iotics.api.UpdateFeedRequest.PayloadR\x07payload\x1a\xab\x01\n\x07Payload\x12\x38\n\tstoreLast\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\tstoreLast\x12*\n\x06values\x18\x03 \x01(\x0b\x32\x12.iotics.api.ValuesR\x06values\x12:\n\nproperties\x18\x06 \x01(\x0b\x32\x1a.iotics.api.PropertyUpdateR\nproperties\x1a\x37\n\tArguments\x12*\n\x06\x66\x65\x65\x64Id\x18\x01 \x01(\x0b\x32\x12.iotics.api.FeedIDR\x06\x66\x65\x65\x64Id\"\xbc\x01\n\x12UpdateFeedResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12@\n\x07payload\x18\x02 \x01(\x0b\x32&.iotics.api.UpdateFeedResponse.PayloadR\x07payload\x1a\x35\n\x07Payload\x12*\n\x06\x66\x65\x65\x64Id\x18\x01 \x01(\x0b\x32\x12.iotics.api.FeedIDR\x06\x66\x65\x65\x64Id\"\xbb\x02\n\x14ShareFeedDataRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12>\n\x04\x61rgs\x18\x02 \x01(\x0b\x32*.iotics.api.ShareFeedDataRequest.ArgumentsR\x04\x61rgs\x12\x42\n\x07payload\x18\x03 \x01(\x0b\x32(.iotics.api.ShareFeedDataRequest.PayloadR\x07payload\x1a\x37\n\x07Payload\x12,\n\x06sample\x18\x01 \x01(\x0b\x32\x14.iotics.api.FeedDataR\x06sample\x1a\x37\n\tArguments\x12*\n\x06\x66\x65\x65\x64Id\x18\x01 \x01(\x0b\x32\x12.iotics.api.FeedIDR\x06\x66\x65\x65\x64Id\"F\n\x15ShareFeedDataResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\"\xe5\x01\n\x13ListAllFeedsRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12=\n\x04\x61rgs\x18\x02 \x01(\x0b\x32).iotics.api.ListAllFeedsRequest.ArgumentsR\x04\x61rgs\x12\'\n\x05range\x18\x03 \x01(\x0b\x32\x11.iotics.api.RangeR\x05range\x1a\x37\n\tArguments\x12*\n\x06twinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x06twinId\"\xc2\x01\n\x14ListAllFeedsResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x42\n\x07payload\x18\x02 \x01(\x0b\x32(.iotics.api.ListAllFeedsResponse.PayloadR\x07payload\x1a\x37\n\x07Payload\x12,\n\x07\x66\x65\x65\x64Ids\x18\x01 \x03(\x0b\x32\x12.iotics.api.FeedIDR\x07\x66\x65\x65\x64Ids\"\xbc\x01\n\x13\x44\x65scribeFeedRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12=\n\x04\x61rgs\x18\x03 \x01(\x0b\x32).iotics.api.DescribeFeedRequest.ArgumentsR\x04\x61rgs\x1a\x37\n\tArguments\x12*\n\x06\x66\x65\x65\x64Id\x18\x01 \x01(\x0b\x32\x12.iotics.api.FeedIDR\x06\x66\x65\x65\x64Id\"\x93\x03\n\x14\x44\x65scribeFeedResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x42\n\x07payload\x18\x02 \x01(\x0b\x32(.iotics.api.DescribeFeedResponse.PayloadR\x07payload\x1a\x8b\x01\n\nMetaResult\x12)\n\x06values\x18\x02 \x03(\x0b\x32\x11.iotics.api.ValueR\x06values\x12\x1c\n\tstoreLast\x18\x05 \x01(\x08R\tstoreLast\x12\x34\n\nproperties\x18\x06 \x03(\x0b\x32\x14.iotics.api.PropertyR\nproperties\x1az\n\x07Payload\x12*\n\x06\x66\x65\x65\x64Id\x18\x01 \x01(\x0b\x32\x12.iotics.api.FeedIDR\x06\x66\x65\x65\x64Id\x12\x43\n\x06result\x18\x02 \x01(\x0b\x32+.iotics.api.DescribeFeedResponse.MetaResultR\x06result\"\xa3\x01\n\x12UpsertFeedWithMeta\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x1c\n\tstoreLast\x18\x04 \x01(\x08R\tstoreLast\x12)\n\x06values\x18\x05 \x03(\x0b\x32\x11.iotics.api.ValueR\x06values\x12\x34\n\nproperties\x18\x06 \x03(\x0b\x32\x14.iotics.api.PropertyR\nproperties2\xd3\x04\n\x07\x46\x65\x65\x64\x41PI\x12M\n\nCreateFeed\x12\x1d.iotics.api.CreateFeedRequest\x1a\x1e.iotics.api.CreateFeedResponse\"\x00\x12M\n\nDeleteFeed\x12\x1d.iotics.api.DeleteFeedRequest\x1a\x1e.iotics.api.DeleteFeedResponse\"\x00\x12M\n\nUpdateFeed\x12\x1d.iotics.api.UpdateFeedRequest\x1a\x1e.iotics.api.UpdateFeedResponse\"\x00\x12V\n\rShareFeedData\x12 .iotics.api.ShareFeedDataRequest\x1a!.iotics.api.ShareFeedDataResponse\"\x00\x12Y\n\x0eStreamFeedData\x12 .iotics.api.ShareFeedDataRequest\x1a!.iotics.api.ShareFeedDataResponse\"\x00(\x01\x12S\n\x0cListAllFeeds\x12\x1f.iotics.api.ListAllFeedsRequest\x1a .iotics.api.ListAllFeedsResponse\"\x00\x12S\n\x0c\x44\x65scribeFeed\x12\x1f.iotics.api.DescribeFeedRequest\x1a .iotics.api.DescribeFeedResponse\"\x00\x42}\n\x0e\x63om.iotics.apiB\tFeedProtoP\x01Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\xa2\x02\x03IAX\xaa\x02\nIotics.Api\xca\x02\nIotics\\Apib\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iotics.api.feed_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iotics.api.feed_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.iotics.apiB\tFeedProtoP\001Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\242\002\003IAX\252\002\nIotics.Api\312\002\nIotics\\Api'
-  _FEEDID._serialized_start=94
-  _FEEDID._serialized_end=166
-  _CREATEFEEDREQUEST._serialized_start=169
-  _CREATEFEEDREQUEST._serialized_end=445
-  _CREATEFEEDREQUEST_PAYLOAD._serialized_start=363
-  _CREATEFEEDREQUEST_PAYLOAD._serialized_end=388
-  _CREATEFEEDREQUEST_ARGUMENTS._serialized_start=390
-  _CREATEFEEDREQUEST_ARGUMENTS._serialized_end=445
-  _CREATEFEEDRESPONSE._serialized_start=448
-  _CREATEFEEDRESPONSE._serialized_end=636
-  _CREATEFEEDRESPONSE_PAYLOAD._serialized_start=583
-  _CREATEFEEDRESPONSE_PAYLOAD._serialized_end=636
-  _DELETEFEEDREQUEST._serialized_start=639
-  _DELETEFEEDREQUEST._serialized_end=823
-  _DELETEFEEDREQUEST_ARGUMENTS._serialized_start=768
-  _DELETEFEEDREQUEST_ARGUMENTS._serialized_end=823
-  _DELETEFEEDRESPONSE._serialized_start=826
-  _DELETEFEEDRESPONSE._serialized_end=1014
-  _DELETEFEEDRESPONSE_PAYLOAD._serialized_start=583
-  _DELETEFEEDRESPONSE_PAYLOAD._serialized_end=636
-  _UPDATEFEEDREQUEST._serialized_start=1017
-  _UPDATEFEEDREQUEST._serialized_end=1440
-  _UPDATEFEEDREQUEST_PAYLOAD._serialized_start=1212
-  _UPDATEFEEDREQUEST_PAYLOAD._serialized_end=1383
-  _UPDATEFEEDREQUEST_ARGUMENTS._serialized_start=768
-  _UPDATEFEEDREQUEST_ARGUMENTS._serialized_end=823
-  _UPDATEFEEDRESPONSE._serialized_start=1443
-  _UPDATEFEEDRESPONSE._serialized_end=1631
-  _UPDATEFEEDRESPONSE_PAYLOAD._serialized_start=583
-  _UPDATEFEEDRESPONSE_PAYLOAD._serialized_end=636
-  _SHAREFEEDDATAREQUEST._serialized_start=1634
-  _SHAREFEEDDATAREQUEST._serialized_end=1949
-  _SHAREFEEDDATAREQUEST_PAYLOAD._serialized_start=1837
-  _SHAREFEEDDATAREQUEST_PAYLOAD._serialized_end=1892
-  _SHAREFEEDDATAREQUEST_ARGUMENTS._serialized_start=768
-  _SHAREFEEDDATAREQUEST_ARGUMENTS._serialized_end=823
-  _SHAREFEEDDATARESPONSE._serialized_start=1951
-  _SHAREFEEDDATARESPONSE._serialized_end=2021
-  _LISTALLFEEDSREQUEST._serialized_start=2024
-  _LISTALLFEEDSREQUEST._serialized_end=2253
-  _LISTALLFEEDSREQUEST_ARGUMENTS._serialized_start=390
-  _LISTALLFEEDSREQUEST_ARGUMENTS._serialized_end=445
-  _LISTALLFEEDSRESPONSE._serialized_start=2256
-  _LISTALLFEEDSRESPONSE._serialized_end=2450
-  _LISTALLFEEDSRESPONSE_PAYLOAD._serialized_start=2395
-  _LISTALLFEEDSRESPONSE_PAYLOAD._serialized_end=2450
-  _DESCRIBEFEEDREQUEST._serialized_start=2453
-  _DESCRIBEFEEDREQUEST._serialized_end=2641
-  _DESCRIBEFEEDREQUEST_ARGUMENTS._serialized_start=768
-  _DESCRIBEFEEDREQUEST_ARGUMENTS._serialized_end=823
-  _DESCRIBEFEEDRESPONSE._serialized_start=2644
-  _DESCRIBEFEEDRESPONSE._serialized_end=3047
-  _DESCRIBEFEEDRESPONSE_METARESULT._serialized_start=2784
-  _DESCRIBEFEEDRESPONSE_METARESULT._serialized_end=2923
-  _DESCRIBEFEEDRESPONSE_PAYLOAD._serialized_start=2925
-  _DESCRIBEFEEDRESPONSE_PAYLOAD._serialized_end=3047
-  _UPSERTFEEDWITHMETA._serialized_start=3050
-  _UPSERTFEEDWITHMETA._serialized_end=3213
-  _FEEDAPI._serialized_start=3216
-  _FEEDAPI._serialized_end=3811
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\016com.iotics.apiB\tFeedProtoP\001Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\242\002\003IAX\252\002\nIotics.Api\312\002\nIotics\\Api'
+  _globals['_FEEDID']._serialized_start=94
+  _globals['_FEEDID']._serialized_end=166
+  _globals['_CREATEFEEDREQUEST']._serialized_start=169
+  _globals['_CREATEFEEDREQUEST']._serialized_end=445
+  _globals['_CREATEFEEDREQUEST_PAYLOAD']._serialized_start=363
+  _globals['_CREATEFEEDREQUEST_PAYLOAD']._serialized_end=388
+  _globals['_CREATEFEEDREQUEST_ARGUMENTS']._serialized_start=390
+  _globals['_CREATEFEEDREQUEST_ARGUMENTS']._serialized_end=445
+  _globals['_CREATEFEEDRESPONSE']._serialized_start=448
+  _globals['_CREATEFEEDRESPONSE']._serialized_end=636
+  _globals['_CREATEFEEDRESPONSE_PAYLOAD']._serialized_start=583
+  _globals['_CREATEFEEDRESPONSE_PAYLOAD']._serialized_end=636
+  _globals['_DELETEFEEDREQUEST']._serialized_start=639
+  _globals['_DELETEFEEDREQUEST']._serialized_end=823
+  _globals['_DELETEFEEDREQUEST_ARGUMENTS']._serialized_start=768
+  _globals['_DELETEFEEDREQUEST_ARGUMENTS']._serialized_end=823
+  _globals['_DELETEFEEDRESPONSE']._serialized_start=826
+  _globals['_DELETEFEEDRESPONSE']._serialized_end=1014
+  _globals['_DELETEFEEDRESPONSE_PAYLOAD']._serialized_start=583
+  _globals['_DELETEFEEDRESPONSE_PAYLOAD']._serialized_end=636
+  _globals['_UPDATEFEEDREQUEST']._serialized_start=1017
+  _globals['_UPDATEFEEDREQUEST']._serialized_end=1440
+  _globals['_UPDATEFEEDREQUEST_PAYLOAD']._serialized_start=1212
+  _globals['_UPDATEFEEDREQUEST_PAYLOAD']._serialized_end=1383
+  _globals['_UPDATEFEEDREQUEST_ARGUMENTS']._serialized_start=768
+  _globals['_UPDATEFEEDREQUEST_ARGUMENTS']._serialized_end=823
+  _globals['_UPDATEFEEDRESPONSE']._serialized_start=1443
+  _globals['_UPDATEFEEDRESPONSE']._serialized_end=1631
+  _globals['_UPDATEFEEDRESPONSE_PAYLOAD']._serialized_start=583
+  _globals['_UPDATEFEEDRESPONSE_PAYLOAD']._serialized_end=636
+  _globals['_SHAREFEEDDATAREQUEST']._serialized_start=1634
+  _globals['_SHAREFEEDDATAREQUEST']._serialized_end=1949
+  _globals['_SHAREFEEDDATAREQUEST_PAYLOAD']._serialized_start=1837
+  _globals['_SHAREFEEDDATAREQUEST_PAYLOAD']._serialized_end=1892
+  _globals['_SHAREFEEDDATAREQUEST_ARGUMENTS']._serialized_start=768
+  _globals['_SHAREFEEDDATAREQUEST_ARGUMENTS']._serialized_end=823
+  _globals['_SHAREFEEDDATARESPONSE']._serialized_start=1951
+  _globals['_SHAREFEEDDATARESPONSE']._serialized_end=2021
+  _globals['_LISTALLFEEDSREQUEST']._serialized_start=2024
+  _globals['_LISTALLFEEDSREQUEST']._serialized_end=2253
+  _globals['_LISTALLFEEDSREQUEST_ARGUMENTS']._serialized_start=390
+  _globals['_LISTALLFEEDSREQUEST_ARGUMENTS']._serialized_end=445
+  _globals['_LISTALLFEEDSRESPONSE']._serialized_start=2256
+  _globals['_LISTALLFEEDSRESPONSE']._serialized_end=2450
+  _globals['_LISTALLFEEDSRESPONSE_PAYLOAD']._serialized_start=2395
+  _globals['_LISTALLFEEDSRESPONSE_PAYLOAD']._serialized_end=2450
+  _globals['_DESCRIBEFEEDREQUEST']._serialized_start=2453
+  _globals['_DESCRIBEFEEDREQUEST']._serialized_end=2641
+  _globals['_DESCRIBEFEEDREQUEST_ARGUMENTS']._serialized_start=768
+  _globals['_DESCRIBEFEEDREQUEST_ARGUMENTS']._serialized_end=823
+  _globals['_DESCRIBEFEEDRESPONSE']._serialized_start=2644
+  _globals['_DESCRIBEFEEDRESPONSE']._serialized_end=3047
+  _globals['_DESCRIBEFEEDRESPONSE_METARESULT']._serialized_start=2784
+  _globals['_DESCRIBEFEEDRESPONSE_METARESULT']._serialized_end=2923
+  _globals['_DESCRIBEFEEDRESPONSE_PAYLOAD']._serialized_start=2925
+  _globals['_DESCRIBEFEEDRESPONSE_PAYLOAD']._serialized_end=3047
+  _globals['_UPSERTFEEDWITHMETA']._serialized_start=3050
+  _globals['_UPSERTFEEDWITHMETA']._serialized_end=3213
+  _globals['_FEEDAPI']._serialized_start=3216
+  _globals['_FEEDAPI']._serialized_end=3811
 # @@protoc_insertion_point(module_scope)
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/api/feed_pb2_grpc.py` & `iotics-grpc-client-6.0.0/src/iotics/api/feed_pb2_grpc.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,45 +20,45 @@
         Args:
             channel: A grpc.Channel.
         """
         self.CreateFeed = channel.unary_unary(
                 '/iotics.api.FeedAPI/CreateFeed',
                 request_serializer=iotics_dot_api_dot_feed__pb2.CreateFeedRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_feed__pb2.CreateFeedResponse.FromString,
-                )
+                _registered_method=True)
         self.DeleteFeed = channel.unary_unary(
                 '/iotics.api.FeedAPI/DeleteFeed',
                 request_serializer=iotics_dot_api_dot_feed__pb2.DeleteFeedRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_feed__pb2.DeleteFeedResponse.FromString,
-                )
+                _registered_method=True)
         self.UpdateFeed = channel.unary_unary(
                 '/iotics.api.FeedAPI/UpdateFeed',
                 request_serializer=iotics_dot_api_dot_feed__pb2.UpdateFeedRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_feed__pb2.UpdateFeedResponse.FromString,
-                )
+                _registered_method=True)
         self.ShareFeedData = channel.unary_unary(
                 '/iotics.api.FeedAPI/ShareFeedData',
                 request_serializer=iotics_dot_api_dot_feed__pb2.ShareFeedDataRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_feed__pb2.ShareFeedDataResponse.FromString,
-                )
+                _registered_method=True)
         self.StreamFeedData = channel.stream_unary(
                 '/iotics.api.FeedAPI/StreamFeedData',
                 request_serializer=iotics_dot_api_dot_feed__pb2.ShareFeedDataRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_feed__pb2.ShareFeedDataResponse.FromString,
-                )
+                _registered_method=True)
         self.ListAllFeeds = channel.unary_unary(
                 '/iotics.api.FeedAPI/ListAllFeeds',
                 request_serializer=iotics_dot_api_dot_feed__pb2.ListAllFeedsRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_feed__pb2.ListAllFeedsResponse.FromString,
-                )
+                _registered_method=True)
         self.DescribeFeed = channel.unary_unary(
                 '/iotics.api.FeedAPI/DescribeFeed',
                 request_serializer=iotics_dot_api_dot_feed__pb2.DescribeFeedRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_feed__pb2.DescribeFeedResponse.FromString,
-                )
+                _registered_method=True)
 
 
 class FeedAPIServicer(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     Create a feed owned by the provided twin.
     A twin may have one or more feeds. Any twin can subscribe to a feed (access control permitting).
@@ -154,14 +154,15 @@
                     request_deserializer=iotics_dot_api_dot_feed__pb2.DescribeFeedRequest.FromString,
                     response_serializer=iotics_dot_api_dot_feed__pb2.DescribeFeedResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'iotics.api.FeedAPI', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('iotics.api.FeedAPI', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class FeedAPI(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     Create a feed owned by the provided twin.
@@ -177,114 +178,184 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.FeedAPI/CreateFeed',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.FeedAPI/CreateFeed',
             iotics_dot_api_dot_feed__pb2.CreateFeedRequest.SerializeToString,
             iotics_dot_api_dot_feed__pb2.CreateFeedResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def DeleteFeed(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.FeedAPI/DeleteFeed',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.FeedAPI/DeleteFeed',
             iotics_dot_api_dot_feed__pb2.DeleteFeedRequest.SerializeToString,
             iotics_dot_api_dot_feed__pb2.DeleteFeedResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def UpdateFeed(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.FeedAPI/UpdateFeed',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.FeedAPI/UpdateFeed',
             iotics_dot_api_dot_feed__pb2.UpdateFeedRequest.SerializeToString,
             iotics_dot_api_dot_feed__pb2.UpdateFeedResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def ShareFeedData(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.FeedAPI/ShareFeedData',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.FeedAPI/ShareFeedData',
             iotics_dot_api_dot_feed__pb2.ShareFeedDataRequest.SerializeToString,
             iotics_dot_api_dot_feed__pb2.ShareFeedDataResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def StreamFeedData(request_iterator,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.stream_unary(request_iterator, target, '/iotics.api.FeedAPI/StreamFeedData',
+        return grpc.experimental.stream_unary(
+            request_iterator,
+            target,
+            '/iotics.api.FeedAPI/StreamFeedData',
             iotics_dot_api_dot_feed__pb2.ShareFeedDataRequest.SerializeToString,
             iotics_dot_api_dot_feed__pb2.ShareFeedDataResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def ListAllFeeds(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.FeedAPI/ListAllFeeds',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.FeedAPI/ListAllFeeds',
             iotics_dot_api_dot_feed__pb2.ListAllFeedsRequest.SerializeToString,
             iotics_dot_api_dot_feed__pb2.ListAllFeedsResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def DescribeFeed(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.FeedAPI/DescribeFeed',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.FeedAPI/DescribeFeed',
             iotics_dot_api_dot_feed__pb2.DescribeFeedRequest.SerializeToString,
             iotics_dot_api_dot_feed__pb2.DescribeFeedResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/api/host_pb2.py` & `iotics-grpc-client-6.0.0/src/iotics/api/host_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: iotics/api/host.proto
+# Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from iotics.api import common_pb2 as iotics_dot_api_dot_common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15iotics/api/host.proto\x12\niotics.api\x1a\x17iotics/api/common.proto\"A\n\x10GetHostIDRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\"\xa6\x01\n\x11GetHostIDResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12?\n\x07payload\x18\x02 \x01(\x0b\x32%.iotics.api.GetHostIDResponse.PayloadR\x07payload\x1a!\n\x07Payload\x12\x16\n\x06hostId\x18\x01 \x01(\tR\x06hostId2U\n\x07HostAPI\x12J\n\tGetHostID\x12\x1c.iotics.api.GetHostIDRequest\x1a\x1d.iotics.api.GetHostIDResponse\"\x00\x42}\n\x0e\x63om.iotics.apiB\tHostProtoP\x01Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\xa2\x02\x03IAX\xaa\x02\nIotics.Api\xca\x02\nIotics\\Apib\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iotics.api.host_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iotics.api.host_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.iotics.apiB\tHostProtoP\001Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\242\002\003IAX\252\002\nIotics.Api\312\002\nIotics\\Api'
-  _GETHOSTIDREQUEST._serialized_start=62
-  _GETHOSTIDREQUEST._serialized_end=127
-  _GETHOSTIDRESPONSE._serialized_start=130
-  _GETHOSTIDRESPONSE._serialized_end=296
-  _GETHOSTIDRESPONSE_PAYLOAD._serialized_start=263
-  _GETHOSTIDRESPONSE_PAYLOAD._serialized_end=296
-  _HOSTAPI._serialized_start=298
-  _HOSTAPI._serialized_end=383
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\016com.iotics.apiB\tHostProtoP\001Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\242\002\003IAX\252\002\nIotics.Api\312\002\nIotics\\Api'
+  _globals['_GETHOSTIDREQUEST']._serialized_start=62
+  _globals['_GETHOSTIDREQUEST']._serialized_end=127
+  _globals['_GETHOSTIDRESPONSE']._serialized_start=130
+  _globals['_GETHOSTIDRESPONSE']._serialized_end=296
+  _globals['_GETHOSTIDRESPONSE_PAYLOAD']._serialized_start=263
+  _globals['_GETHOSTIDRESPONSE_PAYLOAD']._serialized_end=296
+  _globals['_HOSTAPI']._serialized_start=298
+  _globals['_HOSTAPI']._serialized_end=383
 # @@protoc_insertion_point(module_scope)
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/api/host_pb2_grpc.py` & `iotics-grpc-client-6.0.0/src/iotics/api/host_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Args:
             channel: A grpc.Channel.
         """
         self.GetHostID = channel.unary_unary(
                 '/iotics.api.HostAPI/GetHostID',
                 request_serializer=iotics_dot_api_dot_host__pb2.GetHostIDRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_host__pb2.GetHostIDResponse.FromString,
-                )
+                _registered_method=True)
 
 
 class HostAPIServicer(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     HostAPI enables management of Iotics host twins.
     Services only affect local resources, unless stated otherwise.
@@ -47,14 +47,15 @@
                     request_deserializer=iotics_dot_api_dot_host__pb2.GetHostIDRequest.FromString,
                     response_serializer=iotics_dot_api_dot_host__pb2.GetHostIDResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'iotics.api.HostAPI', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('iotics.api.HostAPI', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class HostAPI(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     HostAPI enables management of Iotics host twins.
@@ -68,12 +69,22 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.HostAPI/GetHostID',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.HostAPI/GetHostID',
             iotics_dot_api_dot_host__pb2.GetHostIDRequest.SerializeToString,
             iotics_dot_api_dot_host__pb2.GetHostIDResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/api/input_pb2.py` & `iotics-grpc-client-6.0.0/src/iotics/api/input_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,81 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: iotics/api/input.proto
+# Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from iotics.api import common_pb2 as iotics_dot_api_dot_common__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16iotics/api/input.proto\x12\niotics.api\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17iotics/api/common.proto\"I\n\x07InputID\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x16\n\x06twinId\x18\x02 \x01(\tR\x06twinId\x12\x16\n\x06hostId\x18\x03 \x01(\tR\x06hostId\"\xbd\x01\n\x12\x44\x65leteInputRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12<\n\x04\x61rgs\x18\x02 \x01(\x0b\x32(.iotics.api.DeleteInputRequest.ArgumentsR\x04\x61rgs\x1a:\n\tArguments\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\xc1\x01\n\x13\x44\x65leteInputResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x41\n\x07payload\x18\x02 \x01(\x0b\x32\'.iotics.api.DeleteInputResponse.PayloadR\x07payload\x1a\x38\n\x07Payload\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\x97\x02\n\x12\x43reateInputRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12<\n\x04\x61rgs\x18\x02 \x01(\x0b\x32(.iotics.api.CreateInputRequest.ArgumentsR\x04\x61rgs\x12@\n\x07payload\x18\x03 \x01(\x0b\x32&.iotics.api.CreateInputRequest.PayloadR\x07payload\x1a\x19\n\x07Payload\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x1a\x37\n\tArguments\x12*\n\x06twinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x06twinId\"\xc1\x01\n\x13\x43reateInputResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x41\n\x07payload\x18\x02 \x01(\x0b\x32\'.iotics.api.CreateInputResponse.PayloadR\x07payload\x1a\x38\n\x07Payload\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\xf2\x02\n\x12UpdateInputRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12<\n\x04\x61rgs\x18\x02 \x01(\x0b\x32(.iotics.api.UpdateInputRequest.ArgumentsR\x04\x61rgs\x12@\n\x07payload\x18\x03 \x01(\x0b\x32&.iotics.api.UpdateInputRequest.PayloadR\x07payload\x1aq\n\x07Payload\x12*\n\x06values\x18\x01 \x01(\x0b\x32\x12.iotics.api.ValuesR\x06values\x12:\n\nproperties\x18\x02 \x01(\x0b\x32\x1a.iotics.api.PropertyUpdateR\nproperties\x1a:\n\tArguments\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\xc1\x01\n\x13UpdateInputResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x41\n\x07payload\x18\x02 \x01(\x0b\x32\'.iotics.api.UpdateInputResponse.PayloadR\x07payload\x1a\x38\n\x07Payload\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\xc1\x01\n\x14\x44\x65scribeInputRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12>\n\x04\x61rgs\x18\x02 \x01(\x0b\x32*.iotics.api.DescribeInputRequest.ArgumentsR\x04\x61rgs\x1a:\n\tArguments\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\xfa\x02\n\x15\x44\x65scribeInputResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x43\n\x07payload\x18\x02 \x01(\x0b\x32).iotics.api.DescribeInputResponse.PayloadR\x07payload\x1am\n\nMetaResult\x12)\n\x06values\x18\x01 \x03(\x0b\x32\x11.iotics.api.ValueR\x06values\x12\x34\n\nproperties\x18\x02 \x03(\x0b\x32\x14.iotics.api.PropertyR\nproperties\x1a~\n\x07Payload\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\x12\x44\n\x06result\x18\x02 \x01(\x0b\x32,.iotics.api.DescribeInputResponse.MetaResultR\x06result\"\x86\x01\n\x13UpsertInputWithMeta\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12)\n\x06values\x18\x02 \x03(\x0b\x32\x11.iotics.api.ValueR\x06values\x12\x34\n\nproperties\x18\x03 \x03(\x0b\x32\x14.iotics.api.PropertyR\nproperties\"r\n\x0cInputMessage\x12:\n\noccurredAt\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\noccurredAt\x12\x12\n\x04mime\x18\x02 \x01(\tR\x04mime\x12\x12\n\x04\x64\x61ta\x18\x03 \x01(\x0cR\x04\x64\x61ta\"\xcd\x01\n\x1aReceiveInputMessageRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x44\n\x04\x61rgs\x18\x02 \x01(\x0b\x32\x30.iotics.api.ReceiveInputMessageRequest.ArgumentsR\x04\x61rgs\x1a:\n\tArguments\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\x85\x02\n\x1bReceiveInputMessageResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12I\n\x07payload\x18\x02 \x01(\x0b\x32/.iotics.api.ReceiveInputMessageResponse.PayloadR\x07payload\x1al\n\x07Payload\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\x12\x32\n\x07message\x18\x02 \x01(\x0b\x32\x18.iotics.api.InputMessageR\x07message2\xc5\x03\n\x08InputAPI\x12P\n\x0b\x44\x65leteInput\x12\x1e.iotics.api.DeleteInputRequest\x1a\x1f.iotics.api.DeleteInputResponse\"\x00\x12V\n\rDescribeInput\x12 .iotics.api.DescribeInputRequest\x1a!.iotics.api.DescribeInputResponse\"\x00\x12k\n\x14ReceiveInputMessages\x12&.iotics.api.ReceiveInputMessageRequest\x1a\'.iotics.api.ReceiveInputMessageResponse\"\x00\x30\x01\x12P\n\x0b\x43reateInput\x12\x1e.iotics.api.CreateInputRequest\x1a\x1f.iotics.api.CreateInputResponse\"\x00\x12P\n\x0bUpdateInput\x12\x1e.iotics.api.UpdateInputRequest\x1a\x1f.iotics.api.UpdateInputResponse\"\x00\x42~\n\x0e\x63om.iotics.apiB\nInputProtoP\x01Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\xa2\x02\x03IAX\xaa\x02\nIotics.Api\xca\x02\nIotics\\Apib\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iotics.api.input_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iotics.api.input_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.iotics.apiB\nInputProtoP\001Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\242\002\003IAX\252\002\nIotics.Api\312\002\nIotics\\Api'
-  _INPUTID._serialized_start=96
-  _INPUTID._serialized_end=169
-  _DELETEINPUTREQUEST._serialized_start=172
-  _DELETEINPUTREQUEST._serialized_end=361
-  _DELETEINPUTREQUEST_ARGUMENTS._serialized_start=303
-  _DELETEINPUTREQUEST_ARGUMENTS._serialized_end=361
-  _DELETEINPUTRESPONSE._serialized_start=364
-  _DELETEINPUTRESPONSE._serialized_end=557
-  _DELETEINPUTRESPONSE_PAYLOAD._serialized_start=501
-  _DELETEINPUTRESPONSE_PAYLOAD._serialized_end=557
-  _CREATEINPUTREQUEST._serialized_start=560
-  _CREATEINPUTREQUEST._serialized_end=839
-  _CREATEINPUTREQUEST_PAYLOAD._serialized_start=757
-  _CREATEINPUTREQUEST_PAYLOAD._serialized_end=782
-  _CREATEINPUTREQUEST_ARGUMENTS._serialized_start=784
-  _CREATEINPUTREQUEST_ARGUMENTS._serialized_end=839
-  _CREATEINPUTRESPONSE._serialized_start=842
-  _CREATEINPUTRESPONSE._serialized_end=1035
-  _CREATEINPUTRESPONSE_PAYLOAD._serialized_start=501
-  _CREATEINPUTRESPONSE_PAYLOAD._serialized_end=557
-  _UPDATEINPUTREQUEST._serialized_start=1038
-  _UPDATEINPUTREQUEST._serialized_end=1408
-  _UPDATEINPUTREQUEST_PAYLOAD._serialized_start=1235
-  _UPDATEINPUTREQUEST_PAYLOAD._serialized_end=1348
-  _UPDATEINPUTREQUEST_ARGUMENTS._serialized_start=303
-  _UPDATEINPUTREQUEST_ARGUMENTS._serialized_end=361
-  _UPDATEINPUTRESPONSE._serialized_start=1411
-  _UPDATEINPUTRESPONSE._serialized_end=1604
-  _UPDATEINPUTRESPONSE_PAYLOAD._serialized_start=501
-  _UPDATEINPUTRESPONSE_PAYLOAD._serialized_end=557
-  _DESCRIBEINPUTREQUEST._serialized_start=1607
-  _DESCRIBEINPUTREQUEST._serialized_end=1800
-  _DESCRIBEINPUTREQUEST_ARGUMENTS._serialized_start=303
-  _DESCRIBEINPUTREQUEST_ARGUMENTS._serialized_end=361
-  _DESCRIBEINPUTRESPONSE._serialized_start=1803
-  _DESCRIBEINPUTRESPONSE._serialized_end=2181
-  _DESCRIBEINPUTRESPONSE_METARESULT._serialized_start=1944
-  _DESCRIBEINPUTRESPONSE_METARESULT._serialized_end=2053
-  _DESCRIBEINPUTRESPONSE_PAYLOAD._serialized_start=2055
-  _DESCRIBEINPUTRESPONSE_PAYLOAD._serialized_end=2181
-  _UPSERTINPUTWITHMETA._serialized_start=2184
-  _UPSERTINPUTWITHMETA._serialized_end=2318
-  _INPUTMESSAGE._serialized_start=2320
-  _INPUTMESSAGE._serialized_end=2434
-  _RECEIVEINPUTMESSAGEREQUEST._serialized_start=2437
-  _RECEIVEINPUTMESSAGEREQUEST._serialized_end=2642
-  _RECEIVEINPUTMESSAGEREQUEST_ARGUMENTS._serialized_start=303
-  _RECEIVEINPUTMESSAGEREQUEST_ARGUMENTS._serialized_end=361
-  _RECEIVEINPUTMESSAGERESPONSE._serialized_start=2645
-  _RECEIVEINPUTMESSAGERESPONSE._serialized_end=2906
-  _RECEIVEINPUTMESSAGERESPONSE_PAYLOAD._serialized_start=2798
-  _RECEIVEINPUTMESSAGERESPONSE_PAYLOAD._serialized_end=2906
-  _INPUTAPI._serialized_start=2909
-  _INPUTAPI._serialized_end=3362
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\016com.iotics.apiB\nInputProtoP\001Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\242\002\003IAX\252\002\nIotics.Api\312\002\nIotics\\Api'
+  _globals['_INPUTID']._serialized_start=96
+  _globals['_INPUTID']._serialized_end=169
+  _globals['_DELETEINPUTREQUEST']._serialized_start=172
+  _globals['_DELETEINPUTREQUEST']._serialized_end=361
+  _globals['_DELETEINPUTREQUEST_ARGUMENTS']._serialized_start=303
+  _globals['_DELETEINPUTREQUEST_ARGUMENTS']._serialized_end=361
+  _globals['_DELETEINPUTRESPONSE']._serialized_start=364
+  _globals['_DELETEINPUTRESPONSE']._serialized_end=557
+  _globals['_DELETEINPUTRESPONSE_PAYLOAD']._serialized_start=501
+  _globals['_DELETEINPUTRESPONSE_PAYLOAD']._serialized_end=557
+  _globals['_CREATEINPUTREQUEST']._serialized_start=560
+  _globals['_CREATEINPUTREQUEST']._serialized_end=839
+  _globals['_CREATEINPUTREQUEST_PAYLOAD']._serialized_start=757
+  _globals['_CREATEINPUTREQUEST_PAYLOAD']._serialized_end=782
+  _globals['_CREATEINPUTREQUEST_ARGUMENTS']._serialized_start=784
+  _globals['_CREATEINPUTREQUEST_ARGUMENTS']._serialized_end=839
+  _globals['_CREATEINPUTRESPONSE']._serialized_start=842
+  _globals['_CREATEINPUTRESPONSE']._serialized_end=1035
+  _globals['_CREATEINPUTRESPONSE_PAYLOAD']._serialized_start=501
+  _globals['_CREATEINPUTRESPONSE_PAYLOAD']._serialized_end=557
+  _globals['_UPDATEINPUTREQUEST']._serialized_start=1038
+  _globals['_UPDATEINPUTREQUEST']._serialized_end=1408
+  _globals['_UPDATEINPUTREQUEST_PAYLOAD']._serialized_start=1235
+  _globals['_UPDATEINPUTREQUEST_PAYLOAD']._serialized_end=1348
+  _globals['_UPDATEINPUTREQUEST_ARGUMENTS']._serialized_start=303
+  _globals['_UPDATEINPUTREQUEST_ARGUMENTS']._serialized_end=361
+  _globals['_UPDATEINPUTRESPONSE']._serialized_start=1411
+  _globals['_UPDATEINPUTRESPONSE']._serialized_end=1604
+  _globals['_UPDATEINPUTRESPONSE_PAYLOAD']._serialized_start=501
+  _globals['_UPDATEINPUTRESPONSE_PAYLOAD']._serialized_end=557
+  _globals['_DESCRIBEINPUTREQUEST']._serialized_start=1607
+  _globals['_DESCRIBEINPUTREQUEST']._serialized_end=1800
+  _globals['_DESCRIBEINPUTREQUEST_ARGUMENTS']._serialized_start=303
+  _globals['_DESCRIBEINPUTREQUEST_ARGUMENTS']._serialized_end=361
+  _globals['_DESCRIBEINPUTRESPONSE']._serialized_start=1803
+  _globals['_DESCRIBEINPUTRESPONSE']._serialized_end=2181
+  _globals['_DESCRIBEINPUTRESPONSE_METARESULT']._serialized_start=1944
+  _globals['_DESCRIBEINPUTRESPONSE_METARESULT']._serialized_end=2053
+  _globals['_DESCRIBEINPUTRESPONSE_PAYLOAD']._serialized_start=2055
+  _globals['_DESCRIBEINPUTRESPONSE_PAYLOAD']._serialized_end=2181
+  _globals['_UPSERTINPUTWITHMETA']._serialized_start=2184
+  _globals['_UPSERTINPUTWITHMETA']._serialized_end=2318
+  _globals['_INPUTMESSAGE']._serialized_start=2320
+  _globals['_INPUTMESSAGE']._serialized_end=2434
+  _globals['_RECEIVEINPUTMESSAGEREQUEST']._serialized_start=2437
+  _globals['_RECEIVEINPUTMESSAGEREQUEST']._serialized_end=2642
+  _globals['_RECEIVEINPUTMESSAGEREQUEST_ARGUMENTS']._serialized_start=303
+  _globals['_RECEIVEINPUTMESSAGEREQUEST_ARGUMENTS']._serialized_end=361
+  _globals['_RECEIVEINPUTMESSAGERESPONSE']._serialized_start=2645
+  _globals['_RECEIVEINPUTMESSAGERESPONSE']._serialized_end=2906
+  _globals['_RECEIVEINPUTMESSAGERESPONSE_PAYLOAD']._serialized_start=2798
+  _globals['_RECEIVEINPUTMESSAGERESPONSE_PAYLOAD']._serialized_end=2906
+  _globals['_INPUTAPI']._serialized_start=2909
+  _globals['_INPUTAPI']._serialized_end=3362
 # @@protoc_insertion_point(module_scope)
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/api/input_pb2_grpc.py` & `iotics-grpc-client-6.0.0/src/iotics/api/input_pb2_grpc.py`

 * *Files 19% similar despite different names*

```diff
@@ -18,35 +18,35 @@
         Args:
             channel: A grpc.Channel.
         """
         self.DeleteInput = channel.unary_unary(
                 '/iotics.api.InputAPI/DeleteInput',
                 request_serializer=iotics_dot_api_dot_input__pb2.DeleteInputRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_input__pb2.DeleteInputResponse.FromString,
-                )
+                _registered_method=True)
         self.DescribeInput = channel.unary_unary(
                 '/iotics.api.InputAPI/DescribeInput',
                 request_serializer=iotics_dot_api_dot_input__pb2.DescribeInputRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_input__pb2.DescribeInputResponse.FromString,
-                )
+                _registered_method=True)
         self.ReceiveInputMessages = channel.unary_stream(
                 '/iotics.api.InputAPI/ReceiveInputMessages',
                 request_serializer=iotics_dot_api_dot_input__pb2.ReceiveInputMessageRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_input__pb2.ReceiveInputMessageResponse.FromString,
-                )
+                _registered_method=True)
         self.CreateInput = channel.unary_unary(
                 '/iotics.api.InputAPI/CreateInput',
                 request_serializer=iotics_dot_api_dot_input__pb2.CreateInputRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_input__pb2.CreateInputResponse.FromString,
-                )
+                _registered_method=True)
         self.UpdateInput = channel.unary_unary(
                 '/iotics.api.InputAPI/UpdateInput',
                 request_serializer=iotics_dot_api_dot_input__pb2.UpdateInputRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_input__pb2.UpdateInputResponse.FromString,
-                )
+                _registered_method=True)
 
 
 class InputAPIServicer(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     Input API groups all the actions link to a twin input.
     Services only affect local resources, unless stated otherwise.
@@ -115,14 +115,15 @@
                     request_deserializer=iotics_dot_api_dot_input__pb2.UpdateInputRequest.FromString,
                     response_serializer=iotics_dot_api_dot_input__pb2.UpdateInputResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'iotics.api.InputAPI', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('iotics.api.InputAPI', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class InputAPI(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     Input API groups all the actions link to a twin input.
@@ -136,80 +137,130 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.InputAPI/DeleteInput',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.InputAPI/DeleteInput',
             iotics_dot_api_dot_input__pb2.DeleteInputRequest.SerializeToString,
             iotics_dot_api_dot_input__pb2.DeleteInputResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def DescribeInput(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.InputAPI/DescribeInput',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.InputAPI/DescribeInput',
             iotics_dot_api_dot_input__pb2.DescribeInputRequest.SerializeToString,
             iotics_dot_api_dot_input__pb2.DescribeInputResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def ReceiveInputMessages(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/iotics.api.InputAPI/ReceiveInputMessages',
+        return grpc.experimental.unary_stream(
+            request,
+            target,
+            '/iotics.api.InputAPI/ReceiveInputMessages',
             iotics_dot_api_dot_input__pb2.ReceiveInputMessageRequest.SerializeToString,
             iotics_dot_api_dot_input__pb2.ReceiveInputMessageResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def CreateInput(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.InputAPI/CreateInput',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.InputAPI/CreateInput',
             iotics_dot_api_dot_input__pb2.CreateInputRequest.SerializeToString,
             iotics_dot_api_dot_input__pb2.CreateInputResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def UpdateInput(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.InputAPI/UpdateInput',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.InputAPI/UpdateInput',
             iotics_dot_api_dot_input__pb2.UpdateInputRequest.SerializeToString,
             iotics_dot_api_dot_input__pb2.UpdateInputResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/api/interest_pb2.py` & `iotics-grpc-client-6.0.0/src/iotics/api/meta_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,54 +1,53 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: iotics/api/interest.proto
+# source: iotics/api/meta.proto
+# Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
+from google.rpc import status_pb2 as google_dot_rpc_dot_status__pb2
 from iotics.api import common_pb2 as iotics_dot_api_dot_common__pb2
-from iotics.api import feed_pb2 as iotics_dot_api_dot_feed__pb2
-from iotics.api import input_pb2 as iotics_dot_api_dot_input__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19iotics/api/interest.proto\x12\niotics.api\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x17iotics/api/common.proto\x1a\x15iotics/api/feed.proto\x1a\x16iotics/api/input.proto\"~\n\rInputInterest\x12\x36\n\x0csenderTwinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x0csenderTwinId\x12\x35\n\x0b\x64\x65stInputId\x18\x02 \x01(\x0b\x32\x13.iotics.api.InputIDR\x0b\x64\x65stInputId\"\xd5\x02\n\x17SendInputMessageRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x41\n\x04\x61rgs\x18\x02 \x01(\x0b\x32-.iotics.api.SendInputMessageRequest.ArgumentsR\x04\x61rgs\x12\x45\n\x07payload\x18\x03 \x01(\x0b\x32+.iotics.api.SendInputMessageRequest.PayloadR\x07payload\x1a=\n\x07Payload\x12\x32\n\x07message\x18\x01 \x01(\x0b\x32\x18.iotics.api.InputMessageR\x07message\x1a\x42\n\tArguments\x12\x35\n\x08interest\x18\x01 \x01(\x0b\x32\x19.iotics.api.InputInterestR\x08interest\"I\n\x18SendInputMessageResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\"\x82\x01\n\x08Interest\x12:\n\x0e\x66ollowerTwinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x0e\x66ollowerTwinId\x12:\n\x0e\x66ollowedFeedId\x18\x02 \x01(\x0b\x32\x12.iotics.api.FeedIDR\x0e\x66ollowedFeedId\"\x8a\x02\n\x14\x46\x65tchInterestRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12>\n\x04\x61rgs\x18\x02 \x01(\x0b\x32*.iotics.api.FetchInterestRequest.ArgumentsR\x04\x61rgs\x12\x44\n\x0f\x66\x65tchLastStored\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValueR\x0f\x66\x65tchLastStored\x1a=\n\tArguments\x12\x30\n\x08interest\x18\x01 \x01(\x0b\x32\x14.iotics.api.InterestR\x08interest\"\xfa\x01\n\x15\x46\x65tchInterestResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x43\n\x07payload\x18\x02 \x01(\x0b\x32).iotics.api.FetchInterestResponse.PayloadR\x07payload\x1am\n\x07Payload\x12\x30\n\x08interest\x18\x01 \x01(\x0b\x32\x14.iotics.api.InterestR\x08interest\x12\x30\n\x08\x66\x65\x65\x64\x44\x61ta\x18\x02 \x01(\x0b\x32\x14.iotics.api.FeedDataR\x08\x66\x65\x65\x64\x44\x61ta\"\xc8\x01\n\x16\x46\x65tchLastStoredRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12@\n\x04\x61rgs\x18\x02 \x01(\x0b\x32,.iotics.api.FetchLastStoredRequest.ArgumentsR\x04\x61rgs\x1a=\n\tArguments\x12\x30\n\x08interest\x18\x01 \x01(\x0b\x32\x14.iotics.api.InterestR\x08interest2\xa5\x02\n\x0bInterestAPI\x12Y\n\x0e\x46\x65tchInterests\x12 .iotics.api.FetchInterestRequest\x1a!.iotics.api.FetchInterestResponse\"\x00\x30\x01\x12Z\n\x0f\x46\x65tchLastStored\x12\".iotics.api.FetchLastStoredRequest\x1a!.iotics.api.FetchInterestResponse\"\x00\x12_\n\x10SendInputMessage\x12#.iotics.api.SendInputMessageRequest\x1a$.iotics.api.SendInputMessageResponse\"\x00\x42\x81\x01\n\x0e\x63om.iotics.apiB\rInterestProtoP\x01Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\xa2\x02\x03IAX\xaa\x02\nIotics.Api\xca\x02\nIotics\\Apib\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15iotics/api/meta.proto\x12\niotics.api\x1a\x17google/rpc/status.proto\x1a\x17iotics/api/common.proto\"\x99\x02\n\x0f\x45xplorerRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\'\n\x05scope\x18\x02 \x01(\x0e\x32\x11.iotics.api.ScopeR\x05scope\x12=\n\x07payload\x18\x03 \x01(\x0b\x32#.iotics.api.ExplorerRequest.PayloadR\x07payload\x1ao\n\x07Payload\x12J\n\x11resultContentType\x18\x01 \x01(\x0e\x32\x1c.iotics.api.SparqlResultTypeR\x11resultContentType\x12\x18\n\x07keyword\x18\x02 \x01(\tR\x07keyword\"\x9b\x02\n\x12SparqlQueryRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\'\n\x05scope\x18\x02 \x01(\x0e\x32\x11.iotics.api.ScopeR\x05scope\x12@\n\x07payload\x18\x03 \x01(\x0b\x32&.iotics.api.SparqlQueryRequest.PayloadR\x07payload\x1ak\n\x07Payload\x12J\n\x11resultContentType\x18\x01 \x01(\x0e\x32\x1c.iotics.api.SparqlResultTypeR\x11resultContentType\x12\x14\n\x05query\x18\x02 \x01(\x0cR\x05query\"\xcd\x02\n\x13SparqlQueryResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x41\n\x07payload\x18\x02 \x01(\x0b\x32\'.iotics.api.SparqlQueryResponse.PayloadR\x07payload\x1a\xc3\x01\n\x07Payload\x12\x16\n\x06seqNum\x18\x01 \x01(\x04R\x06seqNum\x12\x12\n\x04last\x18\x02 \x01(\x08R\x04last\x12*\n\x06status\x18\x03 \x01(\x0b\x32\x12.google.rpc.StatusR\x06status\x12>\n\x0b\x63ontentType\x18\x04 \x01(\x0e\x32\x1c.iotics.api.SparqlResultTypeR\x0b\x63ontentType\x12 \n\x0bresultChunk\x18\x05 \x01(\x0cR\x0bresultChunk\"\xdf\x02\n\x10\x45xplorerResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12>\n\x07payload\x18\x02 \x01(\x0b\x32$.iotics.api.ExplorerResponse.PayloadR\x07payload\x1a\xdb\x01\n\x07Payload\x12\x16\n\x06hostId\x18\x01 \x01(\tR\x06hostId\x12\x16\n\x06seqNum\x18\x02 \x01(\x04R\x06seqNum\x12\x12\n\x04last\x18\x03 \x01(\x08R\x04last\x12*\n\x06status\x18\x04 \x01(\x0b\x32\x12.google.rpc.StatusR\x06status\x12>\n\x0b\x63ontentType\x18\x05 \x01(\x0e\x32\x1c.iotics.api.SparqlResultTypeR\x0b\x63ontentType\x12 \n\x0bresultChunk\x18\x06 \x01(\x0cR\x0bresultChunk\"\xaa\x01\n\x13SparqlUpdateRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x41\n\x07payload\x18\x02 \x01(\x0b\x32\'.iotics.api.SparqlUpdateRequest.PayloadR\x07payload\x1a!\n\x07Payload\x12\x16\n\x06update\x18\x01 \x01(\x0cR\x06update\"E\n\x14SparqlUpdateResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers*r\n\x10SparqlResultType\x12\x0f\n\x0bSPARQL_JSON\x10\x00\x12\x0e\n\nSPARQL_XML\x10\x01\x12\x0e\n\nSPARQL_CSV\x10\x02\x12\x0e\n\nRDF_TURTLE\x10\x03\x12\x0b\n\x07RDF_XML\x10\x04\x12\x10\n\x0cRDF_NTRIPLES\x10\x05\x32\x82\x02\n\x07MetaAPI\x12R\n\x0bSparqlQuery\x12\x1e.iotics.api.SparqlQueryRequest\x1a\x1f.iotics.api.SparqlQueryResponse\"\x00\x30\x01\x12S\n\x0cSparqlUpdate\x12\x1f.iotics.api.SparqlUpdateRequest\x1a .iotics.api.SparqlUpdateResponse\"\x00\x12N\n\rExplorerQuery\x12\x1b.iotics.api.ExplorerRequest\x1a\x1c.iotics.api.ExplorerResponse\"\x00\x30\x01\x42}\n\x0e\x63om.iotics.apiB\tMetaProtoP\x01Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\xa2\x02\x03IAX\xaa\x02\nIotics.Api\xca\x02\nIotics\\Apib\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iotics.api.interest_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iotics.api.meta_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.iotics.apiB\rInterestProtoP\001Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\242\002\003IAX\252\002\nIotics.Api\312\002\nIotics\\Api'
-  _INPUTINTEREST._serialized_start=145
-  _INPUTINTEREST._serialized_end=271
-  _SENDINPUTMESSAGEREQUEST._serialized_start=274
-  _SENDINPUTMESSAGEREQUEST._serialized_end=615
-  _SENDINPUTMESSAGEREQUEST_PAYLOAD._serialized_start=486
-  _SENDINPUTMESSAGEREQUEST_PAYLOAD._serialized_end=547
-  _SENDINPUTMESSAGEREQUEST_ARGUMENTS._serialized_start=549
-  _SENDINPUTMESSAGEREQUEST_ARGUMENTS._serialized_end=615
-  _SENDINPUTMESSAGERESPONSE._serialized_start=617
-  _SENDINPUTMESSAGERESPONSE._serialized_end=690
-  _INTEREST._serialized_start=693
-  _INTEREST._serialized_end=823
-  _FETCHINTERESTREQUEST._serialized_start=826
-  _FETCHINTERESTREQUEST._serialized_end=1092
-  _FETCHINTERESTREQUEST_ARGUMENTS._serialized_start=1031
-  _FETCHINTERESTREQUEST_ARGUMENTS._serialized_end=1092
-  _FETCHINTERESTRESPONSE._serialized_start=1095
-  _FETCHINTERESTRESPONSE._serialized_end=1345
-  _FETCHINTERESTRESPONSE_PAYLOAD._serialized_start=1236
-  _FETCHINTERESTRESPONSE_PAYLOAD._serialized_end=1345
-  _FETCHLASTSTOREDREQUEST._serialized_start=1348
-  _FETCHLASTSTOREDREQUEST._serialized_end=1548
-  _FETCHLASTSTOREDREQUEST_ARGUMENTS._serialized_start=1031
-  _FETCHLASTSTOREDREQUEST_ARGUMENTS._serialized_end=1092
-  _INTERESTAPI._serialized_start=1551
-  _INTERESTAPI._serialized_end=1844
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\016com.iotics.apiB\tMetaProtoP\001Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\242\002\003IAX\252\002\nIotics.Api\312\002\nIotics\\Api'
+  _globals['_SPARQLRESULTTYPE']._serialized_start=1591
+  _globals['_SPARQLRESULTTYPE']._serialized_end=1705
+  _globals['_EXPLORERREQUEST']._serialized_start=88
+  _globals['_EXPLORERREQUEST']._serialized_end=369
+  _globals['_EXPLORERREQUEST_PAYLOAD']._serialized_start=258
+  _globals['_EXPLORERREQUEST_PAYLOAD']._serialized_end=369
+  _globals['_SPARQLQUERYREQUEST']._serialized_start=372
+  _globals['_SPARQLQUERYREQUEST']._serialized_end=655
+  _globals['_SPARQLQUERYREQUEST_PAYLOAD']._serialized_start=548
+  _globals['_SPARQLQUERYREQUEST_PAYLOAD']._serialized_end=655
+  _globals['_SPARQLQUERYRESPONSE']._serialized_start=658
+  _globals['_SPARQLQUERYRESPONSE']._serialized_end=991
+  _globals['_SPARQLQUERYRESPONSE_PAYLOAD']._serialized_start=796
+  _globals['_SPARQLQUERYRESPONSE_PAYLOAD']._serialized_end=991
+  _globals['_EXPLORERRESPONSE']._serialized_start=994
+  _globals['_EXPLORERRESPONSE']._serialized_end=1345
+  _globals['_EXPLORERRESPONSE_PAYLOAD']._serialized_start=1126
+  _globals['_EXPLORERRESPONSE_PAYLOAD']._serialized_end=1345
+  _globals['_SPARQLUPDATEREQUEST']._serialized_start=1348
+  _globals['_SPARQLUPDATEREQUEST']._serialized_end=1518
+  _globals['_SPARQLUPDATEREQUEST_PAYLOAD']._serialized_start=1485
+  _globals['_SPARQLUPDATEREQUEST_PAYLOAD']._serialized_end=1518
+  _globals['_SPARQLUPDATERESPONSE']._serialized_start=1520
+  _globals['_SPARQLUPDATERESPONSE']._serialized_end=1589
+  _globals['_METAAPI']._serialized_start=1708
+  _globals['_METAAPI']._serialized_end=1966
 # @@protoc_insertion_point(module_scope)
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/api/interest_pb2_grpc.py` & `iotics-grpc-client-6.0.0/src/iotics/api/interest_pb2_grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,25 +17,25 @@
         Args:
             channel: A grpc.Channel.
         """
         self.FetchInterests = channel.unary_stream(
                 '/iotics.api.InterestAPI/FetchInterests',
                 request_serializer=iotics_dot_api_dot_interest__pb2.FetchInterestRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_interest__pb2.FetchInterestResponse.FromString,
-                )
+                _registered_method=True)
         self.FetchLastStored = channel.unary_unary(
                 '/iotics.api.InterestAPI/FetchLastStored',
                 request_serializer=iotics_dot_api_dot_interest__pb2.FetchLastStoredRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_interest__pb2.FetchInterestResponse.FromString,
-                )
+                _registered_method=True)
         self.SendInputMessage = channel.unary_unary(
                 '/iotics.api.InterestAPI/SendInputMessage',
                 request_serializer=iotics_dot_api_dot_interest__pb2.SendInputMessageRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_interest__pb2.SendInputMessageResponse.FromString,
-                )
+                _registered_method=True)
 
 
 class InterestAPIServicer(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     InterestAPI enables creation and management of interests between a twin and a feed or an input.
     """
@@ -79,14 +79,15 @@
                     request_deserializer=iotics_dot_api_dot_interest__pb2.SendInputMessageRequest.FromString,
                     response_serializer=iotics_dot_api_dot_interest__pb2.SendInputMessageResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'iotics.api.InterestAPI', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('iotics.api.InterestAPI', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class InterestAPI(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     InterestAPI enables creation and management of interests between a twin and a feed or an input.
@@ -99,46 +100,76 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/iotics.api.InterestAPI/FetchInterests',
+        return grpc.experimental.unary_stream(
+            request,
+            target,
+            '/iotics.api.InterestAPI/FetchInterests',
             iotics_dot_api_dot_interest__pb2.FetchInterestRequest.SerializeToString,
             iotics_dot_api_dot_interest__pb2.FetchInterestResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def FetchLastStored(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.InterestAPI/FetchLastStored',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.InterestAPI/FetchLastStored',
             iotics_dot_api_dot_interest__pb2.FetchLastStoredRequest.SerializeToString,
             iotics_dot_api_dot_interest__pb2.FetchInterestResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def SendInputMessage(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.InterestAPI/SendInputMessage',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.InterestAPI/SendInputMessage',
             iotics_dot_api_dot_interest__pb2.SendInputMessageRequest.SerializeToString,
             iotics_dot_api_dot_interest__pb2.SendInputMessageResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/api/meta_pb2_grpc.py` & `iotics-grpc-client-6.0.0/src/iotics/api/meta_pb2_grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,41 +18,42 @@
         Args:
             channel: A grpc.Channel.
         """
         self.SparqlQuery = channel.unary_stream(
                 '/iotics.api.MetaAPI/SparqlQuery',
                 request_serializer=iotics_dot_api_dot_meta__pb2.SparqlQueryRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_meta__pb2.SparqlQueryResponse.FromString,
-                )
+                _registered_method=True)
         self.SparqlUpdate = channel.unary_unary(
                 '/iotics.api.MetaAPI/SparqlUpdate',
                 request_serializer=iotics_dot_api_dot_meta__pb2.SparqlUpdateRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_meta__pb2.SparqlUpdateResponse.FromString,
-                )
+                _registered_method=True)
         self.ExplorerQuery = channel.unary_stream(
                 '/iotics.api.MetaAPI/ExplorerQuery',
                 request_serializer=iotics_dot_api_dot_meta__pb2.ExplorerRequest.SerializeToString,
-                response_deserializer=iotics_dot_api_dot_meta__pb2.SparqlQueryResponse.FromString,
-                )
+                response_deserializer=iotics_dot_api_dot_meta__pb2.ExplorerResponse.FromString,
+                _registered_method=True)
 
 
 class MetaAPIServicer(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     MetaAPI enables querying of metadata associated with Twins and Feeds.
     Services only affect local resources, unless stated otherwise.
     """
 
     def SparqlQuery(self, request, context):
-        """SparqlQuery performs a SPARQL 1.1 query and returns one or more results, each as a sequence of chunks. Note that:
-        - Chunks for a particular result will arrive in-order though they might be interleaved with chunks from other
-        results (when performing a non-local query). See scope parameter in SparqlQueryRequest;
-        - The call will only complete once the (specified or host default) request timeout has been reached. The client can
-        choose to end the stream early once they have received enough results. (E.g. in the case of Scope.LOCAL this
-        would be after the one and only sequence of chunks has been received.). (local and remote)
+        """SparqlQuery performs a SPARQL 1.1 query against the Federated Knowledge Graph of the Iotics network to which this
+        host belongs. The result is returned as a sequence of chunks. Note that:
+        - Result chunks MIGHT arrive out of order and it is the client's responsibility to re-assemble them.
+        - This RPC is currently in beta, it means:
+        - the logic should remain unchanged,
+        - the rpc call should remain unchanged,
+        - the service can be interrupted without notice.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def SparqlUpdate(self, request, context):
         """SparqlUpdate performs a SPARQL 1.1 update. When performing an update, the update query must contain a reference to
@@ -83,20 +84,21 @@
                     servicer.SparqlUpdate,
                     request_deserializer=iotics_dot_api_dot_meta__pb2.SparqlUpdateRequest.FromString,
                     response_serializer=iotics_dot_api_dot_meta__pb2.SparqlUpdateResponse.SerializeToString,
             ),
             'ExplorerQuery': grpc.unary_stream_rpc_method_handler(
                     servicer.ExplorerQuery,
                     request_deserializer=iotics_dot_api_dot_meta__pb2.ExplorerRequest.FromString,
-                    response_serializer=iotics_dot_api_dot_meta__pb2.SparqlQueryResponse.SerializeToString,
+                    response_serializer=iotics_dot_api_dot_meta__pb2.ExplorerResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'iotics.api.MetaAPI', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('iotics.api.MetaAPI', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class MetaAPI(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     MetaAPI enables querying of metadata associated with Twins and Feeds.
@@ -110,46 +112,76 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/iotics.api.MetaAPI/SparqlQuery',
+        return grpc.experimental.unary_stream(
+            request,
+            target,
+            '/iotics.api.MetaAPI/SparqlQuery',
             iotics_dot_api_dot_meta__pb2.SparqlQueryRequest.SerializeToString,
             iotics_dot_api_dot_meta__pb2.SparqlQueryResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def SparqlUpdate(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.MetaAPI/SparqlUpdate',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.MetaAPI/SparqlUpdate',
             iotics_dot_api_dot_meta__pb2.SparqlUpdateRequest.SerializeToString,
             iotics_dot_api_dot_meta__pb2.SparqlUpdateResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def ExplorerQuery(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/iotics.api.MetaAPI/ExplorerQuery',
+        return grpc.experimental.unary_stream(
+            request,
+            target,
+            '/iotics.api.MetaAPI/ExplorerQuery',
             iotics_dot_api_dot_meta__pb2.ExplorerRequest.SerializeToString,
-            iotics_dot_api_dot_meta__pb2.SparqlQueryResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            iotics_dot_api_dot_meta__pb2.ExplorerResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/api/search_pb2_grpc.py` & `iotics-grpc-client-6.0.0/src/iotics/api/search_pb2_grpc.py`

 * *Files 21% similar despite different names*

```diff
@@ -19,30 +19,30 @@
         Args:
             channel: A grpc.Channel.
         """
         self.DispatchSearchRequest = channel.unary_unary(
                 '/iotics.api.SearchAPI/DispatchSearchRequest',
                 request_serializer=iotics_dot_api_dot_search__pb2.SearchRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_search__pb2.DispatchSearchResponse.FromString,
-                )
+                _registered_method=True)
         self.SynchronousSearch = channel.unary_stream(
                 '/iotics.api.SearchAPI/SynchronousSearch',
                 request_serializer=iotics_dot_api_dot_search__pb2.SearchRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_search__pb2.SearchResponse.FromString,
-                )
+                _registered_method=True)
         self.ReceiveAllSearchResponses = channel.unary_stream(
                 '/iotics.api.SearchAPI/ReceiveAllSearchResponses',
                 request_serializer=iotics_dot_api_dot_common__pb2.SubscriptionHeaders.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_search__pb2.SearchResponse.FromString,
-                )
+                _registered_method=True)
         self.AdvancedSearch = channel.unary_stream(
                 '/iotics.api.SearchAPI/AdvancedSearch',
                 request_serializer=iotics_dot_api_dot_search__pb2.AdvancedSearchRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_search__pb2.SearchResponse.FromString,
-                )
+                _registered_method=True)
 
 
 class SearchAPIServicer(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     SearchAPI provides a set of services to run synchronous and asynchronous search.
     Services only affect local resources, unless stated otherwise.
@@ -99,14 +99,15 @@
                     request_deserializer=iotics_dot_api_dot_search__pb2.AdvancedSearchRequest.FromString,
                     response_serializer=iotics_dot_api_dot_search__pb2.SearchResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'iotics.api.SearchAPI', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('iotics.api.SearchAPI', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class SearchAPI(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     SearchAPI provides a set of services to run synchronous and asynchronous search.
@@ -120,63 +121,103 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.SearchAPI/DispatchSearchRequest',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.SearchAPI/DispatchSearchRequest',
             iotics_dot_api_dot_search__pb2.SearchRequest.SerializeToString,
             iotics_dot_api_dot_search__pb2.DispatchSearchResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def SynchronousSearch(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/iotics.api.SearchAPI/SynchronousSearch',
+        return grpc.experimental.unary_stream(
+            request,
+            target,
+            '/iotics.api.SearchAPI/SynchronousSearch',
             iotics_dot_api_dot_search__pb2.SearchRequest.SerializeToString,
             iotics_dot_api_dot_search__pb2.SearchResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def ReceiveAllSearchResponses(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/iotics.api.SearchAPI/ReceiveAllSearchResponses',
+        return grpc.experimental.unary_stream(
+            request,
+            target,
+            '/iotics.api.SearchAPI/ReceiveAllSearchResponses',
             iotics_dot_api_dot_common__pb2.SubscriptionHeaders.SerializeToString,
             iotics_dot_api_dot_search__pb2.SearchResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def AdvancedSearch(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_stream(request, target, '/iotics.api.SearchAPI/AdvancedSearch',
+        return grpc.experimental.unary_stream(
+            request,
+            target,
+            '/iotics.api.SearchAPI/AdvancedSearch',
             iotics_dot_api_dot_search__pb2.AdvancedSearchRequest.SerializeToString,
             iotics_dot_api_dot_search__pb2.SearchResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/api/twin_pb2.py` & `iotics-grpc-client-6.0.0/src/iotics/api/twin_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,89 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: iotics/api/twin.proto
+# Protobuf Python Version: 4.25.3
 """Generated protocol buffer code."""
-from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from iotics.api import common_pb2 as iotics_dot_api_dot_common__pb2
 from iotics.api import feed_pb2 as iotics_dot_api_dot_feed__pb2
 from iotics.api import input_pb2 as iotics_dot_api_dot_input__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15iotics/api/twin.proto\x12\niotics.api\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17iotics/api/common.proto\x1a\x15iotics/api/feed.proto\x1a\x16iotics/api/input.proto\"m\n\x13ListAllTwinsRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\'\n\x05range\x18\x14 \x01(\x0b\x32\x11.iotics.api.RangeR\x05range\"\xb9\x03\n\x14ListAllTwinsResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x42\n\x07payload\x18\x02 \x01(\x0b\x32(.iotics.api.ListAllTwinsResponse.PayloadR\x07payload\x1a\xde\x01\n\x0bTwinDetails\x12*\n\x06twinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x06twinId\x12\x33\n\x08location\x18\x03 \x01(\x0b\x32\x17.iotics.api.GeoLocationR\x08location\x12\x34\n\nproperties\x18\x05 \x03(\x0b\x32\x14.iotics.api.PropertyR\nproperties\x12\x38\n\tupdatedAt\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x1aM\n\x07Payload\x12\x42\n\x05twins\x18\x01 \x03(\x0b\x32,.iotics.api.ListAllTwinsResponse.TwinDetailsR\x05twins\"\x9e\x01\n\x11\x43reateTwinRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12?\n\x07payload\x18\x02 \x01(\x0b\x32%.iotics.api.CreateTwinRequest.PayloadR\x07payload\x1a\x19\n\x07Payload\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\"\xbc\x01\n\x12\x43reateTwinResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12@\n\x07payload\x18\x02 \x01(\x0b\x32&.iotics.api.CreateTwinResponse.PayloadR\x07payload\x1a\x35\n\x07Payload\x12*\n\x06twinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x06twinId\"\xb8\x01\n\x11\x44\x65leteTwinRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12;\n\x04\x61rgs\x18\x02 \x01(\x0b\x32\'.iotics.api.DeleteTwinRequest.ArgumentsR\x04\x61rgs\x1a\x37\n\tArguments\x12*\n\x06twinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x06twinId\"\xbc\x01\n\x12\x44\x65leteTwinResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12@\n\x07payload\x18\x02 \x01(\x0b\x32&.iotics.api.DeleteTwinResponse.PayloadR\x07payload\x1a\x35\n\x07Payload\x12*\n\x06twinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x06twinId\"\xbc\x01\n\x13\x44\x65scribeTwinRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12=\n\x04\x61rgs\x18\x03 \x01(\x0b\x32).iotics.api.DescribeTwinRequest.ArgumentsR\x04\x61rgs\x1a\x37\n\tArguments\x12*\n\x06twinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x06twinId\"T\n\x08\x46\x65\x65\x64Meta\x12*\n\x06\x66\x65\x65\x64Id\x18\x01 \x01(\x0b\x32\x12.iotics.api.FeedIDR\x06\x66\x65\x65\x64Id\x12\x1c\n\tstoreLast\x18\x03 \x01(\x08R\tstoreLast\":\n\tInputMeta\x12-\n\x07inputId\x18\x01 \x01(\x0b\x32\x13.iotics.api.InputIDR\x07inputId\"\x94\x04\n\x14\x44\x65scribeTwinResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12\x42\n\x07payload\x18\x02 \x01(\x0b\x32(.iotics.api.DescribeTwinResponse.PayloadR\x07payload\x1a\x8c\x02\n\nMetaResult\x12\x33\n\x08location\x18\x01 \x01(\x0b\x32\x17.iotics.api.GeoLocationR\x08location\x12*\n\x05\x66\x65\x65\x64s\x18\x04 \x03(\x0b\x32\x14.iotics.api.FeedMetaR\x05\x66\x65\x65\x64s\x12-\n\x06inputs\x18\x05 \x03(\x0b\x32\x15.iotics.api.InputMetaR\x06inputs\x12\x34\n\nproperties\x18\x06 \x03(\x0b\x32\x14.iotics.api.PropertyR\nproperties\x12\x38\n\tupdatedAt\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x1az\n\x07Payload\x12*\n\x06twinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x06twinId\x12\x43\n\x06result\x18\x02 \x01(\x0b\x32+.iotics.api.DescribeTwinResponse.MetaResultR\x06result\"H\n\x11GeoLocationUpdate\x12\x33\n\x08location\x18\x01 \x01(\x0b\x32\x17.iotics.api.GeoLocationR\x08location\"\xfc\x02\n\x11UpdateTwinRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12;\n\x04\x61rgs\x18\x02 \x01(\x0b\x32\'.iotics.api.UpdateTwinRequest.ArgumentsR\x04\x61rgs\x12?\n\x07payload\x18\x03 \x01(\x0b\x32%.iotics.api.UpdateTwinRequest.PayloadR\x07payload\x1a\x37\n\tArguments\x12*\n\x06twinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x06twinId\x1a\x80\x01\n\x07Payload\x12:\n\nproperties\x18\x03 \x01(\x0b\x32\x1a.iotics.api.PropertyUpdateR\nproperties\x12\x39\n\x08location\x18\x06 \x01(\x0b\x32\x1d.iotics.api.GeoLocationUpdateR\x08location\"\xbc\x01\n\x12UpdateTwinResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12@\n\x07payload\x18\x02 \x01(\x0b\x32&.iotics.api.UpdateTwinResponse.PayloadR\x07payload\x1a\x35\n\x07Payload\x12*\n\x06twinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x06twinId\"\x95\x03\n\x11UpsertTwinRequest\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12?\n\x07payload\x18\x02 \x01(\x0b\x32%.iotics.api.UpsertTwinRequest.PayloadR\x07payload\x1a\x8f\x02\n\x07Payload\x12*\n\x06twinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x06twinId\x12\x34\n\nproperties\x18\x05 \x03(\x0b\x32\x14.iotics.api.PropertyR\nproperties\x12\x33\n\x08location\x18\x06 \x01(\x0b\x32\x17.iotics.api.GeoLocationR\x08location\x12\x34\n\x05\x66\x65\x65\x64s\x18\x07 \x03(\x0b\x32\x1e.iotics.api.UpsertFeedWithMetaR\x05\x66\x65\x65\x64s\x12\x37\n\x06inputs\x18\x08 \x03(\x0b\x32\x1f.iotics.api.UpsertInputWithMetaR\x06inputs\"\xbc\x01\n\x12UpsertTwinResponse\x12-\n\x07headers\x18\x01 \x01(\x0b\x32\x13.iotics.api.HeadersR\x07headers\x12@\n\x07payload\x18\x02 \x01(\x0b\x32&.iotics.api.UpsertTwinResponse.PayloadR\x07payload\x1a\x35\n\x07Payload\x12*\n\x06twinId\x18\x01 \x01(\x0b\x32\x12.iotics.api.TwinIDR\x06twinId2\xef\x03\n\x07TwinAPI\x12M\n\nCreateTwin\x12\x1d.iotics.api.CreateTwinRequest\x1a\x1e.iotics.api.CreateTwinResponse\"\x00\x12M\n\nUpsertTwin\x12\x1d.iotics.api.UpsertTwinRequest\x1a\x1e.iotics.api.UpsertTwinResponse\"\x00\x12M\n\nDeleteTwin\x12\x1d.iotics.api.DeleteTwinRequest\x1a\x1e.iotics.api.DeleteTwinResponse\"\x00\x12M\n\nUpdateTwin\x12\x1d.iotics.api.UpdateTwinRequest\x1a\x1e.iotics.api.UpdateTwinResponse\"\x00\x12S\n\x0c\x44\x65scribeTwin\x12\x1f.iotics.api.DescribeTwinRequest\x1a .iotics.api.DescribeTwinResponse\"\x00\x12S\n\x0cListAllTwins\x12\x1f.iotics.api.ListAllTwinsRequest\x1a .iotics.api.ListAllTwinsResponse\"\x00\x42}\n\x0e\x63om.iotics.apiB\tTwinProtoP\x01Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\xa2\x02\x03IAX\xaa\x02\nIotics.Api\xca\x02\nIotics\\Apib\x06proto3')
 
-_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iotics.api.twin_pb2', globals())
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'iotics.api.twin_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
-
-  DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n\016com.iotics.apiB\tTwinProtoP\001Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\242\002\003IAX\252\002\nIotics.Api\312\002\nIotics\\Api'
-  _LISTALLTWINSREQUEST._serialized_start=142
-  _LISTALLTWINSREQUEST._serialized_end=251
-  _LISTALLTWINSRESPONSE._serialized_start=254
-  _LISTALLTWINSRESPONSE._serialized_end=695
-  _LISTALLTWINSRESPONSE_TWINDETAILS._serialized_start=394
-  _LISTALLTWINSRESPONSE_TWINDETAILS._serialized_end=616
-  _LISTALLTWINSRESPONSE_PAYLOAD._serialized_start=618
-  _LISTALLTWINSRESPONSE_PAYLOAD._serialized_end=695
-  _CREATETWINREQUEST._serialized_start=698
-  _CREATETWINREQUEST._serialized_end=856
-  _CREATETWINREQUEST_PAYLOAD._serialized_start=831
-  _CREATETWINREQUEST_PAYLOAD._serialized_end=856
-  _CREATETWINRESPONSE._serialized_start=859
-  _CREATETWINRESPONSE._serialized_end=1047
-  _CREATETWINRESPONSE_PAYLOAD._serialized_start=994
-  _CREATETWINRESPONSE_PAYLOAD._serialized_end=1047
-  _DELETETWINREQUEST._serialized_start=1050
-  _DELETETWINREQUEST._serialized_end=1234
-  _DELETETWINREQUEST_ARGUMENTS._serialized_start=1179
-  _DELETETWINREQUEST_ARGUMENTS._serialized_end=1234
-  _DELETETWINRESPONSE._serialized_start=1237
-  _DELETETWINRESPONSE._serialized_end=1425
-  _DELETETWINRESPONSE_PAYLOAD._serialized_start=994
-  _DELETETWINRESPONSE_PAYLOAD._serialized_end=1047
-  _DESCRIBETWINREQUEST._serialized_start=1428
-  _DESCRIBETWINREQUEST._serialized_end=1616
-  _DESCRIBETWINREQUEST_ARGUMENTS._serialized_start=1179
-  _DESCRIBETWINREQUEST_ARGUMENTS._serialized_end=1234
-  _FEEDMETA._serialized_start=1618
-  _FEEDMETA._serialized_end=1702
-  _INPUTMETA._serialized_start=1704
-  _INPUTMETA._serialized_end=1762
-  _DESCRIBETWINRESPONSE._serialized_start=1765
-  _DESCRIBETWINRESPONSE._serialized_end=2297
-  _DESCRIBETWINRESPONSE_METARESULT._serialized_start=1905
-  _DESCRIBETWINRESPONSE_METARESULT._serialized_end=2173
-  _DESCRIBETWINRESPONSE_PAYLOAD._serialized_start=2175
-  _DESCRIBETWINRESPONSE_PAYLOAD._serialized_end=2297
-  _GEOLOCATIONUPDATE._serialized_start=2299
-  _GEOLOCATIONUPDATE._serialized_end=2371
-  _UPDATETWINREQUEST._serialized_start=2374
-  _UPDATETWINREQUEST._serialized_end=2754
-  _UPDATETWINREQUEST_ARGUMENTS._serialized_start=1179
-  _UPDATETWINREQUEST_ARGUMENTS._serialized_end=1234
-  _UPDATETWINREQUEST_PAYLOAD._serialized_start=2626
-  _UPDATETWINREQUEST_PAYLOAD._serialized_end=2754
-  _UPDATETWINRESPONSE._serialized_start=2757
-  _UPDATETWINRESPONSE._serialized_end=2945
-  _UPDATETWINRESPONSE_PAYLOAD._serialized_start=994
-  _UPDATETWINRESPONSE_PAYLOAD._serialized_end=1047
-  _UPSERTTWINREQUEST._serialized_start=2948
-  _UPSERTTWINREQUEST._serialized_end=3353
-  _UPSERTTWINREQUEST_PAYLOAD._serialized_start=3082
-  _UPSERTTWINREQUEST_PAYLOAD._serialized_end=3353
-  _UPSERTTWINRESPONSE._serialized_start=3356
-  _UPSERTTWINRESPONSE._serialized_end=3544
-  _UPSERTTWINRESPONSE_PAYLOAD._serialized_start=994
-  _UPSERTTWINRESPONSE_PAYLOAD._serialized_end=1047
-  _TWINAPI._serialized_start=3547
-  _TWINAPI._serialized_end=4042
+  _globals['DESCRIPTOR']._options = None
+  _globals['DESCRIPTOR']._serialized_options = b'\n\016com.iotics.apiB\tTwinProtoP\001Z>github.com/Iotic-Labs/iotic-go-proto-qapi/iotics/api;ioticsapi\242\002\003IAX\252\002\nIotics.Api\312\002\nIotics\\Api'
+  _globals['_LISTALLTWINSREQUEST']._serialized_start=142
+  _globals['_LISTALLTWINSREQUEST']._serialized_end=251
+  _globals['_LISTALLTWINSRESPONSE']._serialized_start=254
+  _globals['_LISTALLTWINSRESPONSE']._serialized_end=695
+  _globals['_LISTALLTWINSRESPONSE_TWINDETAILS']._serialized_start=394
+  _globals['_LISTALLTWINSRESPONSE_TWINDETAILS']._serialized_end=616
+  _globals['_LISTALLTWINSRESPONSE_PAYLOAD']._serialized_start=618
+  _globals['_LISTALLTWINSRESPONSE_PAYLOAD']._serialized_end=695
+  _globals['_CREATETWINREQUEST']._serialized_start=698
+  _globals['_CREATETWINREQUEST']._serialized_end=856
+  _globals['_CREATETWINREQUEST_PAYLOAD']._serialized_start=831
+  _globals['_CREATETWINREQUEST_PAYLOAD']._serialized_end=856
+  _globals['_CREATETWINRESPONSE']._serialized_start=859
+  _globals['_CREATETWINRESPONSE']._serialized_end=1047
+  _globals['_CREATETWINRESPONSE_PAYLOAD']._serialized_start=994
+  _globals['_CREATETWINRESPONSE_PAYLOAD']._serialized_end=1047
+  _globals['_DELETETWINREQUEST']._serialized_start=1050
+  _globals['_DELETETWINREQUEST']._serialized_end=1234
+  _globals['_DELETETWINREQUEST_ARGUMENTS']._serialized_start=1179
+  _globals['_DELETETWINREQUEST_ARGUMENTS']._serialized_end=1234
+  _globals['_DELETETWINRESPONSE']._serialized_start=1237
+  _globals['_DELETETWINRESPONSE']._serialized_end=1425
+  _globals['_DELETETWINRESPONSE_PAYLOAD']._serialized_start=994
+  _globals['_DELETETWINRESPONSE_PAYLOAD']._serialized_end=1047
+  _globals['_DESCRIBETWINREQUEST']._serialized_start=1428
+  _globals['_DESCRIBETWINREQUEST']._serialized_end=1616
+  _globals['_DESCRIBETWINREQUEST_ARGUMENTS']._serialized_start=1179
+  _globals['_DESCRIBETWINREQUEST_ARGUMENTS']._serialized_end=1234
+  _globals['_FEEDMETA']._serialized_start=1618
+  _globals['_FEEDMETA']._serialized_end=1702
+  _globals['_INPUTMETA']._serialized_start=1704
+  _globals['_INPUTMETA']._serialized_end=1762
+  _globals['_DESCRIBETWINRESPONSE']._serialized_start=1765
+  _globals['_DESCRIBETWINRESPONSE']._serialized_end=2297
+  _globals['_DESCRIBETWINRESPONSE_METARESULT']._serialized_start=1905
+  _globals['_DESCRIBETWINRESPONSE_METARESULT']._serialized_end=2173
+  _globals['_DESCRIBETWINRESPONSE_PAYLOAD']._serialized_start=2175
+  _globals['_DESCRIBETWINRESPONSE_PAYLOAD']._serialized_end=2297
+  _globals['_GEOLOCATIONUPDATE']._serialized_start=2299
+  _globals['_GEOLOCATIONUPDATE']._serialized_end=2371
+  _globals['_UPDATETWINREQUEST']._serialized_start=2374
+  _globals['_UPDATETWINREQUEST']._serialized_end=2754
+  _globals['_UPDATETWINREQUEST_ARGUMENTS']._serialized_start=1179
+  _globals['_UPDATETWINREQUEST_ARGUMENTS']._serialized_end=1234
+  _globals['_UPDATETWINREQUEST_PAYLOAD']._serialized_start=2626
+  _globals['_UPDATETWINREQUEST_PAYLOAD']._serialized_end=2754
+  _globals['_UPDATETWINRESPONSE']._serialized_start=2757
+  _globals['_UPDATETWINRESPONSE']._serialized_end=2945
+  _globals['_UPDATETWINRESPONSE_PAYLOAD']._serialized_start=994
+  _globals['_UPDATETWINRESPONSE_PAYLOAD']._serialized_end=1047
+  _globals['_UPSERTTWINREQUEST']._serialized_start=2948
+  _globals['_UPSERTTWINREQUEST']._serialized_end=3353
+  _globals['_UPSERTTWINREQUEST_PAYLOAD']._serialized_start=3082
+  _globals['_UPSERTTWINREQUEST_PAYLOAD']._serialized_end=3353
+  _globals['_UPSERTTWINRESPONSE']._serialized_start=3356
+  _globals['_UPSERTTWINRESPONSE']._serialized_end=3544
+  _globals['_UPSERTTWINRESPONSE_PAYLOAD']._serialized_start=994
+  _globals['_UPSERTTWINRESPONSE_PAYLOAD']._serialized_end=1047
+  _globals['_TWINAPI']._serialized_start=3547
+  _globals['_TWINAPI']._serialized_end=4042
 # @@protoc_insertion_point(module_scope)
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/api/twin_pb2_grpc.py` & `iotics-grpc-client-6.0.0/src/iotics/api/twin_pb2_grpc.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,40 +18,40 @@
         Args:
             channel: A grpc.Channel.
         """
         self.CreateTwin = channel.unary_unary(
                 '/iotics.api.TwinAPI/CreateTwin',
                 request_serializer=iotics_dot_api_dot_twin__pb2.CreateTwinRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_twin__pb2.CreateTwinResponse.FromString,
-                )
+                _registered_method=True)
         self.UpsertTwin = channel.unary_unary(
                 '/iotics.api.TwinAPI/UpsertTwin',
                 request_serializer=iotics_dot_api_dot_twin__pb2.UpsertTwinRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_twin__pb2.UpsertTwinResponse.FromString,
-                )
+                _registered_method=True)
         self.DeleteTwin = channel.unary_unary(
                 '/iotics.api.TwinAPI/DeleteTwin',
                 request_serializer=iotics_dot_api_dot_twin__pb2.DeleteTwinRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_twin__pb2.DeleteTwinResponse.FromString,
-                )
+                _registered_method=True)
         self.UpdateTwin = channel.unary_unary(
                 '/iotics.api.TwinAPI/UpdateTwin',
                 request_serializer=iotics_dot_api_dot_twin__pb2.UpdateTwinRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_twin__pb2.UpdateTwinResponse.FromString,
-                )
+                _registered_method=True)
         self.DescribeTwin = channel.unary_unary(
                 '/iotics.api.TwinAPI/DescribeTwin',
                 request_serializer=iotics_dot_api_dot_twin__pb2.DescribeTwinRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_twin__pb2.DescribeTwinResponse.FromString,
-                )
+                _registered_method=True)
         self.ListAllTwins = channel.unary_unary(
                 '/iotics.api.TwinAPI/ListAllTwins',
                 request_serializer=iotics_dot_api_dot_twin__pb2.ListAllTwinsRequest.SerializeToString,
                 response_deserializer=iotics_dot_api_dot_twin__pb2.ListAllTwinsResponse.FromString,
-                )
+                _registered_method=True)
 
 
 class TwinAPIServicer(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     TwinAPI enables creation and management of Iotics twins.
     Services only affect local resources, unless stated otherwise.
@@ -134,14 +134,15 @@
                     request_deserializer=iotics_dot_api_dot_twin__pb2.ListAllTwinsRequest.FromString,
                     response_serializer=iotics_dot_api_dot_twin__pb2.ListAllTwinsResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'iotics.api.TwinAPI', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
+    server.add_registered_method_handlers('iotics.api.TwinAPI', rpc_method_handlers)
 
 
  # This class is part of an EXPERIMENTAL API.
 class TwinAPI(object):
     """---------------------------------------------------------------------------------------------------------------------
 
     TwinAPI enables creation and management of Iotics twins.
@@ -155,97 +156,157 @@
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.TwinAPI/CreateTwin',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.TwinAPI/CreateTwin',
             iotics_dot_api_dot_twin__pb2.CreateTwinRequest.SerializeToString,
             iotics_dot_api_dot_twin__pb2.CreateTwinResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def UpsertTwin(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.TwinAPI/UpsertTwin',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.TwinAPI/UpsertTwin',
             iotics_dot_api_dot_twin__pb2.UpsertTwinRequest.SerializeToString,
             iotics_dot_api_dot_twin__pb2.UpsertTwinResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def DeleteTwin(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.TwinAPI/DeleteTwin',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.TwinAPI/DeleteTwin',
             iotics_dot_api_dot_twin__pb2.DeleteTwinRequest.SerializeToString,
             iotics_dot_api_dot_twin__pb2.DeleteTwinResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def UpdateTwin(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.TwinAPI/UpdateTwin',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.TwinAPI/UpdateTwin',
             iotics_dot_api_dot_twin__pb2.UpdateTwinRequest.SerializeToString,
             iotics_dot_api_dot_twin__pb2.UpdateTwinResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def DescribeTwin(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.TwinAPI/DescribeTwin',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.TwinAPI/DescribeTwin',
             iotics_dot_api_dot_twin__pb2.DescribeTwinRequest.SerializeToString,
             iotics_dot_api_dot_twin__pb2.DescribeTwinResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
 
     @staticmethod
     def ListAllTwins(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/iotics.api.TwinAPI/ListAllTwins',
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            '/iotics.api.TwinAPI/ListAllTwins',
             iotics_dot_api_dot_twin__pb2.ListAllTwinsRequest.SerializeToString,
             iotics_dot_api_dot_twin__pb2.ListAllTwinsResponse.FromString,
-            options, channel_credentials,
-            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
+            metadata,
+            _registered_method=True)
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/lib/__init__.py` & `iotics-grpc-client-6.0.0/src/iotics/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-5.0.0/src/iotics/lib/grpc/__init__.py` & `iotics-grpc-client-6.0.0/src/iotics/lib/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-5.0.0/src/iotics/lib/grpc/auth.py` & `iotics-grpc-client-6.0.0/src/iotics/lib/grpc/auth.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-5.0.0/src/iotics/lib/grpc/base.py` & `iotics-grpc-client-6.0.0/src/iotics/lib/grpc/base.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-5.0.0/src/iotics/lib/grpc/feeds.py` & `iotics-grpc-client-6.0.0/src/iotics/lib/grpc/feeds.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-5.0.0/src/iotics/lib/grpc/helpers.py` & `iotics-grpc-client-6.0.0/src/iotics/lib/grpc/helpers.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-5.0.0/src/iotics/lib/grpc/host.py` & `iotics-grpc-client-6.0.0/src/iotics/lib/grpc/host.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-5.0.0/src/iotics/lib/grpc/input.py` & `iotics-grpc-client-6.0.0/src/iotics/lib/grpc/input.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-5.0.0/src/iotics/lib/grpc/interest.py` & `iotics-grpc-client-6.0.0/src/iotics/lib/grpc/interest.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-5.0.0/src/iotics/lib/grpc/iotics_api.py` & `iotics-grpc-client-6.0.0/src/iotics/lib/grpc/iotics_api.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-5.0.0/src/iotics/lib/grpc/search.py` & `iotics-grpc-client-6.0.0/src/iotics/lib/grpc/search.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-5.0.0/src/iotics/lib/grpc/sparql.py` & `iotics-grpc-client-6.0.0/src/iotics/lib/grpc/sparql.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,26 +32,25 @@
             self,
             query: str,
             result_content_type: meta_pb2.SparqlResultType = meta_pb2.SparqlResultType.SPARQL_JSON,
             scope: common_pb2.Scope = common_pb2.Scope.LOCAL,
             timeout: int = 5,
             headers: typing.Optional[common_pb2.Headers] = None
     ) -> meta_pb2.SparqlQueryResponse:
-        """Submit a SPARQL query to the network of IOTIC Hosts and receive a chunked stream of responses
+        """Submit a SPARQL query against the Federated Knowledge Graph of the Iotics network and receive a chunked stream of responses.
 
         Args:
             query: the SPARQL query to submit
             result_content_type: Choice of response type among SPARQL_JSON, SPARQL_XML, SPARQL_CSV, RDF_TURTLE, RDF_XML,
                 and RDF_NTRIPLES
             scope: GLOBAL or LOCAL, whether to submit this query to only the local host or all hosts on the network
             timeout: How long to wait for responses, in seconds
             headers: optional request headers
 
-        Returns: A result chunk with details of what host it came from, where it is in that host's sequence, and whether
-        it is the last chunk
+        Returns: A result chunk with details of where it is in the sequence, and whether it is the last chunk
         """
         req = meta_pb2.SparqlQueryRequest(
             headers=headers or create_headers(),
             payload=meta_pb2.SparqlQueryRequest.Payload(
                 query=query.encode('utf-8'),
                 resultContentType=result_content_type
             ), scope=scope
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics/lib/grpc/twins.py` & `iotics-grpc-client-6.0.0/src/iotics/lib/grpc/twins.py`

 * *Files identical despite different names*

### Comparing `iotics-grpc-client-5.0.0/src/iotics_grpc_client.egg-info/PKG-INFO` & `iotics-grpc-client-6.0.0/src/iotics_grpc_client.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,129 +1,129 @@
 Metadata-Version: 2.1
 Name: iotics-grpc-client
-Version: 5.0.0
+Version: 6.0.0
 Summary: Iotics gRPC client library
 Home-page: https://github.com/Iotic-Labs/iotics-grpc-client-py
 Author: Iotics
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Iotic-Labs/iotics-grpc-client-py/issues
 Project-URL: Changelog, https://github.com/Iotic-Labs/iotics-grpc-client-py/releases
 Description: # Iotics gRPC Python Client
-        A Python library for interacting with Iotics API.
         
+        A Python library for interacting with Iotics API.
         
-        ## Usage and Version Compatibility with Iotics host:
+        ## Usage and Version Compatibility with Iotics host
         
         | iotics-grpc-client-py | iotics-host |
         |----------------------| ----------- |
+        |      `pip install iotics-grpc-client~=6.0`       | `>= 7`       |
         |      `pip install iotics-grpc-client~=5.0`       | `>= 6`       |
         |      `pip install iotics-grpc-client~=4.0`       | `>= 6`       |
         |      `pip install iotics-grpc-client~=3.0`       | `>= 6`       |
         |      `pip install iotics-grpc-client~=2.0`       | `>= 5`       |
-        |      `pip install iotics-grpc-client~=0.10.0`      | `>= 4`     |
+        |      `pip install iotics-grpc-client~=0.10.0`    | `>= 4`       |
         
+        ## Examples
         
+        ### Configuring identity
         
-        # Examples
-        ## Configuring identity
         To run examples, either set up required environment variables or create an `.env` file with the following values. For
-        more information on the meaning of these values and how to create them, consult https://docs.iotics.com/docs/identity-api-and-credentials
+        more information on the meaning of these values and how to create them, consult [identity-api-and-credentials](https://docs.iotics.com/docs/identity-api-and-credentials)
+        
         * __Required__:
           * `SPACE` - Domain name of the IOTICSpace with which to communicate. The scheme can be omitted, eg. examplecorp.
             iotics.space
           * `USER_DID` - Identity of the user
           * `AGENT_DID` - Identity of the agent authorised to operate on the user's behalf
           * `AGENT_KEY_NAME` - __secret__ value used to (re)create multiple key pairs
           * `AGENT_NAME` - registered identity name that can be used to e.g. identify public keys
           * `AGENT_SECRET` - __secret__ value, the agent's private key
         
         * __Optional__:
-          * `DID_RESOLVER_URL` - Where the database of identity documents is accessible, defaults to the one used by the given 
+          * `DID_RESOLVER_URL` - Where the database of identity documents is accessible, defaults to the one used by the given
             space.
           * `TOKEN_TTL` - How long in seconds auth tokens will last if not specified in the method call, defaults to 30
-        ## Running example scripts
-        Next, create and activate your virtual environment and run any of the scripts in the [examples](https://github.com/Iotic-Labs/iotics-grpc-client-py/tree/main/examples) directory, 
+        
+        ### Running example scripts
+        
+        Next, create and activate your virtual environment and run any of the scripts in the [examples](https://github.com/Iotic-Labs/iotics-grpc-client-py/tree/main/examples) directory,
         e.g.:
-        ```bash
+        
+        ```shell
         make deps-py
         . env/bin/activate
         python examples/search_twin_models.py
         ```
         
+        ## FAQs
         
-        # FAQs
-        
-        ## Installing on Raspberry PI get: Import error GLIBC_2.33 not found
+        ### Installing on Raspberry PI get: Import error GLIBC_2.33 not found
         
         If you see this error running the exmaples on a Rapberry PI, the current workaround is to install Ubuntu for RPi which has a later version of glibc.
         
-        ```bash
+        ```shell
         ImportError: /lib/arm-linux-gnueabihf/libc.so.6: version 'GLIBC_2.33' not found (required by /home/pi/work/starting/iotics-grpc-client-py/env/lib/python3.9/site-packages/grpc/_cython/cygrpc.cpython-39-arm-linux-gnueabihf.so)
         ```
         
+        ## Contributing
         
+        ### Installing dependencies and generating gRPC client
         
-        # Contributing
-        
+        * To satisfy all dependencies, lint proto files and regenerate client files:
         
-        ## Installing dependencies and generating gRPC client
-        * To satisfy all dependencies, lint proto files and regenerate client files (inside a Docker container):
           ```shell
           make build
           ```
-          * To generate gRPC Python files outside a Docker container the following command can be used: `make generate`.
-            Currently, there is no official binary for Python gRPC plugin, but there is one built from the official repository
-            inside the docker (the following will work on Linux machines):
-            ```bash
-            docker run --rm -dit --name iotics-grpc-client-py-builder iotics-grpc-client-py-builder /bin/bash
-            docker cp iotics-grpc-client-py-builder:/bin/protoc-gen-python_grpc env/bin/protoc-gen-python_grpc
-            docker stop iotics-grpc-client-py-builder
-            make generate
-            ```
-        * To update the Iotics API version and regenerate client  
+        
+        * To generate gRPC Python files:
+        
+          ```shell
+          make generate
+          ```
+        
+        * To update the Iotics API version and regenerate client
           (proto files are submoduled in [./iotics-api.git/](./iotics-api.git)
           from [Iotics API](https://github.com/Iotic-Labs/api) repo):
-          ```bash
+        
+          ```shell
           _ver=vX.X.X
           make GIT_TAG=$_ver deps-proto-update build
           # Address usages of the new client in `src`, update "Unreleased" section in CHANGELOG.md, then:
           git add CHANGELOG.md iotics-api.git src
           git commit -m "Update Iotics API to $_ver"
           # Push your branch and create a PR
           ```
+        
         * Other `make` commands:
           * `clean` - remove artifacts created inside the project.
           * `deps-*` - install specific requirements if missing.
           * `deps-*-update` - update specific requirements when applicable.
         
+        ### PRs
         
-        ## PRs
         Should contain a summary of the changes in [CHANGELOG.md](https://github.com/Iotic-Labs/iotics-grpc-client-py/blob/main/CHANGELOG.md) under the "Unreleased" section.
         
-        
-        ## Versioning
+        ### Versioning
         
         This package adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html)
         
+        ### Releasing
         
-        ## Releasing
         * Update package version in [setup.cfg](./setup.cfg) for the release:
         * Update [CHANGELOG.md](./CHANGELOG.md) (move notes from unreleased section, ensure right tags are used, etc.)
           and any other files as needed.
         * Commit changes and create a [PR](https://github.com/Iotic-Labs/iotics-grpc-client-py/compare).
         * Once PR is merged manually run the [Create Draft Release GitHub Action](https://github.com/Iotic-Labs/iotics-grpc-client-py/actions/workflows/draft_release.yml), this will create a tag with the version in setup.py and create a draft release in [releases](https://github.com/Iotic-Labs/iotics-grpc-client-py/releases).
         * Update the release's information and press the publish button on the release to publish it.
         * The [Publish GitHub Action](https://github.com/Iotic-Labs/iotics-grpc-client-ts/actions/workflows/publish.yml)
           will create a package and will publish it to [PyPI](https://pypi.org/project/iotics-grpc-client).
         
+        ## License
         
-        # License
-        
-        Copyright © 2022 IOTIC LABS LTD. info@iotics.com. All rights reserved. Licensed under the Apache License, Version 2.0. See [LICENSE](https://github.com/Iotic-Labs/iotics-grpc-client-py/tree/main/LICENSE) in the project root for license information.
-        
+        Copyright © 2024 IOTIC LABS LTD. info@iotics.com. All rights reserved. Licensed under the Apache License, Version 2.0. See [LICENSE](https://github.com/Iotic-Labs/iotics-grpc-client-py/tree/main/LICENSE) in the project root for license information.
         
 Keywords: iotics,grpc,digital twin
 Platform: any
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `iotics-grpc-client-5.0.0/src/iotics_grpc_client.egg-info/SOURCES.txt` & `iotics-grpc-client-6.0.0/src/iotics_grpc_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

