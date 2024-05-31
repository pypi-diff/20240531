# Comparing `tmp/psychopy-visionscience-0.0.5.tar.gz` & `tmp/psychopy_visionscience-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychopy-visionscience-0.0.5.tar", last modified: Thu Feb 15 22:40:33 2024, max compression
+gzip compressed data, was "psychopy_visionscience-0.0.6.tar", last modified: Fri May 31 15:19:55 2024, max compression
```

## Comparing `psychopy-visionscience-0.0.5.tar` & `psychopy_visionscience-0.0.6.tar`

### file list

```diff
@@ -1,57 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.473853 psychopy-visionscience-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-02-15 22:40:33.473853 psychopy-visionscience-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.469853 psychopy-visionscience-0.0.5/psychopy_visionscience/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.469853 psychopy-visionscience-0.0.5/psychopy_visionscience/components/
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.469853 psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/
--rw-r--r--   0 runner    (1001) docker     (127)    15272 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.469853 psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/classic/
--rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/classic/envelope_grating@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/classic/envelopegrating.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.469853 psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/dark/
--rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/dark/envelopegrating.png
--rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/dark/envelopegrating@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.469853 psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/light/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/light/envelopegrating.png
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/light/envelopegrating@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.469853 psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/
--rw-r--r--   0 runner    (1001) docker     (127)    20944 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.473853 psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/classic/
--rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/classic/noise.png
--rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/classic/noise@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.473853 psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/dark/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/dark/noise.png
--rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/dark/noise@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.473853 psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/light/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/light/noise.png
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/light/noise@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.473853 psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.473853 psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/classic/
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/classic/radial.png
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/classic/radial@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.473853 psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/dark/
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/dark/radial.png
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/dark/radial@2x.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.473853 psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/light/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/light/radial.png
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/light/radial@2x.png
--rw-r--r--   0 runner    (1001) docker     (127)    36103 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    21731 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/radial.py
--rw-r--r--   0 runner    (1001) docker     (127)    26765 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/secondorder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.473853 psychopy-visionscience-0.0.5/psychopy_visionscience/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.473853 psychopy-visionscience-0.0.5/psychopy_visionscience/tests/test_visual/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/tests/test_visual/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/psychopy_visionscience/tests/test_visual/test_all_stimuli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 22:40:33.473853 psychopy-visionscience-0.0.5/psychopy_visionscience.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-02-15 22:40:33.000000 psychopy-visionscience-0.0.5/psychopy_visionscience.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-02-15 22:40:33.000000 psychopy-visionscience-0.0.5/psychopy_visionscience.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 22:40:33.000000 psychopy-visionscience-0.0.5/psychopy_visionscience.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-02-15 22:40:33.000000 psychopy-visionscience-0.0.5/psychopy_visionscience.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-15 22:40:33.000000 psychopy-visionscience-0.0.5/psychopy_visionscience.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-02-15 22:40:22.000000 psychopy-visionscience-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-15 22:40:33.473853 psychopy-visionscience-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.211149 psychopy_visionscience-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-31 15:19:55.211149 psychopy_visionscience-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.203149 psychopy_visionscience-0.0.6/docs_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/docs_src/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/docs_src/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.199149 psychopy_visionscience-0.0.6/docs_src/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.199149 psychopy_visionscience-0.0.6/docs_src/themes/psychopy_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.203149 psychopy_visionscience-0.0.6/docs_src/themes/psychopy_plugin/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    65201 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/docs_src/themes/psychopy_plugin/static/Nottingham Supported.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22964 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Large.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9576 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/docs_src/themes/psychopy_plugin/static/Psychopy Plugin Header Small.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.203149 psychopy_visionscience-0.0.6/psychopy_visionscience/
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.207149 psychopy_visionscience-0.0.6/psychopy_visionscience/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.207149 psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/
+-rw-r--r--   0 runner    (1001) docker     (127)    15272 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.207149 psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/classic/
+-rw-r--r--   0 runner    (1001) docker     (127)     8930 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/classic/envelope_grating@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/classic/envelopegrating.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.207149 psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/dark/
+-rw-r--r--   0 runner    (1001) docker     (127)     3149 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/dark/envelopegrating.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7137 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/dark/envelopegrating@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.207149 psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/light/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/light/envelopegrating.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/light/envelopegrating@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.207149 psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/
+-rw-r--r--   0 runner    (1001) docker     (127)    20944 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.207149 psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/classic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2881 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/classic/noise.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/classic/noise@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.207149 psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/dark/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/dark/noise.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/dark/noise@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.207149 psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/light/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/light/noise.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/light/noise@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.207149 psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/
+-rw-r--r--   0 runner    (1001) docker     (127)     7792 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.211149 psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/classic/
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/classic/radial.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/classic/radial@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.211149 psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/dark/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/dark/radial.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/dark/radial@2x.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.211149 psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/light/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/light/radial.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/light/radial@2x.png
+-rw-r--r--   0 runner    (1001) docker     (127)    36172 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21731 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/radial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26773 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/psychopy_visionscience/secondorder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.211149 psychopy_visionscience-0.0.6/psychopy_visionscience.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-31 15:19:55.000000 psychopy_visionscience-0.0.6/psychopy_visionscience.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-05-31 15:19:55.000000 psychopy_visionscience-0.0.6/psychopy_visionscience.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:19:55.000000 psychopy_visionscience-0.0.6/psychopy_visionscience.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-31 15:19:55.000000 psychopy_visionscience-0.0.6/psychopy_visionscience.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-31 15:19:55.000000 psychopy_visionscience-0.0.6/psychopy_visionscience.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-31 15:19:55.000000 psychopy_visionscience-0.0.6/psychopy_visionscience.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-31 15:19:55.211149 psychopy_visionscience-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.211149 psychopy_visionscience-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.211149 psychopy_visionscience-0.0.6/tests/test_builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/tests/test_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/tests/test_builder/test_EnvGratingComponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/tests/test_builder/test_NoiseComponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/tests/test_builder/test_RadialStimComponent.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:55.211149 psychopy_visionscience-0.0.6/tests/test_coder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/tests/test_coder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15427 2024-05-31 15:19:46.000000 psychopy_visionscience-0.0.6/tests/test_coder/test_all_stimuli.py
```

### Comparing `psychopy-visionscience-0.0.5/LICENSE` & `psychopy_visionscience-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/PKG-INFO` & `psychopy_visionscience-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 Metadata-Version: 2.1
 Name: psychopy-visionscience
