# Comparing `tmp/Spinmob-3.5.8.tar.gz` & `tmp/Spinmob-3.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Spinmob-3.5.8.tar", last modified: Thu Oct 15 21:29:53 2020, max compression
+gzip compressed data, was "dist/Spinmob-3.5.9.tar", last modified: Thu Jan 14 20:52:13 2021, max compression
```

## Comparing `Spinmob-3.5.8.tar` & `Spinmob-3.5.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2020-10-15 21:29:53.000000 Spinmob-3.5.8/
--rw-rw-r--   0 jack      (1000) jack      (1000)      290 2020-10-15 21:29:53.000000 Spinmob-3.5.8/PKG-INFO
--rw-rw-r--   0 jack      (1000) jack      (1000)      217 2020-07-13 18:23:03.000000 Spinmob-3.5.8/README.rst
--rw-rw-r--   0 jack      (1000) jack      (1000)     3152 2020-10-03 20:35:44.000000 Spinmob-3.5.8/__init__.py
--rwxrwxr-x   0 jack      (1000) jack      (1000)   114832 2020-10-08 17:15:48.000000 Spinmob-3.5.8/_data.py
--rw-rw-r--   0 jack      (1000) jack      (1000)   122760 2020-09-08 22:14:36.000000 Spinmob-3.5.8/_data_old.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     6181 2020-08-03 17:39:55.000000 Spinmob-3.5.8/_dialogs.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    55671 2020-09-09 13:50:08.000000 Spinmob-3.5.8/_functions.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      378 2020-07-13 18:23:03.000000 Spinmob-3.5.8/_plot.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      207 2020-07-13 18:23:03.000000 Spinmob-3.5.8/_plot_complex.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      159 2020-07-13 18:23:03.000000 Spinmob-3.5.8/_plot_image.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      229 2020-07-13 18:23:03.000000 Spinmob-3.5.8/_plot_magphase.py
--rw-rw-r--   0 jack      (1000) jack      (1000)       75 2020-07-13 18:23:03.000000 Spinmob-3.5.8/_plot_parametric.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      212 2020-07-13 18:23:03.000000 Spinmob-3.5.8/_plot_realimag.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      187 2020-07-13 18:23:03.000000 Spinmob-3.5.8/_plot_xy.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      601 2020-07-13 18:23:03.000000 Spinmob-3.5.8/_plotting.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    40481 2020-07-31 17:53:53.000000 Spinmob-3.5.8/_plotting_mess.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     3581 2020-07-13 18:23:03.000000 Spinmob-3.5.8/_prefs.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    18278 2020-07-27 17:14:19.000000 Spinmob-3.5.8/_pylab_colormap.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    61900 2020-08-01 01:51:11.000000 Spinmob-3.5.8/_pylab_tweaks.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     5629 2020-10-03 20:35:44.000000 Spinmob-3.5.8/_settings.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    22410 2020-07-13 18:23:03.000000 Spinmob-3.5.8/_spline.py
--rwxrwxr-x   0 jack      (1000) jack      (1000)     1736 2020-08-01 02:35:27.000000 Spinmob-3.5.8/_theme_fusion_dark.py
--rwxrwxr-x   0 jack      (1000) jack      (1000)     5241 2020-08-19 15:21:44.000000 Spinmob-3.5.8/_thread.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2020-10-15 21:29:53.000000 Spinmob-3.5.8/egg/
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2020-10-15 21:29:53.000000 Spinmob-3.5.8/egg/DataboxProcessor/
--rw-rw-r--   0 jack      (1000) jack      (1000)     1034 2020-07-27 17:14:19.000000 Spinmob-3.5.8/egg/DataboxProcessor/histogram_plot_script.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      402 2020-08-18 13:00:15.000000 Spinmob-3.5.8/egg/__init__.py
--rw-rw-r--   0 jack      (1000) jack      (1000)   180738 2020-10-08 18:00:57.000000 Spinmob-3.5.8/egg/_gui.py
--rwxrwxr-x   0 jack      (1000) jack      (1000)     8913 2020-07-31 18:08:56.000000 Spinmob-3.5.8/egg/_syntax.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     5112 2020-07-13 18:23:03.000000 Spinmob-3.5.8/egg/example_daq.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1802 2020-07-13 18:23:03.000000 Spinmob-3.5.8/egg/example_from_wiki.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1593 2020-07-13 18:23:03.000000 Spinmob-3.5.8/egg/example_from_wiki_2.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     7700 2020-07-13 18:23:03.000000 Spinmob-3.5.8/egg/example_other_widgets.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      518 2020-07-13 18:23:03.000000 Spinmob-3.5.8/egg/example_really_basic.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     1528 2020-07-27 17:14:19.000000 Spinmob-3.5.8/egg/example_sliders.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     4795 2020-07-29 14:41:24.000000 Spinmob-3.5.8/egg/example_sweeper.py
--rwxrwxr-x   0 jack      (1000) jack      (1000)     1534 2020-07-30 14:29:22.000000 Spinmob-3.5.8/lm_fitter_concept.py
--rwxrwxr-x   0 jack      (1000) jack      (1000)     2066 2020-07-30 15:27:57.000000 Spinmob-3.5.8/lm_fitter_test.py
--rw-rw-r--   0 jack      (1000) jack      (1000)      926 2020-10-15 20:41:06.000000 Spinmob-3.5.8/setup.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2020-10-15 21:29:53.000000 Spinmob-3.5.8/tests/
--rw-rw-r--   0 jack      (1000) jack      (1000)        0 2020-07-31 20:09:49.000000 Spinmob-3.5.8/tests/__init__.py
-drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2020-10-15 21:29:53.000000 Spinmob-3.5.8/tests/fixtures/
--rw-rw-r--   0 jack      (1000) jack      (1000)      311 2020-07-13 18:23:03.000000 Spinmob-3.5.8/tests/fixtures/basic.dat
--rw-rw-r--   0 jack      (1000) jack      (1000)      311 2020-07-13 18:23:03.000000 Spinmob-3.5.8/tests/fixtures/basic2.dat
--rw-rw-r--   0 jack      (1000) jack      (1000)      311 2020-07-13 18:23:03.000000 Spinmob-3.5.8/tests/fixtures/basic3.dat
--rw-rw-r--   0 jack      (1000) jack      (1000)      335 2020-07-13 18:23:03.000000 Spinmob-3.5.8/tests/fixtures/comma.dat
--rw-rw-r--   0 jack      (1000) jack      (1000)    12523 2020-07-13 18:23:03.000000 Spinmob-3.5.8/tests/fixtures/difficult.binary
--rw-rw-r--   0 jack      (1000) jack      (1000)      277 2020-07-13 18:23:03.000000 Spinmob-3.5.8/tests/fixtures/fit.csv
--rw-rw-r--   0 jack      (1000) jack      (1000)     6844 2020-07-13 18:23:03.000000 Spinmob-3.5.8/tests/fixtures/float16.binary
--rw-rw-r--   0 jack      (1000) jack      (1000)      343 2020-07-13 18:23:03.000000 Spinmob-3.5.8/tests/fixtures/headers.dat
--rw-rw-r--   0 jack      (1000) jack      (1000)       71 2020-07-13 18:23:03.000000 Spinmob-3.5.8/tests/fixtures/mixed_complex.dat
--rw-rw-r--   0 jack      (1000) jack      (1000)       13 2020-07-13 18:23:03.000000 Spinmob-3.5.8/tests/fixtures/one_column.dat
--rw-rw-r--   0 jack      (1000) jack      (1000)       22 2020-07-13 18:23:03.000000 Spinmob-3.5.8/tests/fixtures/one_row.dat
--rw-rw-r--   0 jack      (1000) jack      (1000)      336 2020-07-13 18:23:03.000000 Spinmob-3.5.8/tests/fixtures/semicolon.dat
--rw-rw-r--   0 jack      (1000) jack      (1000)      338 2020-07-31 19:35:58.000000 Spinmob-3.5.8/tests/spinmob_tests.py
--rw-rw-r--   0 jack      (1000) jack      (1000)    16097 2020-09-09 14:43:11.000000 Spinmob-3.5.8/tests/test__databox.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     2027 2020-07-13 18:23:03.000000 Spinmob-3.5.8/tests/test__dialogs.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     6981 2020-08-27 16:00:55.000000 Spinmob-3.5.8/tests/test__egg.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     7361 2020-09-08 23:04:52.000000 Spinmob-3.5.8/tests/test__fitter.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     9562 2020-07-30 15:00:14.000000 Spinmob-3.5.8/tests/test__functions.py
--rw-rw-r--   0 jack      (1000) jack      (1000)     2360 2020-08-03 15:44:14.000000 Spinmob-3.5.8/tests/test__plot.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2021-01-14 20:52:13.000000 Spinmob-3.5.9/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      290 2021-01-14 20:52:13.000000 Spinmob-3.5.9/PKG-INFO
+-rw-rw-r--   0 jack      (1000) jack      (1000)      217 2020-07-13 18:23:03.000000 Spinmob-3.5.9/README.rst
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3152 2020-10-03 20:35:44.000000 Spinmob-3.5.9/__init__.py
+-rwxrwxr-x   0 jack      (1000) jack      (1000)   114849 2021-01-14 20:50:15.000000 Spinmob-3.5.9/_data.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)   122760 2020-09-08 22:14:36.000000 Spinmob-3.5.9/_data_old.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     6181 2020-08-03 17:39:55.000000 Spinmob-3.5.9/_dialogs.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    55671 2020-09-09 13:50:08.000000 Spinmob-3.5.9/_functions.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      378 2020-07-13 18:23:03.000000 Spinmob-3.5.9/_plot.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      207 2020-07-13 18:23:03.000000 Spinmob-3.5.9/_plot_complex.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      159 2020-07-13 18:23:03.000000 Spinmob-3.5.9/_plot_image.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      229 2020-07-13 18:23:03.000000 Spinmob-3.5.9/_plot_magphase.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)       75 2020-07-13 18:23:03.000000 Spinmob-3.5.9/_plot_parametric.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      212 2020-07-13 18:23:03.000000 Spinmob-3.5.9/_plot_realimag.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      187 2020-07-13 18:23:03.000000 Spinmob-3.5.9/_plot_xy.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      601 2020-07-13 18:23:03.000000 Spinmob-3.5.9/_plotting.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    40481 2020-07-31 17:53:53.000000 Spinmob-3.5.9/_plotting_mess.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     3581 2020-07-13 18:23:03.000000 Spinmob-3.5.9/_prefs.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    18278 2020-07-27 17:14:19.000000 Spinmob-3.5.9/_pylab_colormap.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    61900 2020-08-01 01:51:11.000000 Spinmob-3.5.9/_pylab_tweaks.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5629 2020-10-03 20:35:44.000000 Spinmob-3.5.9/_settings.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    22410 2020-07-13 18:23:03.000000 Spinmob-3.5.9/_spline.py
+-rwxrwxr-x   0 jack      (1000) jack      (1000)     1736 2020-08-01 02:35:27.000000 Spinmob-3.5.9/_theme_fusion_dark.py
+-rwxrwxr-x   0 jack      (1000) jack      (1000)     5241 2020-08-19 15:21:44.000000 Spinmob-3.5.9/_thread.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2021-01-14 20:52:13.000000 Spinmob-3.5.9/egg/
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2021-01-14 20:52:13.000000 Spinmob-3.5.9/egg/DataboxProcessor/
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1034 2020-07-27 17:14:19.000000 Spinmob-3.5.9/egg/DataboxProcessor/histogram_plot_script.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      402 2020-08-18 13:00:15.000000 Spinmob-3.5.9/egg/__init__.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)   183692 2020-11-26 20:05:46.000000 Spinmob-3.5.9/egg/_gui.py
+-rwxrwxr-x   0 jack      (1000) jack      (1000)     8913 2020-07-31 18:08:56.000000 Spinmob-3.5.9/egg/_syntax.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     5112 2020-07-13 18:23:03.000000 Spinmob-3.5.9/egg/example_daq.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1802 2020-07-13 18:23:03.000000 Spinmob-3.5.9/egg/example_from_wiki.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1593 2020-07-13 18:23:03.000000 Spinmob-3.5.9/egg/example_from_wiki_2.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     7700 2020-07-13 18:23:03.000000 Spinmob-3.5.9/egg/example_other_widgets.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      518 2020-07-13 18:23:03.000000 Spinmob-3.5.9/egg/example_really_basic.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     1528 2020-07-27 17:14:19.000000 Spinmob-3.5.9/egg/example_sliders.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     4795 2020-07-29 14:41:24.000000 Spinmob-3.5.9/egg/example_sweeper.py
+-rwxrwxr-x   0 jack      (1000) jack      (1000)     1534 2020-07-30 14:29:22.000000 Spinmob-3.5.9/lm_fitter_concept.py
+-rwxrwxr-x   0 jack      (1000) jack      (1000)     2066 2020-07-30 15:27:57.000000 Spinmob-3.5.9/lm_fitter_test.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)      926 2021-01-14 20:52:03.000000 Spinmob-3.5.9/setup.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2021-01-14 20:52:13.000000 Spinmob-3.5.9/tests/
+-rw-rw-r--   0 jack      (1000) jack      (1000)        0 2020-07-31 20:09:49.000000 Spinmob-3.5.9/tests/__init__.py
+drwxrwxr-x   0 jack      (1000) jack      (1000)        0 2021-01-14 20:52:13.000000 Spinmob-3.5.9/tests/fixtures/
+-rw-rw-r--   0 jack      (1000) jack      (1000)      311 2020-07-13 18:23:03.000000 Spinmob-3.5.9/tests/fixtures/basic.dat
+-rw-rw-r--   0 jack      (1000) jack      (1000)      311 2020-07-13 18:23:03.000000 Spinmob-3.5.9/tests/fixtures/basic2.dat
+-rw-rw-r--   0 jack      (1000) jack      (1000)      311 2020-07-13 18:23:03.000000 Spinmob-3.5.9/tests/fixtures/basic3.dat
+-rw-rw-r--   0 jack      (1000) jack      (1000)      335 2020-07-13 18:23:03.000000 Spinmob-3.5.9/tests/fixtures/comma.dat
+-rw-rw-r--   0 jack      (1000) jack      (1000)    12523 2020-07-13 18:23:03.000000 Spinmob-3.5.9/tests/fixtures/difficult.binary
+-rw-rw-r--   0 jack      (1000) jack      (1000)      277 2020-07-13 18:23:03.000000 Spinmob-3.5.9/tests/fixtures/fit.csv
+-rw-rw-r--   0 jack      (1000) jack      (1000)     6844 2020-07-13 18:23:03.000000 Spinmob-3.5.9/tests/fixtures/float16.binary
+-rw-rw-r--   0 jack      (1000) jack      (1000)      343 2020-07-13 18:23:03.000000 Spinmob-3.5.9/tests/fixtures/headers.dat
+-rw-rw-r--   0 jack      (1000) jack      (1000)       71 2020-07-13 18:23:03.000000 Spinmob-3.5.9/tests/fixtures/mixed_complex.dat
+-rw-rw-r--   0 jack      (1000) jack      (1000)       13 2020-07-13 18:23:03.000000 Spinmob-3.5.9/tests/fixtures/one_column.dat
+-rw-rw-r--   0 jack      (1000) jack      (1000)       22 2020-07-13 18:23:03.000000 Spinmob-3.5.9/tests/fixtures/one_row.dat
+-rw-rw-r--   0 jack      (1000) jack      (1000)      336 2020-07-13 18:23:03.000000 Spinmob-3.5.9/tests/fixtures/semicolon.dat
+-rw-rw-r--   0 jack      (1000) jack      (1000)      338 2020-07-31 19:35:58.000000 Spinmob-3.5.9/tests/spinmob_tests.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)    16097 2020-09-09 14:43:11.000000 Spinmob-3.5.9/tests/test__databox.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     2027 2020-07-13 18:23:03.000000 Spinmob-3.5.9/tests/test__dialogs.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     6981 2020-08-27 16:00:55.000000 Spinmob-3.5.9/tests/test__egg.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     7361 2020-09-08 23:04:52.000000 Spinmob-3.5.9/tests/test__fitter.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     9562 2020-07-30 15:00:14.000000 Spinmob-3.5.9/tests/test__functions.py
+-rw-rw-r--   0 jack      (1000) jack      (1000)     2360 2020-08-03 15:44:14.000000 Spinmob-3.5.9/tests/test__plot.py
```

### Comparing `Spinmob-3.5.8/__init__.py` & `Spinmob-3.5.9/__init__.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/_data.py` & `Spinmob-3.5.9/_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,15 +263,15 @@
 
 
         # If we're not in binary mode, we can read all the lines and find
         # the delimiter as usual. (In binary mode, the delimiter is specified)
         if not 'SPINMOB_BINARY' in self.hkeys:
 
             # For non-binary files, we always read all the lines.
