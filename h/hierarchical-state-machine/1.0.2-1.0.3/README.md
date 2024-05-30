# Comparing `tmp/hierarchical_state_machine-1.0.2.tar.gz` & `tmp/hierarchical_state_machine-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hierarchical_state_machine-1.0.2.tar", last modified: Thu May 30 18:32:46 2024, max compression
+gzip compressed data, was "hierarchical_state_machine-1.0.3.tar", last modified: Thu May 30 22:15:18 2024, max compression
```

## Comparing `hierarchical_state_machine-1.0.2.tar` & `hierarchical_state_machine-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1087 2024-05-30 18:04:28.128791 hierarchical_state_machine-1.0.2/LICENSE
--rw-r--r--   0        0        0      241 2024-05-29 21:28:23.126922 hierarchical_state_machine-1.0.2/README.md
--rw-r--r--   0        0        0     1189 2024-05-30 18:32:46.156843 hierarchical_state_machine-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 17:33:23.395851 hierarchical_state_machine-1.0.2/src/hierarchical_state_machine/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 14:11:19.164310 hierarchical_state_machine-1.0.2/src/hierarchical_state_machine/example/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 14:11:19.164310 hierarchical_state_machine-1.0.2/src/hierarchical_state_machine/example/pedestrian_crosswalk/__init__.py
--rw-r--r--   0        0        0       58 2024-05-30 14:24:26.019014 hierarchical_state_machine-1.0.2/src/hierarchical_state_machine/example/pedestrian_crosswalk/__main__.py
--rw-r--r--   0        0        0    11124 2023-08-27 15:51:55.551817 hierarchical_state_machine-1.0.2/src/hierarchical_state_machine/example/pedestrian_crosswalk/ascii_crosswalk.py
--rw-r--r--   0        0        0     6890 2023-08-28 02:06:54.516126 hierarchical_state_machine-1.0.2/src/hierarchical_state_machine/example/pedestrian_crosswalk/crosswalk_light_simulator.py
--rw-r--r--   0        0        0    42622 2023-08-28 02:01:54.608211 hierarchical_state_machine-1.0.2/src/hierarchical_state_machine/example/pedestrian_crosswalk/hierarchical_example_pedestrian_crosswalk_signaler.png
--rw-r--r--   0        0        0    18560 2023-08-28 02:10:52.404931 hierarchical_state_machine-1.0.2/src/hierarchical_state_machine/state_machine.py
--rw-r--r--   0        0        0    17122 2023-08-26 19:58:34.146079 hierarchical_state_machine-1.0.2/src/hierarchical_state_machine/state_machine_state.py
--rw-r--r--   0        0        0        0 2024-05-30 14:52:45.418130 hierarchical_state_machine-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 hierarchical_state_machine-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-30 18:04:28.128791 hierarchical_state_machine-1.0.3/LICENSE
+-rw-r--r--   0        0        0      241 2024-05-29 21:28:23.126922 hierarchical_state_machine-1.0.3/README.md
+-rw-r--r--   0        0        0     1238 2024-05-30 22:15:18.766796 hierarchical_state_machine-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 17:33:23.395851 hierarchical_state_machine-1.0.3/src/hierarchical_state_machine/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:11:19.164310 hierarchical_state_machine-1.0.3/src/hierarchical_state_machine/example/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:11:19.164310 hierarchical_state_machine-1.0.3/src/hierarchical_state_machine/example/pedestrian_crosswalk/__init__.py
+-rw-r--r--   0        0        0       58 2024-05-30 14:24:26.019014 hierarchical_state_machine-1.0.3/src/hierarchical_state_machine/example/pedestrian_crosswalk/__main__.py
+-rw-r--r--   0        0        0    11124 2023-08-27 15:51:55.551817 hierarchical_state_machine-1.0.3/src/hierarchical_state_machine/example/pedestrian_crosswalk/ascii_crosswalk.py
+-rw-r--r--   0        0        0     6890 2023-08-28 02:06:54.516126 hierarchical_state_machine-1.0.3/src/hierarchical_state_machine/example/pedestrian_crosswalk/crosswalk_light_simulator.py
+-rw-r--r--   0        0        0    42622 2023-08-28 02:01:54.608211 hierarchical_state_machine-1.0.3/src/hierarchical_state_machine/example/pedestrian_crosswalk/hierarchical_example_pedestrian_crosswalk_signaler.png
+-rw-r--r--   0        0        0    18560 2023-08-28 02:10:52.404931 hierarchical_state_machine-1.0.3/src/hierarchical_state_machine/state_machine.py
+-rw-r--r--   0        0        0    17122 2023-08-26 19:58:34.146079 hierarchical_state_machine-1.0.3/src/hierarchical_state_machine/state_machine_state.py
+-rw-r--r--   0        0        0        0 2024-05-30 14:52:45.418130 hierarchical_state_machine-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      968 1970-01-01 00:00:00.000000 hierarchical_state_machine-1.0.3/PKG-INFO
```

### Comparing `hierarchical_state_machine-1.0.2/LICENSE` & `hierarchical_state_machine-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hierarchical_state_machine-1.0.2/pyproject.toml` & `hierarchical_state_machine-1.0.3/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hierarchical_state_machine"
-version = "1.0.2"
+version = "1.0.3"
 description = "This python library provides an easy-to-learn and easy-to-use API for using Hierarchical State Machines in your project. The state machine is defined using a basic JSON string, and includes convenience timers."
 authors = [
     { name = "Dan Tebbs", email = "dantebbs@gmail.com" },
 ]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -33,14 +33,17 @@
 ]
 build-backend = "pdm.backend"
 
 [tool.pdm]
 distribution = true
 
 [tool.pdm.build]
