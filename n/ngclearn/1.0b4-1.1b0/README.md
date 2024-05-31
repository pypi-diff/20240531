# Comparing `tmp/ngclearn-1.0b4.tar.gz` & `tmp/ngclearn-1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngclearn-1.0b4.tar", last modified: Thu May  2 19:09:59 2024, max compression
+gzip compressed data, was "ngclearn-1.1b0.tar", last modified: Fri May 31 17:44:32 2024, max compression
```

## Comparing `ngclearn-1.0b4.tar` & `ngclearn-1.1b0.tar`

### file list

```diff
@@ -1,81 +1,109 @@
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.754975 ngclearn-1.0b4/
--rw-rw-r--   0 ago       (1001) ago       (1001)      368 2024-03-27 21:42:18.000000 ngclearn-1.0b4/AUTHORS
--rw-rw-r--   0 ago       (1001) ago       (1001)     1548 2024-03-27 21:42:18.000000 ngclearn-1.0b4/LICENSE
--rw-r--r--   0 ago       (1001) ago       (1001)     7754 2024-05-02 19:09:59.754975 ngclearn-1.0b4/PKG-INFO
--rw-rw-r--   0 ago       (1001) ago       (1001)     6030 2024-05-02 19:09:14.000000 ngclearn-1.0b4/README.md
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.658976 ngclearn-1.0b4/UPDATED_cells/
--rw-r--r--   0 ago       (1001) ago       (1001)    13935 2024-04-23 19:01:05.000000 ngclearn-1.0b4/UPDATED_cells/LIFCell.py
--rw-r--r--   0 ago       (1001) ago       (1001)    14887 2024-04-22 01:12:58.000000 ngclearn-1.0b4/UPDATED_cells/older_sLIF.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.670976 ngclearn-1.0b4/ngclearn/
--rw-rw-r--   0 ago       (1001) ago       (1001)      706 2024-05-02 19:09:05.000000 ngclearn-1.0b4/ngclearn/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.674976 ngclearn-1.0b4/ngclearn/commands/
--rw-rw-r--   0 ago       (1001) ago       (1001)       33 2024-03-28 23:58:59.000000 ngclearn-1.0b4/ngclearn/commands/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.674976 ngclearn-1.0b4/ngclearn/components/
--rw-rw-r--   0 ago       (1001) ago       (1001)     1087 2024-04-04 05:00:32.000000 ngclearn-1.0b4/ngclearn/components/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     1081 2024-03-28 22:29:48.000000 ngclearn-1.0b4/ngclearn/components/baseComponentTemplate.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.674976 ngclearn-1.0b4/ngclearn/components/input_encoders/
--rw-rw-r--   0 ago       (1001) ago       (1001)      118 2024-03-30 04:48:51.000000 ngclearn-1.0b4/ngclearn/components/input_encoders/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     3568 2024-04-17 19:56:59.000000 ngclearn-1.0b4/ngclearn/components/input_encoders/bernoulliCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     8904 2024-04-01 16:58:48.000000 ngclearn-1.0b4/ngclearn/components/input_encoders/latencyCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     3933 2024-03-30 20:38:16.000000 ngclearn-1.0b4/ngclearn/components/input_encoders/poissonCell.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.674976 ngclearn-1.0b4/ngclearn/components/neurons/
--rw-rw-r--   0 ago       (1001) ago       (1001)      486 2024-04-01 02:25:22.000000 ngclearn-1.0b4/ngclearn/components/neurons/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.678976 ngclearn-1.0b4/ngclearn/components/neurons/graded/
--rw-rw-r--   0 ago       (1001) ago       (1001)      178 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/components/neurons/graded/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     5403 2024-04-15 21:14:40.000000 ngclearn-1.0b4/ngclearn/components/neurons/graded/gaussianErrorCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     5439 2024-04-09 02:58:27.000000 ngclearn-1.0b4/ngclearn/components/neurons/graded/laplacianErrorCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     9985 2024-04-25 16:59:38.000000 ngclearn-1.0b4/ngclearn/components/neurons/graded/rateCell.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.690976 ngclearn-1.0b4/ngclearn/components/neurons/spiking/
--rw-rw-r--   0 ago       (1001) ago       (1001)    11036 2024-03-28 22:31:05.000000 ngclearn-1.0b4/ngclearn/components/neurons/spiking/LIFCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)      247 2024-04-01 02:25:22.000000 ngclearn-1.0b4/ngclearn/components/neurons/spiking/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     9077 2024-04-23 18:48:03.000000 ngclearn-1.0b4/ngclearn/components/neurons/spiking/fitzhughNagumoCell.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)    11418 2024-04-23 18:48:14.000000 ngclearn-1.0b4/ngclearn/components/neurons/spiking/izhikevichCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)    11707 2024-03-28 22:31:11.000000 ngclearn-1.0b4/ngclearn/components/neurons/spiking/quadLIFCell.py
--rw-rw-r--   0 ago       (1001) ago       (1001)    15059 2024-04-27 16:21:39.000000 ngclearn-1.0b4/ngclearn/components/neurons/spiking/sLIFCell.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.694975 ngclearn-1.0b4/ngclearn/components/other/
--rw-rw-r--   0 ago       (1001) ago       (1001)       64 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/components/other/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     4379 2024-04-09 02:58:27.000000 ngclearn-1.0b4/ngclearn/components/other/expKernel.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     5084 2024-04-15 21:33:31.000000 ngclearn-1.0b4/ngclearn/components/other/varTrace.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.694975 ngclearn-1.0b4/ngclearn/components/synapses/
--rw-rw-r--   0 ago       (1001) ago       (1001)      160 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/components/synapses/__init__.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.698975 ngclearn-1.0b4/ngclearn/components/synapses/hebbian/
--rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/components/synapses/hebbian/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     8378 2024-03-28 22:31:56.000000 ngclearn-1.0b4/ngclearn/components/synapses/hebbian/expSTDPSynapse.py
--rw-rw-r--   0 ago       (1001) ago       (1001)    11195 2024-04-18 22:52:48.000000 ngclearn-1.0b4/ngclearn/components/synapses/hebbian/hebbianSynapse.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     9793 2024-04-09 23:34:39.000000 ngclearn-1.0b4/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py
--rw-rw-r--   0 ago       (1001) ago       (1001)      263 2024-03-29 00:03:17.000000 ngclearn-1.0b4/ngclearn/components/wrappers.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.698975 ngclearn-1.0b4/ngclearn/utils/
--rwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/utils/__init__.py
--rw-r--r--   0 ago       (1001) ago       (1001)     3232 2024-04-05 17:47:38.000000 ngclearn-1.0b4/ngclearn/utils/data_loader.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.702975 ngclearn-1.0b4/ngclearn/utils/density/
--rw-r--r--   0 ago       (1001) ago       (1001)        0 2024-03-28 00:06:24.000000 ngclearn-1.0b4/ngclearn/utils/density/__init__.py
--rw-r--r--   0 ago       (1001) ago       (1001)     2816 2024-03-28 02:06:50.000000 ngclearn-1.0b4/ngclearn/utils/density/gmm.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.726975 ngclearn-1.0b4/ngclearn/utils/diffeq/
--rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-04-06 17:34:24.000000 ngclearn-1.0b4/ngclearn/utils/diffeq/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     6043 2024-04-23 18:35:18.000000 ngclearn-1.0b4/ngclearn/utils/diffeq/_ode_utils.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     6586 2024-04-23 18:39:06.000000 ngclearn-1.0b4/ngclearn/utils/diffeq/ode_utils.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     1629 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/utils/io_utils.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     5638 2024-04-27 19:34:14.000000 ngclearn-1.0b4/ngclearn/utils/metric_utils.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)    19071 2024-04-27 19:34:14.000000 ngclearn-1.0b4/ngclearn/utils/model_utils.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.754975 ngclearn-1.0b4/ngclearn/utils/optim/
--rw-rw-r--   0 ago       (1001) ago       (1001)       46 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/utils/optim/__init__.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     3090 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/utils/optim/adam.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)      783 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/utils/optim/opt.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     1122 2024-04-05 17:34:57.000000 ngclearn-1.0b4/ngclearn/utils/optim/sgd.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     3164 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/utils/patch_utils.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     5690 2024-04-17 20:19:32.000000 ngclearn-1.0b4/ngclearn/utils/surrogate_fx.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.754975 ngclearn-1.0b4/ngclearn/utils/viz/
--rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-03-27 21:42:18.000000 ngclearn-1.0b4/ngclearn/utils/viz/__init__.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     3503 2024-05-01 23:29:33.000000 ngclearn-1.0b4/ngclearn/utils/viz/dim_reduce.py
--rwxrwxr-x   0 ago       (1001) ago       (1001)     6699 2024-04-03 17:27:35.000000 ngclearn-1.0b4/ngclearn/utils/viz/raster.py
--rw-r--r--   0 ago       (1001) ago       (1001)     2513 2024-04-03 17:26:57.000000 ngclearn-1.0b4/ngclearn/utils/viz/spike_plot.py
--rw-rw-r--   0 ago       (1001) ago       (1001)     4936 2024-04-19 16:42:21.000000 ngclearn-1.0b4/ngclearn/utils/viz/synapse_plot.py
-drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-02 19:09:59.754975 ngclearn-1.0b4/ngclearn.egg-info/
--rw-r--r--   0 ago       (1001) ago       (1001)     7754 2024-05-02 19:09:59.000000 ngclearn-1.0b4/ngclearn.egg-info/PKG-INFO
--rw-rw-r--   0 ago       (1001) ago       (1001)     2208 2024-05-02 19:09:59.000000 ngclearn-1.0b4/ngclearn.egg-info/SOURCES.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)        1 2024-05-02 19:09:59.000000 ngclearn-1.0b4/ngclearn.egg-info/dependency_links.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-05-02 19:09:59.000000 ngclearn-1.0b4/ngclearn.egg-info/requires.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)       67 2024-05-02 19:09:59.000000 ngclearn-1.0b4/ngclearn.egg-info/top_level.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)     1838 2024-05-02 19:08:29.000000 ngclearn-1.0b4/pyproject.toml
--rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-05-02 19:09:51.000000 ngclearn-1.0b4/requirements.txt
--rw-rw-r--   0 ago       (1001) ago       (1001)       38 2024-05-02 19:09:59.754975 ngclearn-1.0b4/setup.cfg
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.284391 ngclearn-1.1b0/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      368 2024-05-14 18:04:38.000000 ngclearn-1.1b0/AUTHORS
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1548 2024-05-14 18:04:38.000000 ngclearn-1.1b0/LICENSE
+-rw-r--r--   0 ago       (1001) ago       (1001)     8044 2024-05-31 17:44:32.284391 ngclearn-1.1b0/PKG-INFO
+-rw-rw-r--   0 ago       (1001) ago       (1001)     6321 2024-05-30 17:48:13.000000 ngclearn-1.1b0/README.md
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.276391 ngclearn-1.1b0/ngclearn/
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1929 2024-05-31 17:33:18.000000 ngclearn-1.1b0/ngclearn/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.276391 ngclearn-1.1b0/ngclearn/commands/
+-rw-rw-r--   0 ago       (1001) ago       (1001)       33 2024-05-14 18:04:38.000000 ngclearn-1.1b0/ngclearn/commands/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.276391 ngclearn-1.1b0/ngclearn/components/
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1295 2024-05-30 17:49:04.000000 ngclearn-1.1b0/ngclearn/components/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.276391 ngclearn-1.1b0/ngclearn/components/input_encoders/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      118 2024-05-14 18:04:38.000000 ngclearn-1.1b0/ngclearn/components/input_encoders/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     3787 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/input_encoders/bernoulliCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     9426 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/input_encoders/latencyCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     4123 2024-05-31 02:48:25.000000 ngclearn-1.1b0/ngclearn/components/input_encoders/poissonCell.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.276391 ngclearn-1.1b0/ngclearn/components/lava/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      331 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/components/lava/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.276391 ngclearn-1.1b0/ngclearn/components/lava/neurons/
+-rw-rw-r--   0 ago       (1001) ago       (1001)     6339 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/lava/neurons/LIFCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)       29 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/components/lava/neurons/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.276391 ngclearn-1.1b0/ngclearn/components/lava/synapses/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      131 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/components/lava/synapses/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     4441 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/lava/synapses/hebbianSynapse.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     3339 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/lava/synapses/staticSynapse.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     5544 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/lava/synapses/traceSTDPSynapse.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.276391 ngclearn-1.1b0/ngclearn/components/lava/traces/
+-rwxrwxr-x   0 ago       (1001) ago       (1001)       36 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/components/lava/traces/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     2190 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/lava/traces/gatedTrace.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.280391 ngclearn-1.1b0/ngclearn/components/neurons/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      566 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/components/neurons/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.280391 ngclearn-1.1b0/ngclearn/components/neurons/graded/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      178 2024-05-14 18:04:38.000000 ngclearn-1.1b0/ngclearn/components/neurons/graded/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     4442 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/neurons/graded/gaussianErrorCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     4447 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/neurons/graded/laplacianErrorCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     9107 2024-05-31 15:46:43.000000 ngclearn-1.1b0/ngclearn/components/neurons/graded/rateCell.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.280391 ngclearn-1.1b0/ngclearn/components/neurons/spiking/
+-rw-rw-r--   0 ago       (1001) ago       (1001)    11905 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/neurons/spiking/LIFCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     6832 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/neurons/spiking/WTASCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)      311 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/components/neurons/spiking/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     7943 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/neurons/spiking/adExCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     8218 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/neurons/spiking/fitzhughNagumoCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)    10544 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/neurons/spiking/izhikevichCell.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)    10762 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/neurons/spiking/quadLIFCell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)    13349 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/neurons/spiking/sLIFCell.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.280391 ngclearn-1.1b0/ngclearn/components/other/
+-rw-rw-r--   0 ago       (1001) ago       (1001)       64 2024-05-26 02:51:19.000000 ngclearn-1.1b0/ngclearn/components/other/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     3882 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/other/expKernel.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     4991 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/components/other/varTrace.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.280391 ngclearn-1.1b0/ngclearn/components/synapses/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      258 2024-05-30 18:14:10.000000 ngclearn-1.1b0/ngclearn/components/synapses/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.280391 ngclearn-1.1b0/ngclearn/components/synapses/hebbian/
+-rw-rw-r--   0 ago       (1001) ago       (1001)      184 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/components/synapses/hebbian/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     7020 2024-05-31 15:46:43.000000 ngclearn-1.1b0/ngclearn/components/synapses/hebbian/eventSTDPSynapse.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     8872 2024-05-31 15:46:43.000000 ngclearn-1.1b0/ngclearn/components/synapses/hebbian/expSTDPSynapse.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)    11041 2024-05-31 15:46:43.000000 ngclearn-1.1b0/ngclearn/components/synapses/hebbian/hebbianSynapse.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     9272 2024-05-31 15:46:43.000000 ngclearn-1.1b0/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     4614 2024-05-31 15:46:43.000000 ngclearn-1.1b0/ngclearn/components/synapses/staticSynapse.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.280391 ngclearn-1.1b0/ngclearn/operations/
+-rw-rw-r--   0 ago       (1001) ago       (1001)       34 2024-05-31 14:19:32.000000 ngclearn-1.1b0/ngclearn/operations/__init__.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.280391 ngclearn-1.1b0/ngclearn/utils/
+-rwxrwxr-x   0 ago       (1001) ago       (1001)       37 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/utils/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     3230 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/utils/data_loader.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.280391 ngclearn-1.1b0/ngclearn/utils/density/
+-rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-05-14 18:04:38.000000 ngclearn-1.1b0/ngclearn/utils/density/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2816 2024-05-14 18:04:38.000000 ngclearn-1.1b0/ngclearn/utils/density/gmm.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.280391 ngclearn-1.1b0/ngclearn/utils/diffeq/
+-rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-05-14 18:04:38.000000 ngclearn-1.1b0/ngclearn/utils/diffeq/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     7349 2024-05-14 18:04:38.000000 ngclearn-1.1b0/ngclearn/utils/diffeq/ode_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     1629 2024-05-14 18:04:38.000000 ngclearn-1.1b0/ngclearn/utils/io_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     7970 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/utils/metric_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)    16804 2024-05-31 14:06:30.000000 ngclearn-1.1b0/ngclearn/utils/model_utils.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.280391 ngclearn-1.1b0/ngclearn/utils/optim/
+-rw-rw-r--   0 ago       (1001) ago       (1001)       59 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/utils/optim/__init__.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     3769 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/utils/optim/adam.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)      487 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/utils/optim/optim_utils.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     1583 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/utils/optim/sgd.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     3177 2024-05-31 15:46:43.000000 ngclearn-1.1b0/ngclearn/utils/patch_utils.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     5690 2024-05-14 18:04:38.000000 ngclearn-1.1b0/ngclearn/utils/surrogate_fx.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.280391 ngclearn-1.1b0/ngclearn/utils/viz/
+-rw-rw-r--   0 ago       (1001) ago       (1001)        0 2024-05-14 18:04:38.000000 ngclearn-1.1b0/ngclearn/utils/viz/__init__.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     3485 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/utils/viz/dim_reduce.py
+-rwxrwxr-x   0 ago       (1001) ago       (1001)     5418 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/utils/viz/raster.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     2673 2024-05-30 17:48:13.000000 ngclearn-1.1b0/ngclearn/utils/viz/spike_plot.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     6382 2024-05-31 14:19:32.000000 ngclearn-1.1b0/ngclearn/utils/viz/synapse_plot.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.284391 ngclearn-1.1b0/ngclearn.egg-info/
+-rw-r--r--   0 ago       (1001) ago       (1001)     8044 2024-05-31 17:44:32.000000 ngclearn-1.1b0/ngclearn.egg-info/PKG-INFO
+-rw-rw-r--   0 ago       (1001) ago       (1001)     3017 2024-05-31 17:44:32.000000 ngclearn-1.1b0/ngclearn.egg-info/SOURCES.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)        1 2024-05-31 17:44:32.000000 ngclearn-1.1b0/ngclearn.egg-info/dependency_links.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-05-31 17:44:32.000000 ngclearn-1.1b0/ngclearn.egg-info/requires.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)       54 2024-05-31 17:44:32.000000 ngclearn-1.1b0/ngclearn.egg-info/top_level.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1711 2024-05-31 17:28:27.000000 ngclearn-1.1b0/pyproject.toml
+-rw-rw-r--   0 ago       (1001) ago       (1001)      136 2024-05-31 17:26:37.000000 ngclearn-1.1b0/requirements.txt
+-rw-rw-r--   0 ago       (1001) ago       (1001)       38 2024-05-31 17:44:32.284391 ngclearn-1.1b0/setup.cfg
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.284391 ngclearn-1.1b0/test_code/
+-rwxr-xr-x   0 ago       (1001) ago       (1001)     3072 2024-05-28 21:11:49.000000 ngclearn-1.1b0/test_code/_run_trstdp.py
+-rw-r--r--   0 ago       (1001) ago       (1001)      968 2024-05-18 01:01:58.000000 ngclearn-1.1b0/test_code/adex.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1194 2024-05-25 16:47:53.000000 ngclearn-1.1b0/test_code/calc_fanoFactor.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)      971 2024-05-25 21:40:48.000000 ngclearn-1.1b0/test_code/run2_metrics.py
+-rwxr-xr-x   0 ago       (1001) ago       (1001)     2634 2024-05-26 04:20:56.000000 ngclearn-1.1b0/test_code/run_expkernel.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)      889 2024-05-25 21:04:53.000000 ngclearn-1.1b0/test_code/run_metrics.py
+-rwxr-xr-x   0 ago       (1001) ago       (1001)     2423 2024-05-25 23:21:31.000000 ngclearn-1.1b0/test_code/run_trace.py
+-rwxr-xr-x   0 ago       (1001) ago       (1001)     3437 2024-05-29 02:43:08.000000 ngclearn-1.1b0/test_code/run_trstdp.py
+-rw-r--r--   0 ago       (1001) ago       (1001)     5589 2024-05-18 01:04:05.000000 ngclearn-1.1b0/test_code/test_adex.py
+-rw-r--r--   0 ago       (1001) ago       (1001)     4518 2024-05-16 23:45:02.000000 ngclearn-1.1b0/test_code/test_fhcell.py
+-rwxr-xr-x   0 ago       (1001) ago       (1001)     5396 2024-05-18 00:09:30.000000 ngclearn-1.1b0/test_code/test_izhcell.py
+-rw-rw-r--   0 ago       (1001) ago       (1001)     1213 2024-05-25 22:26:28.000000 ngclearn-1.1b0/test_code/viz_data.py
+drwxrwxr-x   0 ago       (1001) ago       (1001)        0 2024-05-31 17:44:32.284391 ngclearn-1.1b0/test_lava/
+-rwxr-xr-x   0 ago       (1001) ago       (1001)     6684 2024-05-29 21:05:11.000000 ngclearn-1.1b0/test_lava/run_xotSNN.py
```

### Comparing `ngclearn-1.0b4/LICENSE` & `ngclearn-1.1b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b4/PKG-INFO` & `ngclearn-1.1b0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngclearn
-Version: 1.0b4
+Version: 1.1b0
 Summary: Simulation software for building and analyzing arbitrary predictive coding, spiking network, and biomimetic neural systems.
 Author-email: Alexander Ororbia <ago@cs.rit.edu>, William Gebhardt <wdg1351@rit.edu>
 License: BSD-3-Clause License
 Project-URL: Homepage, https://github.com/NACLab/ngc-learn
 Project-URL: Documentation, https://ngc-learn.readthedocs.io/
 Project-URL: Lab Page, https://www.cs.rit.edu/~ago/nac_lab.html
 Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/main/history.txt
@@ -18,26 +18,26 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: numpy>=1.26.0
+Requires-Dist: numpy>=1.24.0
 Requires-Dist: scikit-learn>=0.24.2
 Requires-Dist: scipy>=1.7.0
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: patchify
 Requires-Dist: jax>=0.4.18
 Requires-Dist: jaxlib>=0.4.18