-            f = open(path, 'r')
+            f = open(path, 'r', errors='ignore')
             lines = f.readlines()
             f.close()
 
             # Determine the delimiter
             if self.delimiter is None:
 
                 # loop from the end of the file until we get something other than white space
```

### Comparing `Spinmob-3.5.8/_data_old.py` & `Spinmob-3.5.9/_data_old.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/_dialogs.py` & `Spinmob-3.5.9/_dialogs.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/_functions.py` & `Spinmob-3.5.9/_functions.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/_plotting.py` & `Spinmob-3.5.9/_plotting.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/_plotting_mess.py` & `Spinmob-3.5.9/_plotting_mess.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/_prefs.py` & `Spinmob-3.5.9/_prefs.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/_pylab_colormap.py` & `Spinmob-3.5.9/_pylab_colormap.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/_pylab_tweaks.py` & `Spinmob-3.5.9/_pylab_tweaks.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/_settings.py` & `Spinmob-3.5.9/_settings.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/_spline.py` & `Spinmob-3.5.9/_spline.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/_theme_fusion_dark.py` & `Spinmob-3.5.9/_theme_fusion_dark.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/_thread.py` & `Spinmob-3.5.9/_thread.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/egg/DataboxProcessor/histogram_plot_script.py` & `Spinmob-3.5.9/egg/DataboxProcessor/histogram_plot_script.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/egg/_gui.py` & `Spinmob-3.5.9/egg/_gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     """
     Base object containing stuff common to all of our objects. When
     deriving objects from this, call BaseObject.__init__(self) as the
     LAST step of the new __init__ function.
     """
 
     log = None