+packages = [
+    "hierarchical_state_machine",
+]
 source-includes = [
     "src/",
     "tests/",
 ]
 includes = [
     "example/pedestrian_crosswalk/hierarchical_example_pedestrian_crosswalk_signaler.png",
 ]
```

### Comparing `hierarchical_state_machine-1.0.2/src/hierarchical_state_machine/example/pedestrian_crosswalk/ascii_crosswalk.py` & `hierarchical_state_machine-1.0.3/src/hierarchical_state_machine/example/pedestrian_crosswalk/ascii_crosswalk.py`

 * *Files identical despite different names*

### Comparing `hierarchical_state_machine-1.0.2/src/hierarchical_state_machine/example/pedestrian_crosswalk/crosswalk_light_simulator.py` & `hierarchical_state_machine-1.0.3/src/hierarchical_state_machine/example/pedestrian_crosswalk/crosswalk_light_simulator.py`

 * *Files identical despite different names*

### Comparing `hierarchical_state_machine-1.0.2/src/hierarchical_state_machine/example/pedestrian_crosswalk/hierarchical_example_pedestrian_crosswalk_signaler.png` & `hierarchical_state_machine-1.0.3/src/hierarchical_state_machine/example/pedestrian_crosswalk/hierarchical_example_pedestrian_crosswalk_signaler.png`

 * *Files identical despite different names*

### Comparing `hierarchical_state_machine-1.0.2/src/hierarchical_state_machine/state_machine.py` & `hierarchical_state_machine-1.0.3/src/hierarchical_state_machine/state_machine.py`

 * *Files identical despite different names*

### Comparing `hierarchical_state_machine-1.0.2/src/hierarchical_state_machine/state_machine_state.py` & `hierarchical_state_machine-1.0.3/src/hierarchical_state_machine/state_machine_state.py`

 * *Files identical despite different names*

### Comparing `hierarchical_state_machine-1.0.2/PKG-INFO` & `hierarchical_state_machine-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hierarchical_state_machine
-Version: 1.0.2
+Version: 1.0.3
 Summary: This python library provides an easy-to-learn and easy-to-use API for using Hierarchical State Machines in your project. The state machine is defined using a basic JSON string, and includes convenience timers.
 Author-Email: Dan Tebbs <dantebbs@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/dantebbs/hierarchical_state_machine
```