-Version: 0.0.5
+Version: 0.0.6
 Summary: Stimuli useful for vision scientists.
 Author-email: Jon Peirce <jon@opensceincetools.org>, Matthew Cutone <mcutone@opensceincetools.org>
 License: GNU General Public License v3 (GPLv3)
-Project-URL: homepage, https://github.com/mdcutone/psychopy-visionscience
-Project-URL: changelog, https://github.com/mdcutone/psychopy-visionscience/blob/main/CHANGELOG.txt
-Project-URL: documentation, https://pages.github.com/psychopy/psychopy-visionscience
+Project-URL: homepage, https://psychopy.github.io/psychopy-visionscience
+Project-URL: changelog, https://github.com/psychopy/psychopy-visionscience/blob/main/CHANGELOG.txt
+Project-URL: documentation, https://psychopy.github.io/psychopy-visionscience
 Project-URL: repository, https://github.com/psychopy/psychopy-visionscience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: docs
+Requires-Dist: psychopy; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: furo; extra == "docs"
+Provides-Extra: tests
+Requires-Dist: psychopy; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
 
 # psychopy-visionscience
 
 Plugin package for PsychoPy which adds stimuli useful for vision science.
 
 ## Features
```

### Comparing `psychopy-visionscience-0.0.5/README.md` & `psychopy_visionscience-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/__init__.py` & `psychopy_visionscience-0.0.6/psychopy_visionscience/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,15 +5,20 @@
 # Copyright (C) 2002-2018 Jonathan Peirce (C) 2019-2022 Open Science Tools Ltd.
 # Distributed under the terms of the GNU General Public License (GPL).
 
 """Various visual stimuli classes and Builder components useful to vision
 scientists.
 """
 
-__version__ = '0.0.5'
+import importlib.metadata
+
+try:
+    __version__ = importlib.metadata.version("psychopy-visionscience")
+except importlib.metadata.PackageNotFoundError:
+    __version__ = "0.dev"
 
 # NOTE: Be sure to register entry points in the `pyproject.toml` file.
 
 # ------------------------------------------------------------------------------
 # Library Classes
 #
 from .noise import NoiseStim