-Requires-Dist: ngcsimlib>=0.2.b2
+Requires-Dist: ngcsimlib>=0.3.b0
 Requires-Dist: imageio>=2.31.5
 
 [![Python Version](https://img.shields.io/badge/python-3.10%20%7C%203.11-blue.svg)](https://www.python.org/downloads)[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)[![Documentation Status](https://readthedocs.org/projects/ngc-learn/badge/?version=latest)](http://ngc-learn.readthedocs.io/en/latest/?badge=latest)[![DOI](https://zenodo.org/badge/483413212.svg)](https://zenodo.org/badge/latestdoi/483413212)
 
 <img src="docs/images/ngc-learn-logo.png" width="300">
 
 <b>ngc-learn</b> is a Python library for building, simulating, and analyzing
@@ -90,19 +90,24 @@
 tools (routines within ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2).
 Many of the tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-learn (>=0.24.2).
 <!-- (Note: if using the `_generate_patch_set()` within the
 image patching utilities, then Patchify will be needed).-->
 
 ### User Installation
 
-<i>Setup</i>: The easiest way to install ngc-learn (CPU version) is through <code>pip</code>:
+<i>Setup</i>: The easiest way to install ngc-learn is through <code>pip</code>:
 <pre>
 $ pip install ngclearn
 </pre>
 
+Note that installing the official pip package without any form of JAX installed
+on your system will default to downloading the CPU version of ngc-learn; make
+sure you have installed the Cuda 12 version of Jax/Jaxlib on your system before
+running the above pip command if you want to use the GPU version.
+
 The documentation includes more detailed
 <a href="https://ngc-learn.readthedocs.io/en/latest/installation.html">installation instructions</a>.
 Note that this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
 
 If the installation was successful, you should see the following if you test
 it against your Python interpreter, i.e., run the <code>$ python</code> command
 and complete the following sequence of steps as depicted in the screenshot below
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ngclearn Version: 1.0b4 Summary: Simulation
+Metadata-Version: 2.1 Name: ngclearn Version: 1.1b0 Summary: Simulation
 software for building and analyzing arbitrary predictive coding, spiking
 network, and biomimetic neural systems. Author-email: Alexander Ororbia
 cs.rit.edu>, William Gebhardt
 rit.edu> License: BSD-3-Clause License Project-URL: Homepage, https://
 github.com/NACLab/ngc-learn Project-URL: Documentation, https://ngc-
 learn.readthedocs.io/ Project-URL: Lab Page, https://www.cs.rit.edu/~ago/
 nac_lab.html Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/
@@ -12,20 +12,20 @@
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: BSD License Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Unix Requires-Python: >=3.10 Description-
+Classifier: Operating System :: Unix Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE License-File: AUTHORS
-Requires-Dist: numpy>=1.26.0 Requires-Dist: scikit-learn>=0.24.2 Requires-Dist:
+Requires-Dist: numpy>=1.24.0 Requires-Dist: scikit-learn>=0.24.2 Requires-Dist:
 scipy>=1.7.0 Requires-Dist: matplotlib>=3.8.0 Requires-Dist: patchify Requires-
 Dist: jax>=0.4.18 Requires-Dist: jaxlib>=0.4.18 Requires-Dist:
-ngcsimlib>=0.2.b2 Requires-Dist: imageio>=2.31.5 [![Python Version](https://
+ngcsimlib>=0.3.b0 Requires-Dist: imageio>=2.31.5 [![Python Version](https://
 img.shields.io/badge/python-3.10%20%7C%203.11-blue.svg)](https://
 www.python.org/downloads)[![License](https://img.shields.io/badge/License-
 BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)[!
 [Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https:
 //GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)[![Documentation
 Status](https://readthedocs.org/projects/ngc-learn/badge/?version=latest)]
 (http://ngc-learn.readthedocs.io/en/latest/?badge=latest)[![DOI](https://
@@ -49,29 +49,33 @@
 CUDA variants) --- ngc-learn 1.0.beta0 and later require Python 3.10 or newer
 as well as ngcsimlib >=0.2.b2. ngc-learn's plotting capabilities (routines
 within `ngclearn.utils.viz`) require Matplotlib (>=3.8.0) and imageio
 (>=2.31.5) and both plotting and density estimation tools (routines within
 ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2). Many of the
 tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-
 learn (>=0.24.2). ### User Installation Setup: The easiest way to install ngc-
-learn (CPU version) is through pip:
+learn is through pip:
 $ pip install ngclearn
-The documentation includes more detailed _i_n_s_t_a_l_l_a_t_i_o_n_ _i_n_s_t_r_u_c_t_i_o_n_s. Note that
-this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and
-20.04. If the installation was successful, you should see the following if you
-test it against your Python interpreter, i.e., run the $ python command and
-complete the following sequence of steps as depicted in the screenshot below
-(you should see at the bottom of your output something akin to the right major
-and minor version of ngc-learn): ```console Python 3.11.4 (main, MONTH DAY
-YEAR, TIME) [GCC XX.X.X] on linux Type "help", "copyright", "credits" or
-"license" for more information. >>> import ngclearn >>> ngclearn.__version__
-'1.0b3' ``` Note: For access to the previous Tensorflow-2 version of ngc-learn
-(of which we no longer support), please visit the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ##
-AAttttrriibbuuttiioonn:: If you use this code in any form in your project(s), please cite
-its source paper (as well as ngc-learn's official software citation):
+Note that installing the official pip package without any form of JAX installed
+on your system will default to downloading the CPU version of ngc-learn; make
+sure you have installed the Cuda 12 version of Jax/Jaxlib on your system before
+running the above pip command if you want to use the GPU version. The
+documentation includes more detailed _i_n_s_t_a_l_l_a_t_i_o_n_ _i_n_s_t_r_u_c_t_i_o_n_s. Note that this
+library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
+If the installation was successful, you should see the following if you test it
+against your Python interpreter, i.e., run the $ python command and complete
+the following sequence of steps as depicted in the screenshot below (you should
+see at the bottom of your output something akin to the right major and minor
+version of ngc-learn): ```console Python 3.11.4 (main, MONTH DAY YEAR, TIME)
+[GCC XX.X.X] on linux Type "help", "copyright", "credits" or "license" for more
+information. >>> import ngclearn >>> ngclearn.__version__ '1.0b3' ``` Note: For
+access to the previous Tensorflow-2 version of ngc-learn (of which we no longer
+support), please visit the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ## AAttttrriibbuuttiioonn:: If you
+use this code in any form in your project(s), please cite its source paper (as
+well as ngc-learn's official software citation):
 @article{Ororbia2022,
   author={Ororbia, Alexander and Kifer, Daniel},
   title={The neural coding framework for learning generative models},
   journal={Nature Communications},
   year={2022},
   month={Apr},
   day={19},
```

### Comparing `ngclearn-1.0b4/README.md` & `ngclearn-1.1b0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,19 +52,24 @@
 tools (routines within ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2).
 Many of the tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-learn (>=0.24.2).
 <!-- (Note: if using the `_generate_patch_set()` within the
 image patching utilities, then Patchify will be needed).-->
 
 ### User Installation
 
-<i>Setup</i>: The easiest way to install ngc-learn (CPU version) is through <code>pip</code>:
+<i>Setup</i>: The easiest way to install ngc-learn is through <code>pip</code>:
 <pre>
 $ pip install ngclearn
 </pre>
 
+Note that installing the official pip package without any form of JAX installed
+on your system will default to downloading the CPU version of ngc-learn; make
+sure you have installed the Cuda 12 version of Jax/Jaxlib on your system before
+running the above pip command if you want to use the GPU version.
+
 The documentation includes more detailed
 <a href="https://ngc-learn.readthedocs.io/en/latest/installation.html">installation instructions</a>.
 Note that this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
 
 If the installation was successful, you should see the following if you test
 it against your Python interpreter, i.e., run the <code>$ python</code> command
 and complete the following sequence of steps as depicted in the screenshot below
```

#### html2text {}

```diff
@@ -25,29 +25,33 @@
 CUDA variants) --- ngc-learn 1.0.beta0 and later require Python 3.10 or newer
 as well as ngcsimlib >=0.2.b2. ngc-learn's plotting capabilities (routines
 within `ngclearn.utils.viz`) require Matplotlib (>=3.8.0) and imageio
 (>=2.31.5) and both plotting and density estimation tools (routines within
 ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2). Many of the
 tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-
 learn (>=0.24.2). ### User Installation Setup: The easiest way to install ngc-
-learn (CPU version) is through pip:
+learn is through pip:
 $ pip install ngclearn
-The documentation includes more detailed _i_n_s_t_a_l_l_a_t_i_o_n_ _i_n_s_t_r_u_c_t_i_o_n_s. Note that
-this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and
-20.04. If the installation was successful, you should see the following if you
-test it against your Python interpreter, i.e., run the $ python command and
-complete the following sequence of steps as depicted in the screenshot below
-(you should see at the bottom of your output something akin to the right major
-and minor version of ngc-learn): ```console Python 3.11.4 (main, MONTH DAY
-YEAR, TIME) [GCC XX.X.X] on linux Type "help", "copyright", "credits" or
-"license" for more information. >>> import ngclearn >>> ngclearn.__version__
-'1.0b3' ``` Note: For access to the previous Tensorflow-2 version of ngc-learn
-(of which we no longer support), please visit the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ##
-AAttttrriibbuuttiioonn:: If you use this code in any form in your project(s), please cite
-its source paper (as well as ngc-learn's official software citation):
+Note that installing the official pip package without any form of JAX installed
+on your system will default to downloading the CPU version of ngc-learn; make
+sure you have installed the Cuda 12 version of Jax/Jaxlib on your system before
+running the above pip command if you want to use the GPU version. The
+documentation includes more detailed _i_n_s_t_a_l_l_a_t_i_o_n_ _i_n_s_t_r_u_c_t_i_o_n_s. Note that this
+library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
+If the installation was successful, you should see the following if you test it
+against your Python interpreter, i.e., run the $ python command and complete
+the following sequence of steps as depicted in the screenshot below (you should
+see at the bottom of your output something akin to the right major and minor
+version of ngc-learn): ```console Python 3.11.4 (main, MONTH DAY YEAR, TIME)
+[GCC XX.X.X] on linux Type "help", "copyright", "credits" or "license" for more
+information. >>> import ngclearn >>> ngclearn.__version__ '1.0b3' ``` Note: For
+access to the previous Tensorflow-2 version of ngc-learn (of which we no longer
+support), please visit the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ## AAttttrriibbuuttiioonn:: If you
+use this code in any form in your project(s), please cite its source paper (as
+well as ngc-learn's official software citation):
 @article{Ororbia2022,
   author={Ororbia, Alexander and Kifer, Daniel},
   title={The neural coding framework for learning generative models},
   journal={Nature Communications},
   year={2022},
   month={Apr},
   day={19},
```

### Comparing `ngclearn-1.0b4/UPDATED_cells/older_sLIF.py` & `ngclearn-1.1b0/ngclearn/components/neurons/spiking/sLIFCell.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from ngcsimlib.component import Component
 from jax import numpy as jnp, random, jit
 from functools import partial
 import time, sys
-from ngclearn.utils.diffeq.ode_utils import get_integrator_code, \
-                                            step_euler, step_rk2
+from ngclearn import resolver, Component, Compartment
+from ngclearn.utils.diffeq.ode_utils import get_integrator_code, step_euler
 from ngclearn.utils.surrogate_fx import secant_lif_estimator
+from ngclearn.utils import tensorstats
 
 @jit
 def update_times(t, s, tols):
     """
     Updates time-of-last-spike (tols) variable.
 
     Args:
@@ -53,32 +53,23 @@
         modified electrical current value
     """
     _j = j * R_m
     if inh_R > 0.:
         _j = _j - (jnp.matmul(spikes, inh_weights) * inh_R)
     return _j
 
-## co-routines for run_cell
-# @partial(jit, static_argnums=[4,5,6])
-# def _update_voltage(dt, j, v, rfr, tau_m, refract_T, v_min=None):
-#     mask = (rfr >= refract_T).astype(jnp.float32) # get refractory mask
-#     _v = (v + (-v + j) * (dt / tau_m)) * mask
-#     if v_min is not None:
-#         _v = jnp.maximum(v_min, _v)
-#     #_v = v + (-v) * (dt / tau_m) + j * mask
-#     return _v, mask
-
 @jit
 def _dfv_internal(j, v, rfr, tau_m, refract_T): ## raw voltage dynamics
     mask = (rfr >= refract_T).astype(jnp.float32) # get refractory mask
-    dv_dt = ((-v + j) * (dt / tau_m)) * mask
-    dv_dt = dv_dt * (1./tau_m)
+    #dv_dt = ((-v + j) * (dt / tau_m)) * mask
+    dv_dt = (-v + j)
+    dv_dt = dv_dt * (1./tau_m) * mask
     return dv_dt
 
-def _dfv(v, params): ## voltage dynamics wrapper
+def _dfv(t, v, params): ## voltage dynamics wrapper
     j, rfr, tau_m, refract_T = params
     dv_dt = _dfv_internal(j, v, rfr, tau_m, refract_T)
     return dv_dt
 
 @jit
 def _hyperpolarize(v, s):
     _v = (1. - s) * v ## hyper-polarize cells
@@ -93,15 +84,16 @@
     else: ## run simple adaptive threshold
         thr_gain = spikes * thrGain
         thr_leak = (v_thr * thrLeak)
         _v_thr = v_thr + thr_gain - thr_leak
     return _v_thr
 
 @partial(jit, static_argnums=[4])
-def _update_refract_and_spikes(dt, rfr, s, mask, sticky_spikes=False):
+def _update_refract_and_spikes(dt, rfr, s, refract_T, sticky_spikes=False):
+    mask = (rfr >= refract_T).astype(jnp.float32) ## Note: wasted repeated compute
     ## update refractory variables
     _rfr = (rfr + dt) * (1. - s) + s * dt # set refract to dt
     _s = s
     if sticky_spikes == True: ## pin refractory spikes if configured
         _s = s * mask + (1. - mask)
     return _rfr, _s
 
@@ -140,21 +132,21 @@
             the source paper's core spiking process)
 
     Returns:
         voltage(t+dt), spikes, threshold(t+dt), updated refactory variables
     """
     #new_voltage, mask = _update_voltage(dt, j, v, rfr, tau_m, refract_T, v_min)
     v_params = (j, rfr, tau_m, refract_T)
-    _v = step_euler(v, v_params, _dfv, dt)
+    _, _v = step_euler(0., v, _dfv, dt, v_params) #_v = step_euler(v, v_params, _dfv, dt)
     # if v_min is not None:
     #     _v = jnp.maximum(v_min, _v)
     spikes = spike_fx(_v, v_thr)
     _v = _hyperpolarize(_v, spikes)
     new_thr = _update_threshold(dt, v_thr, spikes, thrGain, thrLeak, rho_b)
-    _rfr, spikes = _update_refract_and_spikes(dt, rfr, spikes, mask, sticky_spikes)
+    _rfr, spikes = _update_refract_and_spikes(dt, rfr, spikes, refract_T, sticky_spikes)
     return _v, spikes, new_thr, _rfr
 
 class SLIFCell(Component): ## leaky integrate-and-fire cell
     """
     A spiking cell based on a simplified leaky integrate-and-fire (sLIF) model.
     This neuronal cell notably contains functionality required by the computational
     model employed by (Samadi et al., 2017, i.e., a surrogate derivative function
@@ -202,194 +194,147 @@
             a key setting used by Samadi et al., 2017
 
         thr_jitter: scale of uniform jitter to add to initialization of thresholds
 
         key: PRNG key to control determinism of any underlying random values
             associated with this cell
 
-        useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
-
         directory: string indicating directory on disk to save sLIF parameter
             values to (i.e., initial threshold values and any persistent adaptive
             threshold values)
     """
 
-    ## Class Methods for Compartment Names
-    @classmethod
-    def inputCompartmentName(cls):
-        return 'j' ## electrical current
-
-    @classmethod
-    def outputCompartmentName(cls):
-        return 's' ## spike/action potential
-
-    @classmethod
-    def timeOfLastSpikeCompartmentName(cls):
-        return 'tols' ## time-of-last-spike (record vector)
-
-    @classmethod
-    def voltageCompartmentName(cls):
-        return 'v' ## membrane potential/voltage
-
-    @classmethod
-    def thresholdCompartmentName(cls):
-        return 'thr' ## action potential threshold
-
-    @classmethod
-    def refractCompartmentName(cls):
-        return 'rfr' ## refractory variable(s)
-
-    @classmethod
-    def surrogateCompartmentName(cls):
-        return 'surrogate'
-
-    ## Bind Properties to Compartments for ease of use
-    @property
-    def current(self):
-        return self.compartments.get(self.inputCompartmentName(), None)
-
-    @current.setter
-    def current(self, inp):
-        self.compartments[self.inputCompartmentName()] = inp
-
-    @property
-    def surrogate(self):
-        return self.compartments.get(self.surrogateCompartmentName(), None)
-
-    @surrogate.setter
-    def surrogate(self, inp):
-        self.compartments[self.surrogateCompartmentName()] = inp
-
-    @property
-    def spikes(self):
-        return self.compartments.get(self.outputCompartmentName(), None)
-
-    @spikes.setter
-    def spikes(self, out):
-        self.compartments[self.outputCompartmentName()] = out
-
-    @property
-    def timeOfLastSpike(self):
-        return self.compartments.get(self.timeOfLastSpikeCompartmentName(), None)
-
-    @timeOfLastSpike.setter
-    def timeOfLastSpike(self, t):
-        self.compartments[self.timeOfLastSpikeCompartmentName()] = t
-
-    @property
-    def voltage(self):
-        return self.compartments.get(self.voltageCompartmentName(), None)
-
-    @voltage.setter
-    def voltage(self, v):
-        self.compartments[self.voltageCompartmentName()] = v
-
-    @property
-    def refract(self):
-        return self.compartments.get(self.refractCompartmentName(), None)
-
-    @refract.setter
-    def refract(self, rfr):
-        self.compartments[self.refractCompartmentName()] = rfr
-
-    @property
-    def threshold(self):
-        return self.compartments.get(self.thresholdCompartmentName(), None)
-
-    @threshold.setter
-    def threshold(self, thr):
-        self.compartments[self.thresholdCompartmentName()] = thr
-
     # Define Functions
     def __init__(self, name, n_units, tau_m, R_m, thr, inhibit_R=0., thr_persist=False,
                  thrGain=0.0, thrLeak=0.0, rho_b=0., refract_T=0., sticky_spikes=False,
-                 thr_jitter=0.05, key=None, useVerboseDict=False, directory=None, **kwargs):
-        super().__init__(name, useVerboseDict, **kwargs)
+                 thr_jitter=0.05, key=None, directory=None, **kwargs):
+        super().__init__(name, **kwargs)
 
-        ##Random Number Set up
-        self.key = key
-        if self.key is None:
-            self.key = random.PRNGKey(time.time_ns())
+        key = random.PRNGKey(time.time_ns()) if key is None else key
 
         ## membrane parameter setup (affects ODE integration)
         self.tau_m = tau_m ## membrane time constant
         self.R_m = R_m ## resistance value
         self.refract_T = refract_T #5. # 2. ## refractory period  # ms
         self.v_min = -3.
         ## variable below determines if spikes pinned at 1 during refractory period?
         self.sticky_spikes = sticky_spikes
 
         ## set up surrogate function for spike emission
         self.spike_fx, self.d_spike_fx = secant_lif_estimator()
 
         ## create simple recurrent inhibitory pressure
         self.inh_R = inhibit_R ## lateral inhibitory magnitude
-        self.key, subkey = random.split(self.key)
+        key, subkey = random.split(key)
         self.inh_weights = random.uniform(subkey, (n_units, n_units), minval=0.025, maxval=1.)
         MV = 1. - jnp.eye(n_units)
         self.inh_weights = self.inh_weights * MV
 
         ##Layer Size Setup
         self.n_units = n_units
         self.batch_size = 1
 
         ## adaptive threshold setup
         self.rho_b = rho_b
         self.thr_persist = thr_persist ## are adapted thresholds persistent? True (persistent)
         self.thrGain = thrGain #0.0005
         self.thrLeak = thrLeak #0.00005
-        if directory is None:
-            self.thr_jitter =  thr_jitter ## some random jitter to ensure thresholds start off different
-            self.key, subkey = random.split(self.key)
-            #self.threshold = random.uniform(subkey, (1, n_units), minval=thr, maxval=1.25 * thr)
-            self.threshold0 = thr + random.uniform(subkey, (1, n_units),
-                                                  minval=-self.thr_jitter, maxval=self.thr_jitter,
-                                                  dtype=jnp.float32)
-            self.threshold = self.threshold0 + 0 ## save initial threshold
-        else:
-            self.load(directory)
 
-        self.reset()
-
-    def verify_connections(self):
-        self.metadata.check_incoming_connections(self.inputCompartmentName(), min_connections=1)
-
-    def advance_state(self, t, dt, **kwargs):
-        if self.spikes is None:
-            self.spikes = jnp.zeros((self.batch_size, self.n_units))
-        if self.refract is None:
-            self.refract = jnp.zeros((self.batch_size, self.n_units)) + self.refract_T
+        # thr_jitter: some random jitter to ensure thresholds start off different
+        key, subkey = random.split(key)
+        self.threshold0 = thr + random.uniform(subkey, (1, n_units),
+                                               minval=-thr_jitter, maxval=thr_jitter,
+                                               dtype=jnp.float32)
+
+        ## Compartments
+        restVals = jnp.zeros((self.batch_size, self.n_units))
+        self.j = Compartment(restVals) ## electrical current, input
+        self.s = Compartment(restVals) ## spike/action potential, output
+        self.tols = Compartment(restVals) ## time-of-last-spike (record vector)
+        self.v = Compartment(restVals) ## membrane potential/voltage
+        self.thr = Compartment(self.threshold0 + 0.) ## action potential threshold
+        self.rfr = Compartment(restVals + self.refract_T) ## refractory variable(s)
+        self.surrogate = Compartment(restVals + 1.) ## surrogate signal
+
+    @staticmethod
+    def _advance_state(t, dt, inh_weights, R_m, inh_R, d_spike_fx, tau_m, spike_fx,
+                 refract_T, thrGain, thrLeak, rho_b, sticky_spikes, v_min,
+                 j, s, v, thr, rfr, tols):
         ## run one step of Euler integration over neuronal dynamics
-        j_curr = self.current
+        j_curr = j
         ## apply simplified inhibitory pressure
-        j_curr = modify_current(j_curr, self.spikes, self.inh_weights, self.R_m, self.inh_R)
-        self.current = j_curr # None ## store electrical current
-        self.surrogate = self.d_spike_fx(j_curr, c1=0.82, c2=0.08)
-        self.voltage, self.spikes, self.threshold, self.refract = \
-            run_cell(dt, j_curr, self.voltage, self.threshold, self.tau_m,
-                     self.refract, self.spike_fx, self.refract_T, self.thrGain, self.thrLeak,
-                     self.rho_b, sticky_spikes=self.sticky_spikes, v_min=self.v_min)
+        j_curr = modify_current(j_curr, s, inh_weights, R_m, inh_R)
+        j = j_curr # None ## store electrical current
+        surrogate = d_spike_fx(j_curr, c1=0.82, c2=0.08)
+        v, s, thr, rfr = \
+            run_cell(dt, j_curr, v, thr, tau_m,
+                     rfr, spike_fx, refract_T, thrGain, thrLeak,
+                     rho_b, sticky_spikes=sticky_spikes, v_min=v_min)
         ## update tols
-        self.timeOfLastSpike = update_times(t, self.spikes, self.timeOfLastSpike)
+        tols = update_times(t, s, tols)
+        return j, s, tols, v, thr, rfr, surrogate
 
-    def reset(self, **kwargs):
-        self.voltage = jnp.zeros((self.batch_size, self.n_units))
-        self.refract = jnp.zeros((self.batch_size, self.n_units)) + self.refract_T
-        self.current = None
-        self.surrogate = None
-        self.timeOfLastSpike = jnp.zeros((self.batch_size, self.n_units))
-        self.spikes = jnp.zeros((self.batch_size, self.n_units)) #None
-        if self.thr_persist == False: ## if thresh non-persistent, reset to base value
-            self.threshold = self.threshold0 + 0
+    @resolver(_advance_state)
+    def advance_state(self, j, s, tols, v, thr, rfr, surrogate):
+        self.j.set(j)
+        self.s.set(s)
+        self.tols.set(tols)
+        self.thr.set(thr)
+        self.rfr.set(rfr)
+        self.surrogate.set(surrogate)
+        self.v.set(v)
+
+    @staticmethod
+    def _reset(refract_T, thr_persist, threshold0, batch_size, n_units, thr):
+        restVals = jnp.zeros((batch_size, n_units))
+        voltage = restVals
+        refract = restVals + refract_T
+        current = restVals
+        surrogate = restVals + 1.
+        timeOfLastSpike = restVals
+        spikes = restVals
+        if not thr_persist: ## if thresh non-persistent, reset to base value
+            thr = threshold0 + 0
+        return current, spikes, timeOfLastSpike, voltage, thr, refract, surrogate
+
+    @resolver(_reset)
+    def reset(self, j, s, tols, v, thr, rfr, surrogate):
+        self.j.set(j)
+        self.s.set(s)
+        self.tols.set(tols)
+        self.thr.set(thr)
+        self.rfr.set(rfr)
+        self.surrogate.set(surrogate)
+        self.v.set(v)
 
     def save(self, directory, **kwargs):
         file_name = directory + "/" + self.name + ".npz"
         if self.thr_persist == False:
-            jnp.savez(file_name, threshold=self.threshold0)
+            jnp.savez(file_name, threshold=self.threshold0) # save threshold0
         else:
-            jnp.savez(file_name, threshold=self.threshold)
+            jnp.savez(file_name, threshold=self.thr.value) # save the actual threshold param/compartment
 
     def load(self, directory, **kwargs):
         file_name = directory + "/" + self.name + ".npz"
         data = jnp.load(file_name)
-        self.threshold = data['threshold']
-        self.threshold0 = self.threshold + 0
+        self.thr.set(data['threshold'])
+        self.threshold0 = self.thr.value + 0
+
+    def __repr__(self):
+        comps = [varname for varname in dir(self) if Compartment.is_compartment(getattr(self, varname))]
+        maxlen = max(len(c) for c in comps) + 5
+        lines = f"[{self.__class__.__name__}] PATH: {self.name}\n"
+        for c in comps:
+            stats = tensorstats(getattr(self, c).value)
+            if stats is not None:
+                line = [f"{k}: {v}" for k, v in stats.items()]
+                line = ", ".join(line)
+            else:
+                line = "None"
+            lines += f"  {f'({c})'.ljust(maxlen)}{line}\n"
+        return lines
+
+if __name__ == '__main__':
+    from ngcsimlib.context import Context
+    with Context("Bar") as bar:
+        X = SLIFCell("X", 9, 0.0004, 3, 0.3)
+    print(X)
```

### Comparing `ngclearn-1.0b4/ngclearn/components/__init__.py` & `ngclearn-1.1b0/ngclearn/components/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 ## point to rate-coded cell componet types
 from .neurons.graded.rateCell import RateCell
 from .neurons.graded.gaussianErrorCell import GaussianErrorCell
 from .neurons.graded.laplacianErrorCell import LaplacianErrorCell
 ## point to standard spiking cell component types
 from .neurons.spiking.sLIFCell import SLIFCell
 from .neurons.spiking.LIFCell import LIFCell
+from .neurons.spiking.WTASCell import WTASCell
 from .neurons.spiking.quadLIFCell import QuadLIFCell
+from .neurons.spiking.adExCell import AdExCell
 from .neurons.spiking.fitzhughNagumoCell import FitzhughNagumoCell
 from .neurons.spiking.izhikevichCell import IzhikevichCell
 ## point to transformer/operater component types
 from .other.varTrace import VarTrace
 from .other.expKernel import ExpKernel
 ## point to input encoder component types
 from .input_encoders.bernoulliCell import BernoulliCell
 from .input_encoders.poissonCell import PoissonCell
 from .input_encoders.latencyCell import LatencyCell
 ## point to synapse component types
+from .synapses.staticSynapse import StaticSynapse
 from .synapses.hebbian.hebbianSynapse import HebbianSynapse
 from .synapses.hebbian.traceSTDPSynapse import TraceSTDPSynapse
 from .synapses.hebbian.expSTDPSynapse import ExpSTDPSynapse
+from .synapses.hebbian.eventSTDPSynapse import EventSTDPSynapse
```

### Comparing `ngclearn-1.0b4/ngclearn/components/input_encoders/latencyCell.py` & `ngclearn-1.1b0/ngclearn/components/input_encoders/latencyCell.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from ngcsimlib.component import Component
+from ngclearn import resolver, Component, Compartment
+from ngclearn.utils import tensorstats
 from ngclearn.utils.model_utils import clamp_min, clamp_max
 from jax import numpy as jnp, random, jit
 from functools import partial
 import time
 
 @jit
 def update_times(t, s, tols):
@@ -138,112 +139,114 @@
                 for the "num_steps" argument (>1), depending on how many steps simulated
 
         num_steps: number of discrete time steps to consider for normalized latency
             code (only useful if "normalize" is set to True) (Default: 1)
 
         key: PRNG key to control determinism of any underlying synapses
             associated with this cell
-
-        useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
     """
 
-    ## Class Methods for Compartment Names
-    @classmethod
-    def inputCompartmentName(cls):
-        return 'in'
-
-    @classmethod
-    def outputCompartmentName(cls):
-        return 'out'
-
-    @classmethod
-    def timeOfLastSpikeCompartmentName(cls):
-        return 'tols'
-
-    ## Bind Properties to Compartments for ease of use
-    @property
-    def inputCompartment(self):
-        return self.compartments.get(self.inputCompartmentName(), None)
-
-    @inputCompartment.setter
-    def inputCompartment(self, inp):
-        self.compartments[self.inputCompartmentName()] = inp
-
-    @property
-    def outputCompartment(self):
-        return self.compartments.get(self.outputCompartmentName(), None)
-
-    @outputCompartment.setter
-    def outputCompartment(self, out):
-        self.compartments[self.outputCompartmentName()] = out
-
-    @property
-    def timeOfLastSpike(self):
-        return self.compartments.get(self.timeOfLastSpikeCompartmentName(), None)
-
-    @timeOfLastSpike.setter
-    def timeOfLastSpike(self, t):
-        self.compartments[self.timeOfLastSpikeCompartmentName()] = t
-
     # Define Functions
     def __init__(self, name, n_units, tau=1., threshold=0.01, first_spike_time=0.,
-                 linearize=False, normalize=False, num_steps=1., key=None,
-                 useVerboseDict=False, **kwargs):
-        super().__init__(name, useVerboseDict, **kwargs)
-
-        ##Random Number Set up
-        self.key = key
-        if self.key is None:
-            self.key = random.PRNGKey(time.time_ns())
+                 linearize=False, normalize=False, num_steps=1., key=None, **kwargs):
+        super().__init__(name, **kwargs)
 
+        ## latency meta-parameters
         self.first_spike_time = first_spike_time
         self.tau = tau
         self.threshold = threshold
         self.linearize = linearize
         ## normalize latency code s.t. final spike(s) occur w/in num_steps
         self.normalize = normalize
         self.num_steps = num_steps
 
-        self.target_spike_times = None
-        self._mask = None
-
-        ##Layer Size Setup
+        ## Layer Size Setup
         self.batch_size = 1
         self.n_units = n_units
-        self.reset()
-
-    def verify_connections(self):
-        pass
-
-    def advance_state(self, t, dt, **kwargs):
-        self.key, *subkeys = random.split(self.key, 2)
-        tau = self.tau
-        data = self.inputCompartment ## get sensory pattern data / features
-
-        if self.target_spike_times == None: ## calc spike times if not called yet
-            if self.linearize == True: ## linearize spike time calculation
-                stimes = calc_spike_times_linear(data, tau, self.threshold,
-                                                 self.first_spike_time,
-                                                 self.num_steps, self.normalize)
-                self.target_spike_times = stimes
-            else: ## standard nonlinear spike time calculation
-                stimes = calc_spike_times_nonlinear(data, tau, self.threshold,
-                                                    self.first_spike_time,
-                                                    num_steps=self.num_steps,
-                                                    normalize=self.normalize)
-                self.target_spike_times = stimes
-            #print(self.target_spike_times)
-            #sys.exit(0)
-        spk_mask = self._mask
-        spikes, spk_mask = extract_spike(self.target_spike_times, t, spk_mask) ## get spikes at t
-        self._mask = spk_mask
-        self.outputCompartment = spikes
-        self.timeOfLastSpike = update_times(t, self.outputCompartment, self.timeOfLastSpike)
-
-    def reset(self, **kwargs):
-        self.inputCompartment = None
-        self.outputCompartment = jnp.zeros((self.batch_size, self.n_units)) #None
-        self.timeOfLastSpike = jnp.zeros((self.batch_size, self.n_units))
-        self._mask = jnp.zeros((self.batch_size, self.n_units))
 
-    def save(self, **kwargs):
-        pass
+        ## Compartment setup
+        restVals = jnp.zeros((self.batch_size, self.n_units))
+        self.inputs = Compartment(restVals) # input compartment
+        self.outputs = Compartment(restVals) # output compartment
+        self.tols = Compartment(restVals) # time of last spike
+        self.key = Compartment(random.PRNGKey(time.time_ns()) if key is None else key)
+        self.targ_sp_times = Compartment(restVals)
+        #self.reset()
+
+    @staticmethod
+    def _calc_spike_times(t, dt, linearize, tau, threshold, first_spike_time,
+        num_steps, normalize, inputs):
+        ## would call this function before processing a spike train (at start)
+        data = inputs
+        if linearize == True: ## linearize spike time calculation
+            stimes = calc_spike_times_linear(data, tau, threshold,
+                                             first_spike_time,
+                                             num_steps, normalize)
+            targ_sp_times = stimes #* calcEvent + targ_sp_times * (1. - calcEvent)
+        else: ## standard nonlinear spike time calculation
+            stimes = calc_spike_times_nonlinear(data, tau, threshold,
+                                                first_spike_time,
+                                                num_steps=num_steps,
+                                                normalize=normalize)
+            targ_sp_times = stimes #* calcEvent + targ_sp_times * (1. - calcEvent)
+        return targ_sp_times
+
+    @resolver(_calc_spike_times)
+    def calc_spike_times(self, targ_sp_times):
+        self.targ_sp_times.set(targ_sp_times)
+
+    @staticmethod
+    def _advance_state(t, dt, key, inputs, mask, targ_sp_times, tols):
+        key, *subkeys = random.split(key, 2)
+        data = inputs ## get sensory pattern data / features
+        spikes, spk_mask = extract_spike(targ_sp_times, t, mask) ## get spikes at t
+        return spikes, tols, spk_mask, targ_sp_times, key
+
+    @resolver(_advance_state)
+    def advance_state(self, outputs, tols, mask, targ_sp_times, key):
+        self.outputs.set(outputs)
+        self.tols.set(tols)
+        self.mask.set(mask)
+        self.targ_sp_times.set(targ_sp_times)
+        self.key.set(key)
+
+    @staticmethod
+    def _reset(batch_size, n_units):
+        restVals = jnp.zeros((batch_size, n_units))
+        return (restVals, restVals, restVals, restVals, restVals)
+
+    @resolver(_reset)
+    def reset(self, inputs, outputs, tols, mask, targ_sp_times):
+        self.inputs.set(inputs)
+        self.outputs.set(outputs)
+        self.tols.set(tols)
+        self.mask.set(mask)
+        self.targ_sp_times.set(targ_sp_times)
+
+    def save(self, directory, **kwargs):
+        file_name = directory + "/" + self.name + ".npz"
+        jnp.savez(file_name, key=self.key.value)
+
+    def load(self, directory, **kwargs):
+        file_name = directory + "/" + self.name + ".npz"
+        data = jnp.load(file_name)
+        self.key.set( data['key'] )
+
+    def __repr__(self):
+        comps = [varname for varname in dir(self) if Compartment.is_compartment(getattr(self, varname))]
+        maxlen = max(len(c) for c in comps) + 5
+        lines = f"[{self.__class__.__name__}] PATH: {self.name}\n"
+        for c in comps:
+            stats = tensorstats(getattr(self, c).value)
+            if stats is not None:
+                line = [f"{k}: {v}" for k, v in stats.items()]
+                line = ", ".join(line)
+            else:
+                line = "None"
+            lines += f"  {f'({c})'.ljust(maxlen)}{line}\n"
+        return lines
+
+if __name__ == '__main__':
+    from ngcsimlib.context import Context
+    with Context("Bar") as bar:
+        X = LatencyCell("X", 9)
+    print(X)
```

### Comparing `ngclearn-1.0b4/ngclearn/components/neurons/graded/rateCell.py` & `ngclearn-1.1b0/ngclearn/components/neurons/spiking/fitzhughNagumoCell.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,265 +1,239 @@
-from ngcsimlib.component import Component
-from jax import numpy as jnp, random, jit, nn
+from jax import numpy as jnp, random, jit
 from functools import partial
-from ngclearn.utils.model_utils import create_function, threshold_soft, \
-                                       threshold_cauchy
-import time, sys
+import time
+from ngclearn import resolver, Component, Compartment
+from ngclearn.utils import tensorstats
 from ngclearn.utils.diffeq.ode_utils import get_integrator_code, \
                                             step_euler, step_rk2
 
-## rewritten code
-@partial(jit, static_argnums=[3, 4, 5])
-def _dfz_internal(z, j, j_td, tau_m, leak_gamma, priorType=None): ## raw dynamics
-    z_leak = z # * 2 ## Default: assume Gaussian
-    if priorType != None:
-        if priorType == "laplacian": ## Laplace dist
-            z_leak = jnp.sign(z) ## d/dx of Laplace is signum
-        elif priorType == "cauchy":  ## Cauchy dist: x ~ (1.0 + tf.math.square(z))
-            z_leak = (z * 2)/(1. + jnp.square(z))
-        elif priorType == "exp":  ## Exp dist: x ~ -exp(-x^2)
-            z_leak = jnp.exp(-jnp.square(z)) * z * 2
-    dz_dt = (-z_leak * leak_gamma + (j + j_td)) * (1./tau_m)
-    return dz_dt
-
-def _dfz(t, z, params): ## diff-eq dynamics wrapper
-    j, j_td, tau_m, leak_gamma, priorType = params
-    dz_dt = _dfz_internal(z, j, j_td, tau_m, leak_gamma, priorType)
-    return dz_dt
-
 @jit
-def modulate(j, dfx_val):
+def update_times(t, s, tols):
     """
-    Apply a signal modulator to j (typically of the form of a derivative/dampening function)
+    Updates time-of-last-spike (tols) variable.
 
     Args:
-        j: current/stimulus value to modulate
+        t: current time (a scalar/int value)
+
+        s: binary spike vector
 
-        dfx_val: modulator signal
+        tols: current time-of-last-spike variable
 
     Returns:
-        modulated j value
+        updated tols variable
     """
-    return j * dfx_val
+    _tols = (1. - s) * tols + (s * t)
+    return _tols
+
+@jit
+def _dfv_internal(j, v, w, a, b, g, tau_m): ## raw voltage dynamics
+    dv_dt = v - jnp.power(v, 3)/g - w + j ## dv/dt
+    dv_dt = dv_dt * (1./tau_m)
+    return dv_dt
+
+def _dfv(t, v, params): ## voltage dynamics wrapper
+    j, w, a, b, g, tau_m = params
+    dv_dt = _dfv_internal(j, v, w, a, b, g, tau_m)
+    return dv_dt
+
+@jit
+def _dfw_internal(j, v, w, a, b, g, tau_w): ## raw recovery dynamics
+    dw_dt = v + a - b * w ## dw/dt
+    dw_dt = dw_dt * (1./tau_w)
+    return dw_dt
+
+def _dfw(t, w, params): ## recovery dynamics wrapper
+    j, v, a, b, g, tau_m = params
+    dv_dt = _dfw_internal(j, v, w, a, b, g, tau_m)
+    return dv_dt
+
+@jit
+def _emit_spike(v, v_thr):
+    s = (v > v_thr).astype(jnp.float32)
+    return s
 
-def run_cell(dt, j, j_td, z, tau_m, leak_gamma=0., beta=1., integType=0,
-             priorType=None):
+#@partial(jit, static_argnums=[10])
+def run_cell(dt, j, v, w, v_thr, tau_m, tau_w, a, b, g=3., integType=0):
     """
-    Runs leaky rate-coded state dynamics one step in time.
 
     Args:
         dt: integration time constant
 
-        j: input (bottom-up) electrical/stimulus current
+        j: electrical current
 
-        j_td: modulatory (top-down) electrical/stimulus pressure
+        v: membrane potential / voltage
 
-        z: current value of membrane/state
+        w: recovery variable value(s)
 
-        tau_m: membrane/state time constant
+        v_thr: voltage/membrane threshold (to obtain action potentials in terms
+            of binary spikes)
 
-        leak_gamma: strength of leak to apply to membrane/state
+        tau_m: membrane time constant
 
-        beta: dampening coefficient (Default: 1.)
+        tau_w: recover variable time constant (Default: 12.5 ms)
 
-        integType: integration type to use (0 --> Euler/RK1, 1 --> Midpoint/RK2)
-
-        priorType: scale-shift prior distribution to impose over neural dynamics
+        a: dimensionless recovery variable shift factor "alpha" (Default: 0.7)
 
-    Returns:
-        New value of membrane/state for next time step
-    """
-    if integType == 1:
-        params = (j, j_td, tau_m, leak_gamma, priorType)
-        _, _z = step_rk2(0., z, _dfz, dt, params)
-    else:
-        params = (j, j_td, tau_m, leak_gamma, priorType)
-        _, _z = step_euler(0., z, _dfz, dt, params)
-    return _z
+        b: dimensionless recovery variable scale factor "beta" (Default: 0.8)
 
-@jit
-def run_cell_stateless(j):
-    """
-    A simplification of running a stateless set of dynamics over j (an identity
-    functional form of dynamics).
+        g: power-term divisor 'gamma' (Default: 3.)
 
-    Args:
-        j: stimulus to do nothing to
+        integType: integration type to use (0 --> Euler/RK1, 1 --> Midpoint/RK2)
 
     Returns:
-        the stimulus
-    """
-    return j + 0
-
-class RateCell(Component): ## Rate-coded/real-valued cell
+        updated voltage, updated recovery, spikes
     """
-    A non-spiking cell driven by the gradient dynamics of neural generative
-    coding-driven predictive processing.
+    if integType == 1:
+        v_params = (j, w, a, b, g, tau_m)
+        _, _v = step_rk2(0., v, _dfv, dt, v_params) #_v = step_rk2(v, v_params, _dfv, dt)
+        w_params = (j, v, a, b, g, tau_w)
+        _, _w = step_rk2(0., w, _dfw, dt, w_params) #_w = step_rk2(w, w_params, _dfw, dt)
+    else: # integType == 0 (default -- Euler)
+        v_params = (j, w, a, b, g, tau_m)
+        _, _v = step_euler(0., v, _dfv, dt, v_params) #_v = step_euler(v, v_params, _dfv, dt)
+        w_params = (j, v, a, b, g, tau_w)
+        _, _w = step_euler(0., w, _dfw, dt, w_params) #_w = step_euler(w, w_params, _dfw, dt)
+    #s = (_v > v_thr).astype(jnp.float32)
+    s = _emit_spike(_v, v_thr)
+    return _v, _w, s
+
+class FitzhughNagumoCell(Component):
+    """
+    The Fitzhugh-Nagumo neuronal cell model; a two-variable simplification
+    of the Hodgkin-Huxley (squid axon) model. This cell model iteratively evolves
+    voltage "v" and recovery "w" (which represents the combined effects of
+    sodium channel deinactivation and potassium channel deactivation in the
+    Hodgkin-Huxley model).
+
+    The specific pair of differential equations that characterize this cell
+    are (for adjusting v and w, given current j, over time):
+
+    | tau_m * dv/dt = v - (v^3)/3 - w + j
+    | tau_w * dw/dt = v + a - b * w
+
+    | References:
+    | FitzHugh, Richard. "Impulses and physiological states in theoretical
+    | models of nerve membrane." Biophysical journal 1.6 (1961): 445-466.
+    |
+    | Nagumo, Jinichi, Suguru Arimoto, and Shuji Yoshizawa. "An active pulse
+    | transmission line simulating nerve axon." Proceedings of the IRE 50.10
+    | (1962): 2061-2070.
 
     Args:
         name: the string name of this cell
 
         n_units: number of cellular entities (neural population size)
 
-        tau_m: membrane/state time constant (milliseconds)
+        tau_m: membrane time constant
+
+        tau_w: recover variable time constant (Default: 12.5 ms)
+
+        alpha: dimensionless recovery variable shift factor "a" (Default: 0.7)
+
+        beta: dimensionless recovery variable scale factor "b" (Default: 0.8)
+
+        gamma: power-term divisor (Default: 3.)
 
-        prior: a kernel for specifying the type of centered scale-shift distribution
-            to impose over neuronal dynamics, applied to each neuron or
-            dimension within this component (Default: ("gaussian", 0)); this is
-            a tuple with 1st element containing a string name of the distribution
-            one wants to use while the second value is a `leak rate` scalar
-            that controls the influence/weighting that this distribution
-            has on the dynamics; for example, ("laplacian, 0.001") means that a
-            centered laplacian distribution scaled by `0.001` will be injected
-            into this cell's dynamics ODE each step of simulated time
+        v_thr: voltage/membrane threshold (to obtain action potentials in terms
+            of binary spikes)
 
-            :Note: supported scale-shift distributions include "laplacian",
-                "cauchy", "exp", and "gaussian"
+        v0: initial condition / reset for voltage
 
-        act_fx: string name of activation function/nonlinearity to use
+        w0: initial condition / reset for recovery
 
         integration_type: type of integration to use for this cell's dynamics;
             current supported forms include "euler" (Euler/RK-1 integration)
             and "midpoint" or "rk2" (midpoint method/RK-2 integration) (Default: "euler")
 
             :Note: setting the integration type to the midpoint method will
                 increase the accuray of the estimate of the cell's evolution
                 at an increase in computational cost (and simulation time)
 
-        key: PRNG Key to control determinism of any underlying random values
+        key: PRNG key to control determinism of any underlying synapses
             associated with this cell
-
-        useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
     """
 
-    ## Class Methods for Compartment Names
-    @classmethod
-    def inputCompartmentName(cls):
-        return 'j' ## electrical current
-
-    @classmethod
-    def outputCompartmentName(cls): # OR: activityName()
-        return 'zF' ## rate-coded output
-
-    @classmethod
-    def pressureName(cls):
-        return 'j_td'
-
-    @classmethod
-    def rateActivityName(cls):
-        return 'z'
-
-    ## Bind Properties to Compartments for ease of use
-    @property
-    def inputCompartment(self):
-        return self.compartments.get(self.inputCompartmentName(), None)
-
-    @inputCompartment.setter
-    def inputCompartment(self, out):
-        self.compartments[self.inputCompartmentName()] = out
-
-    @property
-    def outputCompartment(self):
-        return self.compartments.get(self.outputCompartmentName(), None)
-
-    @outputCompartment.setter
-    def outputCompartment(self, out):
-        self.compartments[self.outputCompartmentName()] = out
-
-    @property
-    def current(self):
-        return self.compartments.get(self.inputCompartmentName(), None)
-
-    @current.setter
-    def current(self, inp):
-        self.compartments[self.inputCompartmentName()] = inp
-
-    @property
-    def pressure(self):
-        return self.compartments.get(self.pressureName(), None)
-
-    @pressure.setter
-    def pressure(self, inp):
-        self.compartments[self.pressureName()] = inp
-
-    @property
-    def rateActivity(self):
-        return self.compartments.get(self.rateActivityName(), None)
-
-    @rateActivity.setter
-    def rateActivity(self, out):
-        self.compartments[self.rateActivityName()] = out
-
-    @property
-    def activity(self):
-        return self.compartments.get(self.outputCompartmentName(), None)
-
-    @activity.setter
-    def activity(self, out):
-        self.compartments[self.outputCompartmentName()] = out
-
     # Define Functions
-    def __init__(self, name, n_units, tau_m, prior=("gaussian", 0.),
-                 act_fx="identity", threshold=("none", 0.),
-                 integration_type="euler", key=None, useVerboseDict=False, **kwargs):
-        super().__init__(name, useVerboseDict, **kwargs)
-
-        ##Random Number Set up
-        self.key = key
-        if self.key is None:
-            self.key = random.PRNGKey(time.time_ns())
-
-        ## membrane parameter setup (affects ODE integration)
-        self.tau_m = tau_m ## membrane time constant -- setting to 0 triggers "stateless" mode
-        priorType, leakRate = prior
-        self.priorType = priorType ## type of scale-shift prior to impose over the leak
-        self.priorLeakRate = leakRate ## degree to which rate neurons leak (according to prior)
-        thresholdType, thr_lmbda = threshold
-        self.thresholdType = thresholdType ## type of thresholding function to use
-        self.thr_lmbda = thr_lmbda ## scale to drive thresholding dynamics
+    def __init__(self, name, n_units, tau_m=1., tau_w=12.5, alpha=0.7,
+                 beta=0.8, gamma=3., v_thr=1.07, v0=0., w0=0.,
+                 integration_type="euler", key=None, **kwargs):
+        super().__init__(name, **kwargs)
 
-        ## integration properties
+        ## Integration properties
         self.integrationType = integration_type
         self.intgFlag = get_integrator_code(self.integrationType)
 
-        ##Layer Size Setup
-        self.n_units = n_units
-        self.batch_size = 1
-        self.fx, self.dfx = create_function(fun_name=act_fx)
-        self.reset()
+        ## Cell properties
+        self.tau_m = tau_m
+        self.tau_w = tau_w
+        self.alpha = alpha
+        self.beta = beta
+        self.gamma = gamma
+
+        self.v0 = v0 ## initial membrane potential/voltage condition
+        self.w0 = w0 ## initial w-parameter condition
+        self.v_thr = v_thr
 
-    def verify_connections(self):
-        self.metadata.check_incoming_connections(self.inputCompartmentName(), min_connections=1)
-
-    def advance_state(self, t, dt, **kwargs):
-        if self.tau_m > 0.:
-            ### run a step of integration over neuronal dynamics
-            ## Notes:
-            ## self.pressure <-- "top-down" expectation / contextual pressure
-            ## self.current <-- "bottom-up" data-dependent signal
-            dfx_val = self.dfx(self.rateActivity)
-            self.current = modulate(self.current, dfx_val)
-            z = run_cell(dt, self.current, self.pressure, self.rateActivity,
-                         self.tau_m, leak_gamma=self.priorLeakRate,
-                         integType=self.intgFlag, priorType=self.priorType)
-            ## apply optional thresholding sub-dynamics
-            if self.thresholdType == "soft_threshold":
-                z = threshold_soft(z, self.thr_lmbda)
-            elif self.thresholdType == "cauchy_threshold":
-                z = threshold_cauchy(z, self.thr_lmbda)
-            self.rateActivity = z
-            self.activity = self.fx(self.rateActivity)
-            self.current = None
-        else:
-            ## run in "stateless" mode (when no membrane time constant provided)
-            self.rateActivity = run_cell_stateless(self.current)
-            self.activity = self.fx(self.rateActivity)
-            #self.current = None
-
-    def reset(self, **kwargs):
-        self.current = jnp.zeros((self.batch_size, self.n_units))
-        self.pressure = jnp.zeros((self.batch_size, self.n_units))
-        self.rateActivity = jnp.zeros((self.batch_size, self.n_units))
-        self.activity = jnp.zeros((self.batch_size, self.n_units))
+        ## Layer Size Setup
+        self.batch_size = 1
+        self.n_units = n_units
 
-    def save(self, **kwargs):
-        pass
+        ## Compartment setup
+        restVals = jnp.zeros((self.batch_size, self.n_units))
+        self.j = Compartment(restVals)
+        self.v = Compartment(restVals + self.v0)
+        self.w = Compartment(restVals + self.w0)
+        self.s = Compartment(restVals)
+        self.tols = Compartment(restVals) ## time-of-last-spike
+
+    @staticmethod
+    def _advance_state(t, dt, tau_m, tau_w, v_thr, alpha, beta, gamma, intgFlag,
+                       j, v, w, s, tols):
+        v, w, s = run_cell(dt, j, v, w, v_thr, tau_m, tau_w, alpha, beta, gamma, intgFlag)
+        tols = update_times(t, s, tols)
+        return j, v, w, s, tols
+
+    @resolver(_advance_state)
+    def advance_state(self, j, v, w, s, tols):
+        self.j.set(j)
+        self.w.set(w)
+        self.v.set(v)
+        self.s.set(s)
+        self.tols.set(tols)
+
+    @staticmethod
+    def _reset(batch_size, n_units, v0, w0):
+        restVals = jnp.zeros((batch_size, n_units))
+        j = restVals # None
+        v = restVals + v0
+        w = restVals + w0
+        s = restVals #+ 0
+        tols = restVals #+ 0
+        return j, v, w, s, tols
+
+    @resolver(_reset)
+    def reset(self, j, v, w, s, tols):
+        self.j.set(j)
+        self.v.set(v)
+        self.w.set(w)
+        self.s.set(s)
+        self.tols.set(tols)
+
+    def __repr__(self):
+        comps = [varname for varname in dir(self) if Compartment.is_compartment(getattr(self, varname))]
+        maxlen = max(len(c) for c in comps) + 5
+        lines = f"[{self.__class__.__name__}] PATH: {self.name}\n"
+        for c in comps:
+            stats = tensorstats(getattr(self, c).value)
+            if stats is not None:
+                line = [f"{k}: {v}" for k, v in stats.items()]
+                line = ", ".join(line)
+            else:
+                line = "None"
+            lines += f"  {f'({c})'.ljust(maxlen)}{line}\n"
+        return lines
+
+if __name__ == '__main__':
+    from ngcsimlib.context import Context
+    with Context("Bar") as bar:
+        X = FitzhughNagumoCell("X", 9)
+    print(X)
```

### Comparing `ngclearn-1.0b4/ngclearn/components/neurons/spiking/fitzhughNagumoCell.py` & `ngclearn-1.1b0/ngclearn/components/neurons/spiking/adExCell.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from ngcsimlib.component import Component
 from jax import numpy as jnp, random, jit
 from functools import partial
 import time
+from ngclearn import resolver, Component, Compartment
+from ngclearn.utils import tensorstats
 from ngclearn.utils.diffeq.ode_utils import get_integrator_code, \
                                             step_euler, step_rk2
 
 @jit
 def update_times(t, s, tols):
     """
     Updates time-of-last-spike (tols) variable.
@@ -20,257 +21,204 @@
     Returns:
         updated tols variable
     """
     _tols = (1. - s) * tols + (s * t)
     return _tols
 
 @jit
-def _dfv_internal(j, v, w, a, b, g, tau_m): ## raw voltage dynamics
-    dv_dt = v - jnp.power(v, 3)/g - w + j ## dv/dt
+def _dfv_internal(j, v, w, tau_m, v_rest, sharpV, vT, R_m): ## raw voltage dynamics
+    dv_dt = -(v - v_rest) + sharpV * jnp.exp((v - vT)/sharpV) - R_m * w + R_m * j ## dv/dt
     dv_dt = dv_dt * (1./tau_m)
     return dv_dt
 
 def _dfv(t, v, params): ## voltage dynamics wrapper
-    j, w, a, b, g, tau_m = params
-    dv_dt = _dfv_internal(j, v, w, a, b, g, tau_m)
+    j, w, tau_m, v_rest, sharpV, vT, R_m = params
+    dv_dt = _dfv_internal(j, v, w, tau_m, v_rest, sharpV, vT, R_m)
     return dv_dt
 
 @jit
-def _dfw_internal(j, v, w, a, b, g, tau_w): ## raw recovery dynamics
-    dw_dt = v + a - b * w ## dw/dt
+def _dfw_internal(j, v, w, a, tau_w, v_rest): ## raw recovery dynamics
+    dw_dt = -w + (v - v_rest) * a #+ b * s * tau_w
     dw_dt = dw_dt * (1./tau_w)
     return dw_dt
 
 def _dfw(t, w, params): ## recovery dynamics wrapper
-    j, v, a, b, g, tau_m = params
-    dv_dt = _dfw_internal(j, v, w, a, b, g, tau_m)
+    j, v, a, tau_m, v_rest = params
+    dv_dt = _dfw_internal(j, v, w, a, tau_m, v_rest)
     return dv_dt
 
 @jit
 def _emit_spike(v, v_thr):
     s = (v > v_thr).astype(jnp.float32)
     return s
 
 #@partial(jit, static_argnums=[10])
-def run_cell(dt, j, v, w, v_thr, tau_m, tau_w, a, b, g=3., integType=0):
-    """
-
-    Args:
-        dt: integration time constant
-
-        j: electrical current
-
-        v: membrane potential / voltage
-
-        w: recovery variable value(s)
-
-        v_thr: voltage/membrane threshold (to obtain action potentials in terms
-            of binary spikes)
-
-        tau_m: membrane time constant
-
-        tau_w: recover variable time constant (Default: 12.5 ms)
-
-        a: dimensionless recovery variable shift factor "alpha" (Default: 0.7)
-
-        b: dimensionless recovery variable scale factor "beta" (Default: 0.8)
-
-        g: power-term divisor 'gamma' (Default: 3.)
-
-        integType: integration type to use (0 --> Euler/RK1, 1 --> Midpoint/RK2)
-
-    Returns:
-        updated voltage, updated recovery, spikes
-    """
-    if integType == 1:
-        v_params = (j, w, a, b, g, tau_m)
-        _, _v = step_rk2(0., v, _dfv, dt, v_params) #_v = step_rk2(v, v_params, _dfv, dt)
-        w_params = (j, v, a, b, g, tau_w)
-        _, _w = step_rk2(0., w, _dfw, dt, w_params) #_w = step_rk2(w, w_params, _dfw, dt)
+def run_cell(dt, j, v, w, v_thr, tau_m, tau_w, a, b, sharpV, vT,
+             v_rest, v_reset, R_m, integType=0):
+    if integType == 1: ## RK-2/midpoint
+        v_params = (j, w, tau_m, v_rest, sharpV, vT, R_m)
+        _, _v = step_rk2(0., v, _dfv, dt, v_params)
+        w_params = (j, v, a, tau_w, v_rest)
+        _, _w = step_rk2(0., w, _dfw, dt, w_params)
     else: # integType == 0 (default -- Euler)
-        v_params = (j, w, a, b, g, tau_m)
-        _, _v = step_euler(0., v, _dfv, dt, v_params) #_v = step_euler(v, v_params, _dfv, dt)
-        w_params = (j, v, a, b, g, tau_w)
-        _, _w = step_euler(0., w, _dfw, dt, w_params) #_w = step_euler(w, w_params, _dfw, dt)
+        v_params = (j, w, tau_m, v_rest, sharpV, vT, R_m)
+        _, _v = step_euler(0., v, _dfv, dt, v_params)
+        w_params = (j, v, a, tau_w, v_rest)
+        _, _w = step_euler(0., w, _dfw, dt, w_params)
     #s = (_v > v_thr).astype(jnp.float32)
     s = _emit_spike(_v, v_thr)
+    ## hyperpolarize/reset/snap variables
+    _v = _v * (1. - s) + s * v_reset
+    _w = _w * (1. - s) + s * (_w + b)
     return _v, _w, s
 
-class FitzhughNagumoCell(Component):
+class AdExCell(Component):
     """
-    The Fitzhugh-Nagumo neuronal cell model; a two-variable simplification
-    of the Hodgkin-Huxley (squid axon) model. This cell model iteratively evolves
-    voltage "v" and recovery "w" (which represents the combined effects of
-    sodium channel deinactivation and potassium channel deactivation in the
-    Hodgkin-Huxley model).
+    The AdEx (adaptive exponential leaky integrate-and-fire) neuronal cell
+    model; a two-variable model. This cell model iteratively evolves
+    voltage "v" and recovery "w".
 
     The specific pair of differential equations that characterize this cell
     are (for adjusting v and w, given current j, over time):
 
-    | tau_m * dv/dt = v - (v^3)/3 - w + j
-    | tau_w * dw/dt = v + a - b * w
+    | tau_m * dv/dt = -(v - v_rest) + sharpV * exp((v - vT)/sharpV) - R_m * w + R_m * j
+    | tau_w * dw/dt =  -w + (v - v_rest) * a
+    | where w = w + s * (w + b) [in the event of a spike]
+
 
     | References:
-    | FitzHugh, Richard. "Impulses and physiological states in theoretical
-    | models of nerve membrane." Biophysical journal 1.6 (1961): 445-466.
-    |
-    | Nagumo, Jinichi, Suguru Arimoto, and Shuji Yoshizawa. "An active pulse
-    | transmission line simulating nerve axon." Proceedings of the IRE 50.10
-    | (1962): 2061-2070.
+    | Brette, Romain, and Wulfram Gerstner. "Adaptive exponential integrate-and-fire
+    | model as an effective description of neuronal activity." Journal of
+    | neurophysiology 94.5 (2005): 3637-3642.
 
     Args:
         name: the string name of this cell
 
         n_units: number of cellular entities (neural population size)
 
-        tau_m: membrane time constant
+        tau_m: membrane time constant (Default: 15 ms)
 
-        tau_w: recover variable time constant (Default: 12.5 ms)
+        R_m: membrane resistance (Default: 1 mega-Ohm)
 
-        alpha: dimensionless recovery variable shift factor "a" (Default: 0.7)
+        tau_w: recover variable time constant (Default: 400 ms)
 
-        beta: dimensionless recovery variable scale factor "b" (Default: 0.8)
+        sharpV: slope factor/sharpness constant (Default: 2)
 
-        gamma: power-term divisor (Default: 3.)
+        vT: intrinsic membrane threshold (Default: -55 mV)
 
         v_thr: voltage/membrane threshold (to obtain action potentials in terms
-            of binary spikes)
+            of binary spikes) (Default: 5 mV)
+
+        v_rest: membrane resting potential (Default: -72 mV)
+
+        a: adaptation coupling parameter (Default: 0.1)
 
-        v0: initial condition / reset for voltage
+        b: adaption/recover increment value (Default: 0.75)
 
-        w0: initial condition / reset for recovery
+        v0: initial condition / reset for voltage (Default: -70 mV)
+
+        w0: initial condition / reset for recovery (Default: 0 mV)
 
         integration_type: type of integration to use for this cell's dynamics;
             current supported forms include "euler" (Euler/RK-1 integration)
             and "midpoint" or "rk2" (midpoint method/RK-2 integration) (Default: "euler")
 
             :Note: setting the integration type to the midpoint method will
                 increase the accuray of the estimate of the cell's evolution
                 at an increase in computational cost (and simulation time)
 
         key: PRNG key to control determinism of any underlying synapses
             associated with this cell
-
-        useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
     """
 
-    ## Class Methods for Compartment Names
-    @classmethod
-    def inputCompartmentName(cls):
-        return 'in'
-
-    @classmethod
-    def outputCompartmentName(cls):
-        return 'out'
-
-    @classmethod
-    def voltageName(cls):
-        return 'v'
-
-    @classmethod
-    def recoveryName(cls):
-        return 'w'
-
-    @classmethod
-    def timeOfLastSpikeCompartmentName(cls):
-        return 'tols'
-
-    ## Bind Properties to Compartments for ease of use
-    @property
-    def inputCompartment(self):
-        return self.compartments.get(self.inputCompartmentName(), None)
-
-    @inputCompartment.setter
-    def inputCompartment(self, inp):
-        self.compartments[self.inputCompartmentName()] = inp
-
-    @property
-    def outputCompartment(self):
-        return self.compartments.get(self.outputCompartmentName(), None)
-
-    @outputCompartment.setter
-    def outputCompartment(self, out):
-        self.compartments[self.outputCompartmentName()] = out
-
-    @property
-    def voltage(self):
-        return self.compartments.get(self.voltageName(), None)
-
-    @voltage.setter
-    def voltage(self, t):
-        self.compartments[self.voltageName()] = t
-
-    @property
-    def recovery(self):
-        return self.compartments.get(self.recoveryName(), None)
-
-    @recovery.setter
-    def recovery(self, t):
-        self.compartments[self.recoveryName()] = t
-
-    @property
-    def timeOfLastSpike(self):
-        return self.compartments.get(self.timeOfLastSpikeCompartmentName(), None)
-
-    @timeOfLastSpike.setter
-    def timeOfLastSpike(self, t):
-        self.compartments[self.timeOfLastSpikeCompartmentName()] = t
-
     # Define Functions
-    def __init__(self, name, n_units, tau_m=1., tau_w=12.5, alpha=0.7,
-                 beta=0.8, gamma=3., v_thr=1.07, v0=0., w0=0.,
-                 integration_type="euler", key=None, useVerboseDict=False,
-                 **kwargs):
-        super().__init__(name, useVerboseDict, **kwargs)
-
-        ## Random Number Set up
-        self.key = key
-        if self.key is None:
-            self.key = random.PRNGKey(time.time_ns())
+    def __init__(self, name, n_units, tau_m=15., R_m=1., tau_w=400.,
+                 sharpV=2., vT=-55., v_thr=5., v_rest=-72., v_reset=-75.,
+                 a=0.1, b=0.75, v0=-70., w0=0.,
+                 integration_type="euler", key=None, **kwargs):
+        super().__init__(name, **kwargs)
 
         ## Integration properties
         self.integrationType = integration_type
         self.intgFlag = get_integrator_code(self.integrationType)
 
         ## Cell properties
         self.tau_m = tau_m
+        self.R_m = R_m
         self.tau_w = tau_w
-        self.alpha = alpha
-        self.beta = beta
-        self.gamma = gamma
+        self.sharpV = sharpV ## sharpness of action potential
+        self.vT = vT ## intrinsic membrane threshold
+        self.a = a
+        self.b = b
+        self.v_rest = v_rest
+        self.v_reset = v_reset
 
         self.v0 = v0 ## initial membrane potential/voltage condition
         self.w0 = w0 ## initial w-parameter condition
         self.v_thr = v_thr
 
         ## Layer Size Setup
         self.batch_size = 1
         self.n_units = n_units
-        self.reset()
-
-    def verify_connections(self):
-        pass
-
-    def advance_state(self, t, dt, **kwargs):
-        self.key, *subkeys = random.split(self.key, 2)
-
-        j = self.inputCompartment
-        v = self.voltage
-        w = self.recovery
-
-        v, w, s = run_cell(dt, j, v, w, self.v_thr, self.tau_m, self.tau_w, self.alpha,
-                           self.beta, self.gamma, self.intgFlag)
-
-        self.voltage = v
-        self.recovery = w
-        self.outputCompartment = s
-        self.timeOfLastSpike = update_times(t, self.outputCompartment, self.timeOfLastSpike)
-
-    def reset(self, **kwargs):
-        self.inputCompartment = None
-        self.voltage = jnp.zeros((self.batch_size, self.n_units)) + self.v0
-        self.recovery = jnp.zeros((self.batch_size, self.n_units)) + self.w0
-        self.outputCompartment = jnp.zeros((self.batch_size, self.n_units)) #None
-        self.timeOfLastSpike = jnp.zeros((self.batch_size, self.n_units))
 
-    def save(self, **kwargs):
-        pass
+        ## Compartment setup
+        restVals = jnp.zeros((self.batch_size, self.n_units))
+        self.j = Compartment(restVals)
+        self.v = Compartment(restVals + self.v0)
+        self.w = Compartment(restVals + self.w0)
+        self.s = Compartment(restVals)
+        self.tols = Compartment(restVals) ## time-of-last-spike
+        #self.reset()
+
+    @staticmethod
+    def _advance_state(t, dt, tau_m, R_m, tau_w, v_thr, a, b, sharpV, vT,
+                     v_rest, v_reset, intgFlag, j, v, w, s, tols):
+        v, w, s = run_cell(dt, j, v, w, v_thr, tau_m, tau_w, a, b, sharpV, vT,
+                           v_rest, v_reset, R_m, intgFlag)
+        tols = update_times(t, s, tols)
+        return j, v, w, s, tols
+
+    @resolver(_advance_state)
+    def advance_state(self, j, v, w, s, tols):
+        self.j.set(j)
+        self.w.set(w)
+        self.v.set(v)
+        self.s.set(s)
+        self.tols.set(tols)
+
+    @staticmethod
+    def _reset(batch_size, n_units, v0, w0):
+        restVals = jnp.zeros((batch_size, n_units))
+        j = restVals # None
+        v = restVals + v0
+        w = restVals + w0
+        s = restVals #+ 0
+        tols = restVals #+ 0
+        return j, v, w, s, tols
+
+    @resolver(_reset)
+    def reset(self, j, v, w, s, tols):
+        self.j.set(j)
+        self.v.set(v)
+        self.w.set(w)
+        self.s.set(s)
+        self.tols.set(tols)
+
+    def __repr__(self):
+        comps = [varname for varname in dir(self) if Compartment.is_compartment(getattr(self, varname))]
+        maxlen = max(len(c) for c in comps) + 5
+        lines = f"[{self.__class__.__name__}] PATH: {self.name}\n"
+        for c in comps:
+            stats = tensorstats(getattr(self, c).value)
+            if stats is not None:
+                line = [f"{k}: {v}" for k, v in stats.items()]
+                line = ", ".join(line)
+            else:
+                line = "None"
+            lines += f"  {f'({c})'.ljust(maxlen)}{line}\n"
+        return lines
+
+if __name__ == '__main__':
+    from ngcsimlib.context import Context
+    with Context("Bar") as bar:
+        X = AdExCell("X", 9)
+    print(X)
```

### Comparing `ngclearn-1.0b4/ngclearn/components/neurons/spiking/izhikevichCell.py` & `ngclearn-1.1b0/ngclearn/components/neurons/spiking/izhikevichCell.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from ngcsimlib.component import Component
 from jax import numpy as jnp, random, jit, nn
 from functools import partial
 import time, sys
+from ngclearn.utils import tensorstats
+from ngclearn import resolver, Component, Compartment
 from ngclearn.utils.diffeq.ode_utils import get_integrator_code, \
                                             step_euler, step_rk2
 
 @jit
 def update_times(t, s, tols):
     """
     Updates time-of-last-spike (tols) variable.
@@ -61,15 +62,14 @@
     return s
 
 @jit
 def _modify_current(j, R_m):
     _j = j * R_m
     return _j
 
-#@partial(jit, static_argnums=[12])
 def run_cell(dt, j, v, s, w, v_thr=30., tau_m=1., tau_w=50., b=0.2, c=-65., d=8.,
              R_m=1., integType=0):
     """
     Runs Izhikevich neuronal dynamics
 
     Args:
         dt: integration time constant (milliseconds, or ms)
@@ -186,85 +186,21 @@
         integration_type: type of integration to use for this cell's dynamics;
             current supported forms include "euler" (Euler/RK-1 integration)
             and "midpoint" or "rk2" (midpoint method/RK-2 integration) (Default: "euler")
 
             :Note: setting the integration type to the midpoint method will
                 increase the accuray of the estimate of the cell's evolution
                 at an increase in computational cost (and simulation time)
-
-        useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
     """
 
-    ## Class Methods for Compartment Names
-    @classmethod
-    def inputCompartmentName(cls):
-        return 'in'
-
-    @classmethod
-    def outputCompartmentName(cls):
-        return 'out'
-
-    @classmethod
-    def voltageName(cls):
-        return 'v'
-
-    @classmethod
-    def recoveryName(cls):
-        return 'w'
-
-    @classmethod
-    def timeOfLastSpikeCompartmentName(cls):
-        return 'tols'
-
-    ## Bind Properties to Compartments for ease of use
-    @property
-    def inputCompartment(self):
-        return self.compartments.get(self.inputCompartmentName(), None)
-
-    @inputCompartment.setter
-    def inputCompartment(self, inp):
-        self.compartments[self.inputCompartmentName()] = inp
-
-    @property
-    def outputCompartment(self):
-        return self.compartments.get(self.outputCompartmentName(), None)
-
-    @outputCompartment.setter
-    def outputCompartment(self, out):
-        self.compartments[self.outputCompartmentName()] = out
-
-    @property
-    def voltage(self):
-        return self.compartments.get(self.voltageName(), None)
-
-    @voltage.setter
-    def voltage(self, t):
-        self.compartments[self.voltageName()] = t
-
-    @property
-    def recovery(self):
-        return self.compartments.get(self.recoveryName(), None)
-
-    @recovery.setter
-    def recovery(self, t):
-        self.compartments[self.recoveryName()] = t
-
-    @property
-    def timeOfLastSpike(self):
-        return self.compartments.get(self.timeOfLastSpikeCompartmentName(), None)
-
-    @timeOfLastSpike.setter
-    def timeOfLastSpike(self, t):
-        self.compartments[self.timeOfLastSpikeCompartmentName()] = t
-
     # Define Functions
     def __init__(self, name, n_units, tau_m=1., R_m=1., v_thr=30., v_reset=-65.,
                  tau_w=50., w_reset=8., coupling_factor=0.2, v0=-65., w0=-14.,
-                 integration_type="euler", key=None, useVerboseDict=False, **kwargs):
-        super().__init__(name, useVerboseDict, **kwargs)
+                 integration_type="euler", key=None, **kwargs):
+        super().__init__(name, **kwargs)
 
         ## Cell properties
         self.R_m = R_m
         self.tau_m = tau_m
         self.tau_w = tau_w
         self.coupling = coupling_factor
         self.v_reset = v_reset
@@ -274,43 +210,73 @@
         self.w0 = w0 ## initial recovery w-parameter condition
         self.v_thr = v_thr
 
         ## Integration properties
         self.integrationType = integration_type
         self.intgFlag = get_integrator_code(self.integrationType)
 
-        ##Random Number Set up
-        self.key = key
-        if self.key is None:
-            self.key = random.PRNGKey(time.time_ns())
-
         ##Layer Size Setup
         self.batch_size = 1
         self.n_units = n_units
 
-        self.reset()
-
-    def verify_connections(self):
-        self.metadata.check_incoming_connections(self.inputCompartmentName(), min_connections=1)
-
-    def advance_state(self, t, dt, **kwargs):
-        j = self.inputCompartment
-        v = self.voltage
-        w = self.recovery
-        s = self.outputCompartment
-        #if self.integration_type == "euler":
-        v, w, s = run_cell(dt, j, v, s, w, v_thr=self.v_thr, tau_m=self.tau_m,
-                           tau_w=self.tau_w, b=self.coupling, c=self.v_reset,
-                           d=self.w_reset, R_m=self.R_m, integType=self.intgFlag)
-        self.voltage = v
-        self.recovery = w
-        self.outputCompartment = s
-
-    def reset(self, **kwargs):
-        self.inputCompartment = None
-        self.voltage = jnp.zeros((self.batch_size, self.n_units)) + self.v0
-        self.recovery = jnp.zeros((self.batch_size, self.n_units)) + self.w0
-        self.outputCompartment = jnp.zeros((self.batch_size, self.n_units)) #None
-        self.timeOfLastSpike = jnp.zeros((self.batch_size, self.n_units))
-
-    def save(self, directory, **kwargs):
-        pass
+        ## Compartment setup
+        restVals = jnp.zeros((self.batch_size, self.n_units))
+        self.j = Compartment(restVals)
+        self.v = Compartment(restVals + self.v0)
+        self.w = Compartment(restVals + self.w0)
+        self.s = Compartment(restVals)
+        self.tols = Compartment(restVals) ## time-of-last-spike
+        #self.reset()
+
+    @staticmethod
+    def _advance_state(t, dt, tau_m, tau_w, v_thr, coupling, v_reset, w_reset, R_m,
+                       intgFlag, j, v, w, s, tols):
+        v, w, s = run_cell(dt, j, v, s, w, v_thr=v_thr, tau_m=tau_m, tau_w=tau_w,
+                           b=coupling, c=v_reset, d=w_reset, R_m=R_m, integType=intgFlag)
+        tols = update_times(t, s, tols)
+        return j, v, w, s, tols
+
+    @resolver(_advance_state)
+    def advance_state(self, j, v, w, s, tols):
+        self.j.set(j)
+        self.w.set(w)
+        self.v.set(v)
+        self.s.set(s)
+        self.tols.set(tols)
+
+    @staticmethod
+    def _reset(batch_size, n_units, v0, w0):
+        restVals = jnp.zeros((batch_size, n_units))
+        j = restVals # None
+        v = restVals + v0
+        w = restVals + w0
+        s = restVals #+ 0
+        tols = restVals #+ 0
+        return j, v, w, s, tols
+
+    @resolver(_reset)
+    def reset(self, j, v, w, s, tols):
+        self.j.set(j)
+        self.v.set(v)
+        self.w.set(w)
+        self.s.set(s)
+        self.tols.set(tols)
+
+    def __repr__(self):
+        comps = [varname for varname in dir(self) if Compartment.is_compartment(getattr(self, varname))]
+        maxlen = max(len(c) for c in comps) + 5
+        lines = f"[{self.__class__.__name__}] PATH: {self.name}\n"
+        for c in comps:
+            stats = tensorstats(getattr(self, c).value)
+            if stats is not None:
+                line = [f"{k}: {v}" for k, v in stats.items()]
+                line = ", ".join(line)
+            else:
+                line = "None"
+            lines += f"  {f'({c})'.ljust(maxlen)}{line}\n"
+        return lines
+
+if __name__ == '__main__':
+    from ngcsimlib.context import Context
+    with Context("Bar") as bar:
+        X = IzhikevichCell("X", 9)
+    print(X)
```

### Comparing `ngclearn-1.0b4/ngclearn/components/other/expKernel.py` & `ngclearn-1.1b0/ngclearn/components/other/expKernel.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,123 +1,108 @@
-from ngcsimlib.component import Component
-from jax import numpy as jnp, random, jit
-from functools import partial
-import time, sys
-
-@partial(jit, static_argnums=[5,6])
-def apply_kernel(tf_curr, s, t, tau_w, win_len, krn_start, krn_end):
-    idx_sub = tf_curr.shape[0]-1
-    tf_new = (s * t) ## track new spike time(s)
-    tf = tf_curr.at[idx_sub,:,:].set(tf_new)
-    tf = jnp.roll(tf, shift=-1, axis=0) # 1,2,3  2,3,1
-
-    ## apply exp time kernel
-    ## EPSP = sum_{tf} exp(-(t - tf)/tau_w)
-    _tf = tf[krn_start:krn_end,:,:]
-    mask = jnp.greater(_tf, 0.).astype(jnp.float32) # 1 for every valid tf (non-zero)
-    epsp = jnp.sum( jnp.exp( -(t - _tf)/tau_w ) * mask, axis=0 )
-    return tf, epsp
-
-class ExpKernel(Component): ## Exponential spike kernel
-    """
-    A spiking function based on an exponential kernel applied to
-    a moving window of spike times.
-
-    Args:
-        name: the string name of this operator
-
-        n_units: number of calculating entities or units
-
-        nu: (ms, spike time interval for window)
-
-        tau_w: spike window time constant (in micro-secs, or nano-s)
-
-        key: PRNG key to control determinism of any underlying random values
-            associated with this cell
-
-        useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
-
-        directory: string indicating directory on disk to save sLIF parameter
-            values to (i.e., initial threshold values and any persistent adaptive
-            threshold values)
-    """
-
-    ## Class Methods for Compartment Names
-    @classmethod
-    def inputCompartmentName(cls):
-        return 'in'
-
-    @classmethod
-    def outputCompartmentName(cls):
-        return 'out'
-
-    ## Bind Properties to Compartments for ease of use
-    @property
-    def inputCompartment(self):
-      return self.compartments.get(self.inputCompartmentName(), None)
-
-    @inputCompartment.setter
-    def inputCompartment(self, inp):
-      self.compartments[self.inputCompartmentName()] = inp
-
-    @property
-    def epsp(self):
-        return self.compartments.get(self.outputCompartmentName(), None)
-
-    @epsp.setter
-    def epsp(self, inp):
-        self.compartments[self.outputCompartmentName()] = inp
-
-    # Define Functions
-    def __init__(self, name, n_units, tau_w=500., nu=4., key=None,
-                 useVerboseDict=False, directory=None, **kwargs):
-        super().__init__(name, useVerboseDict, **kwargs)
-
-        ##Random Number Set up
-        self.key = key
-        if self.key is None:
-            self.key = random.PRNGKey(time.time_ns())
-
-        ##TMP
-        self.key, subkey = random.split(self.key)
-
-        ## trace control coefficients
-        self.tau_w = tau_w ## kernel window time constant
-        self.nu = nu
-        self.win_len = int(nu/dt) + 1 ## window length
-        self.tf = None #[] ## window of spike times
-
-        # cell compartments
-        # self.comp["in"] = None
-        # self.comp["epsp"] = None ## this emits a numeric "pulse" ()
-        # self.comp["tf"] = [] # window of spike times
-
-        ##Layer Size Setup
-        self.n_units = n_units
-        self.reset()
-
-    def verify_connections(self):
-        self.metadata.check_incoming_connections(self.inputCompartmentName(),
-                                                 min_connections=1)
-
-    def advance_state(self, t, dt, **kwargs):
-        #self.t = self.t + self.dt
-        self.gather()
-        s = self.inputCompartment #self.comp["in"] ## get incoming spike readout
-        tf = self.tf #self.comp["tf"] ## get current window/volume
-
-        _tf, epsp = apply_kernel(tf, s, self.t, self.tau_w, self.win_len,
-                                 krn_start=0, krn_end=self.win_len-1) #0:win_len-1)
-        self.tf = _tf ## get 2D batch matrix
-        self.epsp = epsp ## update spike time window
-        # self.comp["epsp"] = epsp ## get 2D batch matrix
-        # self.comp["tf"] = _tf ## update spike time window
-        #self.inputCompartment = None
-
-    def reset(self, **kwargs):
-        self.tf = jnp.zeros([self.win_len, batch_size, self.n_units])
-        #self.comp["tf"] = jnp.zeros([self.win_len, batch_size, self.n_units])
-        self.inputCompartment = None
-        self.outputCompartment = None
-
-    def save(self, **kwargs):
-        pass
+from jax import numpy as jnp, random, jit
+from functools import partial
+from ngclearn import resolver, Component, Compartment
+from ngclearn.utils import tensorstats
+import time, sys
+
+@partial(jit, static_argnums=[5,6])
+def apply_kernel(tf_curr, s, t, tau_w, win_len, krn_start, krn_end):
+    idx_sub = tf_curr.shape[0]-1
+    tf_new = (s * t) ## track new spike time(s)
+    tf = tf_curr.at[idx_sub,:,:].set(tf_new)
+    tf = jnp.roll(tf, shift=-1, axis=0) # 1,2,3  2,3,1
+
+    ## apply exp time kernel
+    ## EPSP = sum_{tf} exp(-(t - tf)/tau_w)
+    _tf = tf[krn_start:krn_end,:,:]
+    mask = jnp.greater(_tf, 0.).astype(jnp.float32) # 1 for every valid tf (non-zero)
+    epsp = jnp.sum( jnp.exp( -(t - _tf)/tau_w ) * mask, axis=0 )
+    return tf, epsp
+
+class ExpKernel(Component): ## exponential kernel
+    """
+    A spiking function based on an exponential kernel applied to
+    a moving window of spike times.
+
+    Args:
+        name: the string name of this operator
+
+        n_units: number of calculating entities or units
+
+        dt: integration time constant (the kernel needs access to this value)
+
+        nu: (ms, spike time interval for window)
+
+        tau_w: spike window time constant (in micro-secs, or nano-s)
+
+        key: PRNG key to control determinism of any underlying random values
+            associated with this cell
+
+        directory: string indicating directory on disk to save sLIF parameter
+            values to (i.e., initial threshold values and any persistent adaptive
+            threshold values)
+    """
+
+    # Define Functions
+    def __init__(self, name, n_units, dt, tau_w=500., nu=4., key=None,
+                 directory=None, **kwargs):
+        super().__init__(name, **kwargs)
+
+        self.tau_w = tau_w ## kernel window time constant
+        self.nu = nu
+        self.win_len = int(nu/dt) + 1 ## window length
+        #tf ## window of spike times
+
+        ## Layer Size Setup
+        self.batch_size = 1
+        self.n_units = n_units
+
+        restVals = jnp.zeros((self.batch_size, self.n_units))
+        self.inputs = Compartment(restVals) # input comp
+        self.epsp = Compartment(restVals) ## output comp
+        self.tf = Compartment(jnp.zeros((self.win_len, self.batch_size, self.n_units))) ## window comp
+        #self.reset()
+
+    @staticmethod
+    def _advance_state(t, dt, tau_w, win_len, inputs, epsp, tf):
+        s = inputs
+        ## update spike time window and corresponding window volume
+        tf, epsp = apply_kernel(tf, s, t, tau_w, win_len, krn_start=0,
+                                krn_end=win_len-1) #0:win_len-1)
+        return epsp, tf
+
+    @resolver(_advance_state)
+    def advance_state(self, epsp, tf):
+        self.epsp.set(epsp)
+        self.tf.set(tf)
+
+    @staticmethod
+    def _reset(batch_size, n_units, win_len):
+        restVals = jnp.zeros((batch_size, n_units))
+        restTensor = jnp.zeros([win_len, batch_size, n_units], jnp.float32) # tf
+        return restVals, restVals, restTensor # inputs, epsp, tf
+
+    @resolver(_reset)
+    def reset(self, inputs, epsp, tf):
+        self.inputs.set(inputs)
+        self.epsp.set(epsp)
+        self.tf.set(tf)
+
+    def __repr__(self):
+        comps = [varname for varname in dir(self) if Compartment.is_compartment(getattr(self, varname))]
+        maxlen = max(len(c) for c in comps) + 5
+        lines = f"[{self.__class__.__name__}] PATH: {self.name}\n"
+        for c in comps:
+            stats = tensorstats(getattr(self, c).value)
+            if stats is not None:
+                line = [f"{k}: {v}" for k, v in stats.items()]
+                line = ", ".join(line)
+            else:
+                line = "None"
+            lines += f"  {f'({c})'.ljust(maxlen)}{line}\n"
+        return lines
+
+if __name__ == '__main__':
+    from ngcsimlib.context import Context
+    with Context("Bar") as bar:
+        X = ExpKernel("X", 1, 1.)
+    print(X)
```

### Comparing `ngclearn-1.0b4/ngclearn/components/other/varTrace.py` & `ngclearn-1.1b0/ngclearn/components/other/varTrace.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from ngcsimlib.component import Component
 from jax import numpy as jnp, random, jit
 from functools import partial
+from ngclearn import resolver, Component, Compartment
+from ngclearn.utils import tensorstats
 import time, sys
 
 @partial(jit, static_argnums=[4])
 def run_varfilter(dt, x, x_tr, decayFactor, a_delta=0.):
     """
     Run variable trace filter (low-pass filter) dynamics one step forward.
 
@@ -52,93 +53,82 @@
                 1) `'lin'` = linear trace filter, i.e., decay = x_tr + (-x_tr) * (dt/tau_tr);
                 2) `'exp'` = exponential trace filter, i.e., decay = exp(-dt/tau_tr) * x_tr;
                 3) `'step'` = step trace, i.e., decay = 0 (a pulse applied upon input value)
 
         key: PRNG key to control determinism of any underlying random values
             associated with this cell
 
-        useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
-
         directory: string indicating directory on disk to save sLIF parameter
             values to (i.e., initial threshold values and any persistent adaptive
             threshold values)
     """
 
-    ## Class Methods for Compartment Names
-    @classmethod
-    def inputCompartmentName(cls):
-        return 'in'
-
-    @classmethod
-    def outputCompartmentName(cls):
-        return 'out'
-
-    @classmethod
-    def traceName(cls):
-        return 'trace'
-
-    ## Bind Properties to Compartments for ease of use
-    @property
-    def inputCompartment(self):
-      return self.compartments.get(self.inputCompartmentName(), None)
-
-    @inputCompartment.setter
-    def inputCompartment(self, inp):
-      self.compartments[self.inputCompartmentName()] = inp
-
-    @property
-    def trace(self):
-        return self.compartments.get(self.traceName(), None)
-
-    @trace.setter
-    def trace(self, inp):
-        self.compartments[self.traceName()] = inp
-
     # Define Functions
     def __init__(self, name, n_units, tau_tr, a_delta, decay_type="exp", key=None,
-                 useVerboseDict=False, directory=None, **kwargs):
-        super().__init__(name, useVerboseDict, **kwargs)
-
-        ##Random Number Set up
-        self.key = key
-        if self.key is None:
-            self.key = random.PRNGKey(time.time_ns())
-
-        ##TMP
-        self.key, subkey = random.split(self.key)
+                 directory=None, **kwargs):
+        super().__init__(name, **kwargs)
 
         ## trace control coefficients
         self.tau_tr = tau_tr ## trace time constant
         self.a_delta = a_delta ## trace increment (if spike occurred)
         self.decay_type = decay_type ## lin --> linear decay; exp --> exponential decay
-        self.decayFactor = None
 
         ##Layer Size Setup
+        self.batch_size = 1
         self.n_units = n_units
-        self.reset()
-
-    def verify_connections(self):
-        self.metadata.check_incoming_connections(self.inputCompartmentName(),
-                                                 min_connections=1)
-
-    def advance_state(self, t, dt, **kwargs):
-        if self.decayFactor is None: ## compute only once the decay factor
-            self.decayFactor = 0. ## <-- pulse filter decay
-            if "exp" in self.decay_type:
-                self.decayFactor = jnp.exp(-dt/self.tau_tr)
-            elif "lin" in self.decay_type:
-                self.decayFactor = (1. - dt/self.tau_tr)
-            ## else "step", yielding a step/pulse-like filter
-        if self.trace is None:
-            self.trace = jnp.zeros((1, self.n_units))
-        s = self.inputCompartment
-        self.trace = run_varfilter(dt, s, self.trace, self.decayFactor, self.a_delta)
-        self.outputCompartment = self.trace
-        #self.inputCompartment = None
-
-    def reset(self, **kwargs):
-        self.trace = jnp.zeros((1, self.n_units))
-        self.outputCompartment = self.trace
-        self.inputCompartment = None
 
-    def save(self, **kwargs):
-        pass
+        restVals = jnp.zeros((self.batch_size, self.n_units))
+        self.inputs = Compartment(restVals) # input compartment
+        self.outputs = Compartment(restVals) # output compartment
+        self.trace = Compartment(restVals)
+        #self.reset()
+
+    @staticmethod
+    def _advance_state(t, dt, decay_type, tau_tr, a_delta, inputs, trace):
+        ## compute the decay factor
+        decayFactor = 0. ## <-- pulse filter decay (default)
+        if "exp" in decay_type:
+            decayFactor = jnp.exp(-dt/tau_tr)
+        elif "lin" in decay_type:
+            decayFactor = (1. - dt/tau_tr)
+        ## else "step" == decay_type, yielding a step/pulse-like filter
+        trace = run_varfilter(dt, inputs, trace, decayFactor, a_delta)
+        outputs = trace
+        inputs = None
+        return inputs, outputs, trace
+
+    @resolver(_advance_state)
+    def advance_state(self, inputs, outputs, trace):
+        self.inputs.set(inputs)
+        self.outputs.set(outputs)
+        self.trace.set(trace)
+
+    @staticmethod
+    def _reset(batch_size, n_units):
+        restVals = jnp.zeros((batch_size, n_units))
+        return restVals, restVals, restVals
+
+    @resolver(_reset)
+    def reset(self, inputs, outputs, trace):
+        self.inputs.set(inputs)
+        self.outputs.set(outputs)
+        self.trace.set(trace)
+
+    def __repr__(self):
+        comps = [varname for varname in dir(self) if Compartment.is_compartment(getattr(self, varname))]
+        maxlen = max(len(c) for c in comps) + 5
+        lines = f"[{self.__class__.__name__}] PATH: {self.name}\n"
+        for c in comps:
+            stats = tensorstats(getattr(self, c).value)
+            if stats is not None:
+                line = [f"{k}: {v}" for k, v in stats.items()]
+                line = ", ".join(line)
+            else:
+                line = "None"
+            lines += f"  {f'({c})'.ljust(maxlen)}{line}\n"
+        return lines
+
+if __name__ == '__main__':
+    from ngcsimlib.context import Context
+    with Context("Bar") as bar:
+        X = VarTrace("X", 9, 0.0004, 3)
+    print(X)
```

### Comparing `ngclearn-1.0b4/ngclearn/components/synapses/hebbian/expSTDPSynapse.py` & `ngclearn-1.1b0/ngclearn/components/synapses/hebbian/expSTDPSynapse.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from ngcsimlib.component import Component
 from jax import random, numpy as jnp, jit
-from functools import partial
+from ngclearn import resolver, Component, Compartment
+from ngclearn.utils import tensorstats
+from ngclearn.utils.model_utils import initialize_params, normalize_matrix
 import time
 
-@partial(jit, static_argnums=[6,7,8,9,10,11,12])
 def evolve(dt, pre, x_pre, post, x_post, W, w_bound=1., eta=0.00005,
-            x_tar=0.7, exp_beta=1., Aplus=1., Aminus=0., w_norm=None):
+            x_tar=0.7, exp_beta=1., Aplus=1., Aminus=0.):
     """
     Evolves/changes the synpatic value matrix underlying this synaptic cable,
     given relevant statistics.
 
     Args:
         pre: pre-synaptic statistic to drive update
 
@@ -29,53 +29,54 @@
 
         exp_beta: controls effect of exponential Hebbian shift/dependency
 
         Aplus: strength of long-term potentiation (LTP)
 
         Aminus: strength of long-term depression (LTD)
 
-        w_norm: if not None, applies an L2 norm constraint to synapses
-
     Returns:
-        the newly evolved synaptic weight value matrix
+        the newly evolved synaptic weight value matrix, synaptic update matrix
     """
     ## equations 4 from Diehl and Cook - full exponential weight-dependent STDP
     ## calculate post-synaptic term
     post_term1 = jnp.exp(-exp_beta * W) * jnp.matmul(x_pre.T, post)
     x_tar_vec = x_pre * 0 + x_tar # need to broadcast scalar x_tar to mat/vec form
     post_term2 = jnp.exp(-exp_beta * (w_bound - W)) * jnp.matmul(x_tar_vec.T, post)
     dWpost = (post_term1 - post_term2) * Aplus
     ## calculate pre-synaptic term
     dWpre = 0.
     if Aminus > 0.:
         dWpre = -jnp.exp(-exp_beta * W) * jnp.matmul(pre.T, x_post) * Aminus
 
     ## calc final weighted adjustment
-    dW = (dWpost + dWpre) * eta
-    _W = W + dW
-    if w_norm is not None:
-        _W = _W * (w_norm/(jnp.linalg.norm(_W, axis=1, keepdims=True) + 1e-5))
-    _W = jnp.clip(_W, 0.01, w_bound) # not in source paper
-    return _W
+    dW = (dWpost + dWpre)
+    _W = W + dW * eta
+    ## enforce non-negativity
+    eps = 0.01 # 0.001
+    _W = jnp.clip(_W, eps, w_bound - eps)
+    return _W, dW
 
 @jit
-def compute_layer(inp, weight):
+def compute_layer(inp, weight, scale=1.):
     """
     Applies the transformation/projection induced by the synaptic efficacie
     associated with this synaptic cable
 
     Args:
         inp: signal input to run through this synaptic cable
 
         weight: this cable's synaptic value matrix
 
+        scale: scale factor to apply to synapses before transform applied
+            to input values
+
     Returns:
         a projection/transformation of input "inp"
     """
-    return jnp.matmul(inp, weight)
+    return jnp.matmul(inp, weight * scale)
 
 class ExpSTDPSynapse(Component):
     """
     A synaptic cable that adjusts its efficacies via trace-based form of
     spike-timing-dependent plasticity (STDP) based on an exponential weight
     dependence (the strength of which is controlled by a factor).
 
@@ -106,129 +107,127 @@
                  (higher -> lower synaptic values)
 
         wInit: a kernel to drive initialization of this synaptic cable's values;
             typically a tuple with 1st element as a string calling the name of
             initialization to use, e.g., ("uniform", -0.1, 0.1) samples U(-1,1)
             for each dimension/value of this cable's underlying value matrix
 
+        Rscale: a fixed scaling (resistance) factor to apply to synaptic transform
+            (Default: 1.), i.e., yields: out = ((W * Rscale) * in) + b
+
         key: PRNG key to control determinism of any underlying random values
             associated with this synaptic cable
 
-        useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
-
         directory: string indicating directory on disk to save synaptic parameter
             values to (i.e., initial threshold values and any persistent adaptive
             threshold values)
     """
-    ## Class Methods for Compartment Names
-    @classmethod
-    def inputCompartmentName(cls):
-        return 'in'
-
-    @classmethod
-    def outputCompartmentName(cls):
-        return 'out'
-
-    @classmethod
-    def presynapticTraceName(cls):
-        return 'x_pre'
-
-    @classmethod
-    def postsynapticTraceName(cls):
-        return 'x_post'
-
-    ## Bind Properties to Compartments for ease of use
-    @property
-    def inputCompartment(self):
-        return self.compartments.get(self.inputCompartmentName(), None)
-
-    @inputCompartment.setter
-    def inputCompartment(self, x):
-        self.compartments[self.inputCompartmentName()] = x
-
-    @property
-    def outputCompartment(self):
-        return self.compartments.get(self.outputCompartmentName(), None)
-
-    @outputCompartment.setter
-    def outputCompartment(self, x):
-        self.compartments[self.outputCompartmentName()] = x
-
-    @property
-    def presynapticTrace(self):
-        return self.compartments.get(self.presynapticTraceName(), None)
-
-    @presynapticTrace.setter
-    def presynapticTrace(self, x):
-        self.compartments[self.presynapticTraceName()] = x
-
-    @property
-    def postsynapticTrace(self):
-        return self.compartments.get(self.postsynapticTraceName(), None)
-
-    @postsynapticTrace.setter
-    def postsynapticTrace(self, x):
-        self.compartments[self.postsynapticTraceName()] = x
 
     # Define Functions
     def __init__(self, name, shape, eta, exp_beta, Aplus, Aminus,
-                 preTrace_target, wInit=(0.025, 0.8), key=None, useVerboseDict=False,
-                 directory=None, **kwargs):
-        super().__init__(name, useVerboseDict, **kwargs)
-
-        ##Random Number Set up
-        self.key = key
-        if self.key is None:
-            self.key = random.PRNGKey(time.time_ns())
+                 preTrace_target, wInit=("uniform", 0.025, 0.8), Rscale=1.,
+                 key=None, directory=None, **kwargs):
+        super().__init__(name, **kwargs)
 
-        ##parms
+        tmp_key = random.PRNGKey(time.time_ns()) if key is None else key
+
+        ## Exp-STDP meta-parameters
         self.shape = shape ## shape of synaptic efficacy matrix
         self.eta = eta ## global learning rate governing plasticity
         self.exp_beta = exp_beta ## if not None, will trigger exp-depend STPD rule
         self.preTrace_target = preTrace_target ## target (pre-synaptic) trace activity value # 0.7
         self.Aplus = Aplus ## LTP strength
         self.Aminus = Aminus ## LTD strength
-        self.shape = shape  # shape of synaptic matrix W
+        self.Rscale = Rscale ## post-transformation scale factor
         self.w_bound = 1. ## soft weight constraint
-        self.w_norm = None ## normalization constant for synaptic matrix after update
-
-        if directory is None:
-            self.key, subkey = random.split(self.key)
-            lb, ub = wInit
-            self.weights = random.uniform(subkey, shape, minval=lb, maxval=ub)
-        else:
-            self.load(directory)
 
-        ##Reset to initialize core compartments
-        self.reset()
+        tmp_key, subkey = random.split(tmp_key)
+        #self.weights = random.uniform(subkey, shape, minval=lb, maxval=ub)
+        weights = initialize_params(subkey, wInit, shape)
+
+        self.batch_size = 1
+        ## Compartment setup
+        preVals = jnp.zeros((self.batch_size, shape[0]))
+        postVals = jnp.zeros((self.batch_size, shape[1]))
+        self.inputs = Compartment(preVals)
+        self.outputs = Compartment(postVals)
+        self.preSpike = Compartment(preVals)
+        self.postSpike = Compartment(postVals)
+        self.preTrace = Compartment(preVals)
+        self.postTrace = Compartment(postVals)
+        self.weights = Compartment(weights)
+        self.dWeights = Compartment(weights * 0)
 
-    def verify_connections(self):
-        self.metadata.check_incoming_connections(self.inputCompartmentName(), min_connections=1)
-
-    def advance_state(self, dt, t, **kwargs):
+    @staticmethod
+    def _advance_state(t, dt, Rscale, inputs, weights):
         ## run signals across synapses
-        self.outputCompartment = compute_layer(self.inputCompartment, self.weights)
+        outputs = compute_layer(inputs, weights, Rscale)
+        return outputs
 
-    def evolve(self, dt, t, **kwargs):
-        pre = self.inputCompartment
-        post = self.outputCompartment
-        x_pre = self.presynapticTrace
-        x_post = self.postsynapticTrace
-        self.weights = evolve(dt, pre, x_pre, post, x_post, self.weights,
-                              w_bound=self.w_bound, eta=self.eta,
-                              x_tar=self.preTrace_target, exp_beta=self.exp_beta,
-                              Aplus=self.Aplus, Aminus=self.Aminus)
-
-    def reset(self, **kwargs):
-        self.inputCompartment = None
-        self.outputCompartment = None
-        self.presynapticTrace = None
-        self.postsynapticTrace = None
+    @resolver(_advance_state)
+    def advance_state(self, outputs):
+        self.outputs.set(outputs)
+
+    @staticmethod
+    def _evolve(t, dt, w_bound, eta, preTrace_target, exp_beta, Aplus, Aminus,
+                    preSpike, postSpike, preTrace, postTrace, weights):
+        weights, dW = evolve(dt, preSpike, preTrace, postSpike, postTrace, weights,
+                             w_bound=w_bound, eta=eta, x_tar=preTrace_target,
+                             exp_beta=exp_beta, Aplus=Aplus, Aminus=Aminus)
+        return weights, dW
+
+    @resolver(_evolve)
+    def evolve(self, weights, dWeights):
+        self.weights.set(weights)
+        self.dWeights.set(dWeights)
+
+    @staticmethod
+    def _reset(batch_size, shape):
+        preVals = jnp.zeros((batch_size, shape[0]))
+        postVals = jnp.zeros((batch_size, shape[1]))
+        inputs = preVals
+        outputs = postVals
+        preSpike = preVals
+        postSpike = postVals
+        preTrace = preVals
+        postTrace = postVals
+        dWeights = jnp.zeros(shape)
+        return inputs, outputs, preSpike, postSpike, preTrace, postTrace, dWeights
+
+    @resolver(_reset)
+    def reset(self, inputs, outputs, preSpike, postSpike, preTrace, postTrace, dWeights):
+        self.inputs.set(inputs)
+        self.outputs.set(outputs)
+        self.preSpike.set(preSpike)
+        self.postSpike.set(postSpike)
+        self.preTrace.set(preTrace)
+        self.postTrace.set(postTrace)
+        self.dWeights.set(dWeights)
 
     def save(self, directory, **kwargs):
         file_name = directory + "/" + self.name + ".npz"
-        jnp.savez(file_name, weights=self.weights)
+        jnp.savez(file_name, weights=self.weights.value)
 
     def load(self, directory, **kwargs):
         file_name = directory + "/" + self.name + ".npz"
         data = jnp.load(file_name)
-        self.weights = data['weights']
+        self.weights.set( data['weights'] )
+
+    def __repr__(self):
+        comps = [varname for varname in dir(self) if Compartment.is_compartment(getattr(self, varname))]
+        maxlen = max(len(c) for c in comps) + 5
+        lines = f"[{self.__class__.__name__}] PATH: {self.name}\n"
+        for c in comps:
+            stats = tensorstats(getattr(self, c).value)
+            if stats is not None:
+                line = [f"{k}: {v}" for k, v in stats.items()]
+                line = ", ".join(line)
+            else:
+                line = "None"
+            lines += f"  {f'({c})'.ljust(maxlen)}{line}\n"
+        return lines
+
+if __name__ == '__main__':
+    from ngcsimlib.context import Context
+    with Context("Bar") as bar:
+        Wab = ExpSTDPSynapse("Wab", (2, 3), 0.0004, 1, 1, 1, 1)
+    print(Wab)
```

### Comparing `ngclearn-1.0b4/ngclearn/components/synapses/hebbian/hebbianSynapse.py` & `ngclearn-1.1b0/ngclearn/components/synapses/hebbian/hebbianSynapse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from ngcsimlib.component import Component
 from jax import random, numpy as jnp, jit
 from functools import partial
 from ngclearn.utils.model_utils import initialize_params
-from ngclearn.utils.optim import SGD, Adam
+from ngclearn.utils.optim import get_opt_init_fn, get_opt_step_fn
+from ngclearn import resolver, Component, Compartment
+from ngclearn.utils import tensorstats
 import time
 
-@partial(jit, static_argnums=[3,4,5,6,7,8])
+@partial(jit, static_argnums=[3, 4, 5, 6, 7, 8])
 def calc_update(pre, post, W, w_bound, is_nonnegative=True, signVal=1., w_decay=0.,
                 pre_wght=1., post_wght=1.):
     """
     Compute a tensor of adjustments to be applied to a synaptic value matrix.
 
     Args:
         pre: pre-synaptic statistic to drive Hebbian update
@@ -140,176 +141,150 @@
 
         Rscale: a fixed scaling factor to apply to synaptic transform
             (Default: 1.), i.e., yields: out = ((W * Rscale) * in) + b
 
         key: PRNG key to control determinism of any underlying random values
             associated with this synaptic cable
 
-        useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
-
         directory: string indicating directory on disk to save synaptic parameter
             values to (i.e., initial threshold values and any persistent adaptive
             threshold values)
     """
 
-    ## Class Methods for Compartment Names
-    @classmethod
-    def inputCompartmentName(cls):
-        return 'in'
-
-    @classmethod
-    def outputCompartmentName(cls):
-        return 'out'
-
-    @classmethod
-    def triggerName(cls):
-        return 'trigger'
-
-    @classmethod
-    def presynapticCompartmentName(cls):
-        return 'pre'
-
-    @classmethod
-    def postsynapticCompartmentName(cls):
-        return 'post'
-
-    ## Bind Properties to Compartments for ease of use
-    @property
-    def trigger(self):
-        return self.compartments.get(self.triggerName(), None)
-
-    @trigger.setter
-    def trigger(self, x):
-        self.compartments[self.triggerName()] = x
-
-    @property
-    def inputCompartment(self):
-        return self.compartments.get(self.inputCompartmentName(), None)
-
-    @inputCompartment.setter
-    def inputCompartment(self, x):
-        self.compartments[self.inputCompartmentName()] = x
-
-    @property
-    def outputCompartment(self):
-        return self.compartments.get(self.outputCompartmentName(), None)
-
-    @outputCompartment.setter
-    def outputCompartment(self, x):
-        self.compartments[self.outputCompartmentName()] = x
-
-    @property
-    def presynapticCompartment(self):
-        return self.compartments.get(self.presynapticCompartmentName(), None)
-
-    @presynapticCompartment.setter
-    def presynapticCompartment(self, x):
-        self.compartments[self.presynapticCompartmentName()] = x
-
-    @property
-    def postsynapticCompartment(self):
-        return self.compartments.get(self.postsynapticCompartmentName(), None)
-
-    @postsynapticCompartment.setter
-    def postsynapticCompartment(self, x):
-        self.compartments[self.postsynapticCompartmentName()] = x
-
     # Define Functions
     def __init__(self, name, shape, eta=0., wInit=("uniform", 0., 0.3),
                  bInit=None, w_bound=1., is_nonnegative=False, w_decay=0.,
                  signVal=1., optim_type="sgd", pre_wght=1., post_wght=1.,
-                 Rscale=1., key=None, useVerboseDict=False, directory=None, **kwargs):
-        super().__init__(name, useVerboseDict, **kwargs)
-
-        ## random Number Set up
-        self.key = key
-        if self.key is None:
-            self.key = random.PRNGKey(time.time_ns())
+                 Rscale=1., key=None, directory=None, **kwargs):
+        super().__init__(name, **kwargs)
 
         ## synaptic plasticity properties and characteristics
         self.shape = shape
         self.Rscale = Rscale
         self.w_bounds = w_bound
         self.w_decay = w_decay ## synaptic decay
         self.pre_wght = pre_wght
         self.post_wght = post_wght
         self.eta = eta
         self.wInit = wInit
         self.bInit = bInit
         self.is_nonnegative = is_nonnegative
         self.signVal = signVal
 
+        self.batch_size = 1
         ## optimization / adjustment properties (given learning dynamics above)
-        self.opt = None
-        if optim_type == "adam":
-            self.opt = Adam(learning_rate=self.eta)
-        else: ## default is SGD
-            self.opt = SGD(learning_rate=self.eta)
-
-        if directory is None:
-            self.key, subkey = random.split(self.key)
-            self.weights = initialize_params(subkey, wInit, shape)
-            if self.bInit is not None:
-                self.key, subkey = random.split(self.key)
-                self.biases = initialize_params(subkey, bInit, (1, shape[1]))
-        else:
-            self.load(directory)
+        self.opt = get_opt_step_fn(optim_type, eta=self.eta)
+
+        key = random.PRNGKey(time.time_ns()) if key is None else key
 
-        ##Reset to initialize stuff
-        self.reset()
+        # compartments (state of the cell, parameters, will be updated through stateless calls)
+        self.preVals = jnp.zeros((self.batch_size, shape[0]))
+        self.postVals = jnp.zeros((self.batch_size, shape[1]))
+        self.inputs = Compartment(self.preVals)
+        self.outputs = Compartment(self.postVals)
+        self.pre = Compartment(self.preVals)
+        self.post = Compartment(self.postVals)
+        self.dW = Compartment(jnp.zeros(shape))
+        self.db = Compartment(jnp.zeros(shape[1]))
+
+        key, subkey = random.split(key)
+        self.weights = Compartment(initialize_params(subkey, wInit, shape))
+        key, subkey = random.split(key)
+        self.biases = Compartment(initialize_params(subkey, bInit, (1, shape[1])) if bInit else 0.0)
+        self.opt_params = Compartment(get_opt_init_fn(optim_type)([self.weights.value, self.biases.value] if bInit else [self.weights.value]))
 
-        self.dW = None
-        self.db = None
+        # loading weights
+        if directory is not None:
+            self.load(directory)
 
-    def verify_connections(self):
-        self.metadata.check_incoming_connections(self.inputCompartmentName(), min_connections=1)
+        self.batch_size = 1
+
+    @staticmethod
+    def _advance_state(t, dt, Rscale, inputs, weights, biases):
+        outputs = compute_layer(inputs, weights, biases, Rscale)
+        return outputs
+
+    @resolver(_advance_state)
+    def advance_state(self, outputs):
+        self.outputs.set(outputs)
+
+    @staticmethod
+    def _evolve(t, dt, opt, w_bounds, is_nonnegative, signVal, w_decay, pre_wght,
+                post_wght, bInit, pre, post, weights, biases, dW, db, opt_params):
+        dW, db = calc_update(pre, post,
+                             weights, w_bounds, is_nonnegative=is_nonnegative,
+                             signVal=signVal, w_decay=w_decay,
+                             pre_wght=pre_wght, post_wght=post_wght)
 
-    def advance_state(self, **kwargs):
-        biases = 0.
-        if self.bInit != None:
-            biases = self.biases
-        self.outputCompartment = compute_layer(self.inputCompartment, self.weights,
-                                               biases, self.Rscale)
-
-    def evolve(self, t, dt, **kwargs):
-        dW, db = calc_update(self.presynapticCompartment, self.postsynapticCompartment,
-                             self.weights, self.w_bounds, is_nonnegative=self.is_nonnegative,
-                             signVal=self.signVal, w_decay=self.w_decay,
-                             pre_wght=self.pre_wght, post_wght=self.post_wght)
-        self.dW = dW
-        self.db = db
         ## conduct a step of optimization - get newly evolved synaptic weight value matrix
-        if self.bInit != None:
-            theta = [self.weights, self.biases]
-            self.opt.update(theta, [dW, db])
-            self.weights = theta[0]
-            self.biases = theta[1]
+        if bInit != None:
+            opt_params, [weights, biases] = opt(opt_params, [weights, biases], [dW, db])
         else:
             # ignore db since no biases configured
-            theta = [self.weights]
-            self.opt.update(theta, [dW])
-            self.weights = theta[0]
+            opt_params, [weights] = opt(opt_params, [weights], [dW])
         ## ensure synaptic efficacies adhere to constraints
-        self.weights = enforce_constraints(self.weights, self.w_bounds,
-                                           is_nonnegative=self.is_nonnegative)
-
-    def reset(self, **kwargs):
-        self.inputCompartment = None
-        self.outputCompartment = None
-        self.presynapticCompartment = None
-        self.postsynapticCompartment = None
-        self.dW = None
-        self.db = None
+        weights = enforce_constraints(weights, w_bounds,
+                                           is_nonnegative=is_nonnegative)
+        return opt_params, weights, biases
+
+    @resolver(_evolve)
+    def evolve(self, opt_params, weights, biases):
+        self.opt_params.set(opt_params)
+        self.weights.set(weights)
+        self.biases.set(biases)
+
+    @staticmethod
+    def _reset(batch_size, shape, wInit, bInit):
+        preVals = jnp.zeros((batch_size, shape[0]))
+        postVals = jnp.zeros((batch_size, shape[1]))
+        return (
+            preVals, # inputs
+            postVals, # outputs
+            preVals, # pre
+            postVals, # post
+            jnp.zeros(shape), # dW
+            jnp.zeros(shape[1]), # db
+        )
+
+    @resolver(_reset)
+    def reset(self, inputs, outputs, pre, post, dW, db):
+        self.inputs.set(inputs)
+        self.outputs.set(outputs)
+        self.pre.set(pre)
+        self.post.set(post)
+        self.dW.set(dW)
+        self.db.set(db)
 
     def save(self, directory, **kwargs):
         file_name = directory + "/" + self.name + ".npz"
         if self.bInit != None:
-            jnp.savez(file_name, weights=self.weights, biases=self.biases)
+            jnp.savez(file_name, weights=self.weights.value, biases=self.biases.value)
         else:
-            jnp.savez(file_name, weights=self.weights)
+            jnp.savez(file_name, weights=self.weights.value)
 
     def load(self, directory, **kwargs):
         file_name = directory + "/" + self.name + ".npz"
         data = jnp.load(file_name)
-        self.weights = data['weights']
+        self.weights.set(data['weights'])
         if "biases" in data.keys():
-            self.biases = data['biases']
+            self.biases.set(data['biases'])
+
+    def __repr__(self):
+        comps = [varname for varname in dir(self) if Compartment.is_compartment(getattr(self, varname))]
+        maxlen = max(len(c) for c in comps) + 5
+        lines = f"[{self.__class__.__name__}] PATH: {self.name}\n"
+        for c in comps:
+            stats = tensorstats(getattr(self, c).value)
+            if stats is not None:
+                line = [f"{k}: {v}" for k, v in stats.items()]
+                line = ", ".join(line)
+            else:
+                line = "None"
+            lines += f"  {f'({c})'.ljust(maxlen)}{line}\n"
+        return lines
+
+if __name__ == '__main__':
+    from ngcsimlib.context import Context
+    with Context("Bar") as bar:
+        Wab = HebbianSynapse("Wab", (2, 3), 0.0004, optim_type='adam',
+            signVal=-1.0, bInit=("constant", 0., 0.))
+    print(Wab)
```

### Comparing `ngclearn-1.0b4/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py` & `ngclearn-1.1b0/ngclearn/components/synapses/hebbian/traceSTDPSynapse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-from ngcsimlib.component import Component
 from jax import random, numpy as jnp, jit
-from functools import partial
-from ngclearn.utils.model_utils import initialize_params, normalize_matrix
+from ngclearn import resolver, Component, Compartment
+from ngclearn.utils import tensorstats
+from ngclearn.utils.model_utils import initialize_params
 import time
 
-@partial(jit, static_argnums=[6,7,8,9,10,11,12])
-def evolve(dt, pre, x_pre, post, x_post, W, w_bound=1., eta=1.,
-            x_tar=0.0, mu=0., Aplus=1., Aminus=0., w_norm=None):
+def evolve(dt, pre, x_pre, post, x_post, W, w_bound=1., eta=1., x_tar=0.0,
+           mu=0., Aplus=1., Aminus=0.):
     """
     Evolves/changes the synpatic value matrix underlying this synaptic cable,
     given relevant statistics.
 
     Args:
         pre: pre-synaptic statistic to drive update
 
@@ -30,57 +29,60 @@
 
         mu: controls the power scale of the Hebbian shift
 
         Aplus: strength of long-term potentiation (LTP)
 
         Aminus: strength of long-term depression (LTD)
 
-        w_norm: (Unused)
-
     Returns:
-        the newly evolved synaptic weight value matrix
+        the newly evolved synaptic weight value matrix, synaptic update matrix
     """
     if mu > 0.:
         ## equations 3, 5, & 6 from Diehl and Cook - full power-law STDP
         post_shift = jnp.power(w_bound - W, mu)
         pre_shift = jnp.power(W, mu)
         dWpost = (post_shift * jnp.matmul((x_pre - x_tar).T, post)) * Aplus
+        dWpre = 0.
         if Aminus > 0.:
             dWpre = -(pre_shift * jnp.matmul(pre.T, x_post)) * Aminus
     else:
         ## calculate post-synaptic term
         dWpost = jnp.matmul((x_pre - x_tar).T, post * Aplus)
         dWpre = 0.
         if Aminus > 0.:
             ## calculate pre-synaptic term
             dWpre = -jnp.matmul(pre.T, x_post * Aminus)
     ## calc final weighted adjustment
-    dW = (dWpost + dWpre) * eta
-    _W = W + dW
-    # if w_norm is not None:
-    #     _W = normalize_matrix(_W, w_norm, order=1, axis=1) ## L1 norm constraint
-    #    #_W = _W * (w_norm/(jnp.linalg.norm(_W, axis=1, keepdims=True) + 1e-5))
-    _W = jnp.clip(_W, 0.001, w_bound) # 0.01, w_bound)
-    return _W
+    dW = (dWpost + dWpre)
+    ## do a gradient ascent update/shift
+    _W = W + dW * eta
+    ## enforce non-negativity
+    eps = 0.01 # 0.001
+    _W = jnp.clip(_W, eps, w_bound - eps) #jnp.abs(w_bound)) # 0.01, w_bound)
+    #print(_W)
+    return _W, dW
 
 @jit
-def compute_layer(inp, weight):
+def compute_layer(inp, weight, scale=1.):
     """
     Applies the transformation/projection induced by the synaptic efficacie
     associated with this synaptic cable
 
     Args:
         inp: signal input to run through this synaptic cable
 
         weight: this cable's synaptic value matrix
 
+        scale: scale factor to apply to synapses before transform applied
+            to input values
+
     Returns:
         a projection/transformation of input "inp"
     """
-    return jnp.matmul(inp, weight)
+    return jnp.matmul(inp, weight * scale)
 
 class TraceSTDPSynapse(Component): # power-law / trace-based STDP
     """
     A synaptic cable that adjusts its efficacies via trace-based form of
     spike-timing-dependent plasticity (STDP), including an optional power-scale
     dependence that can be equipped to the Hebbian adjustment (the strength of
     which is controlled by a scalar factor).
@@ -111,154 +113,130 @@
                  (higher -> lower synaptic values)
 
         wInit: a kernel to drive initialization of this synaptic cable's values;
             typically a tuple with 1st element as a string calling the name of
             initialization to use, e.g., ("uniform", -0.1, 0.1) samples U(-1,1)
             for each dimension/value of this cable's underlying value matrix
 
-        w_norm: if not None, applies an L1 norm constraint to synapses
-
-        norm_T: clocked time at which to apply L1 synaptic norm constraint
+        Rscale: a fixed scaling factor to apply to synaptic transform
+            (Default: 1.), i.e., yields: out = ((W * Rscale) * in)
 
         key: PRNG key to control determinism of any underlying random values
             associated with this synaptic cable
 
-        useVerboseDict: triggers slower, verbose dictionary mode (Default: False)
-
         directory: string indicating directory on disk to save synaptic parameter
             values to (i.e., initial threshold values and any persistent adaptive
             threshold values)
     """
 
-    ## Class Methods for Compartment Names
-    @classmethod
-    def inputCompartmentName(cls):
-        return 'in'
-
-    @classmethod
-    def outputCompartmentName(cls):
-        return 'out'
-
-    @classmethod
-    def presynapticTraceName(cls):
-        return 'x_pre'
-
-    @classmethod
-    def postsynapticTraceName(cls):
-        return 'x_post'
-
-    @classmethod
-    def triggerName(cls):
-        return 'trigger'
-
-    ## Bind Properties to Compartments for ease of use
-    @property
-    def inputCompartment(self):
-        return self.compartments.get(self.inputCompartmentName(), None)
-
-    @inputCompartment.setter
-    def inputCompartment(self, x):
-        self.compartments[self.inputCompartmentName()] = x
-
-    @property
-    def outputCompartment(self):
-        return self.compartments.get(self.outputCompartmentName(), None)
-
-    @outputCompartment.setter
-    def outputCompartment(self, x):
-        self.compartments[self.outputCompartmentName()] = x
-
-    @property
-    def trigger(self):
-        return self.compartments.get(self.triggerName(), None)
-
-    @trigger.setter
-    def trigger(self, x):
-        # FIXME: place a check in here? (should check for single float value)
-        self.compartments[self.triggerName()] = x
-
-    @property
-    def presynapticTrace(self):
-        return self.compartments.get(self.presynapticTraceName(), None)
-
-    @presynapticTrace.setter
-    def presynapticTrace(self, x):
-        self.compartments[self.presynapticTraceName()] = x
-
-    @property
-    def postsynapticTrace(self):
-        return self.compartments.get(self.postsynapticTraceName(), None)
-
-    @postsynapticTrace.setter
-    def postsynapticTrace(self, x):
-        self.compartments[self.postsynapticTraceName()] = x
-
     # Define Functions
     def __init__(self, name, shape, eta, Aplus, Aminus, mu=0.,
-                 preTrace_target=0., wInit=("uniform", 0.025, 0.8), w_norm=None,
-                 norm_T=250., key=None, useVerboseDict=False, directory=None, **kwargs):
-        super().__init__(name, useVerboseDict, **kwargs)
-
-        ##Random Number Set up
-        self.key = key
-        if self.key is None:
-            self.key = random.PRNGKey(time.time_ns())
+                 preTrace_target=0., wInit=("uniform", 0.025, 0.8), Rscale=1.,
+                 key=None, directory=None, **kwargs):
+        super().__init__(name, **kwargs)
+
+        ## constructor-only rng setup
+        tmp_key = random.PRNGKey(time.time_ns()) if key is None else key
 
         ##parms
         self.shape = shape ## shape of synaptic efficacy matrix
         self.eta = eta ## global learning rate governing plasticity
         self.mu = mu ## controls power-scaling of STDP rule
         self.preTrace_target = preTrace_target ## target (pre-synaptic) trace activity value # 0.7
         self.Aplus = Aplus ## LTP strength
         self.Aminus = Aminus ## LTD strength
-        self.shape = shape  # shape of synaptic matrix W
+        self.Rscale = Rscale ## post-transformation scale factor
         self.w_bound = 1. ## soft weight constraint
-        self.w_norm = w_norm ## normalization constant for synaptic matrix after update
-        self.norm_T = norm_T ## scheduling time / checkpoint for synaptic normalization
-
-        if directory is None:
-            self.key, subkey = random.split(self.key)
-            #self.weights = random.uniform(subkey, shape, minval=lb, maxval=ub)
-            self.weights = initialize_params(subkey, wInit, shape)
-        else:
-            self.load(directory)
 
-        ##Reset to initialize core compartments
-        self.reset()
+        tmp_key, subkey = random.split(tmp_key)
+        #self.weights = random.uniform(subkey, shape, minval=lb, maxval=ub)
+        weights = initialize_params(subkey, wInit, shape)
+
+        self.batch_size = 1
+        ## Compartment setup
+        preVals = jnp.zeros((self.batch_size, shape[0]))
+        postVals = jnp.zeros((self.batch_size, shape[1]))
+        self.inputs = Compartment(preVals)
+        self.outputs = Compartment(postVals)
+        self.preSpike = Compartment(preVals)
+        self.postSpike = Compartment(postVals)
+        self.preTrace = Compartment(preVals)
+        self.postTrace = Compartment(postVals)
+        self.weights = Compartment(weights)
+        self.dWeights = Compartment(weights * 0)
+        #self.reset()
 
-    def verify_connections(self):
-        self.metadata.check_incoming_connections(self.inputCompartmentName(), min_connections=1)
-
-    def advance_state(self, dt, t, **kwargs):
+    @staticmethod
+    def _advance_state(t, dt, Rscale, inputs, weights):
         ## run signals across synapses
-        self.outputCompartment = compute_layer(self.inputCompartment, self.weights)
+        outputs = compute_layer(inputs, weights, Rscale)
+        return outputs
 
-    def evolve(self, dt, t, **kwargs):
-        #trigger = self.trigger
-        pre = self.inputCompartment
-        post = self.outputCompartment
-        x_pre = self.presynapticTrace
-        x_post = self.postsynapticTrace
-        self.weights = evolve(dt, pre, x_pre, post, x_post, self.weights,
-                              w_bound=self.w_bound, eta=self.eta,
-                              x_tar=self.preTrace_target, mu=self.mu,
-                              Aplus=self.Aplus, Aminus=self.Aminus,
-                              w_norm=self.w_norm)
-        if self.norm_T > 0:
-            if t % (self.norm_T-1) == 0: #t % self.norm_t == 0:
-                self.weights = normalize_matrix(self.weights, self.w_norm, order=1, axis=0)
-
-    def reset(self, **kwargs):
-        self.inputCompartment = None
-        self.outputCompartment = None
-        self.presynapticTrace = None
-        self.postsynapticTrace = None
-        self.trigger = 1. ## default: assume synaptic change will occur
+    @resolver(_advance_state)
+    def advance_state(self, outputs):
+        self.outputs.set(outputs)
+
+    @staticmethod
+    def _evolve(t, dt, w_bound, eta, preTrace_target, mu, Aplus, Aminus,
+                preSpike, postSpike, preTrace, postTrace, weights):
+        weights, dW = evolve(dt, preSpike, preTrace, postSpike, postTrace, weights,
+                             w_bound=w_bound, eta=eta, x_tar=preTrace_target, mu=mu,
+                             Aplus=Aplus, Aminus=Aminus)
+        return weights, dW
+
+    @resolver(_evolve)
+    def evolve(self, weights, dWeights):
+        self.weights.set(weights)
+        self.dWeights.set(dWeights)
+
+    @staticmethod
+    def _reset(batch_size, shape):
+        preVals = jnp.zeros((batch_size, shape[0]))
+        postVals = jnp.zeros((batch_size, shape[1]))
+        inputs = preVals
+        outputs = postVals
+        preSpike = preVals
+        postSpike = postVals
+        preTrace = preVals
+        postTrace = postVals
+        dWeights = jnp.zeros(shape)
+        return inputs, outputs, preSpike, postSpike, preTrace, postTrace, dWeights
+
+    @resolver(_reset)
+    def reset(self, inputs, outputs, preSpike, postSpike, preTrace, postTrace, dWeights):
+        self.inputs.set(inputs)
+        self.outputs.set(outputs)
+        self.preSpike.set(preSpike)
+        self.postSpike.set(postSpike)
+        self.preTrace.set(preTrace)
+        self.postTrace.set(postTrace)
+        self.dWeights.set(dWeights)
 
     def save(self, directory, **kwargs):
         file_name = directory + "/" + self.name + ".npz"
-        jnp.savez(file_name, weights=self.weights)
+        jnp.savez(file_name,
+                  weights=self.weights.value)
 
     def load(self, directory, **kwargs):
         file_name = directory + "/" + self.name + ".npz"
         data = jnp.load(file_name)
-        self.weights = data['weights']
+        self.weights.set( data['weights'] )
+
+    def __repr__(self):
+        comps = [varname for varname in dir(self) if Compartment.is_compartment(getattr(self, varname))]
+        maxlen = max(len(c) for c in comps) + 5
+        lines = f"[{self.__class__.__name__}] PATH: {self.name}\n"
+        for c in comps:
+            stats = tensorstats(getattr(self, c).value)
+            if stats is not None:
+                line = [f"{k}: {v}" for k, v in stats.items()]
+                line = ", ".join(line)
+            else:
+                line = "None"
+            lines += f"  {f'({c})'.ljust(maxlen)}{line}\n"
+        return lines
+
+if __name__ == '__main__':
+    from ngcsimlib.context import Context
+    with Context("Bar") as bar:
+        Wab = TraceSTDPSynapse("Wab", (2, 3), 0.0004, 1, 1)
+    print(Wab)
```

### Comparing `ngclearn-1.0b4/ngclearn/utils/data_loader.py` & `ngclearn-1.1b0/ngclearn/utils/data_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Data functions and utilies for data loading.
 """
 from jax import random, numpy as jnp, jit, nn
-import io, sys #, math
+import io, sys, time
 
 class DataLoader(object):
     """
         A data loader object, meant to allow sampling w/o replacement of one or
         more named design matrices. Note that this object is iterable (and
         implements an __iter__() method).
```

### Comparing `ngclearn-1.0b4/ngclearn/utils/density/gmm.py` & `ngclearn-1.1b0/ngclearn/utils/density/gmm.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b4/ngclearn/utils/diffeq/_ode_utils.py` & `ngclearn-1.1b0/ngclearn/utils/diffeq/ode_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,157 +1,189 @@
 """
 Routines and co-routines for ngc-learn's differential equation integration backend.
+
+Currently supported back-end forms of integration in ngc-learn include:
+1) Euler integration (RK-1);
+2) Midpoint method (RK-2);
+3) Heun's method (error-corrector RK-2); 
+4) Ralston's method (error-corrector RK-2)
 """
 from jax import numpy as jnp, random, jit #, nn
 from functools import partial
 import time, sys
 
 def get_integrator_code(integrationType):
     """
     Convenience function for mapping integrator type string to ngc-learn's
     internal integer code value.
 
     Args:
         integrationType: string indicating integrator type
             (supported type: rk1` or `euler`, `rk2` or `midpoint`,
-            `rk2_heun` or `heun`)
+            `rk2_heun` or `heun`, `rk2_ralston` or `ralston`)
 
     Returns:
         integator type integer code
     """
     intgFlag = 0 ## Default is Euler (RK1)
     if integrationType == "midpoint" or integrationType == "rk2": ## midpoint method
         intgFlag = 1
     elif integrationType == "rk2_heun" or integrationType == "heun": ## Heun's method
         intgFlag = 2
+    elif integrationType == "rk2_ralston" or integrationType == "ralston": ## Ralston's method
+        intgFlag = 3
     # elif integrationType == "rk4": ## Runge-Kutte 4rd order code
-    #     intgFlag = 3
+    #     intgFlag = 4
     else:
         if integrationType != "euler" or integrationType == "rk1":
             print("ERROR: unrecognized integration method {} provided! Defaulting \
                   to RK-1/Euler routine".format(integrationType))
     return intgFlag
 
-def step_euler(x, params, dfx, dt, dt_div=1., t=None, x_scale=1.): ## RK-1 routine
+@jit
+def _sum_combine(y1, y2, weight1=1., weight2=1.): ## fast co-routine for simple addition
+    return (y1 * weight1 + y2 * weight2)
+
+@jit
+def _step_forward(t, x, dx_dt, dt, x_scale): ## internal step co-routine
+    _t = t + dt
+    _x = x * x_scale + dx_dt * dt
+    return _t, _x
+
+def step_euler(t, x, dfx, dt, params, x_scale=1.):
     """
     Iteratively integrates one step forward via the Euler method, i.e., a
     first-order Runge-Kutta (RK-1) step.
 
     Args:
-        x: current variable values to advance/iteratively integrate (at time `t`)
+        t: current time variable to advance by dt
 
-        params: tuple containing configuration values/hyper-parameters for the
-            (ordinary) differential equation an ngc-learn component will provide
+        x: current variable values to advance/iteratively integrate (at time `t`)
 
         dfx: (ordinary) differential equation co-routine (as implemented in an
             ngc-learn component)
 
         dt: integration time step (also referred to as `h` in mathematics)
 
-        dt_div: factor to divide `dt` by (Default: 1)
-
-        t: (optional) time step (for equations that use t in dt)
+        params: tuple containing configuration values/hyper-parameters for the
+            (ordinary) differential equation an ngc-learn component will provide
 
         x_scale: dampening factor to scale `x` by (Default: 1)
 
     Returns:
         variable values iteratively integrated/advanced to next step (`t + dt`)
     """
-    _t = t
-    if _t == None:
-        _t = 0.
-    dx_dt = dfx(x, params, _t) ## assumed will be a jit-i-fied function
-    print("{} dy: {}  y_ {} dt {}".format(_t, dx_dt, x, dt))
-    print("Out: ",(x + dx_dt * dt))
-    return _step_forward(x, dx_dt, dt, dt_div, x_scale) ## jit-i-fied function
-
-def step_rk2(x, params, dfx, dt, t=None): ## RK-2 routine
-    """
-    Iteratively integrates one step forward via the (explicit) midpoint method, i.e., a
-    second-order Runge-Kutta (RK-2) step. (Note: ngc-learn internally recognizes
-    "rk2" or "midpoint" for this routine)
+    dx_dt = dfx(t, x, params)
+    _t, _x = _step_forward(t, x, dx_dt, dt, x_scale)
+    return _t, _x
+
+def step_heun(t, x, dfx, dt, params, x_scale=1.):
+    """
+    Iteratively integrates one step forward via Heun's method, i.e., a
+    second-order Runge-Kutta (RK-2) error-corrected step. This method utilizes
+    two (differential) function evaluations to estimate the solution at a given
+    point in time.
+    (Note: ngc-learn internally recognizes "rk2_heun" or "heun" for this routine)
+
+    | Reference:
+    | Ascher, Uri M., and Linda R. Petzold. Computer methods for ordinary
+    | differential equations and differential-algebraic equations. Society for
+    | Industrial and Applied Mathematics, 1998.
 
     Args:
-        x: current variable values to advance/iteratively integrate (at time `t`)
+        t: current time variable to advance by dt
 
-        params: tuple containing configuration values/hyper-parameters for the
-            (ordinary) differential equation an ngc-learn component will provide
+        x: current variable values to advance/iteratively integrate (at time `t`)
 
         dfx: (ordinary) differential equation co-routine (as implemented in an
             ngc-learn component)
 
         dt: integration time step (also referred to as `h` in mathematics)
 
-        t: (optional) time step (for equations that use t in dt)
+        params: tuple containing configuration values/hyper-parameters for the
+            (ordinary) differential equation an ngc-learn component will provide
+
+        x_scale: dampening factor to scale `x` by (Default: 1)
 
     Returns:
         variable values iteratively integrated/advanced to next step (`t + dt`)
     """
-    _t = t
-    if _t == None:
-        _t = 0.
-    #print("-- midpoint --")
-    #_x1 = step_euler(x, params, dfx, dt, dt_div=2.) # k1 is inside here
-    _dx_dt = dfx(x, params, _t/2.) ## assumed will be a jit-i-fied function
-    _x1 =  _step_forward(x, _dx_dt, dt, dt_div=2.)
-    dx_dt = dfx(_x1, params, (_t + dt)/2.) ## k2
-    _x2 = _step_forward(x, dx_dt, dt) ## get 2nd order estimate
-    return _x2
-
-def step_rk2_heun(x, params, dfx, dt, t=None): ## Heun's method routine
-    """
-    Iteratively integrates one step forward via Heun's method, i.e., a
-    second-order Runge-Kutta (RK-2) error-corrected step (or the explicit trapezoid method).
-    (Note: ngc-learn internally recognizes "rk2_heun" or "heun" for this routine)
+    dx_dt = dfx(t, x, params)
+    _t, _x = _step_forward(t, x, dx_dt, dt, x_scale)
+    _dx_dt = dfx(_t, _x, params)
+    summed_dx_dt = _sum_combine(dx_dt, _dx_dt)
+    _, _x = _step_forward(t, x, summed_dx_dt, dt * 0.5, x_scale)
+    return _t, _x
+
+def step_rk2(t, x, dfx, dt, params, x_scale=1.):
+    """
+    Iteratively integrates one step forward via the midpoint method, i.e., a
+    second-order Runge-Kutta (RK-2) step.
+    (Note: ngc-learn internally recognizes "rk2" or "midpoint" for this routine)
 
     | Reference:
     | Ascher, Uri M., and Linda R. Petzold. Computer methods for ordinary
     | differential equations and differential-algebraic equations. Society for
     | Industrial and Applied Mathematics, 1998.
 
     Args:
-        x: current variable values to advance/iteratively integrate (at time `t`)
+        t: current time variable to advance by dt
 
-        params: tuple containing configuration values/hyper-parameters for the
-            (ordinary) differential equation an ngc-learn component will provide
+        x: current variable values to advance/iteratively integrate (at time `t`)
 
         dfx: (ordinary) differential equation co-routine (as implemented in an
             ngc-learn component)
 
         dt: integration time step (also referred to as `h` in mathematics)
 
-        t: (optional) time step (for equations that use t in dt)
+        params: tuple containing configuration values/hyper-parameters for the
+            (ordinary) differential equation an ngc-learn component will provide
+
+        x_scale: dampening factor to scale `x` by (Default: 1)
 
     Returns:
         variable values iteratively integrated/advanced to next step (`t + dt`)
     """
-    _t = t
-    if _t == None:
-        _t = 0.
-    #print("-- trapezoid --")
-    ## apply Heun's formulas to update y
-    k1 = dx_dt = dfx(x, params, _t) # k1
-    #print("k1: ",k1)
-    _x = _step_forward(x, k1, dt, dt_div=1.)
-    k2 = dfx(_x, params, _t + dt)
-    #print("k2: ",k2)
-    k_sum = _add(k1, k2)
-    #print(k_sum/2.)
-    _x2 = _step_forward(x, k_sum, dt, dt_div=2.) ## get 2nd order estimate
-    # ## compute
-    # dx1_dt = dfx(_x1, params) ## obtain differential at intermediate step
-    # dx = _avg(dx_dt, dx1_dt) ## get corrected flow (sum of over/under estimates)
-    # _x2 = _step_forward(x, dx, dt, dt_div=1.) ## get 2nd order estimate
-    return _x2
+    dx_dt = dfx(t, x, params)
+    tm, xm = _step_forward(t, x, dx_dt, dt * 0.5, x_scale)
+    _dx_dt = dfx(tm, xm, params)
+    _t, _x = _step_forward(t, x, _dx_dt, dt, x_scale)
+    return _t, _x
+
+def step_ralston(t, x, dfx, dt, params, x_scale=1.):
+    """
+    Iteratively integrates one step forward via Ralston's method, i.e., a
+    second-order Runge-Kutta (RK-2) error-corrected step. This method utilizes
+    two (differential) function evaluations to estimate the solution at a given
+    point in time.
+    (Note: ngc-learn internally recognizes "rk2_ralston" or "ralston" for this
+    routine)
 
-@jit
-def _avg(y1, y2): ## fast co-routine for simple midpoint/average
-    return (y1 + y2)/2.
+    | Reference:
+    | Ralston, Anthony. "Runge-Kutta methods with minimum error bounds."
+    | Mathematics of computation 16.80 (1962): 431-437.
 
-@jit
-def _add(y1, y2): ## fast co-routine for simple addition
-    return (y1 + y2)
+    Args:
+        t: current time variable to advance by dt
 
-@jit #@partial(jit, static_argnums=[3, 4])
-def _step_forward(x, dx_dt, dt, dt_div=1., x_scale=1.): ## internal integration co-routine
-    _x = x * x_scale + dx_dt * (dt/dt_div)
-    return _x
+        x: current variable values to advance/iteratively integrate (at time `t`)
+
+        dfx: (ordinary) differential equation co-routine (as implemented in an
+            ngc-learn component)
+
+        dt: integration time step (also referred to as `h` in mathematics)
+
+        params: tuple containing configuration values/hyper-parameters for the
+            (ordinary) differential equation an ngc-learn component will provide
+
+        x_scale: dampening factor to scale `x` by (Default: 1)
+
+    Returns:
+        variable values iteratively integrated/advanced to next step (`t + dt`)
+    """
+    dx_dt = dfx(t, x, params) ## k1
+    tm, xm = _step_forward(t, x, dx_dt, dt * 0.75, x_scale)
+    _dx_dt = dfx(tm, xm, params)  ## k2
+    ## Note: new step is a weighted combination of k1 and k2
+    summed_dx_dt = _sum_combine(dx_dt, _dx_dt, weight1=(1./3.), weight2=(2./3.))
+    _t, _x = _step_forward(t, x, summed_dx_dt, dt, x_scale)
+    return _t, _x
```

### Comparing `ngclearn-1.0b4/ngclearn/utils/io_utils.py` & `ngclearn-1.1b0/ngclearn/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b4/ngclearn/utils/metric_utils.py` & `ngclearn-1.1b0/ngclearn/utils/metric_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,59 @@
 import jax
 from jax import numpy as jnp, grad, jit, vmap, random, lax, nn
 import os, sys
 from functools import partial
 
+@partial(jit, static_argnums=[1])
+def measure_fanoFactor(spikes, preserve_batch=False):
+    """
+    Calculates the Fano factor, i.e., a secondary statistics that probes the
+    variability of a spike train within a particular time interval.
+
+    Args:
+        spikes: full spike train matrix; shape is (T x D) where D is number of
+            neurons in a group/cluster
+
+        preserve_batch: if True, will return one score per sample in batch
+            (Default: False), otherwise, returns scalar average score
+
+    Returns:
+        a 1 x D Fano factor vector (one factor per neuron) OR a single
+        average Fano factor across the neuronal group
+    """
+    mu = jnp.mean(spikes, axis=0, keepdims=True)
+    sigSqr = jnp.square(jnp.std(spikes, axis=0, keepdims=True))
+    fano = sigSqr/mu
+    if preserve_batch == False:
+        fano = jnp.mean(fano)
+    return fano
+
+@partial(jit, static_argnums=[1])
+def measure_firingRate(spikes, preserve_batch=False):
+    """
+    Calculates the firing rate(s) of a group of neurons given full spike train.(s)
+
+    Args:
+        spikes: full spike train matrix; shape is (T x D) where D is number of
+            neurons in a group/cluster
+
+        preserve_batch: if True, will return one score per sample in batch
+            (Default: False), otherwise, returns scalar average score
+
+    Returns:
+        a 1 x D firing rate vector (one firing rate per neuron) OR a single
+        average firing rate across the neuronal group
+    """
+    counts = jnp.sum(spikes, axis=0, keepdims=True)
+    T = spikes.shape[0] * 1.
+    fireRates = counts/T
+    if preserve_batch == False:
+        fireRates = jnp.mean(fireRates)
+    return fireRates
+
 @jit
 def measure_sparsity(codes, tolerance=0.):
     """
     Calculates the sparsity (ratio) of an input matrix, assuming each row within
     it is a non-negative vector.
 
     Args:
@@ -18,32 +65,41 @@
     Returns:
         sparsity measurements per code (output shape: N x 1)
     """
     m = (codes > tolerance).astype(jnp.float32)
     rho = jnp.sum(m, axis=1, keepdims=True)/(codes.shape[1] * 1.)
     return rho
 
-@jit
-def measure_ACC(mu, y): ## measures/calculates accuracy
+@partial(jit, static_argnums=[2])
+def measure_ACC(mu, y, extract_label_indx=True): ## measures/calculates accuracy
     """
     Calculates the accuracy (ACC) given a matrix of predictions and matrix of targets.
 
     Args:
-        mu: prediction (design) matrix
+        mu: prediction (design) matrix; shape is (N x C) where C is number of classes
+            and N is the number of patterns examined
+
+        y: target / ground-truth (design) matrix; shape is (N x C) OR an array
+            of class integers of length N (with "extract_label_indx = True")
 
-        y: target / ground-truth (design) matrix
+        extract_label_indx: run an argmax to pull class integer indices from
+            "y", assuming y is a one-hot binary encoding matrix (Default: True),
+            otherwise, this assumes "y" is an array of class integer indices
+            of length N
 
     Returns:
         scalar accuracy score
     """
     guess = jnp.argmax(mu, axis=1)
-    lab = jnp.argmax(y, axis=1)
+    if extract_label_indx == True:
+        lab = jnp.argmax(y, axis=1)
     acc = jnp.sum( jnp.equal(guess, lab) )/(y.shape[0] * 1.)
     return acc
 
+@partial(jit, static_argnums=[2])
 def measure_KLD(p_xHat, p_x, preserve_batch=False):
     """
     Measures the (raw) Kullback-Leibler divergence (KLD), assuming that the two
     input arguments contain valid probability distributions (in each row, if
     they are matrices). Note: If batch is preserved, this returns a column
     vector where each row is the KLD(x_pred, x_true) for that row's datapoint.
```

### Comparing `ngclearn-1.0b4/ngclearn/utils/model_utils.py` & `ngclearn-1.1b0/ngclearn/utils/model_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,49 @@
 import jax
 from jax import numpy as jnp, grad, jit, vmap, random, lax, nn
+from jax.lax import scan as _scan
+from ngcsimlib.utils import Get_Compartment_Batch, Set_Compartment_Batch, get_current_context
 import os, sys
 from functools import partial
+import numpy as np
+
+def tensorstats(tensor):
+    """
+    Prints tensor statistics (debugging tool).
+
+    Args:
+        tensor: argument tensor object to examine
+
+    Returns:
+        useful statistics to print to I/O
+    """
+    if isinstance(tensor, (np.ndarray, jax.Array, jnp.ndarray)):
+        _tensor = np.asarray(tensor)
+        return {
+            'mean': _tensor.mean(),
+            'std': _tensor.std(),
+            'mag': np.abs(_tensor).max(),
+            'min': _tensor.min(),
+            'max': _tensor.max(),
+        }
+    elif isinstance(tensor, (list, tuple, dict)):
+        try:
+            values, _ = jax.tree.flatten(jax.tree.map(lambda x: x.flatten(), tensor))
+            values = np.asarray(np.stack(values))
+            return {
+                'mean': values.mean(),
+                'std': values.std(),
+                'mag': np.abs(values).max(),
+                'min': values.min(),
+                'max': values.max(),
+            }
+        except:
+            return None
+    else:
+        return None
 
 def pull_equations(controller):
     """
     Extracts the dynamics string of this controller (model/system).
 
     Args:
         controller: model/system to extract dynamics equation(s) from
@@ -20,145 +58,14 @@
         for attr in dir(component):
             if not callable(getattr(component, attr)) and not attr.startswith("__"):
                 if attr == "equation":
                     eqn = "{}".format(attr) ## extract defined equation
                     eqn_set = "{}\n{}:  {}".format(_name, eqn)
     return eqn_set
 
-@jit
-def measure_ACC(mu, y): ## measures/calculates accuracy
-    """
-    Calculates the accuracy (ACC) given a matrix of predictions and matrix of targets.
-
-    Args:
-        mu: prediction (design) matrix
-
-        y: target / ground-truth (design) matrix
-
-    Returns:
-        scalar accuracy score
-    """
-    guess = jnp.argmax(mu, axis=1)
-    lab = jnp.argmax(y, axis=1)
-    acc = jnp.sum( jnp.equal(guess, lab) )/(y.shape[0] * 1.)
-    return acc
-
-def measure_KLD(p_xHat, p_x, preserve_batch=False):
-    """
-    Measures the (raw) Kullback-Leibler divergence (KLD), assuming that the two
-    input arguments contain valid probability distributions (in each row, if
-    they are matrices). Note: If batch is preserved, this returns a column
-    vector where each row is the KLD(x_pred, x_true) for that row's datapoint.
-
-    | Formula:
-    | KLD(p_xHat, p_x) = (1/N) [ sum_i(p_x * jnp.log(p_x)) - sum_i(p_x * jnp.log(p_xHat)) ]
-    | where sum_i implies summing across dimensions of vector-space of p_x
-
-    Args:
-        p_xHat: predicted probabilities; (N x C matrix, where C is number of categories)
-
-        p_x: ground true probabilities; (N x C matrix, where C is number of categories)
-
-        preserve_batch: if True, will return one score per sample in batch
-            (Default: False), otherwise, returns scalar mean score
-
-    Returns:
-        an (N x 1) column vector (if preserve_batch=True) OR (1,1) scalar otherwise
-    """
-    ## numerical control step
-    offset = 1e-6
-    _p_x = jnp.clip(p_x, offset, 1. - offset)
-    _p_xHat = jnp.clip(p_xHat, offset, 1. - offset)
-    ## calc raw KLD scores
-    N = p_x.shape[1]
-    term1 = jnp.sum(_p_x * jnp.log(_p_x), axis=1, keepdims=True) # * (1/N)
-    term2 = -jnp.sum(_p_x * jnp.log(_p_xHat), axis=1, keepdims=True) # * (1/N)
-    kld = (term1 + term2) * (1/N)
-    if preserve_batch == False:
-        kld = jnp.mean(kld)
-    return kld
-
-@partial(jit, static_argnums=[3])
-def measure_CatNLL(p, x, offset=1e-7, preserve_batch=False):
-    """
-    Measures the negative Categorical log likelihood (Cat.NLL).  Note: If batch is
-    preserved, this returns a column vector where each row is the
-    Cat.NLL(p, x) for that row's datapoint.
-
-    Args:
-        p: predicted probabilities; (N x C matrix, where C is number of categories)
-
-        x: true one-hot encoded targets; (N x C matrix, where C is number of categories)
-
-        offset: factor to control for numerical stability (Default: 1e-7)
-
-        preserve_batch: if True, will return one score per sample in batch
-            (Default: False), otherwise, returns scalar mean score
-
-    Returns:
-        an (N x 1) column vector (if preserve_batch=True) OR (1,1) scalar otherwise
-    """
-    p_ = jnp.clip(p, offset, 1.0 - offset)
-    loss = -(x * jnp.log(p_))
-    nll = jnp.sum(loss, axis=1, keepdims=True) #/(y_true.shape[0] * 1.0)
-    if preserve_batch == False:
-        nll = jnp.mean(nll)
-    return nll #tf.reduce_mean(nll)
-
-@jit
-def measure_MSE(mu, x, preserve_batch=False):
-    """
-    Measures mean squared error (MSE), or the negative Gaussian log likelihood
-    with variance of 1.0. Note: If batch is preserved, this returns a column
-    vector where each row is the MSE(mu, x) for that row's datapoint.
-
-    Args:
-        mu: predicted values (mean); (N x D matrix)
-
-        x: target values (data); (N x D matrix)
-
-        preserve_batch: if True, will return one score per sample in batch
-            (Default: False), otherwise, returns scalar mean score
-
-    Returns:
-        an (N x 1) column vector (if preserve_batch=True) OR (1,1) scalar otherwise
-    """
-    diff = mu - x
-    se = jnp.square(diff) ## squared error
-    mse = jnp.sum(se, axis=1, keepdims=True) # technically se at this point
-    if preserve_batch == False:
-        mse = jnp.mean(mse) # this is proper mse
-    return mse
-
-@jit
-def measure_BCE(p, x, offset=1e-7, preserve_batch=False): #1e-10
-    """
-    Calculates the negative Bernoulli log likelihood or binary cross entropy (BCE).
-    Note: If batch is preserved, this returns a column vector where each row is
-    the BCE(p, x) for that row's datapoint.
-
-    Args:
-        p: predicted probabilities of shape; (N x D matrix)
-
-        x: target binary values (data) of shape; (N x D matrix)
-
-        offset: factor to control for numerical stability (Default: 1e-7)
-
-        preserve_batch: if True, will return one score per sample in batch
-            (Default: False), otherwise, returns scalar mean score
-
-    Returns:
-        an (N x 1) column vector (if preserve_batch=True) OR (1,1) scalar otherwise
-    """
-    p_ = jnp.clip(p, offset, 1 - offset)
-    bce = -jnp.sum(x * jnp.log(p_) + (1.0 - x) * jnp.log(1.0 - p_),axis=1, keepdims=True)
-    if preserve_batch == False:
-        bce = jnp.mean(bce)
-    return bce
-
 def create_function(fun_name, args=None):
     """
     Activation function creation routine.
 
     Args:
         fun_name: string name of activation function to produce
             (Currently supports: "tanh", "relu", "lrelu", "identity")
@@ -266,16 +173,15 @@
         a normalized value matrix
     """
     if order == 2: ## denominator is L2 norm
         wOrdSum = jnp.square(jnp.sum(jnp.square(M), axis=axis, keepdims=True))
     else: ## denominator is L1 norm
         wOrdSum = jnp.sum(jnp.abs(M), axis=axis, keepdims=True)
     m = (wOrdSum == 0.).astype(dtype=jnp.float32)
-    wOrdSum = wOrdSum * (1. - m) + m
-    #wAbsSum[wAbsSum == 0.] = 1.
+    wOrdSum = wOrdSum * (1. - m) + m #wAbsSum[wAbsSum == 0.] = 1.
     _M = M * (wnorm/wOrdSum)
     return _M
 
 @jit
 def clamp_min(x, min_val):
     """
     Clamps values in data x that exceed a minimum value to that value.
@@ -645,7 +551,45 @@
     """
     eps = random.uniform(dkey, (input.shape[0],input.shape[1]),
                          minval=0.0, maxval=1.0)
     mask = (eps <= (1.0 - rate)).astype(jnp.float32)
     mask = mask * (1.0 / (1.0 - rate)) ## apply inverted dropout scheme
     output = input * mask
     return output, mask
+
+
+def scanner(fn):
+    """
+    A wrapper for Jax's scanner that handles the "getting" of the current
+    state and "setting" of the final state to and from the model.
+
+    | @scanner
+    | def process(current_state, args):
+    |    t = args[0]
+    |    dt = args[1]
+    |    current_state = model.advance_state(current_state, t, dt)
+    |    current_state = model.evolve(current_state, t, dt)
+    |    return current_state, (current_state[COMPONENT.COMPARTMENT.path], ...)
+    |
+    | outputs = models.process(jnp.array([[ARG0, ARG1] for i in range(NUM_LOOPS)]))
+
+    | Notes on the scanner function call:
+    | 1) `current_state` is a hash-map mapped to all compartment values by path
+    | 2) `args` is the external arguments defined in the passed Jax array
+    | 3) `outputs` is a tuple containing time-concatenated Jax arrays of the
+    |     compartment statistics you want tracked
+
+    Args:
+        fn: function that is executed at every time step of a Jax-unrolled loop,
+            it must take in the current state and external arguments
+
+    Returns:
+        wrapped (fast) function that is Jax-scanned/jit-i-fied
+    """
+    def _scanned(_xs):
+        vals, stacked = _scan(fn, init=Get_Compartment_Batch(), xs=_xs)
+        Set_Compartment_Batch(vals)
+        return stacked
+
+    if get_current_context() is not None:
+        get_current_context().__setattr__(fn.__name__, _scanned)
+    return _scanned
```

### Comparing `ngclearn-1.0b4/ngclearn/utils/optim/sgd.py` & `ngclearn-1.1b0/ngclearn/utils/optim/sgd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,57 @@
-from ngclearn.utils.optim.opt import Opt
+# %%
+
+from ngcsimlib.component import Component
+from ngcsimlib.compartment import Compartment
+from ngcsimlib.resolver import resolver
+
 import numpy as np
 from jax import jit, numpy as jnp, random, nn, lax
 from functools import partial
 import time
 
-@jit
 def step_update(param, update, lr):
     """
     Runs one step of SGD over a set of parameters given updates.
 
     Args:
         lr: global step size to apply when adjusting parameters
 
     Returns:
         adjusted parameter tensor (same shape as "param")
     """
     _param = param - lr * update
     return _param
 
-class SGD(Opt):
-    """
-    Implements stochastic gradient descent (SGD) as a decoupled update rule
-    given adjustments produced by a credit assignment algorithm/process.
+@jit
+def sgd_step(opt_params, theta, updates, eta=0.001): ## apply adjustment to theta
+    """Return a params update
 
     Args:
-        learning_rate: step size coefficient for SGD update
+        opt_params: (ArrayLike) parameters of the optimization algorithm
+
+        theta: (ArrayLike) the weights of neural networks
+
+        updates: (ArrayLike) the updates of neural networks
+
+        eta: (float, optional) hyperparams. Defaults to 0.001.
+
+    Returns:
+        ArrayLike: opt_params. New opt params, ArrayLike: theta. The updated weights
     """
-    def __init__(self, learning_rate=0.001):
-        super().__init__(name="sgd")
-        self.eta = learning_rate
-        #self.time = 0.
-
-    def update(self, theta, updates): ## apply adjustment to theta
-        self.time += 1
-        for i in range(len(theta)):
-            px_i = step_update(theta[i], updates[i], self.eta)
-            theta[i] = px_i
+    time_step = opt_params
+    time_step = time_step + 1
+    new_theta = []
+    for i in range(len(theta)):
+        px_i = step_update(theta[i], updates[i], eta)
+        new_theta.append(px_i)
+    new_opt_params = time_step
+    return new_opt_params, new_theta
+
+@jit
+def sgd_init(theta):
+    return jnp.asarray(0.0)
+
+
+if __name__ == '__main__':
+    opt_params, theta = sgd_step((2.0), [1.0, 1.0], [3.0, 4.0], 3e-2)
+    print(f"opt_params: {opt_params}, theta: {theta}")
```

### Comparing `ngclearn-1.0b4/ngclearn/utils/patch_utils.py` & `ngclearn-1.1b0/ngclearn/utils/patch_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,79 +1,75 @@
-import jax
 import numpy as np
-from jax import numpy as jnp, grad, jit, vmap, random, lax
-import os, sys, pickle
-from functools import partial
+from jax import numpy as jnp
 from sklearn.feature_extraction.image import extract_patches_2d
 
-def _generate_patch_set(x_batch_, patch_size=(5,5), max_patches=50, center=True):
-    import patchify as ptch
+def generate_patch_set(x_batch, patch_size=(8, 8), max_patches=50, center=True): ## scikit
     """
     Generates a set of patches from an array/list of image arrays (via
-    random sampling with replacement). This uses the patchify library to create
-    a of non-random non-overlapping or overlapping (w/ controllable stride) patches.
+    random sampling with replacement). This uses scikit-learn's patch creation
+    function to generate a set of (px x py) patches.
     Note: this routine also subtracts each patch's mean from itself.
 
     Args:
-        imgs: the array of image arrays to sample from
+        x_batch: the array of image arrays to sample from
 
         patch_size: a 2-tuple of the form (pH = patch height, pW = patch width)
 
-        max_patches: UNUSED
+        max_patches: maximum number of patches to extract/generate from source images
 
         center: centers each patch by subtracting the patch mean (per-patch)
 
     Returns:
         an array (D x (pH * pW)), where each row is a flattened patch sample
     """
-    x_batch = np.array(x_batch_)
-    px = py = int(np.sqrt(x_batch.shape[1])) # get image shape of the data
-    x_batch = np.expand_dims(x_batch.reshape(px, py), axis=2)
-    pch_x = patch_size[0]
-    pch_y = patch_size[1]
-    pX = np.squeeze( ptch.patchify(x_batch, (pch_x,pch_y,1), step=pch_x) ) # step = stride
-    p_patch = []
-    for i in range(pX.shape[0]):
-        for j in range(pX.shape[1]):
-            _p = np.reshape(pX[i,j,:,:], (1, pch_x * pch_y))
-            p_patch.append(_p)
-    p_patch = jnp.concatenate(p_patch, axis=0)
+    _x_batch = np.array(x_batch)
+    px = py = int(np.sqrt(_x_batch.shape[1])) # get image shape of the data
+    p_batch = None
+    for s in range(_x_batch.shape[0]):
+        xs = _x_batch[s, :]
+        xs = xs.reshape(px, py)
+        patches = extract_patches_2d(xs, patch_size, max_patches=max_patches)#, random_state=69)
+        patches = np.reshape(patches, (len(patches), -1)) # flatten each patch in set
+        if s > 0:
+            p_batch = np.concatenate((p_batch,patches),axis=0)
+        else:
+            p_batch = patches
     if center == True:
         mu = np.mean(p_batch,axis=1,keepdims=True)
         p_batch = p_batch - mu
-    return p_patch
+    return jnp.array(p_batch)
 
-def generate_patch_set(x_batch_, patch_size=(8,8), max_patches=50, center=True):
+def generate_pacthify_patch_set(x_batch_, patch_size=(5, 5), center=True): ## patchify
+    ## this is a patchify-specific function (only use if you have patchify installed...)
+    import patchify as ptch
     """
     Generates a set of patches from an array/list of image arrays (via
-    random sampling with replacement). This uses scikit-learn's patch creation
-    function to generate a set of (px x py) patches.
+    random sampling with replacement). This uses the patchify library to create
+    a of non-random non-overlapping or overlapping (w/ controllable stride) patches.
     Note: this routine also subtracts each patch's mean from itself.
 
     Args:
-        imgs: the array of image arrays to sample from
+        x_batch_: the array of image arrays to sample from
 
         patch_size: a 2-tuple of the form (pH = patch height, pW = patch width)
 
-        max_patches: maximum number of patches to extract/generate from source images
-
         center: centers each patch by subtracting the patch mean (per-patch)
 
     Returns:
         an array (D x (pH * pW)), where each row is a flattened patch sample
     """
     x_batch = np.array(x_batch_)
     px = py = int(np.sqrt(x_batch.shape[1])) # get image shape of the data
-    p_batch = None
-    for s in range(x_batch.shape[0]):
-        xs = x_batch[s,:]
-        xs = xs.reshape(px, py)
-        patches = extract_patches_2d(xs, patch_size, max_patches=max_patches)#, random_state=69)
-        patches = np.reshape(patches, (len(patches), -1)) # flatten each patch in set
-        if s > 0:
-            p_batch = np.concatenate((p_batch,patches),axis=0)
-        else:
-            p_batch = patches
+    x_batch = np.expand_dims(x_batch.reshape(px, py), axis=2)
+    pch_x = patch_size[0]
+    pch_y = patch_size[1]
+    pX = np.squeeze( ptch.patchify(x_batch, (pch_x,pch_y,1), step=pch_x) ) # step = stride
+    patchBatch = []
+    for i in range(pX.shape[0]):
+        for j in range(pX.shape[1]):
+            _p = np.reshape(pX[i,j,:,:], (1, pch_x * pch_y))
+            patchBatch.append(_p)
+    patchBatch = jnp.concatenate(patchBatch, axis=0)
     if center == True:
-        mu = np.mean(p_batch,axis=1,keepdims=True)
-        p_batch = p_batch - mu
-    return jnp.array(p_batch)
+        mu = np.mean(patchBatch, axis=1,keepdims=True)
+        patchBatch = patchBatch - mu
+    return patchBatch
```

### Comparing `ngclearn-1.0b4/ngclearn/utils/surrogate_fx.py` & `ngclearn-1.1b0/ngclearn/utils/surrogate_fx.py`

 * *Files identical despite different names*

### Comparing `ngclearn-1.0b4/ngclearn/utils/viz/dim_reduce.py` & `ngclearn-1.1b0/ngclearn/utils/viz/dim_reduce.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     z_2D = None
     if z_dim != 2:
         print(" > Projecting latents via iPCA...")
         n_comp = n_pca_comp #32 #10 #16 #50
         if n_comp > batch_size:
             batch_size = n_comp
         if vectors.shape[1] < n_comp:
-            n_comp = vectors.shape[1] - 2 #z_top.shape[1]-2
+            n_comp = vectors.shape[1] - 2
             n_comp = max(2, n_comp)
         ipca = IncrementalPCA(n_components=n_comp, batch_size=batch_size)
         ipca.fit(vectors)
         z_2D = ipca.transform(vectors)
         print(" PCA.lat.shape = ",z_2D.shape)
         print(" > Finishing projection via t-SNE...")
         z_2D = TSNE(n_components=2,perplexity=perplexity, verbose=1).fit_transform(z_2D)
```

### Comparing `ngclearn-1.0b4/ngclearn/utils/viz/raster.py` & `ngclearn-1.1b0/ngclearn/utils/viz/raster.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,62 +6,23 @@
 #import tensorflow as tf
 import matplotlib.pyplot as plt
 from matplotlib import gridspec
 import numpy as np
 import imageio.v3 as iio
 import jax.numpy as jnp
 
-#suffix = '.jpg' #.png
-
-def _create_raster_plot(spike_train, ax=None, s=1.5, c="black", marker="|",
-                       plot_fname=None, indices=None, suffix='.jpg'):
-    spk_ = spike_train
-    # Process spikes and create the binary coordinate grid
-    if len(spk_.shape) == 1:
-        spk_ = jnp.expand_dims(spk_,axis=1)
-    n_units = spk_.shape[1]
-    if indices is not None and indices.shape[0] < spk_.shape[1]:
-        spk_ = spk_[:,indices] # access specific neurons if requested
-        if len(spk_.shape) > 1:
-            n_units = spk_.shape[1]
-        else:
-            n_units = spk_.shape[0]
-    coords = spk_.nonzero() #jnp.where(spk_) #tf.where(spk_).numpy()
-    spk_x = coords[0] #coords[:,0]
-    spk_y = coords[1] #coords[:,1]
-    if ax is not None:
-        ax.scatter(spk_x, spk_y, s=s, c=c, marker=marker,linewidths=4)
-        yint = range(0, n_units)
-        ax.set_yticks(yint)
-        ax.set_yticklabels(yint, fontsize=12)
-        return ax
-    else:
-        if plot_fname is None:
-            plot_fname = "raster_plot" + suffix
-        fig = plt.figure(facecolor="w", figsize=(10, 5))
-        ax = fig.add_subplot(111)
-        ax.scatter(spk_x, spk_y, s=s, c=c, marker=marker)
-        yint = range(0, n_units)
-        ax.set_yticks(yint)
-        ax.set_yticklabels(yint, fontsize=12)
-        plt.title("Spike Train Raster Plot")
-        plt.xlabel("Time Step")
-        plt.ylabel("Neuron Index")
-        plt.savefig(plot_fname)
-        plt.clf()
-        plt.close()
-
 def create_raster_plot(spike_train, ax=None, s=0.5, c="black",
                        plot_fname=None, indices=None, tag="", suffix='.jpg'):
     """
     Generates a raster plot of a given (binary) spike train (row dimension
     corresponds to the discrete time dimension).
 
     Args:
-        spike_train: a numpy binary array of shape (T x number_neurons)
+        spike_train: a numpy binary array of shape (number_neurons x 1 x T) OR
+            shape (number_neurons x T)
 
         ax: a hook/pointer to a currently external plot that this raster plot
             should be made a sub-figure of
 
         s: size of the spike scatter points (Default = 1.5)
 
         c: color of the spike scatter points (Default = black)
@@ -72,14 +33,19 @@
 
         indices: optional indices of neurons (row integer indices) to focus on plotting
 
         tag:
 
         suffix: output plot file suffix name to append
     """
+    if len(spike_train.shape) == 3 and spike_train.shape[1] == 1:
+        spike_train = jnp.transpose(spike_train, [2,0,1])
+    elif len(spike_train.shape) == 2:
+        spike_train = spike_train.T
+
     n_count = spike_train.shape[0]
     step_count = spike_train.shape[1]
     save = False
     if ax is None:
         if plot_fname is None:
             plot_fname = "raster_plot" + suffix
```

### Comparing `ngclearn-1.0b4/ngclearn/utils/viz/spike_plot.py` & `ngclearn-1.1b0/ngclearn/utils/viz/spike_plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import matplotlib #.pyplot as plt
 matplotlib.use('Agg')
 import matplotlib.pyplot as plt
 cmap = plt.cm.jet
 import jax.numpy as jnp
 import numpy as np
-from ngclearn.utils.viz.raster import _create_raster_plot
 
 def plot_spiking_neuron(curr, mem, spike, ref, dt, thr_line=False,
-                    title=False, min_mem_val=0.0, max_mem_val=1.25, fname=None):
+                    title=False, min_mem_val=0.0, max_mem_val=1.25, 
+                    spike_loc=1., spike_spr=0.05, fname=None):
+    import matplotlib #.pyplot as plt
+    matplotlib.use('Agg')
+    import matplotlib.pyplot as plt
+    cmap = plt.cm.jet
     """
     Simple plotting function for visualizing the trajectory of a single neuron
     (where its input electrical current, membrane potential value, output
     spike readings, and refractory variable states have been recorded into arrays).
 
     This is particularly useful for single neuronal dynamics demonstrations and
     analyses.
@@ -33,42 +37,42 @@
 
         min_mem_val: minimum value bound on membrane potential subplot (min of y-axis)
 
         max_mem_val: maximum value bound on membrane potential subplot (max of y-axis)
 
         fname: the filename to save this plot as, i.e., /path/to/name.png (Default: lif_analysis.png)
     """
+    spk_ = spike + 0
+    mask = 0.
+    if ref != None:
+        mask = np.greater_equal(ref,dt).astype(np.float32)
+    spk_ = spk_ * (1.0 - mask)
+    stat = np.where(spk_ > 0.)
+    indx = (stat[0] * 1. - 1.).tolist()
+
     x_lim = curr.shape[0]
     y_curr_lim = float(np.amax(curr)) + 0.2
-    fig, ax = plt.subplots(3, figsize=(8,6), sharex=True,
-                        gridspec_kw = {'height_ratios': [1, 1, 0.4]})
+    fig, ax = plt.subplots(2, figsize=(8,6), sharex=True,
+                        gridspec_kw = {'height_ratios': [1, 1]})
     # plot input current
     ax[0].plot(curr, c="tab:blue")
     ax[0].set_ylim([0, y_curr_lim])
     ax[0].set_xlim([0, x_lim])
     ax[0].set_ylabel("Input Current ($J_t$)")
     if title:
         ax[0].set_title(title)
 
     # plot membrane potential
     ax[1].plot(mem, c="tab:red")
+    ax[1].vlines(x=indx, ymin=spike_loc-spike_spr, ymax=spike_loc+spike_spr,
+                 colors='black', ls='--', lw=5)
     ax[1].set_ylim([min_mem_val, max_mem_val])
     ax[1].set_ylabel("Membrane Potential ($V_t$)")
     if thr_line:
         ax[1].axhline(y=thr_line, alpha=0.25, linestyle="dashed", c="black", linewidth=2)
     plt.xlabel("Time Step $t$")
 
-    spk_ = spike + 0
-    mask = 0.
-    if ref != None:
-        mask = np.greater_equal(ref,dt).astype(np.float32)
-    spk_ = spk_ * (1.0 - mask)
-
-    # Plot output spike using spikeplot
-    _create_raster_plot(spk_, ax[2], s=100, c="black")
-    plt.ylabel("Output Spikes")
-    plt.yticks([])
     if fname is None:
         fname = "lif_plot.png"
     plt.tight_layout()
     plt.savefig(fname)
     plt.clf()
```

### Comparing `ngclearn-1.0b4/ngclearn/utils/viz/synapse_plot.py` & `ngclearn-1.1b0/ngclearn/utils/viz/synapse_plot.py`

 * *Files 25% similar despite different names*

```diff
@@ -144,9 +144,49 @@
     images = []
     for i in range(f_start, f_end+1, skip):
         print("Reading frame " + str(i))
         images.append(iio.imread(path + "/" + prefix + str(i) + suffix))
     print("writing gif")
     iio.imwrite(path + '/training.gif', images, loop=0, duration=200)
 
-#if __name__ == "__main__":
-#    make_video(0, 50, 'trials/Two_Layer/3', 'joint_')
+
+# def visualize_norm(thetas, sizes, prefix, suffix='.jpg'):
+
+def viz_block(thetas, sizes, prefix, suffix=".jpg", padding=1, low_rez=True):
+    num_filters = [T.shape[1] for T in thetas]
+    n_cols = [math.ceil(math.sqrt(nf)) for nf in num_filters]
+    n_rows = [math.ceil(nf / c) for nf, c in zip(num_filters, n_cols)]
+    idxs = [i for i in range(len(thetas))]
+
+    if not low_rez:
+        n_cols_size = int(sum([(t_c * cols) + padding * (cols - 1) for (t_c, _), cols in zip(sizes, n_cols)]))
+        n_rows_size = int(sum([(t_r * rows) + padding * (rows - 1) for (_, t_r), rows in zip(sizes, n_rows)]))
+        plt.figure(figsize=(n_cols_size, n_rows_size))
+
+
+    for t, num_f, (t_c, t_r), cols, rows, idx in zip(thetas, num_filters, sizes, n_cols, n_rows, idxs):
+        c_dim = (t_c * cols) + padding * (cols - 1)
+        r_dim = (t_r * rows) + padding * (rows - 1)
+
+        full = jnp.ones((r_dim, c_dim)) * np.amax(t)
+
+        for k in range(num_f):
+            r = k // cols
+            c = k % cols
+
+            r_start = (r * (t_r + padding))
+            r_end = (r * (t_r + padding)) + t_r
+
+            c_start = (c * (t_c + padding))
+            c_end = (c * (t_c + padding)) + t_c
+
+            full = full.at[r_start:r_end, c_start:c_end].set(
+                jnp.reshape(t[:, k], (t_r, t_c)))
+
+        plt.subplot(1, len(thetas), idx+1)
+        plt.imshow(full, cmap=plt.cm.bone, interpolation='nearest')
+        plt.axis("off")
+
+    plt.savefig(prefix + suffix, bbox_inches='tight')
+    plt.clf()
+    plt.close()
+
```

### Comparing `ngclearn-1.0b4/ngclearn.egg-info/PKG-INFO` & `ngclearn-1.1b0/ngclearn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngclearn
-Version: 1.0b4
+Version: 1.1b0
 Summary: Simulation software for building and analyzing arbitrary predictive coding, spiking network, and biomimetic neural systems.
 Author-email: Alexander Ororbia <ago@cs.rit.edu>, William Gebhardt <wdg1351@rit.edu>
 License: BSD-3-Clause License
 Project-URL: Homepage, https://github.com/NACLab/ngc-learn
 Project-URL: Documentation, https://ngc-learn.readthedocs.io/
 Project-URL: Lab Page, https://www.cs.rit.edu/~ago/nac_lab.html
 Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/main/history.txt
@@ -18,26 +18,26 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Unix
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS
-Requires-Dist: numpy>=1.26.0
+Requires-Dist: numpy>=1.24.0
 Requires-Dist: scikit-learn>=0.24.2
 Requires-Dist: scipy>=1.7.0
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: patchify
 Requires-Dist: jax>=0.4.18
 Requires-Dist: jaxlib>=0.4.18
-Requires-Dist: ngcsimlib>=0.2.b2
+Requires-Dist: ngcsimlib>=0.3.b0
 Requires-Dist: imageio>=2.31.5
 
 [![Python Version](https://img.shields.io/badge/python-3.10%20%7C%203.11-blue.svg)](https://www.python.org/downloads)[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)[![Documentation Status](https://readthedocs.org/projects/ngc-learn/badge/?version=latest)](http://ngc-learn.readthedocs.io/en/latest/?badge=latest)[![DOI](https://zenodo.org/badge/483413212.svg)](https://zenodo.org/badge/latestdoi/483413212)
 
 <img src="docs/images/ngc-learn-logo.png" width="300">
 
 <b>ngc-learn</b> is a Python library for building, simulating, and analyzing
@@ -90,19 +90,24 @@
 tools (routines within ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2).
 Many of the tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-learn (>=0.24.2).
 <!-- (Note: if using the `_generate_patch_set()` within the
 image patching utilities, then Patchify will be needed).-->
 
 ### User Installation
 
-<i>Setup</i>: The easiest way to install ngc-learn (CPU version) is through <code>pip</code>:
+<i>Setup</i>: The easiest way to install ngc-learn is through <code>pip</code>:
 <pre>
 $ pip install ngclearn
 </pre>
 
+Note that installing the official pip package without any form of JAX installed
+on your system will default to downloading the CPU version of ngc-learn; make
+sure you have installed the Cuda 12 version of Jax/Jaxlib on your system before
+running the above pip command if you want to use the GPU version.
+
 The documentation includes more detailed
 <a href="https://ngc-learn.readthedocs.io/en/latest/installation.html">installation instructions</a>.
 Note that this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
 
 If the installation was successful, you should see the following if you test
 it against your Python interpreter, i.e., run the <code>$ python</code> command
 and complete the following sequence of steps as depicted in the screenshot below
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ngclearn Version: 1.0b4 Summary: Simulation
+Metadata-Version: 2.1 Name: ngclearn Version: 1.1b0 Summary: Simulation
 software for building and analyzing arbitrary predictive coding, spiking
 network, and biomimetic neural systems. Author-email: Alexander Ororbia
 cs.rit.edu>, William Gebhardt
 rit.edu> License: BSD-3-Clause License Project-URL: Homepage, https://
 github.com/NACLab/ngc-learn Project-URL: Documentation, https://ngc-
 learn.readthedocs.io/ Project-URL: Lab Page, https://www.cs.rit.edu/~ago/
 nac_lab.html Project-URL: Changelog, https://github.com/NACLab/ngc-learn/blob/
@@ -12,20 +12,20 @@
 Audience :: Education Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers Classifier: License :: OSI Approved
 :: BSD License Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
 Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: Unix Requires-Python: >=3.10 Description-
+Classifier: Operating System :: Unix Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE License-File: AUTHORS
-Requires-Dist: numpy>=1.26.0 Requires-Dist: scikit-learn>=0.24.2 Requires-Dist:
+Requires-Dist: numpy>=1.24.0 Requires-Dist: scikit-learn>=0.24.2 Requires-Dist:
 scipy>=1.7.0 Requires-Dist: matplotlib>=3.8.0 Requires-Dist: patchify Requires-
 Dist: jax>=0.4.18 Requires-Dist: jaxlib>=0.4.18 Requires-Dist:
-ngcsimlib>=0.2.b2 Requires-Dist: imageio>=2.31.5 [![Python Version](https://
+ngcsimlib>=0.3.b0 Requires-Dist: imageio>=2.31.5 [![Python Version](https://
 img.shields.io/badge/python-3.10%20%7C%203.11-blue.svg)](https://
 www.python.org/downloads)[![License](https://img.shields.io/badge/License-
 BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)[!
 [Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https:
 //GitHub.com/Naereen/StrapDown.js/graphs/commit-activity)[![Documentation
 Status](https://readthedocs.org/projects/ngc-learn/badge/?version=latest)]
 (http://ngc-learn.readthedocs.io/en/latest/?badge=latest)[![DOI](https://
@@ -49,29 +49,33 @@
 CUDA variants) --- ngc-learn 1.0.beta0 and later require Python 3.10 or newer
 as well as ngcsimlib >=0.2.b2. ngc-learn's plotting capabilities (routines
 within `ngclearn.utils.viz`) require Matplotlib (>=3.8.0) and imageio
 (>=2.31.5) and both plotting and density estimation tools (routines within
 ``ngclearn.utils.density``) will require Scikit-learn (>=0.24.2). Many of the
 tutorials will require Matplotlib (>=3.8.0), imageio (>=2.31.5), and Scikit-
 learn (>=0.24.2). ### User Installation Setup: The easiest way to install ngc-
-learn (CPU version) is through pip:
+learn is through pip:
 $ pip install ngclearn
-The documentation includes more detailed _i_n_s_t_a_l_l_a_t_i_o_n_ _i_n_s_t_r_u_c_t_i_o_n_s. Note that
-this library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and
-20.04. If the installation was successful, you should see the following if you
-test it against your Python interpreter, i.e., run the $ python command and
-complete the following sequence of steps as depicted in the screenshot below
-(you should see at the bottom of your output something akin to the right major
-and minor version of ngc-learn): ```console Python 3.11.4 (main, MONTH DAY
-YEAR, TIME) [GCC XX.X.X] on linux Type "help", "copyright", "credits" or
-"license" for more information. >>> import ngclearn >>> ngclearn.__version__
-'1.0b3' ``` Note: For access to the previous Tensorflow-2 version of ngc-learn
-(of which we no longer support), please visit the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ##
-AAttttrriibbuuttiioonn:: If you use this code in any form in your project(s), please cite
-its source paper (as well as ngc-learn's official software citation):
+Note that installing the official pip package without any form of JAX installed
+on your system will default to downloading the CPU version of ngc-learn; make
+sure you have installed the Cuda 12 version of Jax/Jaxlib on your system before
+running the above pip command if you want to use the GPU version. The
+documentation includes more detailed _i_n_s_t_a_l_l_a_t_i_o_n_ _i_n_s_t_r_u_c_t_i_o_n_s. Note that this
+library was developed on Ubuntu 20.04 and tested on Ubuntu(s) 18.04 and 20.04.
+If the installation was successful, you should see the following if you test it
+against your Python interpreter, i.e., run the $ python command and complete
+the following sequence of steps as depicted in the screenshot below (you should
+see at the bottom of your output something akin to the right major and minor
+version of ngc-learn): ```console Python 3.11.4 (main, MONTH DAY YEAR, TIME)
+[GCC XX.X.X] on linux Type "help", "copyright", "credits" or "license" for more
+information. >>> import ngclearn >>> ngclearn.__version__ '1.0b3' ``` Note: For
+access to the previous Tensorflow-2 version of ngc-learn (of which we no longer
+support), please visit the repo for _n_g_c_-_l_e_a_r_n_-_l_e_g_a_c_y. ## AAttttrriibbuuttiioonn:: If you
+use this code in any form in your project(s), please cite its source paper (as
+well as ngc-learn's official software citation):
 @article{Ororbia2022,
   author={Ororbia, Alexander and Kifer, Daniel},
   title={The neural coding framework for learning generative models},
   journal={Nature Communications},
   year={2022},
   month={Apr},
   day={19},
```

### Comparing `ngclearn-1.0b4/ngclearn.egg-info/SOURCES.txt` & `ngclearn-1.1b0/ngclearn.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,83 @@
 AUTHORS
 LICENSE
 README.md
 pyproject.toml
 requirements.txt
-UPDATED_cells/LIFCell.py
-UPDATED_cells/older_sLIF.py
 ngclearn/__init__.py
 ngclearn.egg-info/PKG-INFO
 ngclearn.egg-info/SOURCES.txt
 ngclearn.egg-info/dependency_links.txt
 ngclearn.egg-info/requires.txt
 ngclearn.egg-info/top_level.txt
 ngclearn/commands/__init__.py
 ngclearn/components/__init__.py
-ngclearn/components/baseComponentTemplate.py
-ngclearn/components/wrappers.py
 ngclearn/components/input_encoders/__init__.py
 ngclearn/components/input_encoders/bernoulliCell.py
 ngclearn/components/input_encoders/latencyCell.py
 ngclearn/components/input_encoders/poissonCell.py
+ngclearn/components/lava/__init__.py
+ngclearn/components/lava/neurons/LIFCell.py
+ngclearn/components/lava/neurons/__init__.py
+ngclearn/components/lava/synapses/__init__.py
+ngclearn/components/lava/synapses/hebbianSynapse.py
+ngclearn/components/lava/synapses/staticSynapse.py
+ngclearn/components/lava/synapses/traceSTDPSynapse.py
+ngclearn/components/lava/traces/__init__.py
+ngclearn/components/lava/traces/gatedTrace.py
 ngclearn/components/neurons/__init__.py
 ngclearn/components/neurons/graded/__init__.py
 ngclearn/components/neurons/graded/gaussianErrorCell.py
 ngclearn/components/neurons/graded/laplacianErrorCell.py
 ngclearn/components/neurons/graded/rateCell.py
 ngclearn/components/neurons/spiking/LIFCell.py
+ngclearn/components/neurons/spiking/WTASCell.py
 ngclearn/components/neurons/spiking/__init__.py
+ngclearn/components/neurons/spiking/adExCell.py
 ngclearn/components/neurons/spiking/fitzhughNagumoCell.py
 ngclearn/components/neurons/spiking/izhikevichCell.py
 ngclearn/components/neurons/spiking/quadLIFCell.py
 ngclearn/components/neurons/spiking/sLIFCell.py
 ngclearn/components/other/__init__.py
 ngclearn/components/other/expKernel.py
 ngclearn/components/other/varTrace.py
 ngclearn/components/synapses/__init__.py
+ngclearn/components/synapses/staticSynapse.py
 ngclearn/components/synapses/hebbian/__init__.py
+ngclearn/components/synapses/hebbian/eventSTDPSynapse.py
 ngclearn/components/synapses/hebbian/expSTDPSynapse.py
 ngclearn/components/synapses/hebbian/hebbianSynapse.py
 ngclearn/components/synapses/hebbian/traceSTDPSynapse.py
+ngclearn/operations/__init__.py
 ngclearn/utils/__init__.py
 ngclearn/utils/data_loader.py
 ngclearn/utils/io_utils.py
 ngclearn/utils/metric_utils.py
 ngclearn/utils/model_utils.py
 ngclearn/utils/patch_utils.py
 ngclearn/utils/surrogate_fx.py
 ngclearn/utils/density/__init__.py
 ngclearn/utils/density/gmm.py
 ngclearn/utils/diffeq/__init__.py
-ngclearn/utils/diffeq/_ode_utils.py
 ngclearn/utils/diffeq/ode_utils.py
 ngclearn/utils/optim/__init__.py
 ngclearn/utils/optim/adam.py
-ngclearn/utils/optim/opt.py
+ngclearn/utils/optim/optim_utils.py
 ngclearn/utils/optim/sgd.py
 ngclearn/utils/viz/__init__.py
 ngclearn/utils/viz/dim_reduce.py
 ngclearn/utils/viz/raster.py
 ngclearn/utils/viz/spike_plot.py
-ngclearn/utils/viz/synapse_plot.py
+ngclearn/utils/viz/synapse_plot.py
+test_code/_run_trstdp.py
+test_code/adex.py
+test_code/calc_fanoFactor.py
+test_code/run2_metrics.py
+test_code/run_expkernel.py
+test_code/run_metrics.py
+test_code/run_trace.py
+test_code/run_trstdp.py
+test_code/test_adex.py
+test_code/test_fhcell.py
+test_code/test_izhcell.py
+test_code/viz_data.py
+test_lava/run_xotSNN.py
```

### Comparing `ngclearn-1.0b4/pyproject.toml` & `ngclearn-1.1b0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ngclearn"
-version = "1.0.beta4"
+version = "1.1.beta0"
 description = "Simulation software for building and analyzing arbitrary predictive coding, spiking network, and biomimetic neural systems."
 authors = [
   {name = "Alexander Ororbia", email = "ago@cs.rit.edu"},
   {name = "William Gebhardt", email = "wdg1351@rit.edu"},
 ]
 readme = "README.md"
 keywords = ['python', 'ngc-learn', 'predictive-processing', 'predictive-coding',
             'jax', 'spiking-neural-networks', 'biomimetics', 'bionics', 'computational-neuroscience']
-requires-python = ">=3.10"
+requires-python = ">=3.8" # 3.10
 license = {text = "BSD-3-Clause License"}
 classifiers=[
   "Development Status :: 4 - Beta", #3 - Alpha", # 5 - Production/Stable
   "Intended Audience :: Education",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
@@ -29,21 +29,14 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: Unix"
 ]
 dynamic = ["dependencies"]
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]} ## use classic requirements file
-#dependencies = [
-#  "imageio==2.31.5",
-#  "numpy>=1.26.0",
-#  "scikit-learn>=0.24.2",
-#  "scipy>=1.7.0",
-#  "matplotlib>=3.8.0",
-#]
 
 [project.urls]
 Homepage = "https://github.com/NACLab/ngc-learn"
 Documentation = "https://ngc-learn.readthedocs.io/"
 "Lab Page" = "https://www.cs.rit.edu/~ago/nac_lab.html"
 Changelog = "https://github.com/NACLab/ngc-learn/blob/main/history.txt"
```

