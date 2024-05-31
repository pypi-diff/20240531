# Comparing `tmp/Supermarq-0.5.8.tar.gz` & `tmp/Supermarq-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Supermarq-0.5.8.tar", last modified: Tue Jan 30 18:47:49 2024, max compression
+gzip compressed data, was "Supermarq-0.5.9.tar", last modified: Fri Feb  9 16:13:53 2024, max compression
```

## Comparing `Supermarq-0.5.8.tar` & `Supermarq-0.5.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:49.890163 Supermarq-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-01-30 18:47:49.890163 Supermarq-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-01-30 18:46:39.000000 Supermarq-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:49.890163 Supermarq-0.5.8/Supermarq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-01-30 18:47:49.000000 Supermarq-0.5.8/Supermarq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-01-30 18:47:49.000000 Supermarq-0.5.8/Supermarq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 18:47:49.000000 Supermarq-0.5.8/Supermarq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-30 18:47:49.000000 Supermarq-0.5.8/Supermarq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-30 18:47:49.000000 Supermarq-0.5.8/Supermarq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-30 18:46:39.000000 Supermarq-0.5.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-01-30 18:46:39.000000 Supermarq-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-30 18:46:39.000000 Supermarq-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 18:47:49.890163 Supermarq-0.5.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:49.886163 Supermarq-0.5.8/supermarq/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/_version_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmark_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 18:47:49.890163 Supermarq-0.5.8/supermarq/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/bit_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/bit_code_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/ghz.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/ghz_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/hamiltonian_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/hamiltonian_simulation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/mermin_bell.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/mermin_bell_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/phase_code.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/phase_code_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/qaoa_fermionic_swap_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/qaoa_fermionic_swap_proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/qaoa_vanilla_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/qaoa_vanilla_proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/vqe_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/benchmarks/vqe_proxy_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4707 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/converters_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/features_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/plotting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/run_benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)    12676 2024-01-30 18:46:39.000000 Supermarq-0.5.8/supermarq/stabilizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:53.957393 Supermarq-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-02-09 16:13:53.957393 Supermarq-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-09 16:12:41.000000 Supermarq-0.5.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:53.957393 Supermarq-0.5.9/Supermarq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2175 2024-02-09 16:13:53.000000 Supermarq-0.5.9/Supermarq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-02-09 16:13:53.000000 Supermarq-0.5.9/Supermarq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-09 16:13:53.000000 Supermarq-0.5.9/Supermarq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-09 16:13:53.000000 Supermarq-0.5.9/Supermarq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-09 16:13:53.000000 Supermarq-0.5.9/Supermarq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-09 16:12:41.000000 Supermarq-0.5.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-02-09 16:12:41.000000 Supermarq-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-09 16:12:41.000000 Supermarq-0.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-09 16:13:53.961393 Supermarq-0.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:53.953393 Supermarq-0.5.9/supermarq/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/_version_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmark_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-09 16:13:53.957393 Supermarq-0.5.9/supermarq/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4191 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/bit_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/bit_code_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/ghz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/ghz_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/hamiltonian_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/hamiltonian_simulation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/mermin_bell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/mermin_bell_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/phase_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/phase_code_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7934 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/qaoa_fermionic_swap_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/qaoa_fermionic_swap_proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/qaoa_vanilla_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/qaoa_vanilla_proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/vqe_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/benchmarks/vqe_proxy_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/converters_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/features_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15564 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/plotting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1976 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/run_benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12676 2024-02-09 16:12:41.000000 Supermarq-0.5.9/supermarq/stabilizers.py
```

### Comparing `Supermarq-0.5.8/PKG-INFO` & `Supermarq-0.5.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: Supermarq
-Version: 0.5.8
+Version: 0.5.9
 Summary: Supermarq is a scalable, application-centric quantum benchmarking suite.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Requires-Dist: cirq-superstaq~=0.5.8