```

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/__init__.py` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/__init__.py`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/classic/envelope_grating@2x.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/classic/envelope_grating@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/classic/envelopegrating.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/classic/envelopegrating.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/dark/envelopegrating.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/dark/envelopegrating.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/dark/envelopegrating@2x.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/dark/envelopegrating@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/light/envelopegrating.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/light/envelopegrating.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/envelopegrating/light/envelopegrating@2x.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/envelopegrating/light/envelopegrating@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/__init__.py` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/__init__.py`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/classic/noise.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/classic/noise.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/classic/noise@2x.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/classic/noise@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/dark/noise.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/dark/noise.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/dark/noise@2x.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/dark/noise@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/light/noise.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/light/noise.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/noise/light/noise@2x.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/noise/light/noise@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/__init__.py` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,49 +75,49 @@
             updates='constant',
             allowedUpdates=['constant', 'set every repeat', 'set every frame'],
             hint=msg,
             label=_translate("Mask"))
 
         msg = _translate("Number of texture cycles from centre to periphery, i.e. it controls the number of ‘rings’.")
         self.params['radialCycles'] = Param(
-            radialCycles, valType='num', inputType="single", allowedTypes=[], categ='Texture',
+            radialCycles, valType="code", inputType="single", allowedTypes=[], categ='Texture',
             updates='constant',
             allowedUpdates=['constant', 'set every repeat', 'set every frame'],
             hint=msg,
             label=_translate("Radial Cycles"))
 
         msg = _translate("Number of cycles going around the stimulus. i.e. it controls the number of ‘spokes’.")
         self.params['angularCycles'] = Param(
-            angularCycles, valType='num', inputType="single", allowedTypes=[], categ='Texture',
+            angularCycles, valType="code", inputType="single", allowedTypes=[], categ='Texture',
             updates='constant',
             allowedUpdates=['constant', 'set every repeat', 'set every frame'],
             hint=msg,
             label=_translate("Angular Cycles"))
 
         msg = _translate("This is the phase of the texture from the centre to the perimeter of the stimulus"
                          " (in radians). Can be used to drift concentric rings out/inwards.")
         self.params['radialPhase'] = Param(
-            radialPhase, valType='num', inputType="single", allowedTypes=[], categ='Texture',
+            radialPhase, valType="code", inputType="single", allowedTypes=[], categ='Texture',
             updates='constant',
             allowedUpdates=['constant', 'set every repeat', 'set every frame'],
             hint=msg,
             label=_translate("Radial Phase"))
 
         msg = _translate("This is akin to setting the orientation of the texture around the stimulus in radians."
                          " If possible, it is more efficient to rotate the stimulus using its ori setting instead.")
         self.params['angularPhase'] = Param(
-            angularPhase, valType='num', inputType="single", allowedTypes=[], categ='Texture',
+            angularPhase, valType="code", inputType="single", allowedTypes=[], categ='Texture',
             updates='constant',
             allowedUpdates=['constant', 'set every repeat', 'set every frame'],
             hint=msg,
             label=_translate("Angular Phase"))
 
         msg = _translate("Determines visible range.")
         self.params['visibleWedge'] = Param(
-            visibleWedge, valType='num', inputType="single", allowedTypes=[], categ='Texture',
+            visibleWedge, valType="code", inputType="single", allowedTypes=[], categ='Texture',
             updates='constant',
             allowedUpdates=['constant', 'set every repeat', 'set every frame'],
             hint=msg,
             label=_translate("Visible Wedge"))
 
         msg = _translate("How should the image be interpolated if/when "
                          "rescaled")
@@ -128,15 +128,15 @@
             label=_translate("Interpolate"))
 
         msg = _translate(
             "Resolution of the texture for standard ones such as sin, sqr "
             "etc. For most cases a value of 256 pixels will suffice")
         self.params['texture resolution'] = Param(
             texRes,
-            valType='num', inputType="choice", allowedVals=['32', '64', '128', '256', '512'], categ='Texture',
+            valType="code", inputType="choice", allowedVals=['32', '64', '128', '256', '512'], categ='Texture',
             updates='constant', allowedUpdates=[],
             hint=msg,
             label=_translate("Texture resolution"))
 
         del self.params['fillColor']
         del self.params['borderColor']
