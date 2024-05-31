# Comparing `tmp/etm-dgraham-6.2.7.tar.gz` & `tmp/etm-dgraham-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-6.2.7.tar", last modified: Wed May 22 19:24:26 2024, max compression
+gzip compressed data, was "etm-dgraham-6.3.0.tar", last modified: Fri May 31 12:30:19 2024, max compression
```

## Comparing `etm-dgraham-6.2.7.tar` & `etm-dgraham-6.3.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-22 19:24:26.326642 etm-dgraham-6.2.7/
--rw-r--r--   0 dag        (501) staff       (20)     5315 2024-05-22 19:24:22.000000 etm-dgraham-6.2.7/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.2.7/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   146147 2024-05-22 19:24:26.326381 etm-dgraham-6.2.7/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   144578 2024-05-07 12:58:43.000000 etm-dgraham-6.2.7/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.2.7/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     4516 2024-04-24 18:26:45.000000 etm-dgraham-6.2.7/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-22 19:24:26.319160 etm-dgraham-6.2.7/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.2.7/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.2.7/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.2.7/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-22 19:24:26.322100 etm-dgraham-6.2.7/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.2.7/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    15262 2024-05-04 14:12:33.000000 etm-dgraham-6.2.7/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-05-22 19:24:22.000000 etm-dgraham-6.2.7/etm/__version__.py
--rw-r--r--   0 dag        (501) staff       (20)    26965 2024-05-18 16:18:38.000000 etm-dgraham-6.2.7/etm/common.py
--rwxr-xr-x   0 dag        (501) staff       (20)    29368 2024-04-24 18:26:45.000000 etm-dgraham-6.2.7/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)     9528 2024-04-24 18:26:45.000000 etm-dgraham-6.2.7/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   326500 2024-05-22 19:24:22.000000 etm-dgraham-6.2.7/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    38924 2024-05-06 14:19:59.000000 etm-dgraham-6.2.7/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    27887 2024-05-04 14:12:33.000000 etm-dgraham-6.2.7/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)   126420 2024-05-22 19:11:28.000000 etm-dgraham-6.2.7/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-22 19:24:26.324447 etm-dgraham-6.2.7/etm_dgraham.egg-info/
--rw-r--r--   0 dag        (501) staff       (20)   146147 2024-05-22 19:24:26.000000 etm-dgraham-6.2.7/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.2.7/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.2.7/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      882 2024-05-22 19:24:26.000000 etm-dgraham-6.2.7/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-05-22 19:24:26.000000 etm-dgraham-6.2.7/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-05-22 19:24:26.000000 etm-dgraham-6.2.7/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.2.7/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-05-22 19:24:26.000000 etm-dgraham-6.2.7/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.2.7/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-05-22 19:24:26.000000 etm-dgraham-6.2.7/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.2.7/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.2.7/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.2.7/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.2.7/namedcolors.py
--rw-r--r--   0 dag        (501) staff       (20)   448972 2024-05-06 20:30:20.000000 etm-dgraham-6.2.7/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.2.7/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2024-05-22 19:24:26.326710 etm-dgraham-6.2.7/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.2.7/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-22 19:24:26.324602 etm-dgraham-6.2.7/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.2.7/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-22 19:24:26.325801 etm-dgraham-6.2.7/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.2.7/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2024-04-28 16:49:51.000000 etm-dgraham-6.2.7/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.2.7/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.2.7/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-31 12:30:19.632781 etm-dgraham-6.3.0/
+-rw-r--r--   0 dag        (501) staff       (20)     5351 2024-05-31 12:30:12.000000 etm-dgraham-6.3.0/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.3.0/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   146330 2024-05-31 12:30:19.632408 etm-dgraham-6.3.0/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   144761 2024-05-31 12:30:12.000000 etm-dgraham-6.3.0/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.3.0/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     4516 2024-04-24 18:26:45.000000 etm-dgraham-6.3.0/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-31 12:30:19.624845 etm-dgraham-6.3.0/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.3.0/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.3.0/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.3.0/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-31 12:30:19.628239 etm-dgraham-6.3.0/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.3.0/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    15262 2024-05-23 14:53:47.000000 etm-dgraham-6.3.0/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-05-31 12:30:12.000000 etm-dgraham-6.3.0/etm/__version__.py
+-rw-r--r--   0 dag        (501) staff       (20)    27073 2024-05-31 12:30:12.000000 etm-dgraham-6.3.0/etm/common.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    29418 2024-05-31 12:30:12.000000 etm-dgraham-6.3.0/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     9528 2024-04-24 18:26:45.000000 etm-dgraham-6.3.0/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   338742 2024-05-31 12:30:12.000000 etm-dgraham-6.3.0/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    38924 2024-05-06 14:19:59.000000 etm-dgraham-6.3.0/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    27887 2024-05-04 14:12:33.000000 etm-dgraham-6.3.0/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     1512 2024-05-30 19:08:07.000000 etm-dgraham-6.3.0/etm/rrule-test.py
+-rw-r--r--   0 dag        (501) staff       (20)     1284 2024-05-30 10:36:15.000000 etm-dgraham-6.3.0/etm/rruleset-test.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   126430 2024-05-31 12:30:12.000000 etm-dgraham-6.3.0/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-31 12:30:19.630507 etm-dgraham-6.3.0/etm_dgraham.egg-info/
+-rw-r--r--   0 dag        (501) staff       (20)   146330 2024-05-31 12:30:19.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      921 2024-05-31 12:30:19.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-05-31 12:30:19.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-05-31 12:30:19.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-05-31 12:30:19.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-05-31 12:30:19.000000 etm-dgraham-6.3.0/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.3.0/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.3.0/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.3.0/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.3.0/namedcolors.py
+-rw-r--r--   0 dag        (501) staff       (20)   448972 2024-05-06 20:30:20.000000 etm-dgraham-6.3.0/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.3.0/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2024-05-31 12:30:19.632826 etm-dgraham-6.3.0/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.3.0/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-31 12:30:19.630639 etm-dgraham-6.3.0/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.3.0/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-31 12:30:19.631893 etm-dgraham-6.3.0/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.3.0/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2024-04-28 16:49:51.000000 etm-dgraham-6.3.0/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.3.0/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.3.0/utilities/open_in_mutt
```

### Comparing `etm-dgraham-6.2.7/CHANGES.txt` & `etm-dgraham-6.3.0/CHANGES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,44 @@
-2024-05-22 69a3954 Daniel Graham
+2024-05-31 3cfe871 Daniel Graham
+    Tagged version 6.3.0. Added goal period options for year, quarter
+    and month. Added caching for non-weekly views. Fixed timezone
+    issues associated with the transistions between daylight saving
+    and standard time.
+
+2024-05-31 98f34e5 Daniel Graham
+    Fixed timezone issues associated with daylight/standard time
+    transitions. Flag instances falling within transition.
+
+2024-05-29 45a2a9e Daniel Graham
+    Replaced zoneinto ZoneInfo with dateutil tz gettz - seems to fix
+    daylight savings to standard time problem.
+
+2024-05-29 511a4c1 Daniel Graham
+    typo
+
+2024-05-29 7a044c7 Daniel Graham
+    goal tweaks
+
+2024-05-29 7263136 Daniel Graham
+    Message tweak
+
+2024-05-29 04add19 Daniel Graham
+    Goal category tweaks
+
+2024-05-28 367b3e1 Daniel Graham
+    Use 'w' as default quota period for compatibility with previous
+    version. Formatting tweaks for goals.
+
+2024-05-27 61bf526 Daniel Graham
+    Added year, quarter and month to periods supported by goals.
+
+2024-05-25 92dce3e Daniel Graham
+    Clean up - caches for cacheds views work
+
+2024-05-22 331f590 Daniel Graham
     Tagged version 6.2.7.
 
 2024-05-22 25c994b Daniel Graham
     Fixed date vs datetime bug
 
 2024-05-22 84dce1d Daniel Graham
     Tagged version 6.2.6.
@@ -158,42 +194,7 @@
     active/paused and to end goal.
 
 2024-05-01 41242dd Daniel Graham
     Changed binding for goto link from g to G
 
 2024-05-01 f1c68f0 Daniel Graham
     Corrected typo
-
-2024-05-01 de6647c Daniel Graham
-    Merged working isocalendar fix
-
-2024-05-01 af63365 Daniel Graham
-    Tagged version 6.1.26.
-
-2024-05-01 e9c92ac Daniel Graham
-    Fixed bug in converting (year, week number, weekday number) dates
-    to (year, month, monthday).
-
-2024-05-01 83b2926 Daniel Graham
-    First pass at displaying goal history.
-
-2024-04-30 c513048 Daniel Graham
-    Added itemtype ~ for goal. Set allowed and required and
-    implemented formatting and processing for @q and @h. Displays on
-    current day similar to inbox items and pressing F increments the
-    ticker for done. Still to do - display in completions.
-
-2024-04-28 3458834 Daniel Graham
-    First pass at implementing goals.
-
-2024-04-27 909b86d Daniel Graham
-    Beginning work on weekly goals
-
-2024-04-26 5f1a37a Daniel Graham
-    Tagged version 6.1.25.
-
-2024-04-26 9e3f1c3 Daniel Graham
-    Changed the default for settings.update_command to use pipx if etm
-    was installed using pipx and, otherwise, to use pip.
-
-2024-04-24 25c29af Daniel Graham
-    Tagged version 6.1.24.
```

### Comparing `etm-dgraham-6.2.7/PKG-INFO` & `etm-dgraham-6.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.2.7
+Version: 6.3.0
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -637,15 +637,15 @@
 In the main window, active goals are sorted by their done/quota ratios and given a color indicating the degree of progress toward completing the goal for the current week based on comparing the done/quota fraction to the fraction of the week that has passed. Since the current weekday, Friday, is the 5th day of the week, the fraction of the week that has passed is somewhere between 4/7 (beginning of Friday) and 5/7 (end of Friday).   
 - walk the dog:  colored red because 3/7 is less than 4/7 and thus completions are unambiguously behind schedule for the week - 2 completions today are needed to get back on schedule.
 - wash dishes: colored yellow because 3/5 is between 4/7 and 5/7 - 1 completion today is needed to get back on schedule.
 - interval training: blue because 3/4 > 5/7 and thus completions are ahead of schedule for this week - no completions are needed today to stay on schedule.
 
 This is a normal view in etm and all the normal commands are available. Additionally, these commands are available when a goal is selected:
 - F:  increment the completion count for the current week (by incrementing the count for the current week in @h).
-- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of weeks that has expired) are regarded as *ended*.
+- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of weeks that has expired) are regarded as *ended*. Ending a goal instead of deleting it preserves its history of completions.
 - ^a: toggle the active/inactive status by reversing the sign of the quota component of @q. Goals with negative quotas are regarded as *inactive*. 
 
 A *goal* could, of course, be deleted but this would also delete the history of completions. Ending the goal, on the other hand, preserves the history and places the goal in it's own category at the bottom of the list. And, if you ever want to un-end the goal, just change the zero quota to whatever you like. Similarly, making a goal inactive while you're away on vacation and then making it active again when you return preserves its history and the two key presses required is significantly more convenient than deleting and re-creating the goal.
 
 [↺ contents](#contents)
 
 ### Timer View {#timer-view}
@@ -1796,24 +1796,24 @@
 ### goal {#goal}
 
 Type character: **~**
 
 The goal itemtype is intended to support pursuing S.M.A.R.T. goals (Specific, Measurable, Achievable, Relevant, Timed) in *etm*. Here is an example of a *goal* as it would be entered:
 
 ```
-    ~ interval training @s 2024/4/22 @q 3
+    ~ interval training @s 2024/4/22 @q 3w
 ```
 - It is a *goal* because of the `~` type character. 
 - Because I have a custom interval setting on my exercise bike, "interval training" is *specific* and *measurable*. It is also *achievable* and *relevant* for me.
-- The `@s` entry is required and times the goal to begin on Monday, April 22, 2024. Whatever date is entered will be automatically converted to the Monday of the corresponding week.
-- The `@q` entry is also required and sets to quota for this goal to 3 times per week, repeating indefinitely. Had the quota instead been, say, `@q 3, 5`  then the goal would have been 3 times per week repeated for 5 weeks.
+- The `@s` entry is required and times the goal to begin on Monday, April 22, 2024. Whatever date is entered will be automatically be interpreted as the corresponding week.
+- The `@q` entry is also required and sets to quota for this goal to 3 times per week, repeating indefinitely. Had the quota instead been, say, `@q 3w, 5`  then the goal would have been 5 times per week repeated for 5 weeks. Instead of using 'w' for weekly, it is also possible to use 'y' for yearly, 'q' for quarterly or 'm' for monthly.
 - If this goal were selected in *etm* on, say, Wednesday, April 24 and "F" were pressed, then *etm* would add an `@h 2024:17 1` (history of completions) entry to indicate 1 completion of the goal for the week of *2024:17*. Pressing "F" again in the same week with this goal selected would change this entry to `@h 2024:17 2`.  As one last example, pressing "F" with the goal selected sometime during the week of *2024:18* would leave the recorded entry as
 
     ```
-    ~ interval training @s 2024/4/29 @q 3 @h 2024:17 2, 2024:18 1
+    ~ interval training @s 2024/4/29 @q 3w @h 2024:17 2, 2024:18 1
     ```
 
 [↺ contents](#contents)
 
 ### inbox {#inbox}
 
 Type character: **!**
```

### Comparing `etm-dgraham-6.2.7/README.md` & `etm-dgraham-6.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -594,15 +594,15 @@
 In the main window, active goals are sorted by their done/quota ratios and given a color indicating the degree of progress toward completing the goal for the current week based on comparing the done/quota fraction to the fraction of the week that has passed. Since the current weekday, Friday, is the 5th day of the week, the fraction of the week that has passed is somewhere between 4/7 (beginning of Friday) and 5/7 (end of Friday).   
 - walk the dog:  colored red because 3/7 is less than 4/7 and thus completions are unambiguously behind schedule for the week - 2 completions today are needed to get back on schedule.
 - wash dishes: colored yellow because 3/5 is between 4/7 and 5/7 - 1 completion today is needed to get back on schedule.
 - interval training: blue because 3/4 > 5/7 and thus completions are ahead of schedule for this week - no completions are needed today to stay on schedule.
 
 This is a normal view in etm and all the normal commands are available. Additionally, these commands are available when a goal is selected:
 - F:  increment the completion count for the current week (by incrementing the count for the current week in @h).
-- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of weeks that has expired) are regarded as *ended*.
+- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of weeks that has expired) are regarded as *ended*. Ending a goal instead of deleting it preserves its history of completions.
 - ^a: toggle the active/inactive status by reversing the sign of the quota component of @q. Goals with negative quotas are regarded as *inactive*. 
 
 A *goal* could, of course, be deleted but this would also delete the history of completions. Ending the goal, on the other hand, preserves the history and places the goal in it's own category at the bottom of the list. And, if you ever want to un-end the goal, just change the zero quota to whatever you like. Similarly, making a goal inactive while you're away on vacation and then making it active again when you return preserves its history and the two key presses required is significantly more convenient than deleting and re-creating the goal.
 
 [↺ contents](#contents)
 
 ### Timer View {#timer-view}
@@ -1753,24 +1753,24 @@
 ### goal {#goal}
 
 Type character: **~**
 
 The goal itemtype is intended to support pursuing S.M.A.R.T. goals (Specific, Measurable, Achievable, Relevant, Timed) in *etm*. Here is an example of a *goal* as it would be entered:
 
 ```
-    ~ interval training @s 2024/4/22 @q 3
+    ~ interval training @s 2024/4/22 @q 3w
 ```
 - It is a *goal* because of the `~` type character. 
 - Because I have a custom interval setting on my exercise bike, "interval training" is *specific* and *measurable*. It is also *achievable* and *relevant* for me.
-- The `@s` entry is required and times the goal to begin on Monday, April 22, 2024. Whatever date is entered will be automatically converted to the Monday of the corresponding week.
-- The `@q` entry is also required and sets to quota for this goal to 3 times per week, repeating indefinitely. Had the quota instead been, say, `@q 3, 5`  then the goal would have been 3 times per week repeated for 5 weeks.
+- The `@s` entry is required and times the goal to begin on Monday, April 22, 2024. Whatever date is entered will be automatically be interpreted as the corresponding week.
+- The `@q` entry is also required and sets to quota for this goal to 3 times per week, repeating indefinitely. Had the quota instead been, say, `@q 3w, 5`  then the goal would have been 5 times per week repeated for 5 weeks. Instead of using 'w' for weekly, it is also possible to use 'y' for yearly, 'q' for quarterly or 'm' for monthly.
 - If this goal were selected in *etm* on, say, Wednesday, April 24 and "F" were pressed, then *etm* would add an `@h 2024:17 1` (history of completions) entry to indicate 1 completion of the goal for the week of *2024:17*. Pressing "F" again in the same week with this goal selected would change this entry to `@h 2024:17 2`.  As one last example, pressing "F" with the goal selected sometime during the week of *2024:18* would leave the recorded entry as
 
     ```
-    ~ interval training @s 2024/4/29 @q 3 @h 2024:17 2, 2024:18 1
+    ~ interval training @s 2024/4/29 @q 3w @h 2024:17 2, 2024:18 1
     ```
 
 [↺ contents](#contents)
 
 ### inbox {#inbox}
 
 Type character: **!**
```

### Comparing `etm-dgraham-6.2.7/bump.py` & `etm-dgraham-6.3.0/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/docs/index_konnections.md` & `etm-dgraham-6.3.0/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/docs/index_usedtime.md` & `etm-dgraham-6.3.0/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/docs/multiple_timers.md` & `etm-dgraham-6.3.0/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/etm/__main__.py` & `etm-dgraham-6.3.0/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/etm/common.py` & `etm-dgraham-6.3.0/etm/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -610,23 +610,26 @@
                 initial_indent=initial_indent,
                 subsequent_indent=' ' * indent,
                 width=width - indent - 1,
             )
         )
     return '\n'.join(tmp)
 
+
 def parse(s, **kwd):
     # enable pi when read by main and settings is available
     pi = parserinfo(
         dayfirst=settings['dayfirst'], yearfirst=settings['yearfirst']
     )
+    # logger.debug(f"parsing {s = } with {kwd = }")
     dt = dateutil_parse(s, parserinfo=pi)
     if 'tzinfo' in kwd:
         tzinfo = kwd['tzinfo']
-        if tzinfo == 'float':
+        # logger.debug(f"using {tzinfo = } with {dt = }")
+        if tzinfo == None:
             return dt.replace(tzinfo=None)
         elif tzinfo == 'local':
             return dt.astimezone()
         else:
             return dt.replace(tzinfo=ZoneInfo(tzinfo))
     else:
         return dt.astimezone()
```

### Comparing `etm-dgraham-6.2.7/etm/data.py` & `etm-dgraham-6.3.0/etm/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 from tinydb_serialization import SerializationMiddleware 
 import base64  # for do_mask
 import asyncio
 
 from datetime import datetime, date, timedelta
 
 import dateutil 