+    _alignment_default = 1 # If alignment is not overridden, use this.
 
     def __init__(self, autosettings_path=None):
         if not _s._pyqtgraph_ok: raise Exception('Cannot create egg GUIs without pyqtgraph v0.11.0 or higher.')
 
         # Parent object (to be set)
         self._parent = None
 
@@ -456,30 +457,34 @@
 
     def __init__(self, margins=True, scroll=False, autosettings_path=None):
         """
         This creates a grid layout that can contain other Elements
         (including other grid and docked layouts)
         """
         BaseObject.__init__(self, autosettings_path=autosettings_path)
+        #self._alignment_default = 0 # Default grids fill space.
 
         # Qt widget to house the layout
         self._widget = _pg.Qt.QtGui.QWidget()
+        
+        # Resize event
+        self._widget.resizeEvent = self._event_resize 
 
         # Qt layout object
         self._layout = _pg.Qt.QtGui.QGridLayout()
 
         # stick the layout into the widget
         self._widget.setLayout(self._layout)
 
         # auto-add row and column
         self._auto_row      = 0
         self._auto_column   = 0
 
-        # 2D list of objects
-        self.objects    = []
+        # list of objects
+        self.objects = []
 
         # other useful functions to wrap
         self.get_row_count    = self._layout.rowCount
         self.get_column_count = self._layout.columnCount
 
         # Set the margins
         self.set_margins(margins)
