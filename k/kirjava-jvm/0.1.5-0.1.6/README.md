# Comparing `tmp/kirjava-jvm-0.1.5.tar.gz` & `tmp/kirjava-jvm-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kirjava-jvm-0.1.5.tar", last modified: Wed Mar  6 12:22:17 2024, max compression
+gzip compressed data, was "kirjava-jvm-0.1.6.tar", last modified: Fri May 31 05:13:38 2024, max compression
```

## Comparing `kirjava-jvm-0.1.5.tar` & `kirjava-jvm-0.1.6.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-03-06 12:22:17.769962 kirjava-jvm-0.1.5/
--rw-r--r--   0 iska      (1000) iska      (1000)    35149 2022-12-20 18:02:58.000000 kirjava-jvm-0.1.5/LICENSE.txt
--rw-r--r--   0 iska      (1000) iska      (1000)    10037 2024-03-06 12:22:17.769962 kirjava-jvm-0.1.5/PKG-INFO
--rw-r--r--   0 iska      (1000) iska      (1000)     9694 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/README.md
--rw-r--r--   0 iska      (1000) iska      (1000)       50 2023-08-18 09:27:54.000000 kirjava-jvm-0.1.5/pyproject.toml
--rw-r--r--   0 iska      (1000) iska      (1000)       38 2024-03-06 12:22:17.769962 kirjava-jvm-0.1.5/setup.cfg
--rwxr-xr-x   0 iska      (1000) iska      (1000)     1064 2024-03-06 12:17:07.000000 kirjava-jvm-0.1.5/setup.py
-drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-03-06 12:22:17.756629 kirjava-jvm-0.1.5/src/
-drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-03-06 12:22:17.759962 kirjava-jvm-0.1.5/src/kirjava/
--rw-r--r--   0 iska      (1000) iska      (1000)      680 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/__init__.py
--rw-r--r--   0 iska      (1000) iska      (1000)     4772 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/_argument.py
--rw-r--r--   0 iska      (1000) iska      (1000)     3441 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/_helper.py
--rw-r--r--   0 iska      (1000) iska      (1000)     1351 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/_struct.py
-drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-03-06 12:22:17.759962 kirjava-jvm-0.1.5/src/kirjava/abc/
--rw-r--r--   0 iska      (1000) iska      (1000)      568 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/abc/__init__.py
--rw-r--r--   0 iska      (1000) iska      (1000)     4756 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/abc/class_.py
--rw-r--r--   0 iska      (1000) iska      (1000)      823 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/abc/constant.py
--rw-r--r--   0 iska      (1000) iska      (1000)      719 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/abc/field.py
--rw-r--r--   0 iska      (1000) iska      (1000)    13314 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/abc/graph.py
--rw-r--r--   0 iska      (1000) iska      (1000)      862 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/abc/method.py
--rw-r--r--   0 iska      (1000) iska      (1000)      669 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/abc/source.py
-drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-03-06 12:22:17.759962 kirjava-jvm-0.1.5/src/kirjava/analysis/
--rw-r--r--   0 iska      (1000) iska      (1000)    13152 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/analysis/__init__.py
--rw-r--r--   0 iska      (1000) iska      (1000)     5060 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/analysis/_generify.py
--rw-r--r--   0 iska      (1000) iska      (1000)    12283 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/analysis/_trace.py
--rw-r--r--   0 iska      (1000) iska      (1000)    28641 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/analysis/frame.py
-drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-03-06 12:22:17.763296 kirjava-jvm-0.1.5/src/kirjava/analysis/graph/
--rw-r--r--   0 iska      (1000) iska      (1000)    12539 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/analysis/graph/__init__.py
--rw-r--r--   0 iska      (1000) iska      (1000)    43717 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/analysis/graph/_asm.py
--rw-r--r--   0 iska      (1000) iska      (1000)    16283 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/analysis/graph/_dis.py
--rw-r--r--   0 iska      (1000) iska      (1000)     8254 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/analysis/graph/block.py
--rw-r--r--   0 iska      (1000) iska      (1000)     2068 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/analysis/graph/debug.py
--rw-r--r--   0 iska      (1000) iska      (1000)    14014 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/analysis/graph/edge.py
-drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-03-06 12:22:17.763296 kirjava-jvm-0.1.5/src/kirjava/classfile/
--rw-r--r--   0 iska      (1000) iska      (1000)    20242 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/classfile/__init__.py
--rw-r--r--   0 iska      (1000) iska      (1000)     9537 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/classfile/_constant.py
--rw-r--r--   0 iska      (1000) iska      (1000)     2503 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/classfile/_instructions.py
--rw-r--r--   0 iska      (1000) iska      (1000)     2018 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/classfile/_provider.py
-drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-03-06 12:22:17.763296 kirjava-jvm-0.1.5/src/kirjava/classfile/attributes/
--rw-r--r--   0 iska      (1000) iska      (1000)     5644 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/classfile/attributes/__init__.py
--rw-r--r--   0 iska      (1000) iska      (1000)    23669 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/classfile/attributes/class_.py
--rw-r--r--   0 iska      (1000) iska      (1000)    33029 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/classfile/attributes/code.py
--rw-r--r--   0 iska      (1000) iska      (1000)     1244 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/classfile/attributes/field.py
--rw-r--r--   0 iska      (1000) iska      (1000)    10327 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/classfile/attributes/method.py
--rw-r--r--   0 iska      (1000) iska      (1000)    13197 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/classfile/attributes/shared.py
--rw-r--r--   0 iska      (1000) iska      (1000)    23731 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/classfile/members.py
--rw-r--r--   0 iska      (1000) iska      (1000)    35525 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/constants.py
--rw-r--r--   0 iska      (1000) iska      (1000)     4417 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/environment.py
--rw-r--r--   0 iska      (1000) iska      (1000)     5375 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/error.py
-drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-03-06 12:22:17.766629 kirjava-jvm-0.1.5/src/kirjava/instructions/
--rw-r--r--   0 iska      (1000) iska      (1000)    35771 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/instructions/__init__.py
--rw-r--r--   0 iska      (1000) iska      (1000)     8446 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/instructions/arithmetic.py
--rw-r--r--   0 iska      (1000) iska      (1000)     2705 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/instructions/array.py
--rw-r--r--   0 iska      (1000) iska      (1000)     4511 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/instructions/constant.py
--rw-r--r--   0 iska      (1000) iska      (1000)     5029 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/instructions/conversion.py
--rw-r--r--   0 iska      (1000) iska      (1000)     4177 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/instructions/field.py
--rw-r--r--   0 iska      (1000) iska      (1000)    10447 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/instructions/flow.py
--rw-r--r--   0 iska      (1000) iska      (1000)     7896 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/instructions/invoke.py
--rw-r--r--   0 iska      (1000) iska      (1000)     6746 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/instructions/local.py
--rw-r--r--   0 iska      (1000) iska      (1000)     8866 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/instructions/new.py
--rw-r--r--   0 iska      (1000) iska      (1000)     2948 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/instructions/other.py
--rw-r--r--   0 iska      (1000) iska      (1000)     3621 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/instructions/stack.py
-drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-03-06 12:22:17.766629 kirjava-jvm-0.1.5/src/kirjava/jarfile/
--rw-r--r--   0 iska      (1000) iska      (1000)     1909 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/jarfile/__init__.py
--rw-r--r--   0 iska      (1000) iska      (1000)      665 2023-03-12 09:32:27.000000 kirjava-jvm-0.1.5/src/kirjava/jarfile/abc.py
--rw-r--r--   0 iska      (1000) iska      (1000)      156 2023-03-12 09:32:27.000000 kirjava-jvm-0.1.5/src/kirjava/jarfile/cdfh.py
--rw-r--r--   0 iska      (1000) iska      (1000)     1652 2023-03-12 09:32:27.000000 kirjava-jvm-0.1.5/src/kirjava/jarfile/eocd.py
--rw-r--r--   0 iska      (1000) iska      (1000)      133 2023-03-12 09:32:27.000000 kirjava-jvm-0.1.5/src/kirjava/jarfile/lfh.py
--rw-r--r--   0 iska      (1000) iska      (1000)      351 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/skeleton.py
--rw-r--r--   0 iska      (1000) iska      (1000)     2112 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/source.py
-drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-03-06 12:22:17.769962 kirjava-jvm-0.1.5/src/kirjava/types/
--rw-r--r--   0 iska      (1000) iska      (1000)    15145 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/types/__init__.py
--rw-r--r--   0 iska      (1000) iska      (1000)     8928 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/types/descriptor.py
--rw-r--r--   0 iska      (1000) iska      (1000)    19440 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/types/signature.py
--rw-r--r--   0 iska      (1000) iska      (1000)     5954 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/verifier.py
--rw-r--r--   0 iska      (1000) iska      (1000)     4507 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.5/src/kirjava/version.py
-drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-03-06 12:22:17.769962 kirjava-jvm-0.1.5/src/kirjava_jvm.egg-info/
--rw-r--r--   0 iska      (1000) iska      (1000)    10037 2024-03-06 12:22:17.000000 kirjava-jvm-0.1.5/src/kirjava_jvm.egg-info/PKG-INFO
--rw-r--r--   0 iska      (1000) iska      (1000)     2080 2024-03-06 12:22:17.000000 kirjava-jvm-0.1.5/src/kirjava_jvm.egg-info/SOURCES.txt
--rw-r--r--   0 iska      (1000) iska      (1000)        1 2024-03-06 12:22:17.000000 kirjava-jvm-0.1.5/src/kirjava_jvm.egg-info/dependency_links.txt
--rw-r--r--   0 iska      (1000) iska      (1000)        8 2024-03-06 12:22:17.000000 kirjava-jvm-0.1.5/src/kirjava_jvm.egg-info/top_level.txt
+drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-05-31 05:13:38.702129 kirjava-jvm-0.1.6/
+-rw-r--r--   0 iska      (1000) iska      (1000)    35149 2022-12-20 18:02:58.000000 kirjava-jvm-0.1.6/LICENSE.txt
+-rw-r--r--   0 iska      (1000) iska      (1000)    10624 2024-05-31 05:13:38.702129 kirjava-jvm-0.1.6/PKG-INFO
+-rw-r--r--   0 iska      (1000) iska      (1000)     9578 2024-05-31 05:13:32.000000 kirjava-jvm-0.1.6/README.md
+-rw-r--r--   0 iska      (1000) iska      (1000)       50 2023-08-18 09:27:54.000000 kirjava-jvm-0.1.6/pyproject.toml
+-rw-r--r--   0 iska      (1000) iska      (1000)       38 2024-05-31 05:13:38.702129 kirjava-jvm-0.1.6/setup.cfg
+-rwxr-xr-x   0 iska      (1000) iska      (1000)     2053 2024-05-31 05:07:47.000000 kirjava-jvm-0.1.6/setup.py
+drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-05-31 05:13:38.678795 kirjava-jvm-0.1.6/src/
+drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-05-31 05:13:38.682129 kirjava-jvm-0.1.6/src/kirjava/
+-rw-r--r--   0 iska      (1000) iska      (1000)      680 2024-05-31 04:51:23.000000 kirjava-jvm-0.1.6/src/kirjava/__init__.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     4772 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/_argument.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     3441 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/_helper.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     1351 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/_struct.py
+drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-05-31 05:13:38.685462 kirjava-jvm-0.1.6/src/kirjava/abc/
+-rw-r--r--   0 iska      (1000) iska      (1000)      568 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/abc/__init__.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     4756 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/abc/class_.py
+-rw-r--r--   0 iska      (1000) iska      (1000)      823 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/abc/constant.py
+-rw-r--r--   0 iska      (1000) iska      (1000)      719 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/abc/field.py
+-rw-r--r--   0 iska      (1000) iska      (1000)    13314 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/abc/graph.py
+-rw-r--r--   0 iska      (1000) iska      (1000)      862 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/abc/method.py
+-rw-r--r--   0 iska      (1000) iska      (1000)      669 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/abc/source.py
+drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-05-31 05:13:38.685462 kirjava-jvm-0.1.6/src/kirjava/analysis/
+-rw-r--r--   0 iska      (1000) iska      (1000)    13152 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/analysis/__init__.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     5060 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/analysis/_generify.py
+-rw-r--r--   0 iska      (1000) iska      (1000)    12283 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/analysis/_trace.py
+-rw-r--r--   0 iska      (1000) iska      (1000)    28641 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/analysis/frame.py
+drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-05-31 05:13:38.688795 kirjava-jvm-0.1.6/src/kirjava/analysis/graph/
+-rw-r--r--   0 iska      (1000) iska      (1000)    12539 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/analysis/graph/__init__.py
+-rw-r--r--   0 iska      (1000) iska      (1000)    43717 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/analysis/graph/_asm.py
+-rw-r--r--   0 iska      (1000) iska      (1000)    16283 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/analysis/graph/_dis.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     8254 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/analysis/graph/block.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     2068 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/analysis/graph/debug.py
+-rw-r--r--   0 iska      (1000) iska      (1000)    14014 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/analysis/graph/edge.py
+drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-05-31 05:13:38.692129 kirjava-jvm-0.1.6/src/kirjava/classfile/
+-rw-r--r--   0 iska      (1000) iska      (1000)    20242 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/classfile/__init__.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     9537 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/classfile/_constant.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     2503 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/classfile/_instructions.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     2018 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/classfile/_provider.py
+drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-05-31 05:13:38.692129 kirjava-jvm-0.1.6/src/kirjava/classfile/attributes/
+-rw-r--r--   0 iska      (1000) iska      (1000)     5644 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/classfile/attributes/__init__.py
+-rw-r--r--   0 iska      (1000) iska      (1000)    23669 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/classfile/attributes/class_.py
+-rw-r--r--   0 iska      (1000) iska      (1000)    33029 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/classfile/attributes/code.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     1244 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/classfile/attributes/field.py
+-rw-r--r--   0 iska      (1000) iska      (1000)    10327 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/classfile/attributes/method.py
+-rw-r--r--   0 iska      (1000) iska      (1000)    13197 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/classfile/attributes/shared.py
+-rw-r--r--   0 iska      (1000) iska      (1000)    23731 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/classfile/members.py
+-rw-r--r--   0 iska      (1000) iska      (1000)    35525 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/constants.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     4417 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/environment.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     5375 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/error.py
+drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-05-31 05:13:38.695462 kirjava-jvm-0.1.6/src/kirjava/instructions/
+-rw-r--r--   0 iska      (1000) iska      (1000)    35771 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/instructions/__init__.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     8446 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/instructions/arithmetic.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     2705 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/instructions/array.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     4511 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/instructions/constant.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     5029 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/instructions/conversion.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     4177 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/instructions/field.py
+-rw-r--r--   0 iska      (1000) iska      (1000)    10447 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/instructions/flow.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     7896 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/instructions/invoke.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     6746 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/instructions/local.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     8866 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/instructions/new.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     2948 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/instructions/other.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     3621 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/instructions/stack.py
+drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-05-31 05:13:38.698795 kirjava-jvm-0.1.6/src/kirjava/jarfile/
+-rw-r--r--   0 iska      (1000) iska      (1000)     1909 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/jarfile/__init__.py
+-rw-r--r--   0 iska      (1000) iska      (1000)      665 2023-03-12 09:32:27.000000 kirjava-jvm-0.1.6/src/kirjava/jarfile/abc.py
+-rw-r--r--   0 iska      (1000) iska      (1000)      156 2023-03-12 09:32:27.000000 kirjava-jvm-0.1.6/src/kirjava/jarfile/cdfh.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     1652 2023-03-12 09:32:27.000000 kirjava-jvm-0.1.6/src/kirjava/jarfile/eocd.py
+-rw-r--r--   0 iska      (1000) iska      (1000)      133 2023-03-12 09:32:27.000000 kirjava-jvm-0.1.6/src/kirjava/jarfile/lfh.py
+-rw-r--r--   0 iska      (1000) iska      (1000)      351 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/skeleton.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     2112 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/source.py
+drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-05-31 05:13:38.698795 kirjava-jvm-0.1.6/src/kirjava/types/
+-rw-r--r--   0 iska      (1000) iska      (1000)    15145 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/types/__init__.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     8928 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/types/descriptor.py
+-rw-r--r--   0 iska      (1000) iska      (1000)    19440 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/types/signature.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     5954 2024-03-06 14:03:13.000000 kirjava-jvm-0.1.6/src/kirjava/verifier.py
+-rw-r--r--   0 iska      (1000) iska      (1000)     4507 2024-03-06 11:59:07.000000 kirjava-jvm-0.1.6/src/kirjava/version.py
+drwxr-xr-x   0 iska      (1000) iska      (1000)        0 2024-05-31 05:13:38.702129 kirjava-jvm-0.1.6/src/kirjava_jvm.egg-info/
+-rw-r--r--   0 iska      (1000) iska      (1000)    10624 2024-05-31 05:13:38.000000 kirjava-jvm-0.1.6/src/kirjava_jvm.egg-info/PKG-INFO
+-rw-r--r--   0 iska      (1000) iska      (1000)     2080 2024-05-31 05:13:38.000000 kirjava-jvm-0.1.6/src/kirjava_jvm.egg-info/SOURCES.txt
+-rw-r--r--   0 iska      (1000) iska      (1000)        1 2024-05-31 05:13:38.000000 kirjava-jvm-0.1.6/src/kirjava_jvm.egg-info/dependency_links.txt
+-rw-r--r--   0 iska      (1000) iska      (1000)        8 2024-05-31 05:13:38.000000 kirjava-jvm-0.1.6/src/kirjava_jvm.egg-info/top_level.txt
```

### Comparing `kirjava-jvm-0.1.5/LICENSE.txt` & `kirjava-jvm-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/PKG-INFO` & `kirjava-jvm-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,10 @@
-Metadata-Version: 2.1
-Name: kirjava-jvm
-Version: 0.1.5
-Summary: A Java bytecode library for Python.
-Home-page: https://github.com/notiska/kirjava
-Author: node3112 (Iska)
-Author-email: node3112@protonmail.com
-License: GPL-3.0
-Keywords: java,jvm,bytecode,assembler,disassembler
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 # kirjava
 