-import dateutil.rrule 
-from zoneinfo import ZoneInfo
+from dateutil.rrule import rrule
+from dateutil.tz import gettz
 
 import logging
 logger = logging.getLogger('etmmv')
 
 from dateutil.rrule import * 
 import re
 from etm.common import ( 
@@ -97,14 +97,17 @@
 #         try:
 #             doc_id = doc.doc_id
 #             update_db(db, doc_id, doc)
 #         except Exception as e:
 #             logger.error(f'write_back exception: {e}')
 
 
+local_tz = gettz()
+utc_tz = gettz('UTC')
+
 def insert_db(db, hsh={}):
     """
     Assume hsh has been vetted.
     """
     if not hsh:
 
         return
@@ -585,15 +588,15 @@
         >>> dts.encode(datetime(2018,7,25,10,27).naive())
         '20180725T1027N'
         >>> dts.encode(datetime(2018,7,25,10,27, tz='US/Eastern'))
         '20180725T1427A'
         """
         return encode_datetime(obj)
         if is_aware(obj):
-            return obj.astimezone(ZoneInfo('UTC')).strftime(AWARE_FMT)
+            return obj.astimezone(utc_tz).strftime(AWARE_FMT)
         else:
             return obj.strftime(NAIVE_FMT)
 
     def decode(self, s):
         """
         Return the serialization as a datetime object. If the serializaton ends with 'A',  first interpret as UTC aware and then return the corresponding aware datetime object in the local timezone. If the serialization ends with 'N', returning as an aware datetime object in the local timezone.
         >>> dts = DateTimeSerializer()
@@ -601,19 +604,19 @@
         DateTime(2018, 7, 25, 10, 27, 0, tzinfo=Timezone('America/New_York'))
         >>> dts.decode('20180725T1427A')
         DateTime(2018, 7, 25, 10, 27, 0, tzinfo=Timezone('America/New_York'))
         """
         if s[-1] == 'A':
             return (
                 datetime.strptime(s, AWARE_FMT)
-                .replace(tzinfo=ZoneInfo('UTC'))
-                .astimezone()
+                .replace(tzinfo=utc_tz)
+                .astimezone(local_tz)
             )
         else:
-            return datetime.strptime(s, NAIVE_FMT).astimezone(None)
+            return datetime.strptime(s, NAIVE_FMT).replace(tzinfo=local_tz)
 
 
 class DateSerializer(Serializer):
     """
     This class handles datetime date objects. Encode as date string and decode as a midnight datetime without conversion in the local timezone.
     >>> ds = DateSerializer()
     >>> ds.encode(datetime(2018, 7, 25).date())
```

### Comparing `etm-dgraham-6.2.7/etm/make_examples.py` & `etm-dgraham-6.3.0/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/etm/model.py` & `etm-dgraham-6.3.0/etm/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pyright: reportUndefinedVariable=false
 #  standard sort order for usable ASCII characters
 # usable = ['!', '"', '#', '$', '%', '&', "'", '(', ')', '*', '+', ',', '-', '.', '/', '0', '1', '2', '3', '4', '5', '6', '7', '8', '9', ':', ';', '<', '=', '>', '?', '@', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z', '[', '\\', ']', '^', '_', '`', 'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', '{', '|', '}', '~']
 # len(usable): 94
 
 from typing import Union, Tuple, Optional
+import time
 
 from etm.common import ( 
     VERSION_INFO,
     parse,
     WKDAYS_DECODE,
     WKDAYS_ENCODE,
     # ETM_CHAR,
@@ -52,15 +53,16 @@
 # from tinydb import __version__ as tinydb_version
 # from jinja2 import __version__ as jinja2_version
 # from prompt_toolkit import __version__ as prompt_toolkit_version
 
 from dateutil import rrule as dr 
 from datetime import datetime, date, timedelta
 from zoneinfo import ZoneInfo
-from dateutil.rrule import MO, TU, WE, TH, FR, SA, SU  
+from dateutil.rrule import rrule, rruleset, MO, TU, WE, TH, FR, SA, SU  
+from dateutil.tz import gettz
 
 # for saving timers
 import pickle
 from warnings import filterwarnings
 from ruamel.yaml import YAML 
 from jinja2 import Template 
 import textwrap
@@ -94,14 +96,15 @@
 # NOTE: view.main() will override ampm using the configuration setting
 ampm = True
 logger = None
 goal_counts = {}
 
 active_tasks = {}
 
+local_tz = gettz()
 
 def sortprd(prd):
     # assumes prd is a Period
     return prd.start.strftime('%Y%m%d%H%M')
 
 
 PHONE_REGEX = re.compile(r'[0-9]{10}@.*')
@@ -212,14 +215,17 @@
     '-': ['rr'],
     'rr': ['s'],
     'js': ['s'],
     'ja': ['s'],
     'jb': ['s'],
 }
 
+def is_naive(dt):
+    return dt.tzinfo is None or dt.tzinfo.utcoffset(dt) is None
+
 def truncate_string(s: str, max_length: int)->str:
     if len(s) > max_length:
         return f"{s[:max_length-2]} {EtmChar.ELLIPSIS_CHAR}"
     else:
         return s
 
 def round_to_minutes(obj: timedelta)->timedelta:
@@ -855,33 +861,34 @@
 
     def get_repetitions(self):
         """
         Called with a row, we should have an doc_id and can use relevant
         as aft_dt. Called while editing, we won't have a row or doc_id
         and can use '@s' as aft_dt
         """
-        # doc_id, instance, job = dataview.get_row_details(text_area.document.cursor_position_row)
-
         num = self.settings['num_repetitions']
-        self.update_item_hsh()
+        # self.update_item_hsh()
         item = self.item_hsh
         showing = 'Repetitions'
         if 's' not in item and ('r' not in item or '+' not in item):
             return showing, 'not a repeating item'
+        logger.debug(f"{item['s'] = }; {item = }")
         relevant = date_to_datetime(item['s'])
         at_plus = item.get('+', [])
         if at_plus:
             at_plus.sort()
             relevant = min(relevant, date_to_datetime(at_plus[0]))
 
-        # instances = item_instances(item, relevant, num + 1, False)
-        instances = item_instances(item, None, num + 1, False)
+        logger.debug(f"Item */* get_repetitions {item['s'] = }")
+        instances = item_instances(item, None, num + 1)
         instances.sort()
+        logger.debug(f"Item */* {instances = }")
         relevant = instances[0][0]
-        pairs = [format_datetime(x[0])[1] for x in instances]
+        logger.debug(f"{relevant = }")
+        pairs = [format_instance(x[0]) for x in instances]
         starting = format_datetime(relevant.date())[1]
         if len(pairs) > num:
             showing = f'Next {num} repetitions'
             pairs = pairs[:num]
         elif pairs:
             showing = 'All repetitions'
         else:
@@ -1144,21 +1151,24 @@
         
         self.doc_id = item_id
         # self.created = self.item_hsh['created']
         q = self.item_hsh.get('q', [])
         if not len(q) > 0:
             return False
         quota = q[0]
+        period = q[1]
         now = datetime.now().astimezone()
-        this_week = tuple([int(x) for x in now.strftime("%Y,%W").split(',')])
+        this_period, fraction_passed = get_fraction_of_period_passed(period)
+
+        # this_week = tuple([int(x) for x in now.strftime("%Y,%W").split(',')])
         self.item_hsh.setdefault('h', {})
         hist = self.item_hsh.get('h', {})
-        this_week_str = f"{this_week[0]}:{this_week[1]:02}"
-        done = hist.get(this_week_str, 0)
-        hist[this_week_str] = done + 1
+        # this_week_str = f"{this_week[0]}:{this_week[1]:02}"
+        done = hist.get(this_period, 0)
+        hist[this_period] = done + 1
         self.item_hsh['h'] = hist
         self.item_hsh['modified'] = now
         self.do_update()
         return True
 
     def toggle_goal_active(
             self,
@@ -1167,17 +1177,18 @@
         self.item_hsh = self.db.get(doc_id=item_id)
         if self.item_hsh['itemtype'] != '~':
             return False
         
         self.doc_id = item_id
         # self.created = self.item_hsh['created']
         q = self.item_hsh.get('q', [])
+        # logger.debug(f"{q = }; {self.item_hsh = }")
         if not len(q) > 0 or q[0] == 0:
             return False
-        q[0] = -q[0]
+        q[0] = f"{-int(q[0])}"
         self.item_hsh['q'] = q 
         now = datetime.now().astimezone()
         self.item_hsh['modified'] = now
         self.do_update()
         return True
 
     def end_goal(
@@ -1187,17 +1198,18 @@
         self.item_hsh = self.db.get(doc_id=item_id)
         if self.item_hsh['itemtype'] != '~':
             return False
         
         self.doc_id = item_id
         # self.created = self.item_hsh['created']
         q = self.item_hsh.get('q', [])
-        if not len(q) > 0 or q[0] == 0:
+        if len(q) < 1 or q[0] == 0 or q[0] == '0':
+            # already ended
             return False
-        q[0] = 0
+        q[0] = '0'
         self.item_hsh['q'] = q 
         now = datetime.now().astimezone()
         self.item_hsh['modified'] = now
         self.do_update()
         return True
 
     def finish_item(
@@ -1383,14 +1395,15 @@
 
 
     def text_changed(self, s, pos, modified=True):
         """ """
         # self.is_modified = modified
         self.entry = s
         self.pos_hsh, keyvals = process_entry(s, self.settings)
+        logger.debug(f"{self.pos_hsh = }; {keyvals = }")
         removed, changed = listdiff(self.keyvals, keyvals)
         if self.init_entry != self.entry:
             self.is_modified = True
         # only process changes for kv entries
         update_timezone = False
         for kv in removed + changed:
             if kv[0] == 'z':
@@ -1773,25 +1786,53 @@
             rep = 'Include repetitions falling on or before this datetime'
         return obj, rep
     
 
     def do_quota(self, arg: str)->list[int]:
         """P
         Args:
-            arg (string): an integer quota optionally followed by a comma and an integer number of weeks
+            arg (string): an integer followed by a character in 'yqmw'
+            specifying the period optionally followed by a comma and an 
+            integer number of periods.
         """
         obj = None
         m = quota_regex.match(arg)
+
+        period_dict = {
+                'y': 'year',
+                'q': 'quarter',
+                'm': 'month',
+                'w': 'week'
+        }
+
         if m:
-            obj = [int(x) for x in arg.split(',') if x.strip()]
-            weeks = f"for {obj[1]} weeks" if len(obj) > 1 else "indefinitely" 
-            rep = f'{obj[0]} times/week {weeks}'
-            self.item_hsh['q'] = obj                
+            logger.debug(f"{m.groups() = }")
+            quota, period, num_periods_str = m.groups()
+
+            if not period:
+                period = 'w'
+
+            # period = period_dict.get(period, 'week')
+            num_periods = 0
+            periods_str = 'indefinitely'
+            if num_periods_str:
+                num_periods = int(num_periods_str.lstrip(', '))
+                if num_periods > 0:
+                    periods_str = f"for {num_periods} {period_dict[period]}s"
+                else:
+                    periods_str = 'indefinitely'
+            
+            rep = f'{quota} times/{period_dict[period]} {periods_str}'
+            obj = [quota, period, num_periods]
+            self.item_hsh['q'] = obj
+
         else:
-            rep = "goal: instances per week optionally followed by a comma and the number of weeks"
+            rep = """goal: integer times/period followed by a period from
+                y)ear, q)uarter, m)onth or w)eek 
+            optionally followed by a comma and the number of periods over which the goal applies - the default is 0 for indefinitely""" 
         return obj, rep
         
 
     def do_datetime(self, arg):
         """
         >>> item = Item("")
         >>> item.do_datetime('fr')
@@ -1799,27 +1840,30 @@
         >>> item.do_datetime('2019-01-25')
         (Date(2019, 1, 25), 'Fri Jan 25 2019')
         >>> item.do_datetime('2019-01-25 2p')
         (DateTime(2019, 1, 25, 14, 0, 0, tzinfo=ZoneInfo('America/New_York')), 'Fri Jan 25 2019 2:00pm EST')
         """
         obj = None
         tz = self.item_hsh.get('z', None)
+        logger.debug(f"calling parse_datetime with {arg = } and {tz = }")
         ok, res, z = parse_datetime(arg, tz)
+        logger.debug(f"{arg = }; {tz = }; {ok = };\n*** {res = }; {z = } ***")
         if ok:
+            obj = res
             if self.item_hsh['itemtype'] == '~':
-                # We need Monday of the week containing the datetime for goals
-                obj = datetime.strptime(res.strftime("%Y %W 1"), "%Y %W %w")
-                rep = f'The first day of the specified week: {format_date(obj)[1]}'
+                # We need a date 
+                rep = f'date: {format_date(obj)[1]}'
             else:
                 obj = res
                 rep = (
                     f'local datetime: {format_datetime(obj)[1]}'
                     if ok == 'aware'
                     else format_datetime(obj)[1]
             )
+                logger.debug(f"{rep = }; {obj = }")
         else:
             rep = res
         return obj, rep
 
     def do_datetimes(self, args):
         """
         >>> item = Item("")
@@ -1863,15 +1907,15 @@
         all_ok = True
         rep_lst = []
         bad_lst = []
         completions = []
         if self.item_hsh['itemtype'] == '~':
             obj = {}
             # arg list will be a list of year:weeknum num_done
-            rx = re.compile(r'^\s*\d{4}:\d{2}\s*\d+\s*$')
+            rx = re.compile(r'^\s*\d{4}[:#-]\d{1,2}\s+\d+\s*$')
             for arg in args:
                 match = rx.match(arg.strip())
                 if match:
                     yearweek, done = arg.split()
                     obj[yearweek] = int(done)
                     rep_lst.append(f"{yearweek}: {done}")
                 else:
@@ -2194,42 +2238,46 @@
         elif s[0] in ['+', '-']:
             # must be a dur string
             dur_str = s
         else:
             # must be a dt string
             dt_str = s
 
+        logger.debug(f"{s = }; {dt_str = }; {tzinfo = }")
+
         if dt_str:
+            logger.debug(f"parsing {dt_str = } with {tzinfo = }")
             dt = (
                 datetime.now().astimezone()
                 if dt_str.strip() == 'now'
                 else parse(dt_str, tzinfo=tzinfo)
             )
+            logger.debug(f"got {dt = }")
         else:
             dt = datetime.now().astimezone()
             if dur_str and re.search(r'[dwM]', dur_str):
                 dt = dt.replace(hour=0, minute=0, second=0, microsecond=0)
 
         dur = parse_duration(dur_str)[1] if dur_str else ZERO
         res = dt + dur
 
     except Exception as e:
         return False, f"'{s}' is incomplete or invalid: {e}", z
     else:
-        if tzinfo in ['local', 'float'] and (
-            res.hour,
-            res.minute,
-            res.second,
-            res.microsecond,
-        ) == (0, 0, 0, 0):
-            return 'date', res.astimezone(), z
-        elif ok == 'float':
-            return ok, res.astimezone(None), z
-        else:
-            return ok, res.astimezone(), z
+        # if tzinfo in ['local', 'float'] and (
+        #     res.hour,
+        #     res.minute,
+        #     res.second,
+        #     res.microsecond,
+        # ) == (0, 0, 0, 0):
+        #     return 'date', res.astimezone(), z
+        # elif ok == 'float':
+        #     return ok, res.astimezone(None), z
+        # else:
+        return ok, res, z
 
 
 def timestamp(arg):
     """
     Fuzzy parse a datetime string and return the YYYYMMDDTHHMM formatted version.
     >>> timestamp("6/16/16 4p")
     (True, DateTime(2016, 6, 16, 16, 0, 0, tzinfo=ZoneInfo('UTC')))
@@ -2339,14 +2387,56 @@
     yearfirst = settings.get('yearfirst', False)
     month = obj.strftime('%b')
     day = obj.strftime('%-d')
     weekday = obj.strftime('%a')
     monthday = f'{day} {month}' if dayfirst else f'{month} {day}'
     return f'{weekday} {monthday}'
 
+def format_instance(dt: datetime):
+    flag = " (within dst transition)" if is_within_dst_transition(dt) else ""
+    date_str = dt.strftime("%a %b %-d %Y")
+    if settings.get('ampm', True):
+        time_str = dt.strftime("%-I:%M%p").rstrip('M').lower()
+    else:
+        time_str = dt.strftime("%H:%M")
+    return f"{date_str} {time_str}{flag}"
+
+
+def is_within_dst_transition(dt: datetime)->bool:
+
+    year = dt.year
+    if dt.tzinfo is None:
+        timezone = gettz()
+        dt = dt.replace(tzinfo = timezone)
+    else:
+        timezone = dt.tzinfo 
+    logger.debug(f"using {timezone = }")
+    
+    # Find the first Sunday in November
+    first_november = datetime(year, 11, 1, tzinfo=timezone)
+    first_sunday_november = first_november + timedelta(days=(6 - first_november.weekday()))
+    
+    # Find the second Sunday in March
+    first_march = datetime(year, 3, 1, tzinfo=timezone)
+    second_sunday_march = first_march + timedelta(days=(6 - first_march.weekday() + 7))
+    
+    # Create aware datetime objects for the transitions
+    first_sunday_november_1am = first_sunday_november.replace(hour=1)
+    first_sunday_november_2am = first_sunday_november.replace(hour=2)
+    
+    second_sunday_march_2am = second_sunday_march.replace(hour=2)
+    second_sunday_march_3am = second_sunday_march.replace(hour=3)
+    
+    logger.debug(f"{first_sunday_november_1am = }; ")
+    # Check if the datetime falls within the transition periods
+    is_in_november_transition = first_sunday_november_1am <= dt < first_sunday_november_2am
+    is_in_march_transition = second_sunday_march_2am <= dt < second_sunday_march_3am
+
+    return is_in_november_transition or is_in_march_transition
+
 
 def format_datetime(obj, short=False):
     """
     >>> format_datetime(parse_datetime("20160710T1730")[1])
     , needs(True, 'Sun Jul 10 2016 5:30pm EDT')
     >>> format_datetime(parse_datetime("2015-07-10 5:30p", "float")[1])
     (True, 'Fri Jul 10 2015 5:30pm')
@@ -2391,14 +2481,16 @@
         return True, obj.strftime(date_fmt)
 
     if obj.strftime('Z') == '':
         # naive datetime
         if (obj.hour, obj.minute, obj.second, obj.microsecond) == (0, 0, 0, 0):
             # treat as date
             return True, obj.strftime(date_fmt)
+        else:
+            return True, obj.strftime(f'{date_fmt} {time_fmt}') 
     else:
         # aware datetime
         obj = obj.astimezone()
         if not short:
             time_fmt += ' %Z'
     res = obj.strftime(f'{date_fmt} {time_fmt}')
     if ampm:
@@ -2675,16 +2767,16 @@
     r'(([+-]?)(\d+)\s(week|day|hour|minute|second)s?)+?'
 )
 relative_regex = re.compile(r'(([+-])(\d+)([wdhmys]))+?')
 threeday_regex = re.compile(
     r'([+-]?[1234])(MON|TUE|WED|THU|FRI|SAT|SUN)', re.IGNORECASE
 )
 anniversary_regex = re.compile(r'!(\d{4})!')
+quota_regex = re.compile(r'^\s*(-?\d+)([yqmw]?)(,\s*\d+)?\s*$') # @q 3m, 1
 
-quota_regex = re.compile(r'^\s*-?\d+(,\s*\d+)?\s*$')
 
 def parse_durations(s):
     periods = [x.strip() for x in s.split('+')]
     total = ZERO
     bad = []
     for d in periods:
         ok, p = parse_duration(d)
@@ -2914,24 +3006,27 @@
         self.done_view = ''
         self.effort_view = ''
         self.busy_view = ''
         self.calendar_view = ''
         self.query_view = ''
         self.query_text = ''
         self.last_query = ''
+        self.last_modified = time.time()
         self.query_items = []
         self.query_mode = 'items table'
         self.report_view = ''
         self.report_text = ''
         self.active_str = ''
         self.inactive_str = ''
         self.report_items = []
         self.cal_locale = None
         self.history_view = ''
         self.cache = {}
+        self.view_cache = {} # non-weekly view name -> (timestamp, view, row2id)
+        self.cached_views = ['history', 'forthcoming', 'do_next', 'journal', 'goals', 'tags', 'index', 'location', 'review', 'konnected']
         self.itemcache = {}
         self.current_hsh = {}
         self.used_summary = {}
         self.used_details = {}
         self.used_details2id = {}
         self.effort_details = {}
         self.currMonth()
@@ -3531,14 +3626,43 @@
         self.current_row = None
         self.prior_view = self.active_view
         self.active_view = self.views.get(c, 'agenda')
         if self.active_view != 'query':
             self.use_items()
 
     def show_active_view(self):
+        # logger.debug(f'{self.active_view = }; {self.cached_views = }; {self.active_view in self.cached_views = }')
+
+        if self.active_view not in self.cached_views:
+            cached_view = self.create_view()
+            return cached_view
+
+        # logger.debug('in cached views')
+        if self.active_view in self.view_cache:
+            timestamp, cached_view, row2id = self.view_cache[self.active_view]
+            if timestamp >= self.last_modified:
+                timer_use_cache = TimeIt('use_cache')
+                logger.debug(f"using cache for {self.active_view}")
+                self.row2id = row2id
+                timer_use_cache.stop()
+                return cached_view
+
+        # logger.debug(f"creating cache for {self.active_view}")
+        timer_make_cache = TimeIt('make cache')
+        cached_view = self.create_view()
+        row2id = self.row2id
+        timestamp = time.time()
+        self.view_cache[self.active_view] = (timestamp, cached_view, row2id)
+        timer_make_cache.stop()
+        return cached_view      
+        
+        
+    
+    def create_view(self):
+        # logger.debug(f"creating {self.active_view}")
         if self.active_view != 'query':
             self.hide_query()
         if self.active_view == 'agenda':
             self.refreshAgenda()
             return self.agenda_view
         if self.active_view == 'completed':
             self.refreshAgenda()
@@ -3550,14 +3674,15 @@
             return self.effort_view
         if self.active_view == 'busy':
             self.refreshAgenda()
             return self.busy_view
         if self.active_view == 'yearly':
             self.refreshCalendar()
             return self.calendar_view
+
         if self.active_view == 'history':
             self.history_view, self.row2id = show_history(
                 self.db,
                 True,
                 self.repeat_list,
                 self.pinned_list,
                 self.link_list,
@@ -4090,15 +4215,15 @@
         """
         num = self.settings['num_repetitions']
         res = self.get_row_details(row)
         if not res:
             return None, ''
         item_id = res[0]
         instance = res[1]
-
+        
         if not (item_id and item_id in self.id2relevant):
             return ''
         showing = 'Repetitions'
         item = DBITEM.get(doc_id=item_id)
         details = f"{item['itemtype']} {item['summary']}"
 
         if not ('s' in item and ('r' in item or '+' in item)):
@@ -4108,23 +4233,26 @@
             relevant = instance
         else:
             relevant = date_to_datetime(item['s'])
             at_plus = item.get('+', [])
             if at_plus:
                 at_plus.sort()
                 relevant = min(relevant, date_to_datetime(at_plus[0]))
-
-        # relevant = instance if instance else self.id2relevant.get(item_id)
-        # showing = 'Repetitions'
         if not relevant:
             return 'Repetitons', details + 'none'
-        pairs = [
-            format_datetime(x[0])[1]
-            for x in item_instances(item, relevant, num + 1, False)
-        ]
+        logger.debug(f"Dataview */* get_repetitions {item = }")
+        instances = item_instances(item, None, num + 1)
+        instances = [(x[0].replace(tzinfo=None), x[1]) for x in instances]
+        instances.sort()
+        logger.debug(f"Dataview */* {instances = }")
+        relevant = instances[0][0]
+        logger.debug(f"{relevant = }")
+        # pairs = [format_datetime(x[0])[1] for x in instances]
+        pairs = [format_instance(x[0]) for x in instances]
+        logger.debug(f"Dataview */* {pairs = }")
         starting = format_datetime(relevant.date())[1]
         if len(pairs) > num:
             showing = f'Next {num} repetitions'
             pairs = pairs[:num]
         else:
             showing = f'Remaining repetitions'
         return showing, f'from {starting} for\n{details}:\n  ' + '\n  '.join(
@@ -4278,16 +4406,16 @@
             True,
             f"{item['itemtype']} {item['summary']}\n{due_str}",
             item_id,
             job_id,
             due,
         )
 
-    def clearCache(self):
-        self.cache = {}
+    # def clearCache(self):
+    #     self.cache = {}
 
     def refreshCache(self):
         self.cache = schedule(
             ETMDB,
             self.currentYrWk,
             self.current,
             self.now,
@@ -4854,14 +4982,24 @@
         else:
             return s
     if type(s) is list:
         return ', '.join([_str(x) for x in s])
     else:
         return _str(s)
 
+def quota_as_string(s):
+    logger.debug(f"{s = }")
+    if not type(s) is list:
+        return str(s)
+    if len(s) > 2:
+        return f'{s[0]}{s[1]}, {s[2]}'
+    elif len(s) > 1:
+        return f'{s[0]}{s[1]}'
+    else:
+        return f'{s[0]}w'
 
 def do_string(arg):
     try:
         obj = str(arg)
         rep = arg
     except:
         obj = None
@@ -5064,15 +5202,15 @@
 {%- set title -%}\
 {{ h.itemtype }} {{ h.summary }}\
 {% if 's' in h %}{{ " @s {}".format(dt2str(h['s'])[1]) }}{% endif %}\
 {%- if 'e' in h %}{{ " @e {}".format(in2str(h['e'])) }}{% endif %}\
 {%- if 'w' in h %}{{ " @w {}".format(inlst2str(h['w'])) }}{% endif %}\
 {%- if 'b' in h %}{{ " @b {}".format(h['b']) }}{% endif %}\
 {%- if 'z' in h %}{{ " @z {}".format(h['z']) }}{% endif %}\
-{%- if 'q' in h %}{{ " @q {}".format(one_or_more(h['q'])) }}{% endif %}\
+{%- if 'q' in h %}{{ " @q {}".format(quota_as_string(h['q'])) }}{% endif %}\
 {%- endset %}\
 {{ nowrap(title) }} \
 {% if 'f' in h %}\
 {{ "@f {} ".format(prd2str(h['f'])) }} \
 {% endif -%}\
 {% if 'a' in h %}\
 {%- set alerts %}\
@@ -5175,15 +5313,15 @@
 {%- set title -%}\
 {{ h.itemtype }} {{ h.summary }}\
 {% if 's' in h %}{{ " @s {}".format(dt2str(h['s'])[1]) }}{% endif %}\
 {%- if 'e' in h %}{{ " @e {}".format(in2str(h['e'])) }}{% endif %}\
 {%- if 'w' in h %}{{ " @w {}".format(inlst2str(h['w'])) }}{% endif %}\
 {%- if 'b' in h %}{{ " @b {}".format(h['b']) }}{% endif %}\
 {%- if 'z' in h %}{{ " @z {}".format(h['z']) }}{% endif %}\
-{%- if 'q' in h %}{{ " @q {}".format(one_or_more(h['q'])) }}{% endif %}\
+{%- if 'q' in h %}{{ " @q {}".format(quota_as_string(h['q'])) }}{% endif %}\
 {%- endset %}\
 {{ wrap(title) }} \
 {% if 'f' in h %}\
 {{ "@f {} ".format(prd2str(h['f'])) }} \
 {% endif -%}\
 {% if 'a' in h %}\
 {%- set alerts %}\
@@ -5297,25 +5435,27 @@
 jinja_entry_template.globals['dt2str'] = plain_datetime
 jinja_entry_template.globals['in2str'] = fmt_dur
 jinja_entry_template.globals['dtlst2str'] = plain_datetime_list
 jinja_entry_template.globals['inlst2str'] = format_duration_list
 jinja_entry_template.globals['prd2str'] = format_period
 jinja_entry_template.globals['prdlst2str'] = format_period_list
 jinja_entry_template.globals['one_or_more'] = one_or_more
+jinja_entry_template.globals['quota_as_string'] = quota_as_string
 jinja_entry_template.globals['isinstance'] = isinstance
 jinja_entry_template.globals['nowrap'] = nowrap
 
 jinja_display_template = Template(display_tmpl)
 jinja_display_template.globals['dt2str'] = plain_datetime
 jinja_display_template.globals['in2str'] = fmt_dur
 jinja_display_template.globals['dtlst2str'] = plain_datetime_list
 jinja_display_template.globals['inlst2str'] = format_duration_list
 jinja_display_template.globals['prd2str'] = format_period
 jinja_display_template.globals['prdlst2str'] = format_period_list
 jinja_display_template.globals['one_or_more'] = one_or_more
+jinja_display_template.globals['quota_as_string'] = quota_as_string
 jinja_display_template.globals['isinstance'] = isinstance
 jinja_display_template.globals['wrap'] = wrap
 
 
 def do_beginby(arg):
     beginby_str = 'an integer number of days'
     if not arg:
@@ -6005,15 +6145,18 @@
     return freq, kwd
 
 def get_next_due(item, done, due, from_rrule=False):
     """
     return the next due datetime for an @r and @+ / @- repetition
     """
     def f(dt: datetime)->str:
-        return(dt.astimezone().strftime("%Y-%m-%d %H:%M:%S"))
+        if is_date(dt):
+            return(dt.strftime("%Y-%m-%d"))
+        else:
+            return(dt.astimezone().strftime("%Y-%m-%d %H:%M:%S"))
 
     instances = [f(x[0]) for x in item_instances(item, item['s'], 2, False)]
     lofh = item.get('r')
     if not lofh:
         return ''
     rset = dr.rruleset()
     overdue = item.get('o', 'k')   # make 'k' the default for 'o'
@@ -6074,17 +6217,19 @@
     if nxt:
         if using_dates:
             nxt = nxt.date()
     else:
         nxt = None
     return nxt
 
+def is_date(dt: Union[date, datetime])->bool:
+    return isinstance(dt, date) and not isinstance(dt, datetime)
 
 def date_to_datetime(dt, hour=0, minute=0):
-    if isinstance(dt, date) and not isinstance(dt, datetime):
+    if is_date(dt):
         new_dt = datetime(
             year=dt.year,
             month=dt.month,
             day=dt.day,
             hour=hour,
             minute=minute,
             second=0,
@@ -6133,14 +6278,26 @@
     """
 
     if 's' not in item:
         if 'f' in item:
             return [(item['f'], None)]
         else:
             return []
+    tz = item.get('z', 'local')
+    if tz == 'local':
+        tz_info = gettz()
+    elif tz == 'float':
+        tz_info = None
+    else:
+        try:
+            tz_info = gettz(tz)
+        except Exception as e:
+            logger.warning(f"bad {tz = }: {e}. Using localtime")
+            tz_info = gettz() # default to localtime
+    
     instances = []
     dtstart = item['s']
     if not (isinstance(dtstart, datetime) or isinstance(dtstart, date)):
         return []
     # This should not be necessary since the data store decodes dates as datetimes
     if aft_dt is None:
         if '+' in item:
@@ -6151,32 +6308,32 @@
     if isinstance(dtstart, date) and not isinstance(dtstart, datetime):
         dtstart = datetime(
             year=dtstart.year,
             month=dtstart.month,
             day=dtstart.day,
             hour=0,
             minute=0,
-        ).astimezone()
+        ).replace(tzinfo = tz_info)
         startdst = None
         using_dates = True
     else:
         using_dates = False
         # for discarding daylight saving time differences in repetitions
         try:
             startdst = dtstart.dst()
         except:
             print('dtstart:', dtstart)
             dtstart = dtstart[0]
 
     # all the dateutil instances will be in UTC so these must be as well
-    aft_dt = date_to_datetime(aft_dt).astimezone(ZoneInfo('UTC'))
+    aft_dt = date_to_datetime(aft_dt).astimezone(tz_info)
     bef_dt = (
         bef_dt
         if isinstance(bef_dt, int)
-        else date_to_datetime(bef_dt).astimezone(ZoneInfo('UTC'))
+        else date_to_datetime(bef_dt).astimezone(tz_info)
     )
 
     if 'r' in item:
         lofh = item['r']
         rset = dr.rruleset()
 
         for hsh in lofh:
@@ -6804,14 +6961,18 @@
     >>> drop_zero_minutes(parse('2018-03-07 10am'))
     '10'
     >>> drop_zero_minutes(parse('2018-03-07 2:45pm'))
     '2:45'
     """
     ampm = settings['ampm']
     show_minutes = settings['show_minutes']
+    logger.debug(f"starting {dt = }; {ampm = }; {show_minutes = }")
+    logger.debug(f"{dt.replace(tzinfo=None) = }")
+    dt = dt.replace(tzinfo=None)
+    logger.debug(f"{dt = }")
     if show_minutes:
         if ampm:
             return dt.strftime('%-I:%M').rstrip('M').lower()
         else:
             return dt.strftime('%H:%M')
     else:
         if dt.minute == 0:
@@ -7167,29 +7328,32 @@
                                 update_db(db, item.doc_id, item)
                         else:
                             relevant = cur
 
                     else:   # k or r
                         try:
                             # relevant = rset.after(today, inc=True)
+                            logger.debug(f"relevant {item = }")
                             instances = item_instances(item, None)
                             instances.sort()
+                            logger.debug(f"{instances = }")
                             relevant = date_to_datetime(instances[0][0]) if instances else None
                             # relevant = rset.after(dtstart, inc=True)
                             # if plus_dates:
                             #     plus_dates.sort()
                             #     relevant = min(relevant, plus_dates[0])
                         except Exception as e:
                             logger.debug(f"Exception: {e}\nissue with today: {today} ({type(today)}) or rset: {rset}\nskipping {item}")
                             continue
 
                         already_done = [x.end for x in item.get('h', [])]
                         # relevant will be the first instance after 12am today
                         # it will be the @s entry for the updated repeating item
                         # these are @s entries for the instances to be preserved
+                        # logger.debug(f"{dtstart = }; {today = }")
                         between = rset.between(
                             dtstart, today - ONEMIN, inc=True
                         )
                         # remaining = [x for x in between if x not in already_done and x != dtstart]
                         remaining = [
                             x for x in between if x not in already_done
                         ]
@@ -7215,18 +7379,20 @@
                 else:
                     # get the first instance after today
                     try:
                         relevant = rset.after(today, inc=True)
                     except Exception as e:
                         logger.error(f'error processing {item}; {repr(e)}')
                     if not relevant:
+                        # logger.debug(f"{today = }; {item = }")
                         relevant = rset.before(today, inc=True)
 
                 # rset
                 if instance_interval:
+                    # logger.debug(f"{instance_interval = }")
                     instances = rset.between(
                         instance_interval[0], instance_interval[1], inc=True
                     )
                     if possible_beginby:
                         for instance in instances:
                             if (
                                 ZERO
@@ -8029,14 +8195,139 @@
     for row in rows:
         path = row['path']
         values = row['values']
         rdict.add(path, values)
     tree, row2id = rdict.as_tree(rdict)
     return tree, row2id
 
+def get_fraction_of_period_passed(period:str = 'w'):
+    # if isinstance(input_date, str):
+    #     input_date = datetime.strptime(input_date, '%Y-%m-%d')
+    # elif isinstance(input_date, datetime):
+    #     input_date = input_date.replace(hour=0, minute=0, microsecond=0)
+    # else:
+    #     input_date = date_to_datetime(input_date)
+
+    today = datetime.now().astimezone().replace(
+        hour=0, minute=0, second=0, microsecond=0
+        )
+
+    # Helper function to calculate fraction of the week passed
+    def fraction_of_week_passed():
+        this_period_tup = today.isocalendar()[:2] # yyyy, weeknum
+        this_period = f"{this_period_tup[0]}:{this_period_tup[1]:02}"
+        return this_period, today.weekday() / 6
+
+    # Helper function to calculate fraction of the month passed
+    def fraction_of_month_passed():
+        this_period = f"{today.year}-{today.month:02}"
+        return this_period, (today.day - 1) / (calendar.monthrange(today.year, today.month)[1] - 1)
+
+    # Helper function to calculate fraction of the quarter passed
+    def fraction_of_quarter_passed():
+        quarter_start_month = 3 * ((today.month - 1) // 3) + 1
+        quarter_start_date = datetime(today.year, quarter_start_month, 1).astimezone()
+        quarter_end_month = quarter_start_month + 2
+        quarter_end_date = datetime(today.year, quarter_end_month, calendar.monthrange(today.year, quarter_end_month)[1]).astimezone()
+        this_period = f"{today.year}#{(today.month - 1) // 3 + 1}"
+        return this_period, (today - quarter_start_date).days / (quarter_end_date - quarter_start_date).days
+
+    # Helper function to calculate fraction of the year passed
+    def fraction_of_year_passed():
+        start_of_year = datetime(today.year, 1, 1)
+        end_of_year = datetime(today.year, 12, 31)
+        return (today - start_of_year).days / (end_of_year - start_of_year).days
+
+    if period == 'd':
+        return 0.0
+    elif period == 'w':
+        return fraction_of_week_passed()
+    elif period == 'm':
+        return fraction_of_month_passed()
+    elif period == 'q':
+        return fraction_of_quarter_passed()
+    elif period == 'y':
+        return fraction_of_year_passed()
+    else:
+        return None
+    
+def get_period_begin_date(input_date, period):
+    # Ensure input_date is a datetime object
+    if isinstance(input_date, str):
+        input_date = datetime.strptime(input_date, '%Y-%m-%d')
+    elif isinstance(input_date, datetime):
+        input_date = input_date.replace(hour=0, minute=0, microsecond=0)
+    else:
+        input_date = date_to_datetime(input_date)
+    input_date = input_date.astimezone()
+    
+
+    if period == 'w':
+        return input_date - timedelta(days=input_date.weekday())
+    
+    elif period == 'm':
+        return input_date.replace(day=1)
+
+    elif period == 'q':
+        begin_month = ((input_date.month - 1) // 3) * 3 + 1
+        return input_date.replace(month=begin_month)
+
+    elif period == 'y': 
+        return input_date.replace(month=1)
+
+def get_period_end_date(input_date, period, periods_ahead):
+    # Ensure input_date is a datetime object
+    if isinstance(input_date, str):
+        input_date = datetime.strptime(input_date, '%Y-%m-%d')
+    elif isinstance(input_date, datetime):
+        input_date = input_date.replace(hour=0, minute=0, microsecond=0)
+    else:
+        input_date = date_to_datetime(input_date)
+
+    input_date = input_date.astimezone()
+    
+    periods_ahead = max(periods_ahead, 1)
+    
+    if period == 'w':
+        return input_date + timedelta(days=(6 - input_date.weekday())) + timedelta(weeks=periods_ahead-1) + timedelta(days=1, seconds=-1)
+    
+    # Calculate the last day of the month periods_ahead months from input_date
+    elif period == 'm':
+        month = input_date.month - 1 + (periods_ahead - 1)
+        year = input_date.year + month // 12
+        month = month % 12 + 1
+        return datetime(year, month, calendar.monthrange(year, month)[1]).astimezone() + timedelta(days=1, seconds=-1)
+    
+    # Calculate the last day of the quarter periods_ahead quarters from input_date
+    elif period == 'q':
+        quarter = ((input_date.month - 1) // 3 + periods_ahead) % 4
+        year = input_date.year + ((input_date.month - 1) // 3 + periods_ahead) // 4
+        if quarter == 0:
+            quarter = 4
+            year -= 1
+        last_month_of_quarter = quarter * 3
+        return datetime(year, last_month_of_quarter, calendar.monthrange(year, last_month_of_quarter)[1]).astimezone() + timedelta(days=1, seconds=-1)
+
+    elif period == 'y': 
+        # Calculate the last day of the year periods_ahead years from input_date
+        return datetime(input_date.year + periods_ahead - 1, 12, 31).astimezone() + timedelta(days=1, seconds=-1)
+
+    else:
+        return None
+    
+    return ret
+    
+# # Example usage
+# input_date = '2024-05-26'
+# period = 'm'
+# periods_ahead = 3
+# for period in ['w', 'm', 'q', 'y']:
+#     result = get_period_end_date(input_date, period, periods_ahead)
+#     print(f"{input_date = }, {period = }, end_date = {result}")  # (fatetime.date(2024, 6, 8), datetime.date(2024, 7, 31), datetime.date(2024, 9, 30), datetime.date(2025, 12, 31))
+
 def show_goals(
     db,
     id2relevant,
     repeat_list=[],
     pinned_list=[],
     link_list=[],
     konnected=[],
@@ -8047,93 +8338,108 @@
     """
     global current_hsh
     mk_goals = settings['keep_current'][0] > 0
     goals_width = settings['keep_current'][1] - 1
     rows = []
     path2sort = {
         'Active': 1,
-        'Inactive': 2,
-        'Ended': 3,
+        'Paused': 2,
+        'Upcoming': 3,
+        'Ended': 4,
     }
-    # goal_hsh = {} 
-    today = date.today()
+    today = datetime.today().astimezone()
     current_weekday = today.weekday()         # 0, 1, ..., 6
-    weekdays_remaining = 7 - current_weekday  # 7, 6, ..., 1 
+    # weekdays_remaining = 7 - current_weekday  # 7, 6, ..., 1 
     for item in db:
         itemtype = item.get('itemtype')
         if itemtype != '~':
             continue
         doc_id = item.doc_id
         total = 0
         count = 0
         summary = item.get('summary').strip()
         s = item.get('s', None)
-        q = item.get('q', [])
+        q = item.get('q', None)
         h = item.get('h', {})
         for k, v in h.items():
             count += 1
             total += int(v)
         average = f"{total/count:.2}" if count and total else 0
         path = None
         # status: current, paused, ended, bad
         
-        quota = q[0] if len(q) > 0 else None
         if not s or q is None:
             logger.error(f"bad goal: {item = }")
             continue
-        ss = s.timestamp()
-        weeks = q[1] if len(q) > 1 else None
+        quota = int(q[0]) 
+        period = q[1] if len(q) > 1 else 'w'
+        periods = q[2] if len(q) > 2 else 0
+
+        begin_date = get_period_begin_date(item['s'], period)
+        fraction_used = 0.0
+
+        if periods:
+            end_date = get_period_end_date(item['s'], period, periods)
 
-        if int(quota) == 0 or (weeks and (today - s.date()).days > weeks*7):
+        if quota == 0 or (
+            periods and end_date and today > end_date
+            ):
             path = 'Ended'
-            goal = f'({average})'
+            # goal = f'{average}/{quota}{period}'
+            goal = f'{period}'
             itemtype = EtmChar.ENDED_CHAR
         else:
-            this_week = today.isocalendar()[:2] 
-            this_week_str = f"{this_week[0]}:{this_week[1]:02}"
-            done = int(h.get(this_week_str, 0))
-            ss = done/abs(quota)
-            if int(quota) < 0 or s.date() > today:
-                path = 'Inactive' 
-                goal = f"{done}/{abs(quota)} ({average})"
+            this_period, fraction_used = get_fraction_of_period_passed(period)
+            # logger.debug(f"{begin_date = }; {this_period = }; {fraction_used = }")
+            # period = f"{fraction_used:.2}{period}"
+
+            # this_week = today.isocalendar()[:2] 
+            # this_week_str = f"{this_week[0]}:{this_week[1]:02}"
+            done = int(h.get(this_period, 0))
+            if quota < 0:
+                path = 'Paused' 
+                goal = f"{done}/{abs(quota)}{period}"
+                itemtype = EtmChar.INACTIVE_CHAR
+            elif begin_date > date_to_datetime(today):
+                path = 'Upcoming' 
+                goal = f"{done}/{abs(quota)}{period}"
                 itemtype = EtmChar.INACTIVE_CHAR
             else:
                 path = 'Active'
-                goal = f"{done}/{abs(quota)} ({average})"
+                goal = f"{done}/{abs(quota)}{period}"
                 itemtype='~'
 
-        if path == 'Active' and current_weekday >= 0:
-            fraction_done = done/abs(quota)
-            min_used = (current_weekday)/7 #  0, 1/7, ..., 6/7
-            max_used = (current_weekday+1)/7 # 1/7, 2/7, ..., 1
-            need = math.ceil(max_used*abs(quota) - done)
-            goal = f"{done}/{abs(quota)}+{need} ({average})" if need > 0 else f"{done}/{abs(quota)} ({average})"
-            if current_weekday == 0:
-                # Monday - don't warn about 0 completions
-                itemtype = '~'
-            elif fraction_done >= max_used:
-                # on target
-                itemtype = '~'
-            elif fraction_done >= min_used:
+        srt = 0
+        rep = ""
+        if path == 'Active':
+            srt = -fraction_used*abs(quota)
+            max_need = math.ceil(fraction_used*abs(quota) - done)
+            min_need = math.floor(fraction_used*abs(quota) - done)
+            goal = f"{done}/{abs(quota)}{period}" 
+            rep = f" ({min_need})" if min_need > 0 else ""
+            if min_need >= 2:
+                # behind
+                itemtype = EtmChar.LATE_CHAR
+            elif min_need >= 1:
                 # borderline
                 itemtype = EtmChar.SLOW_CHAR
             else:
-                # behind
-                itemtype = EtmChar.LATE_CHAR
+                # on target
+                itemtype = '~'
 
-        sort = (path2sort[path], ss, summary)
+        sort = (path2sort[path], srt, summary)
 
         flags = get_flags(
             doc_id, repeat_list, link_list, konnected, pinned_list, timers
         )
         rows.append(
             {
                 'sort': sort,
                 'path': path,
-                'values': [itemtype, f"{goal} {summary}", flags, '', doc_id],
+                'values': [itemtype, f"{goal} {summary}{rep}", flags, '', doc_id],
             }
         )
     rows.sort(key=itemgetter('sort'))
     rdict = NDict()
     for row in rows:
         path = row['path']
         values = row['values']
@@ -8612,15 +8918,14 @@
         week_numbers.append(yw)
         week_numbers.sort()
     aft_dt, bef_dt = get_period(dt, weeks_before, weeks_after)
 
     # for the individual weeks
     agenda_hsh = {}     # yw -> agenda_view
     done_hsh = {}       # yw -> done_view
-    # goal_hsh = {}       # yw -> list of goal completions for the week
     busy_hsh = {}       # yw -> busy_view
     row2id_hsh = {}     # yw -> row2id
     done2id_hsh = {}     # yw -> row2id
     goal2id_hsh = {}     # yw -> row2id
     effort_hsh = {}
     effort2id_hsh = {}     # yw -> row2id
     week2day2effort = {}   # year, week -> dayofweek -> period total for day
@@ -8796,16 +9101,19 @@
             continue
 
         # XXX INSTANCES
 
         # keep these for reference for this item
         end_dt = None
 
-        for dt, et in item_instances(item, aft_dt, bef_dt):
-
+        logger.debug(f"schedule */* {item = }")
+        instances = item_instances(item, aft_dt, bef_dt) 
+        instances.sort()
+        logger.debug(f"schedule */* {instances = }")
+        for dt, et in instances:
             yr, wk, dayofweek = dt.isocalendar()
             week = (yr, wk)
             wk_fmt = fmt_week(week).center(width, ' ').rstrip()
             itemday = dt.strftime('%Y%m%d')
             dayDM = format_wkday(dt)
             if itemday == todayYMD:
                 dayDM += ' (Today)'
@@ -9406,23 +9714,25 @@
 Documentation:  dagraham.github.io/etm-dgraham
 PyPi:           pypi.org/project/etm-dgraham
 GitHub:         github.com/dagraham/etm-dgraham
 Developer:      dnlgrhm@gmail.com
 
 {copyright}\
 """
+    userhome = os.path.expanduser('~')
+    sys_argv = os.path.join('~', os.path.relpath(sys.argv[0], userhome)) 
     which_etm = "?"
     ok, msg = check_output('which etm')
     if ok:
-        userhome = os.path.expanduser('~')
         which_etm = os.path.join('~', os.path.relpath(msg, userhome))
 
     ret2 = f"""\
  etm home:           {etmhome}
  path to etm:        {which_etm}\
+ sys_argv[0]:        {sys_argv}
 {VERSION_INFO}
 """
     return ret1, ret2
 
 
 dataview = None
 item = None
```

### Comparing `etm-dgraham-6.2.7/etm/options.py` & `etm-dgraham-6.3.0/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/etm/report.py` & `etm-dgraham-6.3.0/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/etm/view.py` & `etm-dgraham-6.3.0/etm/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1457,14 +1457,15 @@
         ]
     dataview.get_completions()
     dataview.update_konnections(item)
     data_changed(loop)
 
 
 def data_changed(loop):
+    dataview.last_modified = time.time()
     dataview.refreshRelevant()
     dataview.refreshAgenda()
     set_text(dataview.show_active_view())
     dataview.refreshCurrent()
     if dataview.current_row:
         text_area.buffer.cursor_position = (
             text_area.buffer.document.translate_row_col_to_index(
@@ -1503,15 +1504,15 @@
     alert_hsh = {}
     now = datetime.now().astimezone()
     #            0            1         2          3         4       5
     # alerts: alert time, start time, commands, itemtype, summary, doc_id
     for alert in dataview.alerts:
         trigger_time = alert[0]
         start_time = alert[1]
-        logger.debug(f"{alert[4] = }; {trigger_time = }; {now = }; {(trigger_time.replace(tzinfo=None) < now.replace(tzinfo=None)) = }")
+        # logger.debug(f"{alert[4] = }; {trigger_time = }; {now = }; {(trigger_time.replace(tzinfo=None) < now.replace(tzinfo=None)) = }")
         if start_time.date() == now.date():
             start = format_time(start_time)[1]
         else:
             start = format_datetime(start_time, short=True)[1]
         trigger = format_time(trigger_time)[1]
         command = ', '.join(alert[2])
         itemtype = alert[3]
@@ -2801,15 +2802,15 @@
     
     hsh = DBITEM.get(doc_id=doc_id)
     if hsh['itemtype'] != '~':
         return 
     
     changed = item.end_goal(doc_id)
     if changed:
-        show_message('Toggle Paused', 'Toggled the paused status of the goal')
+        show_message('Ended', 'Ended the goal')
         # set_text(dataview.show_active_view())
         loop = asyncio.get_event_loop()
         loop.call_later(0, data_changed, loop)
 
     return
 
 
@@ -2842,18 +2843,16 @@
         # incrementing completions of a goal
         changed = item.increment_goal(doc_id)
         if changed:
             # show_message('Finish', 'Incremented tally for goal')
             # set_text(dataview.show_active_view())
             loop = asyncio.get_event_loop()
             loop.call_later(0, data_changed, loop)
-
         return
 
-
     if hsh['itemtype'] != '-' or 'f' in hsh:
         show_message('Finish', 'Only an unfinished task can be finished.')
         return
 
     # has_timer = doc_id in dataview.timers
     # timer_warning = " and\nits associated timer" if has_timer else ""
     repeating = 's' in hsh and ('r' in hsh or '+' in hsh)
```

### Comparing `etm-dgraham-6.2.7/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-6.3.0/etm_dgraham.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.2.7
+Version: 6.3.0
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -637,15 +637,15 @@
 In the main window, active goals are sorted by their done/quota ratios and given a color indicating the degree of progress toward completing the goal for the current week based on comparing the done/quota fraction to the fraction of the week that has passed. Since the current weekday, Friday, is the 5th day of the week, the fraction of the week that has passed is somewhere between 4/7 (beginning of Friday) and 5/7 (end of Friday).   
 - walk the dog:  colored red because 3/7 is less than 4/7 and thus completions are unambiguously behind schedule for the week - 2 completions today are needed to get back on schedule.
 - wash dishes: colored yellow because 3/5 is between 4/7 and 5/7 - 1 completion today is needed to get back on schedule.
 - interval training: blue because 3/4 > 5/7 and thus completions are ahead of schedule for this week - no completions are needed today to stay on schedule.
 
 This is a normal view in etm and all the normal commands are available. Additionally, these commands are available when a goal is selected:
 - F:  increment the completion count for the current week (by incrementing the count for the current week in @h).
-- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of weeks that has expired) are regarded as *ended*.
+- ^e: end the goal by setting the quota component of `@q` equal to zero. Goals with zero quotas (or goals with quotas specifying a number of weeks that has expired) are regarded as *ended*. Ending a goal instead of deleting it preserves its history of completions.
 - ^a: toggle the active/inactive status by reversing the sign of the quota component of @q. Goals with negative quotas are regarded as *inactive*. 
 
 A *goal* could, of course, be deleted but this would also delete the history of completions. Ending the goal, on the other hand, preserves the history and places the goal in it's own category at the bottom of the list. And, if you ever want to un-end the goal, just change the zero quota to whatever you like. Similarly, making a goal inactive while you're away on vacation and then making it active again when you return preserves its history and the two key presses required is significantly more convenient than deleting and re-creating the goal.
 
 [↺ contents](#contents)
 
 ### Timer View {#timer-view}
@@ -1796,24 +1796,24 @@
 ### goal {#goal}
 
 Type character: **~**
 
 The goal itemtype is intended to support pursuing S.M.A.R.T. goals (Specific, Measurable, Achievable, Relevant, Timed) in *etm*. Here is an example of a *goal* as it would be entered:
 
 ```
-    ~ interval training @s 2024/4/22 @q 3
+    ~ interval training @s 2024/4/22 @q 3w
 ```
 - It is a *goal* because of the `~` type character. 
 - Because I have a custom interval setting on my exercise bike, "interval training" is *specific* and *measurable*. It is also *achievable* and *relevant* for me.
-- The `@s` entry is required and times the goal to begin on Monday, April 22, 2024. Whatever date is entered will be automatically converted to the Monday of the corresponding week.
-- The `@q` entry is also required and sets to quota for this goal to 3 times per week, repeating indefinitely. Had the quota instead been, say, `@q 3, 5`  then the goal would have been 3 times per week repeated for 5 weeks.
+- The `@s` entry is required and times the goal to begin on Monday, April 22, 2024. Whatever date is entered will be automatically be interpreted as the corresponding week.
+- The `@q` entry is also required and sets to quota for this goal to 3 times per week, repeating indefinitely. Had the quota instead been, say, `@q 3w, 5`  then the goal would have been 5 times per week repeated for 5 weeks. Instead of using 'w' for weekly, it is also possible to use 'y' for yearly, 'q' for quarterly or 'm' for monthly.
 - If this goal were selected in *etm* on, say, Wednesday, April 24 and "F" were pressed, then *etm* would add an `@h 2024:17 1` (history of completions) entry to indicate 1 completion of the goal for the week of *2024:17*. Pressing "F" again in the same week with this goal selected would change this entry to `@h 2024:17 2`.  As one last example, pressing "F" with the goal selected sometime during the week of *2024:18* would leave the recorded entry as
 
     ```
-    ~ interval training @s 2024/4/29 @q 3 @h 2024:17 2, 2024:18 1
+    ~ interval training @s 2024/4/29 @q 3w @h 2024:17 2, 2024:18 1
     ```
 
 [↺ contents](#contents)
 
 ### inbox {#inbox}
 
 Type character: **!**
```

### Comparing `etm-dgraham-6.2.7/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-6.3.0/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-6.3.0/etm_dgraham.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 etm/__version__.py
 etm/common.py
 etm/data.py
 etm/make_examples.py
 etm/model.py
 etm/options.py
 etm/report.py
+etm/rrule-test.py
+etm/rruleset-test.py
 etm/view.py
 etm_dgraham.egg-info/PKG-INFO
 etm_dgraham.egg-info/PKG-INFO [conflicted]
 etm_dgraham.egg-info/SOURCES [conflicted].txt
 etm_dgraham.egg-info/SOURCES.txt
 etm_dgraham.egg-info/dependency_links.txt
 etm_dgraham.egg-info/entry_points.txt
```

### Comparing `etm-dgraham-6.2.7/etmlogo.png` & `etm-dgraham-6.3.0/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/etmlogo_small.png` & `etm-dgraham-6.3.0/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/etmview_agenda.png` & `etm-dgraham-6.3.0/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/namedcolors.py` & `etm-dgraham-6.3.0/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/new.png` & `etm-dgraham-6.3.0/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/setup.py` & `etm-dgraham-6.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/test/test_parser.py` & `etm-dgraham-6.3.0/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/utilities/colons_to_slashes.py` & `etm-dgraham-6.3.0/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/utilities/etm_in` & `etm-dgraham-6.3.0/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/utilities/inbasket` & `etm-dgraham-6.3.0/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.7/utilities/open_in_mutt` & `etm-dgraham-6.3.0/utilities/open_in_mutt`

 * *Files identical despite different names*