@@ -487,27 +492,63 @@
         # Expose the show and hide functions
         # The attr check ensures classes inheriting this object's methods
         # don't have their show's and hide's overwritten
         if not hasattr(self, 'show'): self.show = self._widget.show
         if not hasattr(self, 'hide'): self.hide = self._widget.hide
 
 
+    def _event_resize(self, *a):
+        """
+        Called when it resizes.
+        """
+        # print(self)
+        # # Recursively loop over all sub-objects and call their resizers.
+        # for o in self.objects:
+        #     if type(o) == GridLayout:
+        #         o._event_resize()
+        
+        # Now call this one's customized resizer.
+        self.event_resize()
+
+    def event_resize(self):
+        """
+        Dummy function you can overload when the grid is resized.
+        """
+        return
 
     def __getitem__(self, n): return self.objects[n]
 
-    def place_object(self, object, column=None, row=None, column_span=1, row_span=1, alignment=1):
+    def place_object(self, object, column=None, row=None, column_span=1, row_span=1, alignment=None):
         """
-        This adds either one of our simplified objects or a QWidget to the
+        This adds an egg object or a QWidget to the
         grid at the specified position, appends the object to self.objects.
 
-        alignment=0     Fill the space.
-        alignment=1     Left-justified.
-        alignment=2     Right-justified.
-
-        If column isn't specified, the new object will be placed in a new column.
+        Parameters
+        ----------
+        object : egg or QWidget
+            Supply a spinmob egg object or QWidget to place on the grid.
+        
+        column=None, row=None : None or integer
+            Where to place the object on the grid, starting at 0,0 in the upper left.
+            If column isn't specified, the new object will be placed in a new column
+            (i.e., you can add objects like words in a sentence; see also
+            self.new_autorow()).
+
+        column_span=1, row_span=1 : integer
+            How many columns or rows the object should span. See also
+            self.set_column_stretch() and self.set_row_stretch().
+        
+        alignment=None : None, 0, 1, or 2
+            How to align the object. If None is supplied, this uses the default
+            value for the object in question. Otherwise, 0 means "fill space",
+            1 means "left justified", 2 means "right justified".
+      
+        Returns
+        -------
+        self
         """
 
         # pick a column
         if column==None:
             column = self._auto_column
             self._auto_column += 1
 
