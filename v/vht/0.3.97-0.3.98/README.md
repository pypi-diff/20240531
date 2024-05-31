# Comparing `tmp/vht-0.3.97.tar.gz` & `tmp/vht-0.3.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vht-0.3.97.tar", last modified: Fri May 31 14:45:53 2024, max compression
+gzip compressed data, was "vht-0.3.98.tar", last modified: Fri May 31 19:11:27 2024, max compression
```

## Comparing `vht-0.3.97.tar` & `vht-0.3.98.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 14:45:53.812084 vht-0.3.97/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    35148 2024-05-08 12:01:32.000000 vht-0.3.97/LICENSE
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       49 2024-05-08 12:01:32.000000 vht-0.3.97/MANIFEST.in
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1894 2024-05-31 14:45:53.812084 vht-0.3.97/PKG-INFO
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1147 2024-05-28 20:35:49.000000 vht-0.3.97/README.md
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 14:45:53.796084 vht-0.3.97/data/
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 14:45:53.796084 vht-0.3.97/data/bank/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2430 2024-05-08 12:01:32.000000 vht-0.3.97/data/bank/10-gm1
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4875 2024-05-08 12:01:32.000000 vht-0.3.97/data/bank/20-gm2
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 14:45:53.796084 vht-0.3.97/data/ctrl/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      294 2024-05-08 12:01:32.000000 vht-0.3.97/data/ctrl/10-gm
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      166 2024-05-08 12:01:32.000000 vht-0.3.97/data/ctrl/20-zyn
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4550 2024-05-08 12:01:32.000000 vht-0.3.97/data/mandy.png
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1246 2024-05-08 12:01:32.000000 vht-0.3.97/data/menu.ui
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1112 2024-05-31 14:19:09.000000 vht-0.3.97/data/menu_norend.ui
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      318 2024-05-29 20:04:45.000000 vht-0.3.97/data/net.sourceforge.projects.vht.desktop
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2938 2024-05-31 14:28:51.000000 vht-0.3.97/data/net.sourceforge.projects.vht.metainfo.xml
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4458 2024-05-29 19:42:46.000000 vht-0.3.97/data/net.sourceforge.projects.vht.svg
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    11176 2024-05-08 12:01:32.000000 vht-0.3.97/data/vht.png
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4458 2024-05-08 12:01:32.000000 vht-0.3.97/data/vht.svg
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 14:45:53.796084 vht-0.3.97/doc/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2362 2024-05-31 14:25:41.000000 vht-0.3.97/doc/vht.1.gz
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4641 2024-05-31 14:23:55.000000 vht-0.3.97/doc/vht.1.md
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 14:45:53.804083 vht-0.3.97/libvht/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       75 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/__init__.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1538 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/ctrlrow.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1416 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/ctrlrow.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7088 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/envelope.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1612 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/envelope.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2121 2024-05-29 20:50:11.000000 vht-0.3.97/libvht/jack_process.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1212 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/jack_process.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19982 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/libcvht.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    32223 2024-05-31 14:45:41.000000 vht-0.3.97/libvht/libcvht.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)   481702 2024-05-31 14:45:41.000000 vht-0.3.97/libvht/libcvht_wrap.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7542 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/libvht.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    34594 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/mandy.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6088 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/mandy.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2354 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/mandy_pix_scan.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1001 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/mandy_pix_scan.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7405 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/mandy_trk_disp.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      986 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/mandy_trk_disp.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    17045 2024-05-27 12:13:59.000000 vht-0.3.97/libvht/midi_client.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4531 2024-05-27 12:12:54.000000 vht-0.3.97/libvht/midi_client.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3496 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/midi_event.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1540 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/midi_event.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    15996 2024-05-27 12:02:48.000000 vht-0.3.97/libvht/module.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3256 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/module.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3029 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/row.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1670 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/row.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    28972 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/sequence.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4503 2024-05-15 11:24:39.000000 vht-0.3.97/libvht/sequence.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6493 2024-05-08 12:02:30.000000 vht-0.3.97/libvht/smf.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1680 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/smf.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2912 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/stolen.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    29373 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/timeline.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4538 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/timeline.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    41038 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/track.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4153 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/track.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4675 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/tracy.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2370 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/tracy.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1882 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhtcolumn.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2639 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhtctrl.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2012 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhtctrllist.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3639 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhtctrlrow.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1973 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhtextras.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6566 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhtmandy.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    21144 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhtmodule.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3432 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhtport.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2404 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhtports.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1922 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhtquicklist.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5623 2024-05-27 12:45:52.000000 vht-0.3.97/libvht/vhtrow.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    10975 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhtsequence.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3751 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhttimeline.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1887 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhttimelinechange.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2204 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhttimelinechanges.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1686 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhttimelineloop.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1913 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhttimelineslices.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5262 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhttimelinestrip.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3637 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhttimelinestrips.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1454 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhttimelineticks.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9143 2024-05-27 13:05:52.000000 vht-0.3.97/libvht/vhttrack.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2270 2024-05-08 12:01:32.000000 vht-0.3.97/libvht/vhttracy.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1941 2024-05-31 14:27:07.000000 vht-0.3.97/pyproject.toml
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       70 2024-05-31 14:45:53.812084 vht-0.3.97/setup.cfg
--rwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)     1998 2024-05-31 14:26:28.000000 vht-0.3.97/setup.py
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 14:45:53.808084 vht-0.3.97/vht/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      124 2024-05-08 12:01:32.000000 vht-0.3.97/vht/__init__.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1088 2024-05-08 12:01:32.000000 vht-0.3.97/vht/autoexec.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3531 2024-05-08 12:01:32.000000 vht-0.3.97/vht/bankcfg.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1688 2024-05-08 12:01:32.000000 vht-0.3.97/vht/capturebutton.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3834 2024-05-08 12:01:32.000000 vht-0.3.97/vht/codedaemon.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    24274 2024-05-08 12:01:32.000000 vht-0.3.97/vht/configuration.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5836 2024-05-08 12:01:32.000000 vht-0.3.97/vht/console.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    55124 2024-05-09 10:48:54.000000 vht-0.3.97/vht/controllereditor.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6976 2024-05-08 12:01:32.000000 vht-0.3.97/vht/controllersview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5707 2024-05-08 12:01:32.000000 vht-0.3.97/vht/controllersviewrow.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4560 2024-05-08 12:01:32.000000 vht-0.3.97/vht/controllerundobuffer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2909 2024-05-08 12:01:32.000000 vht-0.3.97/vht/ctrlcfg.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1910 2024-05-08 12:01:32.000000 vht-0.3.97/vht/extras.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1298 2024-05-08 12:01:32.000000 vht-0.3.97/vht/filerotator.py
--rwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)    11519 2024-05-31 14:34:24.000000 vht-0.3.97/vht/main.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    18736 2024-05-31 14:20:00.000000 vht-0.3.97/vht/mainwin.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    14192 2024-05-08 12:01:32.000000 vht-0.3.97/vht/mandymenu.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    18144 2024-05-08 12:01:32.000000 vht-0.3.97/vht/mandyview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2401 2024-05-08 12:01:32.000000 vht-0.3.97/vht/midimapview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4176 2024-05-08 12:01:32.000000 vht-0.3.97/vht/midimapviewrow.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1299 2024-05-08 12:01:32.000000 vht-0.3.97/vht/notebooklabel.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4721 2024-05-08 12:01:32.000000 vht-0.3.97/vht/poormanspiano.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2677 2024-05-08 12:01:32.000000 vht-0.3.97/vht/portconfig.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3547 2024-05-08 12:01:32.000000 vht-0.3.97/vht/portconfigpopover.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7770 2024-05-28 19:34:11.000000 vht-0.3.97/vht/portconfigview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    24678 2024-05-28 18:53:13.000000 vht-0.3.97/vht/preferenceswin.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6623 2024-05-08 12:01:32.000000 vht-0.3.97/vht/probeditor.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4996 2024-05-08 12:01:32.000000 vht-0.3.97/vht/propview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1035 2024-05-08 12:01:32.000000 vht-0.3.97/vht/pulsar.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1100 2024-05-08 12:01:32.000000 vht-0.3.97/vht/randomcomposer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     8188 2024-05-28 20:16:35.000000 vht-0.3.97/vht/renderer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9640 2024-05-27 12:29:20.000000 vht-0.3.97/vht/renderwin.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    15715 2024-05-08 12:01:32.000000 vht-0.3.97/vht/sequencelistview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    13404 2024-05-29 20:09:20.000000 vht-0.3.97/vht/sequencelistviewpopover.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    11262 2024-05-08 12:01:32.000000 vht-0.3.97/vht/sequencepropviewpopover.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    12223 2024-05-08 12:01:32.000000 vht-0.3.97/vht/sequencetriggersview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    37321 2024-05-08 12:01:32.000000 vht-0.3.97/vht/sequenceview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6644 2024-05-29 18:59:49.000000 vht-0.3.97/vht/shortcutmayhem.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    20316 2024-05-08 12:01:32.000000 vht-0.3.97/vht/sidetrackview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19612 2024-05-08 12:01:32.000000 vht-0.3.97/vht/statusbar.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2879 2024-05-08 12:01:32.000000 vht-0.3.97/vht/thumbmanager.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    51601 2024-05-08 12:01:32.000000 vht-0.3.97/vht/timelineview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6308 2024-05-08 12:01:32.000000 vht-0.3.97/vht/timeshifteditor.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    22027 2024-05-08 12:01:32.000000 vht-0.3.97/vht/trackpropview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    31965 2024-05-08 12:01:32.000000 vht-0.3.97/vht/trackpropviewpopover.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3229 2024-05-08 12:01:32.000000 vht-0.3.97/vht/trackundobuffer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    96428 2024-05-15 11:23:14.000000 vht-0.3.97/vht/trackview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9212 2024-05-08 12:01:32.000000 vht-0.3.97/vht/trackviewpointer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     8127 2024-05-08 12:01:32.000000 vht-0.3.97/vht/velocityeditor.py
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 14:45:53.808084 vht-0.3.97/vht.egg-info/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1894 2024-05-31 14:45:53.000000 vht-0.3.97/vht.egg-info/PKG-INFO
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2630 2024-05-31 14:45:53.000000 vht-0.3.97/vht.egg-info/SOURCES.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)        1 2024-05-31 14:45:53.000000 vht-0.3.97/vht.egg-info/dependency_links.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       38 2024-05-31 14:45:53.000000 vht-0.3.97/vht.egg-info/entry_points.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       27 2024-05-31 14:45:53.000000 vht-0.3.97/vht.egg-info/top_level.txt
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 19:11:27.447756 vht-0.3.98/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    35148 2024-05-08 12:01:32.000000 vht-0.3.98/LICENSE
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       49 2024-05-08 12:01:32.000000 vht-0.3.98/MANIFEST.in
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1894 2024-05-31 19:11:27.447756 vht-0.3.98/PKG-INFO
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1147 2024-05-28 20:35:49.000000 vht-0.3.98/README.md
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 19:11:27.435761 vht-0.3.98/data/
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 19:11:27.435761 vht-0.3.98/data/bank/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2430 2024-05-08 12:01:32.000000 vht-0.3.98/data/bank/10-gm1
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4875 2024-05-08 12:01:32.000000 vht-0.3.98/data/bank/20-gm2
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 19:11:27.435761 vht-0.3.98/data/ctrl/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      294 2024-05-08 12:01:32.000000 vht-0.3.98/data/ctrl/10-gm
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      166 2024-05-08 12:01:32.000000 vht-0.3.98/data/ctrl/20-zyn
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      310 2024-05-31 18:57:53.000000 vht-0.3.98/data/io.github.rdybka.vht.desktop
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2930 2024-05-31 19:00:17.000000 vht-0.3.98/data/io.github.rdybka.vht.metainfo.xml
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4458 2024-05-29 19:42:46.000000 vht-0.3.98/data/io.github.rdybka.vht.svg
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4550 2024-05-08 12:01:32.000000 vht-0.3.98/data/mandy.png
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1246 2024-05-08 12:01:32.000000 vht-0.3.98/data/menu.ui
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1112 2024-05-31 14:19:09.000000 vht-0.3.98/data/menu_norend.ui
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    11176 2024-05-08 12:01:32.000000 vht-0.3.98/data/vht.png
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4458 2024-05-08 12:01:32.000000 vht-0.3.98/data/vht.svg
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 19:11:27.435761 vht-0.3.98/doc/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2362 2024-05-31 19:11:17.000000 vht-0.3.98/doc/vht.1.gz
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4641 2024-05-31 18:57:24.000000 vht-0.3.98/doc/vht.1.md
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 19:11:27.443757 vht-0.3.98/libvht/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       75 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/__init__.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1538 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/ctrlrow.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1416 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/ctrlrow.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7088 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/envelope.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1612 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/envelope.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2121 2024-05-29 20:50:11.000000 vht-0.3.98/libvht/jack_process.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1212 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/jack_process.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19982 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/libcvht.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    32223 2024-05-31 19:11:16.000000 vht-0.3.98/libvht/libcvht.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)   481702 2024-05-31 19:11:16.000000 vht-0.3.98/libvht/libcvht_wrap.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7542 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/libvht.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    34594 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/mandy.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6088 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/mandy.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2354 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/mandy_pix_scan.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1001 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/mandy_pix_scan.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7405 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/mandy_trk_disp.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      986 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/mandy_trk_disp.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    17045 2024-05-27 12:13:59.000000 vht-0.3.98/libvht/midi_client.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4531 2024-05-27 12:12:54.000000 vht-0.3.98/libvht/midi_client.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3496 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/midi_event.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1540 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/midi_event.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    15996 2024-05-27 12:02:48.000000 vht-0.3.98/libvht/module.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3256 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/module.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3029 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/row.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1670 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/row.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    28972 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/sequence.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4503 2024-05-15 11:24:39.000000 vht-0.3.98/libvht/sequence.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6493 2024-05-08 12:02:30.000000 vht-0.3.98/libvht/smf.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1680 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/smf.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2912 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/stolen.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    29373 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/timeline.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4538 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/timeline.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    41038 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/track.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4153 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/track.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4675 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/tracy.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2370 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/tracy.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1882 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhtcolumn.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2639 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhtctrl.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2012 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhtctrllist.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3639 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhtctrlrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1973 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhtextras.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6566 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhtmandy.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    21144 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhtmodule.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3432 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhtport.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2404 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhtports.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1922 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhtquicklist.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5623 2024-05-27 12:45:52.000000 vht-0.3.98/libvht/vhtrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    10975 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhtsequence.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3751 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhttimeline.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1887 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhttimelinechange.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2204 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhttimelinechanges.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1686 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhttimelineloop.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1913 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhttimelineslices.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5262 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhttimelinestrip.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3637 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhttimelinestrips.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1454 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhttimelineticks.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9143 2024-05-27 13:05:52.000000 vht-0.3.98/libvht/vhttrack.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2270 2024-05-08 12:01:32.000000 vht-0.3.98/libvht/vhttracy.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1909 2024-05-31 19:00:58.000000 vht-0.3.98/pyproject.toml
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       70 2024-05-31 19:11:27.447756 vht-0.3.98/setup.cfg
+-rwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)     1974 2024-05-31 18:56:14.000000 vht-0.3.98/setup.py
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 19:11:27.447756 vht-0.3.98/vht/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      124 2024-05-08 12:01:32.000000 vht-0.3.98/vht/__init__.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1088 2024-05-08 12:01:32.000000 vht-0.3.98/vht/autoexec.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3531 2024-05-08 12:01:32.000000 vht-0.3.98/vht/bankcfg.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1688 2024-05-08 12:01:32.000000 vht-0.3.98/vht/capturebutton.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3834 2024-05-08 12:01:32.000000 vht-0.3.98/vht/codedaemon.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    24274 2024-05-08 12:01:32.000000 vht-0.3.98/vht/configuration.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5836 2024-05-08 12:01:32.000000 vht-0.3.98/vht/console.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    55124 2024-05-09 10:48:54.000000 vht-0.3.98/vht/controllereditor.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6976 2024-05-08 12:01:32.000000 vht-0.3.98/vht/controllersview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5707 2024-05-08 12:01:32.000000 vht-0.3.98/vht/controllersviewrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4560 2024-05-08 12:01:32.000000 vht-0.3.98/vht/controllerundobuffer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2909 2024-05-08 12:01:32.000000 vht-0.3.98/vht/ctrlcfg.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1910 2024-05-08 12:01:32.000000 vht-0.3.98/vht/extras.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1298 2024-05-08 12:01:32.000000 vht-0.3.98/vht/filerotator.py
+-rwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)    11519 2024-05-31 14:34:24.000000 vht-0.3.98/vht/main.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    18736 2024-05-31 14:20:00.000000 vht-0.3.98/vht/mainwin.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    14192 2024-05-08 12:01:32.000000 vht-0.3.98/vht/mandymenu.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    18144 2024-05-08 12:01:32.000000 vht-0.3.98/vht/mandyview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2401 2024-05-08 12:01:32.000000 vht-0.3.98/vht/midimapview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4176 2024-05-08 12:01:32.000000 vht-0.3.98/vht/midimapviewrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1299 2024-05-08 12:01:32.000000 vht-0.3.98/vht/notebooklabel.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4721 2024-05-08 12:01:32.000000 vht-0.3.98/vht/poormanspiano.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2677 2024-05-08 12:01:32.000000 vht-0.3.98/vht/portconfig.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3547 2024-05-08 12:01:32.000000 vht-0.3.98/vht/portconfigpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7770 2024-05-28 19:34:11.000000 vht-0.3.98/vht/portconfigview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    24678 2024-05-28 18:53:13.000000 vht-0.3.98/vht/preferenceswin.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6623 2024-05-08 12:01:32.000000 vht-0.3.98/vht/probeditor.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4996 2024-05-08 12:01:32.000000 vht-0.3.98/vht/propview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1035 2024-05-08 12:01:32.000000 vht-0.3.98/vht/pulsar.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1100 2024-05-08 12:01:32.000000 vht-0.3.98/vht/randomcomposer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     8188 2024-05-28 20:16:35.000000 vht-0.3.98/vht/renderer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9640 2024-05-27 12:29:20.000000 vht-0.3.98/vht/renderwin.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    15715 2024-05-08 12:01:32.000000 vht-0.3.98/vht/sequencelistview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    13404 2024-05-29 20:09:20.000000 vht-0.3.98/vht/sequencelistviewpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    11262 2024-05-08 12:01:32.000000 vht-0.3.98/vht/sequencepropviewpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    12223 2024-05-08 12:01:32.000000 vht-0.3.98/vht/sequencetriggersview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    37321 2024-05-08 12:01:32.000000 vht-0.3.98/vht/sequenceview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6644 2024-05-29 18:59:49.000000 vht-0.3.98/vht/shortcutmayhem.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    20316 2024-05-08 12:01:32.000000 vht-0.3.98/vht/sidetrackview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19612 2024-05-08 12:01:32.000000 vht-0.3.98/vht/statusbar.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2879 2024-05-08 12:01:32.000000 vht-0.3.98/vht/thumbmanager.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    51601 2024-05-08 12:01:32.000000 vht-0.3.98/vht/timelineview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6308 2024-05-08 12:01:32.000000 vht-0.3.98/vht/timeshifteditor.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    22027 2024-05-08 12:01:32.000000 vht-0.3.98/vht/trackpropview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    31965 2024-05-08 12:01:32.000000 vht-0.3.98/vht/trackpropviewpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3229 2024-05-08 12:01:32.000000 vht-0.3.98/vht/trackundobuffer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    96428 2024-05-15 11:23:14.000000 vht-0.3.98/vht/trackview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9212 2024-05-08 12:01:32.000000 vht-0.3.98/vht/trackviewpointer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     8127 2024-05-08 12:01:32.000000 vht-0.3.98/vht/velocityeditor.py
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2024-05-31 19:11:27.447756 vht-0.3.98/vht.egg-info/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1894 2024-05-31 19:11:27.000000 vht-0.3.98/vht.egg-info/PKG-INFO
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2606 2024-05-31 19:11:27.000000 vht-0.3.98/vht.egg-info/SOURCES.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)        1 2024-05-31 19:11:27.000000 vht-0.3.98/vht.egg-info/dependency_links.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       38 2024-05-31 19:11:27.000000 vht-0.3.98/vht.egg-info/entry_points.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       27 2024-05-31 19:11:27.000000 vht-0.3.98/vht.egg-info/top_level.txt
```

### Comparing `vht-0.3.97/LICENSE` & `vht-0.3.98/LICENSE`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/PKG-INFO` & `vht-0.3.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vht
-Version: 0.3.97
+Version: 0.3.98
 Summary: vahatraker - a live MIDI sequencer for pipewire/JACK
 Home-page: https://github.com/rdybka/vht
 Author: Remigiusz Dybka
 Author-email: remigiusz.dybka@gmail.com
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vht-0.3.97/README.md` & `vht-0.3.98/README.md`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/data/bank/10-gm1` & `vht-0.3.98/data/bank/10-gm1`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/data/bank/20-gm2` & `vht-0.3.98/data/bank/20-gm2`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/data/mandy.png` & `vht-0.3.98/data/mandy.png`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/data/menu.ui` & `vht-0.3.98/data/menu.ui`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/data/menu_norend.ui` & `vht-0.3.98/data/menu_norend.ui`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/data/net.sourceforge.projects.vht.metainfo.xml` & `vht-0.3.98/data/io.github.rdybka.vht.metainfo.xml`

 * *Files 1% similar despite different names*