-Requires-Dist: qiskit-superstaq~=0.5.8
+Requires-Dist: cirq-superstaq~=0.5.9
+Requires-Dist: qiskit-superstaq~=0.5.9
 Requires-Dist: scikit-learn>=1.0
 Provides-Extra: dev
-Requires-Dist: checks-superstaq~=0.5.8; extra == "dev"
+Requires-Dist: checks-superstaq~=0.5.9; extra == "dev"
 
 <p align="center">
   <img width="300" src="../docs/source/_static/logos/supermarq-logo.webp">
 </p>
 
 ---
 ![Continuous Integration](https://github.com/Infleqtion/client-superstaq/actions/workflows/ci.yml/badge.svg)
@@ -29,15 +29,15 @@
 
 The Supermarq package is available via `pip` and can be installed in your current Python environment with the command:
 
 ```
 pip install supermarq
 ```
 
-## Install Dev Requirements 
+## Install Dev Requirements
 
 This is required if you intend to run checks locally
 
 ```
 pip install .[dev]
 ```
 
@@ -47,15 +47,15 @@
 The benchmarks are defined as classes within `supermarq/benchmarks/`. Each application
 defines two methods; `circuit` and `score`. These methods are used to generate the benchmarking circuit and evaluate its performance
 after execution on hardware.
 
 The quantum benchmarks within Supermarq are designed to be scalable, meaning that the benchmarks can be
 instantiated and generated for a wide range of circuit sizes and depths.
 
-The [`examples/ghz_example.py`](examples/ghz_example.py) file contains an end-to-end example of how to execute the GHZ benchmark
+The [Supermarq tutorial](examples/Supermarq_HPCA_Tutorial_css.ipynb) notebook contains an end-to-end example of how to execute the GHZ benchmark
 using [Superstaq](https://superstaq.infleqtion.com/). The general workflow is as follows:
 
 ```python
 import supermarq
 
 ghz = supermarq.benchmarks.ghz.GHZ(num_qubits=3)
 ghz_circuit = ghz.circuit()
```

### Comparing `Supermarq-0.5.8/README.md` & `Supermarq-0.5.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 The Supermarq package is available via `pip` and can be installed in your current Python environment with the command:
 
 ```
 pip install supermarq
 ```
 
-## Install Dev Requirements 
+## Install Dev Requirements
 
 This is required if you intend to run checks locally
 
 ```
 pip install .[dev]
 ```
 
@@ -32,15 +32,15 @@
 The benchmarks are defined as classes within `supermarq/benchmarks/`. Each application
 defines two methods; `circuit` and `score`. These methods are used to generate the benchmarking circuit and evaluate its performance
 after execution on hardware.
 
 The quantum benchmarks within Supermarq are designed to be scalable, meaning that the benchmarks can be
 instantiated and generated for a wide range of circuit sizes and depths.
 
-The [`examples/ghz_example.py`](examples/ghz_example.py) file contains an end-to-end example of how to execute the GHZ benchmark
+The [Supermarq tutorial](examples/Supermarq_HPCA_Tutorial_css.ipynb) notebook contains an end-to-end example of how to execute the GHZ benchmark
 using [Superstaq](https://superstaq.infleqtion.com/). The general workflow is as follows:
 
 ```python
 import supermarq
 
 ghz = supermarq.benchmarks.ghz.GHZ(num_qubits=3)
 ghz_circuit = ghz.circuit()
```

### Comparing `Supermarq-0.5.8/Supermarq.egg-info/PKG-INFO` & `Supermarq-0.5.9/Supermarq.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: Supermarq
-Version: 0.5.8
+Version: 0.5.9
 Summary: Supermarq is a scalable, application-centric quantum benchmarking suite.
 Author-email: Superstaq development team <superstaq@infleqtion.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/Infleqtion/client-superstaq
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
-Requires-Dist: cirq-superstaq~=0.5.8
-Requires-Dist: qiskit-superstaq~=0.5.8
+Requires-Dist: cirq-superstaq~=0.5.9
+Requires-Dist: qiskit-superstaq~=0.5.9
 Requires-Dist: scikit-learn>=1.0
 Provides-Extra: dev
-Requires-Dist: checks-superstaq~=0.5.8; extra == "dev"
+Requires-Dist: checks-superstaq~=0.5.9; extra == "dev"
 
 <p align="center">
   <img width="300" src="../docs/source/_static/logos/supermarq-logo.webp">
 </p>
 
 ---
 ![Continuous Integration](https://github.com/Infleqtion/client-superstaq/actions/workflows/ci.yml/badge.svg)
@@ -29,15 +29,15 @@
 
 The Supermarq package is available via `pip` and can be installed in your current Python environment with the command:
 
 ```
 pip install supermarq
 ```
 
-## Install Dev Requirements 
+## Install Dev Requirements
 
 This is required if you intend to run checks locally
 
 ```
 pip install .[dev]
 ```
 
@@ -47,15 +47,15 @@
 The benchmarks are defined as classes within `supermarq/benchmarks/`. Each application
 defines two methods; `circuit` and `score`. These methods are used to generate the benchmarking circuit and evaluate its performance
 after execution on hardware.
 
 The quantum benchmarks within Supermarq are designed to be scalable, meaning that the benchmarks can be
 instantiated and generated for a wide range of circuit sizes and depths.
 
-The [`examples/ghz_example.py`](examples/ghz_example.py) file contains an end-to-end example of how to execute the GHZ benchmark
+The [Supermarq tutorial](examples/Supermarq_HPCA_Tutorial_css.ipynb) notebook contains an end-to-end example of how to execute the GHZ benchmark
 using [Superstaq](https://superstaq.infleqtion.com/). The general workflow is as follows:
 
 ```python
 import supermarq
 
 ghz = supermarq.benchmarks.ghz.GHZ(num_qubits=3)
 ghz_circuit = ghz.circuit()
```

### Comparing `Supermarq-0.5.8/Supermarq.egg-info/SOURCES.txt` & `Supermarq-0.5.9/Supermarq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/pyproject.toml` & `Supermarq-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/__init__.py` & `Supermarq-0.5.9/supermarq/__init__.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/benchmark.py` & `Supermarq-0.5.9/supermarq/benchmark.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import abc
-from collections.abc import Sequence
 from typing import Any
 
 import cirq
+import qiskit
+
+import supermarq
 
 
 class Benchmark:
     """Class representing a quantum benchmark application.
 
     Concrete subclasses must implement the abstract methods ``circuit()`` and
     ``score()``.
@@ -16,17 +18,28 @@
     Each instantiation of a `Benchmark` object represents a single, fully defined
     benchmark application. All the relevant parameters for a benchmark should
     be passed in upon creation, and will be used to generate the correct circuit
     and compute the final score.
     """
 
     @abc.abstractmethod
-    def circuit(self) -> cirq.Circuit | Sequence[cirq.Circuit]:
-        """Returns the quantum circuit corresponding to the current benchmark parameters."""
+    def circuit(self) -> cirq.Circuit | list[cirq.Circuit]:
+        """Returns the quantum circuit(s) corresponding to the current benchmark parameters."""
+
+    def cirq_circuit(self) -> cirq.Circuit | list[cirq.Circuit]:
+        """Returns the cirq circuit(s) corresponding to the current benchmark parameters."""
+        return self.circuit()
+
+    def qiskit_circuit(self) -> qiskit.QuantumCircuit | list[qiskit.QuantumCircuit]:
+        """Returns the qiskit circuit(s) corresponding to the current benchmark parameters."""
+        cirq_circuit = self.cirq_circuit()
+        if isinstance(cirq_circuit, cirq.Circuit):
+            return supermarq.converters.cirq_to_qiskit(cirq_circuit)
+        return [supermarq.converters.cirq_to_qiskit(c) for c in cirq_circuit]
 
     @abc.abstractmethod
     def score(self, counts: Any) -> float:
         """Returns a normalized [0,1] score reflecting device performance.
 
         Args:
-            counts: A dictionary containing the measurement counts from execution.
+            counts: Dictionary(s) containing the measurement counts from execution.
         """
```

### Comparing `Supermarq-0.5.8/supermarq/benchmark_test.py` & `Supermarq-0.5.9/supermarq/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/benchmarks/bit_code.py` & `Supermarq-0.5.9/supermarq/benchmarks/bit_code.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from collections.abc import Iterator
 
 import cirq
-from qiskit.quantum_info import hellinger_fidelity
+import qiskit
 
 from supermarq.benchmark import Benchmark
 
 
 class BitCode(Benchmark):
     """Creates a circuit for syndrome measurement in a bit-flip error correcting code.
 
@@ -104,8 +104,8 @@
 
         Returns:
             A float with the computed score.
         """
         ideal_dist = self._get_ideal_dist()
         total_shots = sum(counts.values())
         experimental_dist = {bitstr: shots / total_shots for bitstr, shots in counts.items()}
-        return hellinger_fidelity(ideal_dist, experimental_dist)
+        return qiskit.quantum_info.hellinger_fidelity(ideal_dist, experimental_dist)
```

### Comparing `Supermarq-0.5.8/supermarq/benchmarks/bit_code_test.py` & `Supermarq-0.5.9/supermarq/benchmarks/bit_code_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/benchmarks/ghz.py` & `Supermarq-0.5.9/supermarq/benchmarks/ghz.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import cirq
+import qiskit
 from qiskit.quantum_info import hellinger_fidelity
 
 from supermarq.benchmark import Benchmark
 
 
 class GHZ(Benchmark):
     """Represents the GHZ state preparation benchmark parameterized by the number of qubits n.
@@ -18,28 +19,42 @@
 
         Args:
             num_qubits: Number of qubits in GHZ circuit.
         """
         self.num_qubits = num_qubits
 
     def circuit(self) -> cirq.Circuit:
-        """Generate an n-qubit GHZ circuit.
+        """Generate an n-qubit GHZ cirq circuit.
 
         Returns:
             A `cirq.Circuit`.
         """
         qubits = cirq.LineQubit.range(self.num_qubits)
         circuit = cirq.Circuit()
         circuit.append(cirq.H(qubits[0]))
         for i in range(self.num_qubits - 1):
             circuit.append(cirq.CNOT(qubits[i], qubits[i + 1]))
         circuit.append(cirq.measure(*qubits))
         return circuit
 
-    def score(self, counts: dict[str, int]) -> float:
+    def qiskit_circuit(self) -> qiskit.QuantumCircuit:
+        """Generate an n-qubit GHZ qiskit circuit.
+
+        Returns:
+            A `qiskit.QuantumCircuit`.
+        """
+        circuit = qiskit.QuantumCircuit(self.num_qubits, self.num_qubits)
+        circuit.h(0)
+        for i in range(self.num_qubits - 1):
+            circuit.cx(i, i + 1)
+        for i in range(self.num_qubits):
+            circuit.measure(i, i)
+        return circuit
+
+    def score(self, counts: dict[str, float]) -> float:
         r"""Compute the Hellinger fidelity between the experimental and ideal results.
 
         The ideal results are 50% probabilty of measuring the all-zero state and 50% probability
         of measuring the all-one state.
 
         The formula for the Hellinger fidelity between two distributions p and q is given by
         $(\sum_i{p_i q_i})^2$.
```

### Comparing `Supermarq-0.5.8/supermarq/benchmarks/hamiltonian_simulation.py` & `Supermarq-0.5.9/supermarq/benchmarks/hamiltonian_simulation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from collections.abc import Mapping
 
 import cirq
 import numpy as np
+import qiskit
 
 import supermarq
 from supermarq.benchmark import Benchmark
 
 
 class HamiltonianSimulation(Benchmark):
     """Quantum benchmark focused on the ability to simulate 1D
@@ -17,28 +18,27 @@
     average magnetization (along the Z-axis) matches the noiseless value.
     Since the 1D TFIM is efficiently simulatable with classical algorithms,
     computing the noiseless average magnetization remains scalable over a large
     range of benchmark sizes.
     """
 
     def __init__(self, num_qubits: int, time_step: int = 1, total_time: int = 1) -> None:
-        """Args:
-        num_qubits: int
-            Size of the TFIM chain, equivalent to the number of qubits.
-        time_step: int
-            Size of the timestep in attoseconds.
-        total_time:
-            Total simulation time of the TFIM chain in attoseconds.
+        """Initializes a `HamiltonianSimulation`.
+
+        Args:
+            num_qubits: Size of the TFIM chain, equivalent to the number of qubits.
+            time_step: Size of the timestep in attoseconds. Defaults to 1.
+            total_time: Total simulation time of the TFIM chain in attoseconds. Defaults to 1.
         """
         self.num_qubits = num_qubits
         self.time_step = time_step
         self.total_time = total_time
 
     def circuit(self) -> cirq.Circuit:
-        """Generate a circuit to simulate the evolution of an n-qubit TFIM
+        """Generates a circuit to simulate the evolution of an n-qubit TFIM
         chain under the Hamiltonian:
 
         H(t) = - Jz * sum_{i=1}^{n-1}(sigma_{z}^{i} * sigma_{z}^{i+1})
                - e_ph * cos(w_ph * t) * sum_{i=1}^{n}(sigma_{x}^{i})
 
         where,
             w_ph: frequency of E" phonon in MoSe2.
@@ -79,14 +79,64 @@
                 circuit.append(cirq.CNOT(qubits[i], qubits[i + 1]))
 
         # End the circuit with measurements of every qubit in the Z-basis
         circuit.append(cirq.measure(*qubits))
 
         return circuit
 
+    def qiskit_circuit(self) -> qiskit.QuantumCircuit:
+        """Generates a circuit to simulate the evolution of an n-qubit TFIM
+        chain under the Hamiltonian:
+
+        H(t) = - Jz * sum_{i=1}^{n-1}(sigma_{z}^{i} * sigma_{z}^{i+1})
+               - e_ph * cos(w_ph * t) * sum_{i=1}^{n}(sigma_{x}^{i})
+
+        where,
+            w_ph: frequency of E" phonon in MoSe2.
+            e_ph: strength of electron-phonon coupling.
+
+        Returns:
+            The circuit for Hamiltonian simulation.
+        """
+        hbar = 0.658212  # eV*fs
+        jz = (
+            hbar * np.pi / 4
+        )  # eV, coupling coeff; Jz<0 is antiferromagnetic, Jz>0 is ferromagnetic
+        freq = 0.0048  # 1/fs, frequency of MoSe2 phonon
+
+        w_ph = 2 * np.pi * freq
+        e_ph = 3 * np.pi * hbar / (8 * np.cos(np.pi * freq))
+
+        circuit = qiskit.QuantumCircuit(self.num_qubits, self.num_qubits)
+
+        # Build up the circuit over total_time / time_step propagation steps
+        for step in range(int(self.total_time / self.time_step)):
+            # Simulate the Hamiltonian term-by-term
+            t = (step + 0.5) * self.time_step
+
+            # Single qubit terms
+            psi = -2.0 * e_ph * np.cos(w_ph * t) * self.time_step / hbar
+            for i in range(self.num_qubits):
+                circuit.h(i)
+                circuit.rz(psi, i)
+                circuit.h(i)
+
+            # Coupling terms
+            psi2 = -2.0 * jz * self.time_step / hbar
+            for i in range(self.num_qubits - 1):
+                circuit.cnot(i, i + 1)
+                circuit.rz(psi2, i + 1)
+                circuit.cnot(i, i + 1)
+
+        # End the circuit with measurements of every qubit in the Z-basis
+        for i in range(self.num_qubits):
+            circuit.measure(i, i)
+
+        return circuit
+
     def _average_magnetization(self, result: Mapping[str, float], shots: int) -> float:
         mag = 0.0
         for spin_str, count in result.items():
             spin_int = [1 - 2 * int(s) for s in spin_str]
             mag += (
                 sum(spin_int) / len(spin_int)
             ) * count  # <Z> weighted by number of times we saw this bitstring
```

### Comparing `Supermarq-0.5.8/supermarq/benchmarks/hamiltonian_simulation_test.py` & `Supermarq-0.5.9/supermarq/benchmarks/hamiltonian_simulation_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import supermarq
 from supermarq.benchmarks.hamiltonian_simulation import HamiltonianSimulation
 
 
 def test_hamiltonian_simulation_circuit() -> None:
     hs = HamiltonianSimulation(4, 1, 1)
     assert len(hs.circuit().all_qubits()) == 4
+    assert hs.qiskit_circuit().num_qubits == 4
 
 
 def test_hamiltonian_simulation_score() -> None:
     hs = HamiltonianSimulation(4, 1, 1)
     assert hs._average_magnetization({"1111": 1}, 1) == -1.0
     assert hs._average_magnetization({"0000": 1}, 1) == 1.0
     assert hs.score(supermarq.simulation.get_ideal_counts(hs.circuit())) > 0.99
```

### Comparing `Supermarq-0.5.8/supermarq/benchmarks/mermin_bell.py` & `Supermarq-0.5.9/supermarq/benchmarks/mermin_bell.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,29 +14,33 @@
     """The Mermin-Bell benchmark is a test of a quantum computer's ability to exploit purely quantum
     phenomemna such as superposition and entanglement. It is based on the famous Bell-inequality
     tests of locality. Performance is based on a QPU's ability to prepare a GHZ state and measure
     the Mermin operator.
     """
 
     def __init__(self, num_qubits: int) -> None:
+        """Initializes a `MerminBell`.
+
+        Args:
+            num_qubits: The number of qubits.
+        """
         self.num_qubits = num_qubits
         self.qubits = cirq.LineQubit.range(self.num_qubits)
 
         self.mermin_operator = self._mermin_operator(self.num_qubits)
         self.stabilizer, self.pauli_basis = stabilizers.construct_stabilizer(
             self.num_qubits, self.mermin_operator
         )
 
     def circuit(self) -> cirq.Circuit:
         """The Mermin-Bell circuit, simultaneously measuring Mermin terms in a GHZ circuit.
 
         Returns:
             The Mermin-Bell `cirq.Circuit`.
         """
-
         circuit = cirq.Circuit()
 
         # Create a GHZ state
         circuit.append(cirq.rx(-np.pi / 2).on(self.qubits[0]))
         for i in range(self.num_qubits - 1):
             circuit.append(cirq.CNOT(self.qubits[i], self.qubits[i + 1]))
```

### Comparing `Supermarq-0.5.8/supermarq/benchmarks/mermin_bell_test.py` & `Supermarq-0.5.9/supermarq/benchmarks/mermin_bell_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 # pylint: disable=missing-function-docstring,missing-class-docstring
+from unittest.mock import patch
+
+import qiskit
+
 import supermarq
 from supermarq.benchmarks.mermin_bell import MerminBell
 
 
 def test_mermin_bell_circuit() -> None:
     mb = MerminBell(3)
     assert len(mb.circuit().all_qubits()) == 3
 
     mb = MerminBell(4)
     assert len(mb.circuit().all_qubits()) == 4
 
     mb = MerminBell(5)
     assert len(mb.circuit().all_qubits()) == 5
+    qiskit_circuit = mb.qiskit_circuit()
+    if isinstance(qiskit_circuit, qiskit.QuantumCircuit):
+        assert qiskit_circuit.num_qubits == 5
+    with patch(
+        "supermarq.benchmarks.mermin_bell.MerminBell.circuit",
+        return_value=[mb.circuit()],
+    ):
+        assert mb.qiskit_circuit()[0].num_qubits == 5
 
 
 def test_mermin_bell_score() -> None:
     mb = MerminBell(3)
     assert mb.score(supermarq.simulation.get_ideal_counts(mb.circuit())) == 1
 
     mb = MerminBell(4)
```

### Comparing `Supermarq-0.5.8/supermarq/benchmarks/phase_code.py` & `Supermarq-0.5.9/supermarq/benchmarks/phase_code.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/benchmarks/phase_code_test.py` & `Supermarq-0.5.9/supermarq/benchmarks/phase_code_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/benchmarks/qaoa_fermionic_swap_proxy.py` & `Supermarq-0.5.9/supermarq/benchmarks/qaoa_fermionic_swap_proxy.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/benchmarks/qaoa_fermionic_swap_proxy_test.py` & `Supermarq-0.5.9/supermarq/benchmarks/qaoa_fermionic_swap_proxy_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/benchmarks/qaoa_vanilla_proxy.py` & `Supermarq-0.5.9/supermarq/benchmarks/qaoa_vanilla_proxy.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/benchmarks/qaoa_vanilla_proxy_test.py` & `Supermarq-0.5.9/supermarq/benchmarks/qaoa_vanilla_proxy_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/benchmarks/vqe_proxy.py` & `Supermarq-0.5.9/supermarq/benchmarks/vqe_proxy.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/converters.py` & `Supermarq-0.5.9/supermarq/converters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import cirq
 import networkx as nx
 import numpy as np
 import qiskit
 
 
-def cirq_to_qiskit(circuit: cirq.Circuit) -> qiskit.circuit.QuantumCircuit:
+def cirq_to_qiskit(circuit: cirq.Circuit) -> qiskit.QuantumCircuit:
     """Convert a circuit from cirq to qiskit.
 
     Args:
         circuit: A `cirq.Circuit` to be converted.
 
     Returns:
         An equivalent `qiskit.QuantumCircuit`.
     """
     qasm = cirq.circuits.QasmOutput(circuit, tuple(sorted(circuit.all_qubits())))
     return qiskit.circuit.QuantumCircuit().from_qasm_str(str(qasm))
 
 
-def compute_communication_with_qiskit(circuit: qiskit.circuit.QuantumCircuit) -> float:
+def compute_communication_with_qiskit(circuit: qiskit.QuantumCircuit) -> float:
     """Compute the program communication of the given quantum circuit.
 
     Program communication = circuit's average qubit degree / degree of a complete graph.
 
     Args:
         circuit: A quantum circuit.
 
@@ -38,15 +38,15 @@
         graph.add_edge(circuit.find_bit(q1).index, circuit.find_bit(q2).index)
 
     degree_sum = sum([graph.degree(n) for n in graph.nodes])
 
     return degree_sum / (num_qubits * (num_qubits - 1))
 
 
-def compute_liveness_with_qiskit(circuit: qiskit.circuit.QuantumCircuit) -> float:
+def compute_liveness_with_qiskit(circuit: qiskit.QuantumCircuit) -> float:
     """Compute the liveness of the given quantum circuit.
 
     Liveness feature = sum of all entries in the liveness matrix / (num_qubits * depth).
 
     Args:
         circuit: A quantum circuit.
 
@@ -64,15 +64,15 @@
         for op in layer["partition"]:
             for qubit in op:
                 activity_matrix[circuit.find_bit(qubit).index, i] = 1
 
     return np.sum(activity_matrix) / (num_qubits * dag.depth())
 
 
-def compute_parallelism_with_qiskit(circuit: qiskit.circuit.QuantumCircuit) -> float:
+def compute_parallelism_with_qiskit(circuit: qiskit.QuantumCircuit) -> float:
     """Compute the parallelism of the given quantum circuit.
 
     Parallelism feature = max(1 - depth / # of gates, 0).
 
     Args:
         circuit: A quantum circuit.
 
@@ -80,15 +80,15 @@
         The value of the parallelism feature for this circuit.
     """
     dag = qiskit.converters.circuit_to_dag(circuit)
     dag.remove_all_ops_named("barrier")
     return max(1 - (circuit.depth() / len(dag.gate_nodes())), 0)
 
 
-def compute_measurement_with_qiskit(circuit: qiskit.circuit.QuantumCircuit) -> float:
+def compute_measurement_with_qiskit(circuit: qiskit.QuantumCircuit) -> float:
     """Compute the measurement feature of the given quantum circuit.
 
     Measurement feature = # of layers of mid-circuit measurement / circuit depth.
 
     Args:
         circuit: A quantum circuit.
 
@@ -109,15 +109,15 @@
                 reset_present = True
         if reset_present:
             reset_moments += 1
 
     return reset_moments / gate_depth
 
 
-def compute_entanglement_with_qiskit(circuit: qiskit.circuit.QuantumCircuit) -> float:
+def compute_entanglement_with_qiskit(circuit: qiskit.QuantumCircuit) -> float:
     """Compute the entanglement-ratio of the given quantum circuit.
 
     Entanglement-ratio = ratio between # of 2-qubit gates and total number of gates in the
     circuit.
 
     Args:
         circuit: A quantum circuit.
@@ -127,33 +127,34 @@
     """
     dag = qiskit.converters.circuit_to_dag(circuit)
     dag.remove_all_ops_named("barrier")
 
     return len(dag.two_qubit_ops()) / len(dag.gate_nodes())
 
 
-def compute_depth_with_qiskit(circuit: qiskit.circuit.QuantumCircuit) -> float:
+def compute_depth_with_qiskit(circuit: qiskit.QuantumCircuit) -> float:
     """Compute the critical depth of the given quantum circuit.
 
     Critical depth = # of 2-qubit gates along the critical path / total # of 2-qubit gates.
 
     Args:
         circuit: A quantum circuit.
 
     Returns:
         The value of the depth feature for this circuit.
     """
     dag = qiskit.converters.circuit_to_dag(circuit)
     dag.remove_all_ops_named("barrier")
-    n_ed = 0
-    two_q_gates = {op.name for op in dag.two_qubit_ops()}
-    for name in two_q_gates:
-        try:
-            n_ed += dag.count_ops_longest_path()[name]
-        except KeyError:
-            continue
+    longest_paths = dag.count_ops_longest_path()
+    n_ed = sum(
+        [
+            longest_paths[name]
+            for name in {op.name for op in dag.two_qubit_ops()}
+            if name in longest_paths
+        ]
+    )
     n_e = len(dag.two_qubit_ops())
 
     if n_ed == 0:
         return 0
 
     return n_ed / n_e
```

### Comparing `Supermarq-0.5.8/supermarq/features.py` & `Supermarq-0.5.9/supermarq/features.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/features_test.py` & `Supermarq-0.5.9/supermarq/features_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/plotting.py` & `Supermarq-0.5.9/supermarq/plotting.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/plotting_test.py` & `Supermarq-0.5.9/supermarq/plotting_test.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/run_benchmarks.py` & `Supermarq-0.5.9/supermarq/run_benchmarks.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/simulation.py` & `Supermarq-0.5.9/supermarq/simulation.py`

 * *Files identical despite different names*

### Comparing `Supermarq-0.5.8/supermarq/stabilizers.py` & `Supermarq-0.5.9/supermarq/stabilizers.py`

 * *Files identical despite different names*