-![](kirjava.png)
+![](https://raw.githubusercontent.com/notiska/kirjava/main/kirjava.png)
 Artwork by [Lou](https://www.instagram.com/devils_destination/).
 
 A pure-Python Java bytecode manipulation library with decent obfuscation resilience.  
 
 Documentation is planned for in the future, but as of right now, a quickstart guide has been provided below.  
 For more usage, see [examples](examples/).
 
@@ -27,16 +15,15 @@
 ## Quickstart
 
 ### Installing
 
 `python>=3.10` is required, any other versions are untested.  
 
 You can install this library by either:
- 1. Installing via pip: `pip3 install git+https://github.com/node3112/kirjava.git`.  
-   **Sidenote:** This library will not be published on [PyPI](https://pypi.org/project/kirjava/) as the name `kirjava` is already taken.
+ 1. Installing via pip: `pip3 install kirjava-jvm`.
  2. Cloning this repository and installing it manually:  
     - `git clone https://github.com/node3112/kirjava.git kirjava`
     - `cd kirjava`
     - `python3 setup.py install` or, if you lack permissions: `python3 setup.py install --user`
 
 *Additionally, [PyPy](https://www.pypy.org/) does appear to work and can result in significant performance gains.*
```

### Comparing `kirjava-jvm-0.1.5/README.md` & `kirjava-jvm-0.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,35 @@
+Metadata-Version: 2.1
+Name: kirjava-jvm
+Version: 0.1.6
+Summary: A Java bytecode library for Python.
+Home-page: https://github.com/notiska/kirjava
+Author-email: node3113@gmail.com
+License: GPL-3.0
+Keywords: java,jvm,bytecode,assembler,disassembler
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: File Formats
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Assemblers
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Disassemblers
+Classifier: Topic :: Software Development :: Libraries :: Java Libraries
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # kirjava
 
-![](kirjava.png)
+![](https://raw.githubusercontent.com/notiska/kirjava/main/kirjava.png)
 Artwork by [Lou](https://www.instagram.com/devils_destination/).
 
 A pure-Python Java bytecode manipulation library with decent obfuscation resilience.  
 
 Documentation is planned for in the future, but as of right now, a quickstart guide has been provided below.  
 For more usage, see [examples](examples/).
 
@@ -15,16 +40,15 @@
 ## Quickstart
 
 ### Installing
 
 `python>=3.10` is required, any other versions are untested.  
 
 You can install this library by either:
- 1. Installing via pip: `pip3 install git+https://github.com/node3112/kirjava.git`.  
-   **Sidenote:** This library will not be published on [PyPI](https://pypi.org/project/kirjava/) as the name `kirjava` is already taken.
+ 1. Installing via pip: `pip3 install kirjava-jvm`.
  2. Cloning this repository and installing it manually:  
     - `git clone https://github.com/node3112/kirjava.git kirjava`
     - `cd kirjava`
     - `python3 setup.py install` or, if you lack permissions: `python3 setup.py install --user`
 
 *Additionally, [PyPy](https://www.pypy.org/) does appear to work and can result in significant performance gains.*
```

### Comparing `kirjava-jvm-0.1.5/src/kirjava/__init__.py` & `kirjava-jvm-0.1.6/src/kirjava/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #     "Version",
 # )
 
 """
 kirjava - a Java bytecode library for Python.
 """
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 from . import (
     abc,
     analysis,
     classfile,
     constants,
     environment,
```

### Comparing `kirjava-jvm-0.1.5/src/kirjava/_argument.py` & `kirjava-jvm-0.1.6/src/kirjava/_argument.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/_helper.py` & `kirjava-jvm-0.1.6/src/kirjava/_helper.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/_struct.py` & `kirjava-jvm-0.1.6/src/kirjava/_struct.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/abc/__init__.py` & `kirjava-jvm-0.1.6/src/kirjava/abc/__init__.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/abc/class_.py` & `kirjava-jvm-0.1.6/src/kirjava/abc/class_.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/abc/constant.py` & `kirjava-jvm-0.1.6/src/kirjava/abc/constant.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/abc/field.py` & `kirjava-jvm-0.1.6/src/kirjava/abc/field.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/abc/graph.py` & `kirjava-jvm-0.1.6/src/kirjava/abc/graph.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/abc/method.py` & `kirjava-jvm-0.1.6/src/kirjava/abc/method.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/abc/source.py` & `kirjava-jvm-0.1.6/src/kirjava/abc/source.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/analysis/__init__.py` & `kirjava-jvm-0.1.6/src/kirjava/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/analysis/_generify.py` & `kirjava-jvm-0.1.6/src/kirjava/analysis/_generify.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/analysis/_trace.py` & `kirjava-jvm-0.1.6/src/kirjava/analysis/_trace.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/analysis/frame.py` & `kirjava-jvm-0.1.6/src/kirjava/analysis/frame.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/analysis/graph/__init__.py` & `kirjava-jvm-0.1.6/src/kirjava/analysis/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/analysis/graph/_asm.py` & `kirjava-jvm-0.1.6/src/kirjava/analysis/graph/_asm.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/analysis/graph/_dis.py` & `kirjava-jvm-0.1.6/src/kirjava/analysis/graph/_dis.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/analysis/graph/block.py` & `kirjava-jvm-0.1.6/src/kirjava/analysis/graph/block.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/analysis/graph/debug.py` & `kirjava-jvm-0.1.6/src/kirjava/analysis/graph/debug.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/analysis/graph/edge.py` & `kirjava-jvm-0.1.6/src/kirjava/analysis/graph/edge.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/classfile/__init__.py` & `kirjava-jvm-0.1.6/src/kirjava/classfile/__init__.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/classfile/_constant.py` & `kirjava-jvm-0.1.6/src/kirjava/classfile/_constant.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/classfile/_instructions.py` & `kirjava-jvm-0.1.6/src/kirjava/classfile/_instructions.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/classfile/_provider.py` & `kirjava-jvm-0.1.6/src/kirjava/classfile/_provider.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/classfile/attributes/__init__.py` & `kirjava-jvm-0.1.6/src/kirjava/classfile/attributes/__init__.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/classfile/attributes/class_.py` & `kirjava-jvm-0.1.6/src/kirjava/classfile/attributes/class_.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/classfile/attributes/code.py` & `kirjava-jvm-0.1.6/src/kirjava/classfile/attributes/code.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/classfile/attributes/field.py` & `kirjava-jvm-0.1.6/src/kirjava/classfile/attributes/field.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/classfile/attributes/method.py` & `kirjava-jvm-0.1.6/src/kirjava/classfile/attributes/method.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/classfile/attributes/shared.py` & `kirjava-jvm-0.1.6/src/kirjava/classfile/attributes/shared.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/classfile/members.py` & `kirjava-jvm-0.1.6/src/kirjava/classfile/members.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/constants.py` & `kirjava-jvm-0.1.6/src/kirjava/constants.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/environment.py` & `kirjava-jvm-0.1.6/src/kirjava/environment.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/error.py` & `kirjava-jvm-0.1.6/src/kirjava/error.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/instructions/__init__.py` & `kirjava-jvm-0.1.6/src/kirjava/instructions/__init__.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/instructions/arithmetic.py` & `kirjava-jvm-0.1.6/src/kirjava/instructions/arithmetic.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/instructions/array.py` & `kirjava-jvm-0.1.6/src/kirjava/instructions/array.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/instructions/constant.py` & `kirjava-jvm-0.1.6/src/kirjava/instructions/constant.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/instructions/conversion.py` & `kirjava-jvm-0.1.6/src/kirjava/instructions/conversion.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/instructions/field.py` & `kirjava-jvm-0.1.6/src/kirjava/instructions/field.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/instructions/flow.py` & `kirjava-jvm-0.1.6/src/kirjava/instructions/flow.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/instructions/invoke.py` & `kirjava-jvm-0.1.6/src/kirjava/instructions/invoke.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/instructions/local.py` & `kirjava-jvm-0.1.6/src/kirjava/instructions/local.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/instructions/new.py` & `kirjava-jvm-0.1.6/src/kirjava/instructions/new.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/instructions/other.py` & `kirjava-jvm-0.1.6/src/kirjava/instructions/other.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/instructions/stack.py` & `kirjava-jvm-0.1.6/src/kirjava/instructions/stack.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/jarfile/__init__.py` & `kirjava-jvm-0.1.6/src/kirjava/jarfile/__init__.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/jarfile/abc.py` & `kirjava-jvm-0.1.6/src/kirjava/jarfile/abc.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/jarfile/eocd.py` & `kirjava-jvm-0.1.6/src/kirjava/jarfile/eocd.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/source.py` & `kirjava-jvm-0.1.6/src/kirjava/source.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/types/__init__.py` & `kirjava-jvm-0.1.6/src/kirjava/types/__init__.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/types/descriptor.py` & `kirjava-jvm-0.1.6/src/kirjava/types/descriptor.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/types/signature.py` & `kirjava-jvm-0.1.6/src/kirjava/types/signature.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/verifier.py` & `kirjava-jvm-0.1.6/src/kirjava/verifier.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava/version.py` & `kirjava-jvm-0.1.6/src/kirjava/version.py`

 * *Files identical despite different names*

### Comparing `kirjava-jvm-0.1.5/src/kirjava_jvm.egg-info/PKG-INFO` & `kirjava-jvm-0.1.6/src/kirjava_jvm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 Metadata-Version: 2.1
 Name: kirjava-jvm
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Java bytecode library for Python.
 Home-page: https://github.com/notiska/kirjava
-Author: node3112 (Iska)
-Author-email: node3112@protonmail.com
+Author-email: node3113@gmail.com
 License: GPL-3.0
 Keywords: java,jvm,bytecode,assembler,disassembler
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: File Formats
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Assemblers
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Disassemblers
+Classifier: Topic :: Software Development :: Libraries :: Java Libraries
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # kirjava
 
-![](kirjava.png)
+![](https://raw.githubusercontent.com/notiska/kirjava/main/kirjava.png)
 Artwork by [Lou](https://www.instagram.com/devils_destination/).
 
 A pure-Python Java bytecode manipulation library with decent obfuscation resilience.  
 
 Documentation is planned for in the future, but as of right now, a quickstart guide has been provided below.  
 For more usage, see [examples](examples/).
 
@@ -27,16 +40,15 @@
 ## Quickstart
 
 ### Installing
 
 `python>=3.10` is required, any other versions are untested.  
 
 You can install this library by either:
- 1. Installing via pip: `pip3 install git+https://github.com/node3112/kirjava.git`.  
-   **Sidenote:** This library will not be published on [PyPI](https://pypi.org/project/kirjava/) as the name `kirjava` is already taken.
+ 1. Installing via pip: `pip3 install kirjava-jvm`.
  2. Cloning this repository and installing it manually:  
     - `git clone https://github.com/node3112/kirjava.git kirjava`
     - `cd kirjava`
     - `python3 setup.py install` or, if you lack permissions: `python3 setup.py install --user`
 
 *Additionally, [PyPy](https://www.pypy.org/) does appear to work and can result in significant performance gains.*
```

### Comparing `kirjava-jvm-0.1.5/src/kirjava_jvm.egg-info/SOURCES.txt` & `kirjava-jvm-0.1.6/src/kirjava_jvm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