#### Comparing `vht-0.3.97/data/net.sourceforge.projects.vht.metainfo.xml` & `vht-0.3.98/data/io.github.rdybka.vht.metainfo.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <component type="desktop-application">
-  <id>net.sourceforge.projects.vht</id>
+  <id>io.github.rdybka.vht</id>
   <developer id="com.github.rdybka">
     <name>Remigiusz Dybka</name>
   </developer>
   <name>vahatraker</name>
   <summary>Live MIDI sequencer</summary>
   <metadata_license>CC0-1.0</metadata_license>
   <project_license>GPL-3.0-or-later</project_license>
@@ -29,15 +29,15 @@
     </screenshot>
     <screenshot>
       <image>https://a.fsdn.com/con/app/proj/vht/screenshots/vhtscrn2.png/max/max/1</image>
     </screenshot>
   </screenshots>
   <content_rating type="oars-1.1"/>
   <releases>
-    <release version="0.3.97" date="2024-05-31">
+    <release version="0.3.98" date="2024-05-31">
       <description>
         <p>Flatpak version zero</p>
       </description>
     </release>
     <release version="0.3.96" date="2024-05-30">
       <description>
         <p>Pipewire integration</p>
```

### Comparing `vht-0.3.97/data/net.sourceforge.projects.vht.svg` & `vht-0.3.98/data/io.github.rdybka.vht.svg`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/data/vht.png` & `vht-0.3.98/data/vht.png`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/data/vht.svg` & `vht-0.3.98/data/vht.svg`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/doc/vht.1.gz` & `vht-0.3.98/doc/vht.1.gz`

 * *Files 3% similar despite different names*

#### filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vht.1", last modified: Fri May 31 14:25:41 2024, from Unix
+gzip compressed data, was "vht.1", last modified: Fri May 31 19:11:17 2024, from Unix
```

#### vht.1

```diff
@@ -1,10 +1,10 @@
 .\" Automatically generated by Pandoc 2.9.2.1
 .\"
-.TH "VHT" "1" "May 2024" "vht 0.3.97" ""
+.TH "VHT" "1" "May 2024" "vht 0.3.98" ""
 .hy
 .SH NAME
 .PP
 \f[B]vht\f[R] - a minimalistic MIDI sequencer for JACK/GNOME
 .SH SYNOPSIS
 .PP
 \f[B]vht\f[R] [file]
```

### Comparing `vht-0.3.97/doc/vht.1.md` & `vht-0.3.98/doc/vht.1.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-% VHT(1) vht 0.3.97
+% VHT(1) vht 0.3.98
 % Remigiusz Dybka
 % May 2024
 
 # NAME
 **vht** - a minimalistic MIDI sequencer for JACK/GNOME
 
 # SYNOPSIS
```

### Comparing `vht-0.3.97/libvht/ctrlrow.c` & `vht-0.3.98/libvht/ctrlrow.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/ctrlrow.h` & `vht-0.3.98/libvht/ctrlrow.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/envelope.c` & `vht-0.3.98/libvht/envelope.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/envelope.h` & `vht-0.3.98/libvht/envelope.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/jack_process.c` & `vht-0.3.98/libvht/jack_process.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/jack_process.h` & `vht-0.3.98/libvht/jack_process.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/libcvht.h` & `vht-0.3.98/libvht/libcvht.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/libcvht.py` & `vht-0.3.98/libvht/libcvht.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/libcvht_wrap.c` & `vht-0.3.98/libvht/libcvht_wrap.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/libvht.c` & `vht-0.3.98/libvht/libvht.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/mandy.c` & `vht-0.3.98/libvht/mandy.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/mandy.h` & `vht-0.3.98/libvht/mandy.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/mandy_pix_scan.c` & `vht-0.3.98/libvht/mandy_pix_scan.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/mandy_pix_scan.h` & `vht-0.3.98/libvht/mandy_pix_scan.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/mandy_trk_disp.c` & `vht-0.3.98/libvht/mandy_trk_disp.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/mandy_trk_disp.h` & `vht-0.3.98/libvht/mandy_trk_disp.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/midi_client.c` & `vht-0.3.98/libvht/midi_client.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/midi_client.h` & `vht-0.3.98/libvht/midi_client.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/midi_event.c` & `vht-0.3.98/libvht/midi_event.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/midi_event.h` & `vht-0.3.98/libvht/midi_event.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/module.c` & `vht-0.3.98/libvht/module.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/module.h` & `vht-0.3.98/libvht/module.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/row.c` & `vht-0.3.98/libvht/row.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/row.h` & `vht-0.3.98/libvht/row.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/sequence.c` & `vht-0.3.98/libvht/sequence.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/sequence.h` & `vht-0.3.98/libvht/sequence.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/smf.c` & `vht-0.3.98/libvht/smf.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/smf.h` & `vht-0.3.98/libvht/smf.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/stolen.c` & `vht-0.3.98/libvht/stolen.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/timeline.c` & `vht-0.3.98/libvht/timeline.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/timeline.h` & `vht-0.3.98/libvht/timeline.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/track.c` & `vht-0.3.98/libvht/track.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/track.h` & `vht-0.3.98/libvht/track.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/tracy.c` & `vht-0.3.98/libvht/tracy.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/tracy.h` & `vht-0.3.98/libvht/tracy.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhtcolumn.py` & `vht-0.3.98/libvht/vhtcolumn.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhtctrl.py` & `vht-0.3.98/libvht/vhtctrl.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhtctrllist.py` & `vht-0.3.98/libvht/vhtctrllist.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhtctrlrow.py` & `vht-0.3.98/libvht/vhtctrlrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhtextras.py` & `vht-0.3.98/libvht/vhtextras.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhtmandy.py` & `vht-0.3.98/libvht/vhtmandy.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhtmodule.py` & `vht-0.3.98/libvht/vhtmodule.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhtport.py` & `vht-0.3.98/libvht/vhtport.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhtports.py` & `vht-0.3.98/libvht/vhtports.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhtquicklist.py` & `vht-0.3.98/libvht/vhtquicklist.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhtrow.py` & `vht-0.3.98/libvht/vhtrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhtsequence.py` & `vht-0.3.98/libvht/vhtsequence.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhttimeline.py` & `vht-0.3.98/libvht/vhttimeline.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhttimelinechange.py` & `vht-0.3.98/libvht/vhttimelinechange.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhttimelinechanges.py` & `vht-0.3.98/libvht/vhttimelinechanges.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhttimelineloop.py` & `vht-0.3.98/libvht/vhttimelineloop.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhttimelineslices.py` & `vht-0.3.98/libvht/vhttimelineslices.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhttimelinestrip.py` & `vht-0.3.98/libvht/vhttimelinestrip.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhttimelinestrips.py` & `vht-0.3.98/libvht/vhttimelinestrips.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhttimelineticks.py` & `vht-0.3.98/libvht/vhttimelineticks.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhttrack.py` & `vht-0.3.98/libvht/vhttrack.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/libvht/vhttracy.py` & `vht-0.3.98/libvht/vhttracy.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/pyproject.toml` & `vht-0.3.98/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = 'setuptools.build_meta'
 requires = ["setuptools>=61.0"]
 [metadata]
 name = "vht"