@@ -521,14 +562,15 @@
         try:
             object._widget
             widget = object._widget
 
         # allows the user to specify a standard widget
         except: widget = object
 
+        if alignment==None: alignment = object._alignment_default
         self._layout.addWidget(widget, row, column,
                                row_span, column_span,
                                _pg.Qt.QtCore.Qt.Alignment(alignment))
 
         # try to store the parent object (self) in the placed object
         try:    object.set_parent(self)
         except: None
@@ -659,14 +701,15 @@
 
     def __init__(self, title='Window', size=[700,500], autosettings_path=None,
                  margins=True, event_close=None):
         self._parent = self
 
         # initialize the grid layout
         GridLayout.__init__(self, margins=margins)
+        self._alignment_default = 0 # By default, fills space.
 
         # create the QtMainWindow,
         self._window = _pg.Qt.QtGui.QMainWindow()
         self.set_size(size)
         self.set_title(title)
 
         #Set some docking options
@@ -1895,18 +1938,19 @@
 
         # tab widget
         self._widget = _pg.Qt.QtGui.QTabWidget()
         self._widget.setTabsClosable(True)
 
         # Other stuff common to all objects
         BaseObject.__init__(self)
+        self._alignment_default = 0 # By default, tabs fill all space.
 
         # tab widgets by index
         self.docked_tabs = []
-        self.all_tabs    = []
+        self.objects    = []
         self.popped_tabs = {}
 
         # signals
         self.signal_switched             = self._widget.currentChanged
         self.signal_tab_close_requested  = self._widget.tabCloseRequested
 
         # connect signals
@@ -1928,27 +1972,27 @@
         if signal_switched: self.signal_switched.connect(signal_switched)
         if signal_tab_close_requested: self.signal_tab_close_requested.connect(signal_tab_close_requested)
 
     def get_total_tab_count(self):
         """
         Returns the total tab count (integer).
         """
-        return len(self.all_tabs)
+        return len(self.objects)
 
     def _tab_closed(self, *a):
         """
         Pops it out.
         """
         # This is the index of the requested closed tab. Pop it out
         self.pop_tab(a[0])
 
 
     def _tab_changed(self, *a): self.save_gui_settings()
 
