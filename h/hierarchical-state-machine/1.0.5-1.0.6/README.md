# Comparing `tmp/hierarchical_state_machine-1.0.5.tar.gz` & `tmp/hierarchical_state_machine-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hierarchical_state_machine-1.0.5.tar", last modified: Fri May 31 16:57:16 2024, max compression
+gzip compressed data, was "hierarchical_state_machine-1.0.6.tar", last modified: Fri May 31 17:33:53 2024, max compression
```

## Comparing `hierarchical_state_machine-1.0.5.tar` & `hierarchical_state_machine-1.0.6.tar`

### file list

```diff
@@ -1,5 +1,14 @@
--rw-r--r--   0        0        0     1087 2024-05-30 18:04:28.128791 hierarchical_state_machine-1.0.5/LICENSE.txt
--rw-r--r--   0        0        0      241 2024-05-29 21:28:23.126922 hierarchical_state_machine-1.0.5/README.md
--rw-r--r--   0        0        0     2493 2024-05-31 16:57:16.605032 hierarchical_state_machine-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 14:52:45.418130 hierarchical_state_machine-1.0.5/tests/__init__.py
--rw-r--r--   0        0        0     3697 1970-01-01 00:00:00.000000 hierarchical_state_machine-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-30 18:04:28.128791 hierarchical_state_machine-1.0.6/LICENSE.txt
+-rw-r--r--   0        0        0      241 2024-05-29 21:28:23.126922 hierarchical_state_machine-1.0.6/README.md
+-rw-r--r--   0        0        0     2557 2024-05-31 17:33:53.025970 hierarchical_state_machine-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 17:33:23.395851 hierarchical_state_machine-1.0.6/src/hierarchical_state_machine/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:11:19.164310 hierarchical_state_machine-1.0.6/src/hierarchical_state_machine/example/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:11:19.164310 hierarchical_state_machine-1.0.6/src/hierarchical_state_machine/example/pedestrian_crosswalk/__init__.py
+-rw-r--r--   0        0        0       58 2024-05-30 14:24:26.019014 hierarchical_state_machine-1.0.6/src/hierarchical_state_machine/example/pedestrian_crosswalk/__main__.py
+-rw-r--r--   0        0        0    11124 2023-08-27 15:51:55.551817 hierarchical_state_machine-1.0.6/src/hierarchical_state_machine/example/pedestrian_crosswalk/ascii_crosswalk.py
+-rw-r--r--   0        0        0     6890 2023-08-28 02:06:54.516126 hierarchical_state_machine-1.0.6/src/hierarchical_state_machine/example/pedestrian_crosswalk/crosswalk_light_simulator.py
+-rw-r--r--   0        0        0    42622 2023-08-28 02:01:54.608211 hierarchical_state_machine-1.0.6/src/hierarchical_state_machine/example/pedestrian_crosswalk/hierarchical_example_pedestrian_crosswalk_signaler.png
+-rw-r--r--   0        0        0    18560 2023-08-28 02:10:52.404931 hierarchical_state_machine-1.0.6/src/hierarchical_state_machine/state_machine.py
+-rw-r--r--   0        0        0    17122 2023-08-26 19:58:34.146079 hierarchical_state_machine-1.0.6/src/hierarchical_state_machine/state_machine_state.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:52:45.418130 hierarchical_state_machine-1.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     3697 1970-01-01 00:00:00.000000 hierarchical_state_machine-1.0.6/PKG-INFO
```

### Comparing `hierarchical_state_machine-1.0.5/LICENSE.txt` & `hierarchical_state_machine-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hierarchical_state_machine-1.0.5/pyproject.toml` & `hierarchical_state_machine-1.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 build-backend = "pdm.backend"
 requires = [
     "pdm-backend",
 ]
 
 [project]
-name = "hierarchical_state_machine"
-version = "1.0.5"
+name = "hierarchical-state-machine"
+version = "1.0.6"
 description = "This python library provides an easy-to-learn and easy-to-use API for using Hierarchical State Machines in your project. The state machine is defined using a basic JSON string, and includes convenience timers."
 authors = [
     { name = "Dan Tebbs", email = "dantebbs@gmail.com" },
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
@@ -69,10 +69,12 @@
 [tool.pdm]
 distribution = true
 
 [tool.pdm.build]
 packages = [
     "hierarchical_state_machine",
 ]
-includes = [
-    "example/pedestrian_crosswalk/hierarchical_example_pedestrian_crosswalk_signaler.png",
+source-includes = [
+    "src/",
+    "tests/",
+    "src/hierarchical_state_machine/example/pedestrian_crosswalk/hierarchical_example_pedestrian_crosswalk_signaler.png",
 ]
```

### Comparing `hierarchical_state_machine-1.0.5/PKG-INFO` & `hierarchical_state_machine-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: hierarchical_state_machine
-Version: 1.0.5
+Name: hierarchical-state-machine
+Version: 1.0.6
 Summary: This python library provides an easy-to-learn and easy-to-use API for using Hierarchical State Machines in your project. The state machine is defined using a basic JSON string, and includes convenience timers.
 Keywords: hierarchical,state,machine,hsm,State Machine,State-Machine,statemachine,sm
 Author-Email: Dan Tebbs <dantebbs@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Dan Tebbs
```