-version = "0.3.97"
+version = "0.3.98"
 description = "vahatraker - a live MIDI sequencer for pipewire/JACK"
 author = "Remigiusz Dybka"
 author_email = "remigiusz.dybka@gmail.com"
 url = "https://github.com/rdybka/vht"
 long_description = "file: README.md"
 long_description_content_type = "text/markdown"
 classifiers = [
@@ -34,18 +34,18 @@
 [options.package_data]
 vht = ["data/*", "data/ctrl/*", "data/bank/*"]
 
 [options.data_files]
 "share/vht" = ["data/mandy.png", "data/vht.svg", "data/vht.png", "data/menu.ui", "data/menu_norend.ui"]
 "share/vht/ctrl" = ["data/ctrl/10-gm", "data/ctrl/20-zyn"]
 "share/vht/bank" = ["data/bank/10-gm1", "data/bank/20-gm2"]
-"share/icons/hicolor/scalable" = ["data/net.sourceforge.projects.vht.svg"]
+"share/icons/hicolor/scalable" = ["data/io.github.rdybka.vht.svg"]
 "share/man/man1" = ["doc/vht.1.gz"]
-"share/applications" = ["data/net.sourceforge.projects.vht.desktop"]
-"share/metainfo" = ["data/net.sourceforge.projects.vht.metainfo.xml"]
+"share/applications" = ["data/io.github.rdybka.desktop"]
+"share/metainfo" = ["data/io.github.rdybka.metainfo.xml"]
 
 [options.extensions]
 "libvht/_libcvht" = ["libvht/libvht.c", 
 "libvht/libcvht_wrap.c",
 "libvht/midi_client.c",
 "libvht/jack_process.c",
 "libvht/midi_event.c",
```

### Comparing `vht-0.3.97/setup.py` & `vht-0.3.98/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, Extension
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name = "vht",
-	version = "0.3.97",
+	version = "0.3.98",
 	description = "vahatraker - a live MIDI sequencer for pipewire/JACK",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	author = "Remigiusz Dybka",
 	author_email = "remigiusz.dybka@gmail.com",
 	url = "https://github.com/rdybka/vht",
 	license = 'GPLv3+',
@@ -40,18 +40,18 @@
 		'vht = vht.main:run',
 		]},
 	
 	data_files = [
 		('share/vht', ['data/mandy.png', 'data/vht.svg', 'data/vht.png', 'data/menu.ui', 'data/menu_norend.ui']),
 		('share/vht/ctrl', ['data/ctrl/10-gm', 'data/ctrl/20-zyn']),
 		('share/vht/bank', ['data/bank/10-gm1', 'data/bank/20-gm2']),
-		('share/icons/hicolor/scalable/apps', ['data/net.sourceforge.projects.vht.svg']),
+		('share/icons/hicolor/scalable/apps', ['data/io.github.rdybka.vht.svg']),
 		('share/man/man1', ['doc/vht.1.gz']),
-		('share/applications', ['data/net.sourceforge.projects.vht.desktop']),
-		('share/metainfo' , ['data/net.sourceforge.projects.vht.metainfo.xml'])
+		('share/applications', ['data/io.github.rdybka.vht.desktop']),
+		('share/metainfo' , ['data/io.github.rdybka.vht.metainfo.xml'])
 		
 	],
 	
 	classifiers=[
 		'Development Status :: 5 - Production/Stable',
 		'Environment :: X11 Applications :: GTK',
 		'Intended Audience :: End Users/Desktop',
```

### Comparing `vht-0.3.97/vht/autoexec.py` & `vht-0.3.98/vht/autoexec.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/bankcfg.py` & `vht-0.3.98/vht/bankcfg.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/capturebutton.py` & `vht-0.3.98/vht/capturebutton.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/codedaemon.py` & `vht-0.3.98/vht/codedaemon.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/configuration.py` & `vht-0.3.98/vht/configuration.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/console.py` & `vht-0.3.98/vht/console.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/controllereditor.py` & `vht-0.3.98/vht/controllereditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/controllersview.py` & `vht-0.3.98/vht/controllersview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/controllersviewrow.py` & `vht-0.3.98/vht/controllersviewrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/controllerundobuffer.py` & `vht-0.3.98/vht/controllerundobuffer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/ctrlcfg.py` & `vht-0.3.98/vht/ctrlcfg.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/extras.py` & `vht-0.3.98/vht/extras.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/filerotator.py` & `vht-0.3.98/vht/filerotator.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/main.py` & `vht-0.3.98/vht/main.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/mainwin.py` & `vht-0.3.98/vht/mainwin.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/mandymenu.py` & `vht-0.3.98/vht/mandymenu.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/mandyview.py` & `vht-0.3.98/vht/mandyview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/midimapview.py` & `vht-0.3.98/vht/midimapview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/midimapviewrow.py` & `vht-0.3.98/vht/midimapviewrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/notebooklabel.py` & `vht-0.3.98/vht/notebooklabel.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/poormanspiano.py` & `vht-0.3.98/vht/poormanspiano.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/portconfig.py` & `vht-0.3.98/vht/portconfig.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/portconfigpopover.py` & `vht-0.3.98/vht/portconfigpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/portconfigview.py` & `vht-0.3.98/vht/portconfigview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/preferenceswin.py` & `vht-0.3.98/vht/preferenceswin.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/probeditor.py` & `vht-0.3.98/vht/probeditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/propview.py` & `vht-0.3.98/vht/propview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/pulsar.py` & `vht-0.3.98/vht/pulsar.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/randomcomposer.py` & `vht-0.3.98/vht/randomcomposer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/renderer.py` & `vht-0.3.98/vht/renderer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/renderwin.py` & `vht-0.3.98/vht/renderwin.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/sequencelistview.py` & `vht-0.3.98/vht/sequencelistview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/sequencelistviewpopover.py` & `vht-0.3.98/vht/sequencelistviewpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/sequencepropviewpopover.py` & `vht-0.3.98/vht/sequencepropviewpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/sequencetriggersview.py` & `vht-0.3.98/vht/sequencetriggersview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/sequenceview.py` & `vht-0.3.98/vht/sequenceview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/shortcutmayhem.py` & `vht-0.3.98/vht/shortcutmayhem.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/sidetrackview.py` & `vht-0.3.98/vht/sidetrackview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/statusbar.py` & `vht-0.3.98/vht/statusbar.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/thumbmanager.py` & `vht-0.3.98/vht/thumbmanager.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/timelineview.py` & `vht-0.3.98/vht/timelineview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/timeshifteditor.py` & `vht-0.3.98/vht/timeshifteditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/trackpropview.py` & `vht-0.3.98/vht/trackpropview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/trackpropviewpopover.py` & `vht-0.3.98/vht/trackpropviewpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/trackundobuffer.py` & `vht-0.3.98/vht/trackundobuffer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/trackview.py` & `vht-0.3.98/vht/trackview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/trackviewpointer.py` & `vht-0.3.98/vht/trackviewpointer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht/velocityeditor.py` & `vht-0.3.98/vht/velocityeditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.97/vht.egg-info/PKG-INFO` & `vht-0.3.98/vht.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vht
-Version: 0.3.97
+Version: 0.3.98
 Summary: vahatraker - a live MIDI sequencer for pipewire/JACK
 Home-page: https://github.com/rdybka/vht
 Author: Remigiusz Dybka
 Author-email: remigiusz.dybka@gmail.com
 License: GPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `vht-0.3.97/vht.egg-info/SOURCES.txt` & `vht-0.3.98/vht.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+data/io.github.rdybka.vht.desktop
+data/io.github.rdybka.vht.metainfo.xml
+data/io.github.rdybka.vht.svg
 data/mandy.png
 data/menu.ui
 data/menu_norend.ui
-data/net.sourceforge.projects.vht.desktop
-data/net.sourceforge.projects.vht.metainfo.xml
-data/net.sourceforge.projects.vht.svg
 data/vht.png
 data/vht.svg
 data/bank/10-gm1
 data/bank/20-gm2
 data/ctrl/10-gm
 data/ctrl/20-zyn
 doc/vht.1.gz
```