```

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/classic/radial.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/classic/radial.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/classic/radial@2x.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/classic/radial@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/dark/radial.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/dark/radial.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/dark/radial@2x.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/dark/radial@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/light/radial.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/light/radial.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/components/radial/light/radial@2x.png` & `psychopy_visionscience-0.0.6/psychopy_visionscience/components/radial/light/radial@2x.png`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/noise.py` & `psychopy_visionscience-0.0.6/psychopy_visionscience/noise.py`

 * *Files 1% similar despite different names*

```diff
@@ -399,14 +399,17 @@
             above whenever a filter is applied to the noise sample, 
             regardless of the initial type of noise requested. 
         """
         
         self.__dict__['noiseClip'] = value
         self._needUpdate = True
         self._needBuild = True
+    
+    def setNoiseOri(self, value):
+        self.noiseOri = value
 
     @attributeSetter
     def filter(self, value):
         """If True apply spatial frequency filter to noise."""
         
         self.__dict__['filter'] = value
         self._needUpdate = True
```

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/radial.py` & `psychopy_visionscience-0.0.6/psychopy_visionscience/radial.py`

 * *Files identical despite different names*

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/secondorder.py` & `psychopy_visionscience-0.0.6/psychopy_visionscience/secondorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,16 +67,17 @@
     }
     '''
 
 
 class EnvelopeGrating(GratingStim):
     """Second-order envelope stimuli with 3 textures; a carrier, an envelope and a mask
 
-    **Examples**::
+    **Examples**
 