-    def __getitem__(self, n): return self.all_tabs[n]
+    def __getitem__(self, n): return self.objects[n]
 
     def add_tab(self, title="Yeah!", margins=True, block_signals=True, **kwargs):
         """
         Adds a tab to the area, and creates the layout for this tab.
 
         Parameters
         ----------
@@ -1970,15 +2014,15 @@
 
         # create a widget to go in the tab
         tab = GridLayout(margins=margins)
         tab.set_parent(self)
         tab.title = title
 
         # Remember this tab.
-        self.all_tabs.append(tab)
+        self.objects.append(tab)
 
         # create and append the tab to the list
         # Note this makes _widget no longer able to be added to a QGridLayout
         # for some unknown reason. This is why we nest the grids
         self._widget.addTab(tab._widget, title)
 
         # Remember the unique tab id (total tab index)
@@ -2421,15 +2465,15 @@
     """
 
     def __init__(self):
         self._widget = _pg.QtGui.QTextEdit()
 
         # Other stuff common to all objects
         BaseObject.__init__(self)
-
+        
         # Expose the show and hide functions
         self.show = self._widget.show
         self.hide = self._widget.hide
 
 
     def get_text(self):
         """
@@ -3849,35 +3893,39 @@
                  name=None, show_logger=False, styles=[], **kwargs):
 
         self.name = name
 
         # Do all the parent class initialization; this sets _widget and _layout
         GridLayout.__init__(self, margins=False)
         _d.databox.__init__(self, **kwargs)
+        self._alignment_default = 0 # By default, fill all space.
 
         # top row is main controls
         self.grid_controls   = self.place_object(GridLayout(margins=False), alignment=0)
-        #self.grid_controls.place_object(Label("Raw Data:"), alignment=1)
-        self.button_clear    = self.grid_controls.place_object(Button("Clear", tip='Clear all header and columns.').set_width(40), alignment=1)
-        self.button_load     = self.grid_controls.place_object(Button("Load",  tip='Load data from file.')         .set_width(40), alignment=1)
-        self.button_save     = self.grid_controls.place_object(Button("Save",  tip='Save data to file.')           .set_width(40), alignment=1)
-        self.combo_binary    = self.grid_controls.place_object(ComboBox(['Text', 'float16', 'float32', 'float64', 'int8', 'int16', 'int32', 'int64', 'complex64', 'complex128', 'complex256'], tip='Format of output file columns.'), alignment=1)
-        self.button_autosave = self.grid_controls.place_object(Button("Auto",   checkable=True, tip='Enable autosaving. Note this will only autosave when self.autosave() is called in the host program.').set_width(40), alignment=1)
-        self.number_file     = self.grid_controls.place_object(NumberBox(int=True, bounds=(0,None), tip='Current autosave file name prefix number. This will increment every autosave().'))
-        self.label_path      = self.grid_controls.place_object(Label(""))
-
-        self.grid_controls.place_object(Label("")) # spacer
-        self.button_script     = self.grid_controls.place_object(Button  ("Script",      checkable=True, checked=True, tip='Show the script box.').set_width(50)).set_checked(False)
-        self.combo_autoscript  = self.grid_controls.place_object(ComboBox(['Edit', 'x=d[0]', 'Pairs', 'Triples', 'x=d[0], ey', 'x=None', 'User'], tip='Script mode. Select "Edit" to modify the script.')).set_value(autoscript)
-        self.button_multi      = self.grid_controls.place_object(Button  ("Multi",       checkable=True, tip="If checked, plot with multiple plots. If unchecked, all data on the same plot.").set_width(40)).set_checked(True)
-        self.button_link_x     = self.grid_controls.place_object(Button  ("Link",        checkable=True, tip="Link the x-axes of all plots.").set_width(40)).set_checked(autoscript==1)
-        self.button_enabled    = self.grid_controls.place_object(Button  ("Enable",      checkable=True, tip="Enable this plot.").set_width(50)).set_checked(True)
+        self.grid_controls.event_resize = self._event_resize_databox_plot
 
-        # keep the buttons shaclackied together
-        self.grid_controls.set_column_stretch(7)
+        self.grid_controls1  = self.grid_controls.place_object(GridLayout(margins=False), 0,0, alignment=1)
+
+        self.button_clear    = self.grid_controls1.place_object(Button("Clear", tip='Clear all header and columns.').set_width(40), alignment=1)
+        self.button_load     = self.grid_controls1.place_object(Button("Load",  tip='Load data from file.')         .set_width(40), alignment=1)
+        self.button_save     = self.grid_controls1.place_object(Button("Save",  tip='Save data to file.')           .set_width(40), alignment=1)
+        self.combo_binary    = self.grid_controls1.place_object(ComboBox(['Text', 'float16', 'float32', 'float64', 'int8', 'int16', 'int32', 'int64', 'complex64', 'complex128', 'complex256'], tip='Format of output file columns.'), alignment=1)
+        self.button_autosave = self.grid_controls1.place_object(Button("Auto",   checkable=True, tip='Enable autosaving. Note this will only autosave when self.autosave() is called in the host program.').set_width(40), alignment=1)
+        self.number_file     = self.grid_controls1.place_object(NumberBox(int=True, bounds=(0,None), tip='Current autosave file name prefix number. This will increment every autosave().'))
+        
+        self.label_path      = self.grid_controls.place_object(Label(""), 1,0)
+
+        self.grid_controls2 = self.grid_controls.place_object(GridLayout(margins=False), 0,1, alignment=1)
+        self.grid_controls.set_column_stretch(2)
+
+        self.button_script     = self.grid_controls2.place_object(Button  ("Script",      checkable=True, checked=True, tip='Show the script box.').set_width(50)).set_checked(False)
+        self.combo_autoscript  = self.grid_controls2.place_object(ComboBox(['Edit', 'x=d[0]', 'Pairs', 'Triples', 'x=d[0], ey', 'x=None', 'User'], tip='Script mode. Select "Edit" to modify the script.')).set_value(autoscript)
+        self.button_multi      = self.grid_controls2.place_object(Button  ("Multi",       checkable=True, tip="If checked, plot with multiple plots. If unchecked, all data on the same plot.").set_width(40)).set_checked(True)
+        self.button_link_x     = self.grid_controls2.place_object(Button  ("Link",        checkable=True, tip="Link the x-axes of all plots.").set_width(40)).set_checked(autoscript==1)
+        self.button_enabled    = self.grid_controls2.place_object(Button  ("Enable",      checkable=True, tip="Enable this plot.").set_width(50)).set_checked(True)
 
         # second rows is the script
         self.new_autorow()
 
         # grid for the script
         self.grid_script = self.place_object(GridLayout(margins=False), 0,1, alignment=0)
 
@@ -4014,14 +4062,22 @@
                                        "self.number_history",
                                        "self.text_log_note", ]
 
         # load settings if a settings file exists and initialize
         self.load_gui_settings()
         self._synchronize_controls()
 
+    def _event_resize_databox_plot(self):
+        """
+        Called when the widget resizes.
+        """
+        # If we're below a certain width, move the right controls below
+        # if self.grid_controls._widget.width() < 700: self.grid_controls.place_object(self.grid_controls2, 0,1, alignment=1)
+        # else:                                        self.grid_controls.place_object(self.grid_controls2, 2,0, alignment=2)
+        
     def _button_log_data_toggled(self, *a):
         """
         Called when someone toggles the dump button. Ask for a path or remove the path.
         """
         if self.button_log_data.is_checked():
             path = _s.dialogs.save(self.file_type, 'Dump incoming data to this file.', force_extension=self.file_type)
 
@@ -4263,40 +4319,57 @@
 
         # save the file using the skeleton function, so as not to recursively
         # call this one again!
         _d.databox.save_file(d, path, self.file_type, self.file_type, force_overwrite, **kwargs)
 
         return self
 
-    def load_file(self, path=None, just_settings=False):
+    def load_file(self, path=None, just_settings=False, just_data=False):
         """
         Loads a data file. After the file is loaded, calls self.after_load_file(self),
         which you can overwrite if you like!
 
