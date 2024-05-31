# Comparing `tmp/hierarchical_state_machine-1.0.4.tar.gz` & `tmp/hierarchical_state_machine-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hierarchical_state_machine-1.0.4.tar", last modified: Fri May 31 16:36:36 2024, max compression
+gzip compressed data, was "hierarchical_state_machine-1.0.5.tar", last modified: Fri May 31 16:57:16 2024, max compression
```

## Comparing `hierarchical_state_machine-1.0.4.tar` & `hierarchical_state_machine-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,5 @@
--rw-r--r--   0        0        0     1087 2024-05-30 18:04:28.128791 hierarchical_state_machine-1.0.4/LICENSE
--rw-r--r--   0        0        0      241 2024-05-29 21:28:23.126922 hierarchical_state_machine-1.0.4/README.md
--rw-r--r--   0        0        0     2487 2024-05-31 16:36:36.911745 hierarchical_state_machine-1.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 17:33:23.395851 hierarchical_state_machine-1.0.4/src/hierarchical_state_machine/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 14:11:19.164310 hierarchical_state_machine-1.0.4/src/hierarchical_state_machine/example/__init__.py
--rw-r--r--   0        0        0        0 2024-05-30 14:11:19.164310 hierarchical_state_machine-1.0.4/src/hierarchical_state_machine/example/pedestrian_crosswalk/__init__.py
--rw-r--r--   0        0        0       58 2024-05-30 14:24:26.019014 hierarchical_state_machine-1.0.4/src/hierarchical_state_machine/example/pedestrian_crosswalk/__main__.py
--rw-r--r--   0        0        0    11124 2023-08-27 15:51:55.551817 hierarchical_state_machine-1.0.4/src/hierarchical_state_machine/example/pedestrian_crosswalk/ascii_crosswalk.py
--rw-r--r--   0        0        0     6890 2023-08-28 02:06:54.516126 hierarchical_state_machine-1.0.4/src/hierarchical_state_machine/example/pedestrian_crosswalk/crosswalk_light_simulator.py
--rw-r--r--   0        0        0    42622 2023-08-28 02:01:54.608211 hierarchical_state_machine-1.0.4/src/hierarchical_state_machine/example/pedestrian_crosswalk/hierarchical_example_pedestrian_crosswalk_signaler.png
--rw-r--r--   0        0        0    18560 2023-08-28 02:10:52.404931 hierarchical_state_machine-1.0.4/src/hierarchical_state_machine/state_machine.py
--rw-r--r--   0        0        0    17122 2023-08-26 19:58:34.146079 hierarchical_state_machine-1.0.4/src/hierarchical_state_machine/state_machine_state.py
--rw-r--r--   0        0        0        0 2024-05-30 14:52:45.418130 hierarchical_state_machine-1.0.4/tests/__init__.py
--rw-r--r--   0        0        0     2432 1970-01-01 00:00:00.000000 hierarchical_state_machine-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-30 18:04:28.128791 hierarchical_state_machine-1.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      241 2024-05-29 21:28:23.126922 hierarchical_state_machine-1.0.5/README.md
+-rw-r--r--   0        0        0     2493 2024-05-31 16:57:16.605032 hierarchical_state_machine-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-30 14:52:45.418130 hierarchical_state_machine-1.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     3697 1970-01-01 00:00:00.000000 hierarchical_state_machine-1.0.5/PKG-INFO
```

### Comparing `hierarchical_state_machine-1.0.4/LICENSE` & `hierarchical_state_machine-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hierarchical_state_machine-1.0.4/pyproject.toml` & `hierarchical_state_machine-1.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,30 @@
+[build-system]
+build-backend = "pdm.backend"
+requires = [
+    "pdm-backend",
+]
+
 [project]
 name = "hierarchical_state_machine"
-version = "1.0.4"
+version = "1.0.5"
 description = "This python library provides an easy-to-learn and easy-to-use API for using Hierarchical State Machines in your project. The state machine is defined using a basic JSON string, and includes convenience timers."
-keywords = [
-    "hierarchical",
-    "state",
-    "machine",
-    "hsm",
-    "State Machine",
-    "State-Machine",
-    "statemachine",
-    "sm",
-]
 authors = [
     { name = "Dan Tebbs", email = "dantebbs@gmail.com" },
 ]
+requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
+    "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Topic :: File Formats :: JSON",
     "Topic :: Games/Entertainment",
@@ -42,40 +40,39 @@
     "Topic :: Software Development :: Compilers",
     "Topic :: Software Development :: Disassemblers",
     "Topic :: Software Development :: Embedded Systems",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Hardware :: Hardware Drivers",
 ]
-requires-python = ">=3.8"
-dependencies = [
-    "requests>2",
+keywords = [
+    "hierarchical",
+    "state",
+    "machine",
+    "hsm",
+    "State Machine",
+    "State-Machine",
+    "statemachine",
+    "sm",
 ]
 
+[project.license]
+file = "LICENSE.txt"
+
 [project.optional-dependencies]
 examples = [
     "curses",
 ]
 
 [project.urls]
 Homepage = "https://github.com/dantebbs/hierarchical_state_machine"
 
-[build-system]
-requires = [
-    "pdm-backend",
-]
-build-backend = "pdm.backend"
-
 [tool.pdm]
 distribution = true
 
 [tool.pdm.build]
 packages = [
     "hierarchical_state_machine",
 ]
-source-includes = [
-    "src/",
-    "tests/",
-]
 includes = [
     "example/pedestrian_crosswalk/hierarchical_example_pedestrian_crosswalk_signaler.png",
 ]
```