+    
     env1 = EnvelopeGrating(win,ori=0, carrier='sin', envelope='sin',
             mask = 'gauss', sf=24, envsf=4, size=1, contrast=0.5,
             moddepth=1.0, envori=0, pos=[-.5,.5],interpolate=0)
             # gives a circular patch of high frequency carrier with a
             # low frequency envelope
     env2 = EnvelopeGrating(win,ori=0, carrier=noise, envelope='sin',
             mask = None, sf=1, envsf=4, size=1, contrast=0.5,
@@ -86,14 +87,15 @@
     env4 = EnvelopeGrating(win,ori=90, carrier='sin', envelope='sin',
             mask = 'gauss', sf=24, envsf=4, size=1, contrast=0.5,
             moddepth=1.0, envori=0, pos=[.5,.5], beat=True, interpolate=0)
             # Setting beat will create a second order beat stimulus which
             # critically contains no net energy at the carrier frequency
             # even though it appears to be present. In this case carrier
             # and envelope are at 90 degree to each other
+    
 
     With an EnvelopeStim the carrier and envelope can have different spatial
     frequencies, phases and orientations. Its position can be shifted as a whole.
 
     contrast controls the contrast of the carrier and moddepth the modulation
     depth of the envelope. contrast and moddepth must work together, for moddepth=1 the max carrier
     contrast is 0.5 otherwise the displayable range will be exceeded. If moddepth < 1 higher contrasts can be accommodated.
```

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience/tests/test_visual/test_all_stimuli.py` & `psychopy_visionscience-0.0.6/tests/test_coder/test_all_stimuli.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,93 +3,102 @@
 
 from psychopy import visual, monitors, prefs, constants
 from psychopy.visual import filters
 from psychopy.tools.coordinatetools import pol2cart
 from psychopy.tests import utils
 from psychopy.tests import skip_under_vm, requires_plugin
 from psychopy.tools import systemtools
+from psychopy_visionscience import secondorder, noise, radial
 import numpy
 import pytest
 import shutil
 from tempfile import mkdtemp
 
 """Each test class creates a context subclasses _baseVisualTest to run a series
 of tests on a single graphics context (e.g. pyglet with shaders)
 
 To add a new stimulus test use _base so that it gets tested in all contexts
 
 """
 
-from psychopy.tests.test_visual.test_all_stimuli import _baseVisualTest
 
+class _TestPluginVisualStim:
+    @classmethod
+    def setup_class(self):#run once for each test class (window)
+        self.win=None
+        self.contextName
+        raise NotImplementedError
+
+    @classmethod
+    def teardown_class(self):#run once for each test class (window)
+        self.win.close()#shutil.rmtree(self.temp_dir)
 
-class TestPluginVisualStim(_baseVisualTest):
+    def setup_method(self):#this is run for each test individually
+        #make sure we start with a clean window
+        self.win.flip()
 
-    @requires_plugin("psychopy-visionscience")
     def test_envelopeGratingAndRaisedCos(self):
         win = self.win
         size = numpy.array([2.0, 2.0]) * self.scaleFactor
         if win.units in ['norm', 'height']:
             sf = 5
         else:
             sf = 5.0 / size  # this will do the flipping and get exactly one cycle
         if win._haveShaders == True:  # can't draw envelope gratings without shaders so skip this test
-            image = visual.EnvelopeGrating(win, carrier='sin', envelope='sin',
+            image = secondorder.EnvelopeGrating(win, carrier='sin', envelope='sin',
                                            size=size, sf=sf, mask='raisedCos',
                                            ori=-45, envsf=sf / 2, envori=45,
                                            envphase=90, moddepth=0.5,
                                            contrast=0.5)
             image.draw()
             utils.compareScreenshot('envelopeandrcos_%s.png' % (self.contextName), win)
             win.flip()
             "{}".format(image)
 
-    @requires_plugin("psychopy-visionscience")
     def test_envelopeGratingPowerAndRaisedCos(self):
         win = self.win
         size = numpy.array([2.0, 2.0]) * self.scaleFactor
         if win.units in ['norm', 'height']:
             sf = 5
         else:
             sf = 5.0 / size  # this will do the flipping and get exactly one cycle
         if win._haveShaders == True:  # can't draw envelope gratings without shaders so skip this test
-            image = visual.EnvelopeGrating(win, carrier='sin', envelope='sin',
+            image = secondorder.EnvelopeGrating(win, carrier='sin', envelope='sin',
                                            size=size, sf=sf, mask='raisedCos',
                                            ori=-45, envsf=sf / 2, envori=45,
                                            envphase=90, moddepth=0.5, power=0.5,
                                            contrast=0.5)
             image.draw()
             utils.compareScreenshot('envelopepowerandrcos_%s.png' % (self.contextName), win)
             win.flip()
             "{}".format(image)
 
-    @requires_plugin("psychopy-visionscience")
     def test_NoiseStim_defaults(self):
         noiseTypes = ['binary', 'uniform', 'normal', 'white', 'filtered']
 
         for noiseType in noiseTypes:
-            stim = visual.NoiseStim(win=self.win,
-                                    noiseType=noiseType,
-                                    size=(32, 32),
-                                    units='pix')
+            stim = noise.NoiseStim(
+                win=self.win,
+                noiseType=noiseType,
+                size=(32, 32),
+                units='pix'
+            )
             stim.updateNoise()
             stim.draw()
 
-    @requires_plugin("psychopy-visionscience")
     def test_NoiseStim_defaults_image(self):
         noiseType = 'image'
 
         # noiseImage kwarg missing.
         with pytest.raises(ValueError):
-            visual.NoiseStim(win=self.win,
+            noise.NoiseStim(win=self.win,
                              noiseType=noiseType,
                              size=(32, 32),
                              units='pix')
 
-    @requires_plugin("psychopy-visionscience")
     def test_noiseAndRaisedCos(self):
         numpy.random.seed(1)
         win = self.win
         size = numpy.array([2.0, 2.0]) * self.scaleFactor
         tres = 128
         elementsize = 4
         sf = None
@@ -113,15 +122,15 @@
             if self.contextName == 'stencil':
                 ntype = 'White'
             elif self.contextName == 'height':
                 ntype = 'Uniform'
             else:
                 ntype = 'Normal'
             elementsize = 1.0 / 8.0
-        image = visual.NoiseStim(win=win, name='noise', units=win.units,
+        image = noise.NoiseStim(win=win, name='noise', units=win.units,
                                  noiseImage=fileName, mask='raisedCos',
                                  ori=0, pos=(0, 0), size=size, sf=sf, phase=0,
                                  color=[1, 1, 1], colorSpace='rgb', opacity=1, blendmode='avg',
                                  contrast=0.5,
                                  texRes=tres,
                                  noiseType=ntype, noiseElementSize=elementsize,
                                  noiseBaseSf=32.0 / size[0],
@@ -129,15 +138,14 @@
                                  noiseFilterLower=4.0 / size[0], noiseFilterUpper=16.0 / size[0],
                                  noiseFilterOrder=1, noiseClip=4.0, interpolate=False, depth=-1.0)
         image.draw()
         utils.compareScreenshot('noiseAndRcos_%s.png' % (self.contextName), win)
         win.flip()
         str(image)
 
-    @requires_plugin("psychopy-visionscience")
     def test_noiseFiltersAndRaisedCos(self):
         numpy.random.seed(1)
         win = self.win
         size = numpy.array([2.0, 2.0]) * self.scaleFactor
         tres = 128
         elementsize = 4
         sf = None
@@ -171,15 +179,15 @@
             elif self.contextName == 'height':
                 ntype = 'Uniform'
                 ftype = 'Butterworth'
             else:
                 ntype = 'Normal'
                 ftype = 'Butterworth'
             elementsize = 1.0 / 8.0
-        image = visual.NoiseStim(win=win, name='noise', units=win.units,
+        image = noise.NoiseStim(win=win, name='noise', units=win.units,
                                  noiseImage=fileName, mask='raisedCos',
                                  ori=0, pos=(0, 0), size=size, sf=sf, phase=0,
                                  color=[1, 1, 1], colorSpace='rgb', opacity=1, blendmode='avg',
                                  contrast=0.5,
                                  texRes=tres,
                                  noiseType=ntype, noiseElementSize=elementsize,
                                  noiseBaseSf=32.0 / size[0],
@@ -190,149 +198,178 @@
                                  interpolate=False, depth=-1.0)
 
         image.draw()
         utils.compareScreenshot('noiseFiltersAndRcos_%s.png' % (self.contextName), win)
         win.flip()
         str(image)
 
-    @requires_plugin("psychopy-visionscience")
     def test_envelopeBeatAndRaisedCos(self):
         win = self.win
         size = numpy.array([2.0, 2.0]) * self.scaleFactor
         if win.units in ['norm', 'height']:
             sf = 5
         else:
             sf = 5.0 / size  # this will do the flipping and get exactly one cycle
         if win._haveShaders == True:  # can't draw envelope gratings without shaders so skip this test
-            image = visual.EnvelopeGrating(win, carrier='sin', envelope='sin',
+            image = secondorder.EnvelopeGrating(win, carrier='sin', envelope='sin',
                                            size=size, sf=sf, mask='raisedCos',
                                            ori=-45, envsf=sf / 2, envori=45,
                                            envphase=90, beat=True, moddepth=0.5,
                                            contrast=0.5)
             image.draw()
             utils.compareScreenshot('beatandrcos_%s.png' % (self.contextName), win)
             win.flip()
             "{}".format(image)
 
+    def test_radial(self):
+        win = self.win
+        #using init
+        wedge = radial.RadialStim(win, tex='sqrXsqr', color=1, size=2* self.scaleFactor,
+            visibleWedge=[0, 45], radialCycles=2, angularCycles=2, interpolate=False)
+        wedge.draw()
+        thresh = 15  # there are often a slight interpolation differences
+        if win.winType != 'pygame':  # pygame definitely gets radialstim wrong!
+            utils.compareScreenshot('wedge1_%s.png' %(self.contextName),
+                                    win, crit=thresh)
+        win.flip()#AFTER compare screenshot
+
+        #using .set()
+        wedge.mask = 'gauss'
+        wedge.size = 3 * self.scaleFactor
+        wedge.angularCycles = 3
+        wedge.radialCycles = 3
+        wedge.ori = 180
+        wedge.contrast = 0.8
+        wedge.opacity = 0.8
+        wedge.radialPhase += 0.1
+        wedge.angularPhase = 0.1
+        wedge.draw()
+        "{}".format(wedge) #check that str(xxx) is working
+        if win.winType != 'pygame': # pygame gets this wrong:
+            utils.compareScreenshot('wedge2_%s.png' %(self.contextName),
+                                    win, crit=thresh)
+        else:
+            pytest.skip("Pygame fails to render RadialStim properly :-/")
+
 # variants of the base tests with different backends (copied from psychopy)
 
-class TestPygletNorm(TestPluginVisualStim):
+class TestPygletNorm(_TestPluginVisualStim):
     @classmethod
     def setup_class(self):
         self.win = visual.Window([128, 128], winType='pyglet', pos=[50, 50],
                                  allowStencil=True, autoLog=False)
         self.contextName = 'norm'
         self.scaleFactor = 1  # applied to size/pos values
 
 
-class TestPygletHexColor(TestPluginVisualStim):
+class TestPygletHexColor(_TestPluginVisualStim):
     @classmethod
     def setup_class(self):
         self.win = visual.Window([128, 128], winType='pyglet', pos=[50, 50],
                                  color="#FF0099",
                                  allowStencil=True, autoLog=False)
         self.contextName = 'normHexbackground'
         self.scaleFactor = 1  # applied to size/pos values
 
 
 if not systemtools.isVM_CI():
-    class TestPygletBlendAdd(TestPluginVisualStim):
+    class TestPygletBlendAdd(_TestPluginVisualStim):
         @classmethod
         def setup_class(self):
             self.win = visual.Window([128, 128], winType='pyglet', pos=[50, 50],
                                      blendMode='add', useFBO=True)
             self.contextName = 'normAddBlend'
             self.scaleFactor = 1  # applied to size/pos values
 
 
-class TestPygletNormFBO(TestPluginVisualStim):
+class TestPygletNormFBO(_TestPluginVisualStim):
     @classmethod
     def setup_class(self):
         self.win = visual.Window([128, 128], units="norm", winType='pyglet', pos=[50, 50],
                                  allowStencil=True, autoLog=False, useFBO=True)
         self.contextName = 'norm'
         self.scaleFactor = 1  # applied to size/pos values
 
 
-class TestPygletHeight(TestPluginVisualStim):
+class TestPygletHeight(_TestPluginVisualStim):
     @classmethod
     def setup_class(self):
         self.win = visual.Window([128, 64], units="height", winType='pyglet', pos=[50, 50],
                                  allowStencil=False, autoLog=False)
         self.contextName = 'height'
         self.scaleFactor = 1  # applied to size/pos values
 
 
-class TestPygletNormStencil(TestPluginVisualStim):
+class TestPygletNormStencil(_TestPluginVisualStim):
     @classmethod
     def setup_class(self):
         self.win = visual.Window([128, 128], units="norm", monitor='testMonitor',
                                  winType='pyglet', pos=[50, 50],
                                  allowStencil=True, autoLog=False)
         self.contextName = 'stencil'
         self.scaleFactor = 1  # applied to size/pos values
 
 
-class TestPygletPix(TestPluginVisualStim):
+class TestPygletPix(_TestPluginVisualStim):
     @classmethod
     def setup_class(self):
         mon = monitors.Monitor('testMonitor')
         mon.setDistance(57)
         mon.setWidth(40.0)
         mon.setSizePix([1024, 768])
         self.win = visual.Window([128, 128], units="pix", monitor=mon,
                                  winType='pyglet', pos=[50, 50],
                                  allowStencil=True, autoLog=False)
         self.contextName = 'pix'
         self.scaleFactor = 60  # applied to size/pos values
 
 
-class TestPygletCm(TestPluginVisualStim):
+class TestPygletCm(_TestPluginVisualStim):
     @classmethod
     def setup_class(self):
         mon = monitors.Monitor('testMonitor')
         mon.setDistance(57.0)
         mon.setWidth(40.0)
         mon.setSizePix([1024, 768])
         self.win = visual.Window([128, 128], units="cm", monitor=mon,
                                  winType='pyglet', pos=[50, 50],
                                  allowStencil=False, autoLog=False)
         self.contextName = 'cm'
         self.scaleFactor = 2  # applied to size/pos values
 
 
-class TestPygletDeg(TestPluginVisualStim):
+class TestPygletDeg(_TestPluginVisualStim):
     @classmethod
     def setup_class(self):
         mon = monitors.Monitor('testMonitor')
         mon.setDistance(57.0)
         mon.setWidth(40.0)
         mon.setSizePix([1024, 768])
         self.win = visual.Window([128, 128], units="deg", monitor=mon,
                                  winType='pyglet', pos=[50, 50], allowStencil=True,
                                  autoLog=False)
         self.contextName = 'deg'
         self.scaleFactor = 2  # applied to size/pos values
 
 
-class TestPygletDegFlat(TestPluginVisualStim):
+class TestPygletDegFlat(_TestPluginVisualStim):
     @classmethod
     def setup_class(self):
         mon = monitors.Monitor('testMonitor')
         mon.setDistance(10.0)  # exaggerate the effect of flatness by setting the monitor close
         mon.setWidth(40.0)
         mon.setSizePix([1024, 768])
         self.win = visual.Window([128, 128], units="degFlat", monitor=mon,
                                  winType='pyglet', pos=[50, 50],
                                  allowStencil=True, autoLog=False)
         self.contextName = 'degFlat'
         self.scaleFactor = 4  # applied to size/pos values
 
 
-class TestPygletDegFlatPos(TestPluginVisualStim):
+class TestPygletDegFlatPos(_TestPluginVisualStim):
     @classmethod
     def setup_class(self):
         mon = monitors.Monitor('testMonitor')
         mon.setDistance(10.0)  # exaggerate the effect of flatness by setting the monitor close
         mon.setWidth(40.0)
         mon.setSizePix([1024, 768])
         self.win = visual.Window([128, 128], units='degFlatPos', monitor=mon,
```

### Comparing `psychopy-visionscience-0.0.5/psychopy_visionscience.egg-info/PKG-INFO` & `psychopy_visionscience-0.0.6/psychopy_visionscience.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 Metadata-Version: 2.1
 Name: psychopy-visionscience
-Version: 0.0.5
+Version: 0.0.6
 Summary: Stimuli useful for vision scientists.
 Author-email: Jon Peirce <jon@opensceincetools.org>, Matthew Cutone <mcutone@opensceincetools.org>
 License: GNU General Public License v3 (GPLv3)
-Project-URL: homepage, https://github.com/mdcutone/psychopy-visionscience
-Project-URL: changelog, https://github.com/mdcutone/psychopy-visionscience/blob/main/CHANGELOG.txt
-Project-URL: documentation, https://pages.github.com/psychopy/psychopy-visionscience
+Project-URL: homepage, https://psychopy.github.io/psychopy-visionscience
+Project-URL: changelog, https://github.com/psychopy/psychopy-visionscience/blob/main/CHANGELOG.txt
+Project-URL: documentation, https://psychopy.github.io/psychopy-visionscience
 Project-URL: repository, https://github.com/psychopy/psychopy-visionscience
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Provides-Extra: docs
+Requires-Dist: psychopy; extra == "docs"
+Requires-Dist: sphinx; extra == "docs"
+Requires-Dist: furo; extra == "docs"
+Provides-Extra: tests
+Requires-Dist: psychopy; extra == "tests"
+Requires-Dist: pytest; extra == "tests"
 
 # psychopy-visionscience
 
 Plugin package for PsychoPy which adds stimuli useful for vision science.
 
 ## Features
```

### Comparing `psychopy-visionscience-0.0.5/pyproject.toml` & `psychopy_visionscience-0.0.6/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.8.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "psychopy-visionscience"
-version = "0.0.5"
+version = "0.0.6"
 description = "Stimuli useful for vision scientists."
 readme = "README.md"
 requires-python = ">= 3.7"
 license = { text = "GNU General Public License v3 (GPLv3)" }
 authors = [
   { name = "Jon Peirce", email = "jon@opensceincetools.org" },
   { name = "Matthew Cutone", email = "mcutone@opensceincetools.org" },
@@ -20,24 +20,39 @@
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
 ]
-urls.homepage = "https://github.com/mdcutone/psychopy-visionscience"
-urls.changelog = "https://github.com/mdcutone/psychopy-visionscience/blob/main/CHANGELOG.txt"
-urls.documentation = "https://pages.github.com/psychopy/psychopy-visionscience"
+urls.homepage = "https://psychopy.github.io/psychopy-visionscience"
+urls.changelog = "https://github.com/psychopy/psychopy-visionscience/blob/main/CHANGELOG.txt"
+urls.documentation = "https://psychopy.github.io/psychopy-visionscience"
 urls.repository = "https://github.com/psychopy/psychopy-visionscience"
-dependencies = [
+
+[project.optional-dependencies]
+# dependencies for building the docs
+docs = [
+  "psychopy",
+  "sphinx",
+  "furo",
+]
+tests = [
+  "psychopy",
+  "pytest",
 ]
 
 [tool.setuptools.packages.find]
 where = ["", "psychopy_visionscience",]
 
 [tool.setuptools.package-data]
 "*" = ["*.png",]
 
 [project.entry-points."psychopy.experiment.components"]
 NoiseStimComponent = "psychopy_visionscience:NoiseStimComponent"
 EnvGratingComponent = "psychopy_visionscience:EnvGratingComponent"
-RadialStimComponent = "psychopy_visionscience:RadialStimComponent"
+RadialStimComponent = "psychopy_visionscience:RadialStimComponent"
+
+[project.entry-points."psychopy.visual"]
+NoiseStim = "psychopy_visionscience.noise:NoiseStim"
+RadialStim = "psychopy_visionscience.radial:RadialStim"
+EnvelopeGrating = "psychopy_visionscience.secondorder:EnvelopeGrating"
```