-        just_settings=True will only load the configuration of the controls,
-        and will not plot anything or run after_load_file
+        Parameters
+        ----------
+        path=None
+            Optional path. If not specified, pops up a dialog.
+        
+        just_settings=False
+            Load only the settings, not the data
+        
+        just_data=False
+            Load only the data, not the settings.
+
+        Returns
+        -------
+        self
         """
         # if it's just the settings file, make a new databox
         if just_settings:
             d = _d.databox()
             header_only = True
 
         # otherwise use the internal databox
         else:
             d = self
             header_only = False
 
+        # Load the file
+        result = _d.databox.load_file(d, path, filters=self.file_type, header_only=header_only, quiet=just_settings)
+
         # import the settings if they exist in the header
-        if not None == _d.databox.load_file(d, path, filters=self.file_type, header_only=header_only, quiet=just_settings):
+        if not just_data:
 
-            # loop over the autosettings and update the gui
-            for x in self._autosettings_controls: self._load_gui_setting(x,d)
-
-        # always sync the internal data
-        self._synchronize_controls()
+            if not None == result:
+    
+                # loop over the autosettings and update the gui
+                for x in self._autosettings_controls: self._load_gui_setting(x,d)
+    
+            # always sync the internal data
+            self._synchronize_controls()
 
         # plot the data if this isn't just a settings load
         if not just_settings:
             self.plot()
             self.after_load_file()
 
 
@@ -4495,17 +4568,21 @@
             # Make sure these are iterable lists
             if not type(xlabels) in [tuple,list]: xlabels = [xlabels]
             if not type(ylabels) in [tuple,list]: ylabels = [ylabels]
 
             xlabels = list(xlabels)
             ylabels = list(ylabels)
 
-            # Adjust the length
-            while len(xlabels) < len(x): xlabels.append(xlabels[-1])
-            while len(ylabels) < len(y): ylabels.append(ylabels[-1])
+            # Increase the length to match
+            while len(xlabels) < len(x): xlabels.append('')
+            while len(ylabels) < len(y): ylabels.append('')
+
+            # Decrease the label length to match
+            while len(xlabels) > len(x): xlabels.pop(-1)
+            while len(ylabels) > len(y): ylabels.pop(-1)
 
             # Get the styles
             self._styles = g['styles']
 
             # make sure we have exactly the right number of plots
             self._set_number_of_plots(y, ey)
             self._update_linked_axes()
@@ -4780,14 +4857,15 @@
         Margins around the window's inside edges. Can be True, False, or a 4-length tuple.
     """
 
     def __init__(self, name='processor', databox_source=None, file_type='*.dp', margins=False):
 
         # Run the window init
         Window.__init__(self, 'Databox Processor', autosettings_path=name+'.window', margins=margins)
+        self._alignment_default = 0 # By default, fill all space.
 
         # Store variables and create the window.
         self.name        = name
         self._clear_dump = False
         self.t0          = _t.time()
 
         # Remembers when user edits it
@@ -4815,15 +4893,15 @@
 
         # Add the PSD settings
         self.settings.add_parameter('Enabled',      False, tip='Enable or disable all analyses below.')
         self.settings.add_parameter('Coarsen',          0, bounds=(0,None), tip='Break the data into groups of this many, and average each group into a single data point. 0 to disable.')
 
         self.settings.add_parameter('PSD',          False, tip='Calculate the power spectral density')
         self.settings.add_parameter('PSD/pow2',     False, tip='Truncate the data into the nearest 2^N data points, to speed up the PSD.')
-        self.settings.add_parameter('PSD/Window',  'None', values=['hanning', 'None'], tip='Apply this windowing function to the time domain prior to PSD.')
+        self.settings.add_parameter('PSD/Window',       1, values=['hanning', 'None'], default_list_index=1, tip='Apply this windowing function to the time domain prior to PSD.')
         self.settings.add_parameter('PSD/Rescale',  False, tip='Whether to rescale the PSD after windowing so that the integrated value is the RMS in the time-domain.')
         self.settings.add_parameter('PSD/Coarsen',      0, bounds=(0,None), tip='Break the PSD data into groups of this many, and average each group into a single data point. 0 to disable.')
 
         self.settings.add_parameter('Histogram',    False, tip='Perform a histogram on the data.')
         self.settings.add_parameter('Histogram/Bins', 100, bounds=(2,None), tip='How many bins to use for the histogram.')
 
         self.settings.add_parameter('Average',      False, tip='Calculate a running average of the data.')
@@ -5301,17 +5379,21 @@
 
 
 
 
 if __name__ == '__main__':
     import spinmob
     #runfile(spinmob.__path__[0] + '/tests/test__egg.py')
-
-    self = DataboxPlot(autosettings_path='pants')
-    self.show()
+    
+    w = Window()
+    ts = w.add(TabArea())
+    t = ts.add('test')
+    p = t.add(DataboxPlot())
+    
+    w.show()
```

### Comparing `Spinmob-3.5.8/egg/_syntax.py` & `Spinmob-3.5.9/egg/_syntax.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/egg/example_daq.py` & `Spinmob-3.5.9/egg/example_daq.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/egg/example_from_wiki.py` & `Spinmob-3.5.9/egg/example_from_wiki.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/egg/example_from_wiki_2.py` & `Spinmob-3.5.9/egg/example_from_wiki_2.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/egg/example_other_widgets.py` & `Spinmob-3.5.9/egg/example_other_widgets.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/egg/example_really_basic.py` & `Spinmob-3.5.9/egg/example_really_basic.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/egg/example_sliders.py` & `Spinmob-3.5.9/egg/example_sliders.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/egg/example_sweeper.py` & `Spinmob-3.5.9/egg/example_sweeper.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/lm_fitter_concept.py` & `Spinmob-3.5.9/lm_fitter_concept.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/lm_fitter_test.py` & `Spinmob-3.5.9/lm_fitter_test.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/setup.py` & `Spinmob-3.5.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '3.5.8' # Keep this on the first line so it's easy for __init__.py to grab.
+__version__ = '3.5.9' # Keep this on the first line so it's easy for __init__.py to grab.
 
 
 
 from distutils.core import setup
 setup(name           = 'Spinmob',
       version        = __version__,
       description    = 'Data handling, plotting, analysis, and GUI building for scientific labs',
```

### Comparing `Spinmob-3.5.8/tests/fixtures/difficult.binary` & `Spinmob-3.5.9/tests/fixtures/difficult.binary`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/tests/fixtures/float16.binary` & `Spinmob-3.5.9/tests/fixtures/float16.binary`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/tests/test__databox.py` & `Spinmob-3.5.9/tests/test__databox.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/tests/test__dialogs.py` & `Spinmob-3.5.9/tests/test__dialogs.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/tests/test__egg.py` & `Spinmob-3.5.9/tests/test__egg.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/tests/test__fitter.py` & `Spinmob-3.5.9/tests/test__fitter.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/tests/test__functions.py` & `Spinmob-3.5.9/tests/test__functions.py`

 * *Files identical despite different names*

### Comparing `Spinmob-3.5.8/tests/test__plot.py` & `Spinmob-3.5.9/tests/test__plot.py`

 * *Files identical despite different names*

