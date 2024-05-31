# Comparing `tmp/limnoria-2024.4.26.tar.gz` & `tmp/limnoria-2024.5.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "limnoria-2024.4.26.tar", last modified: Sun May  5 15:43:06 2024, max compression
+gzip compressed data, was "limnoria-2024.5.30.tar", last modified: Fri May 31 21:10:53 2024, max compression
```

## Comparing `limnoria-2024.4.26.tar` & `limnoria-2024.5.30.tar`

### file list

```diff
@@ -1,767 +1,767 @@
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.326961 limnoria-2024.4.26/
--rw-r--r--   0 val       (1000) val       (1000)     1654 2024-05-05 15:42:57.000000 limnoria-2024.4.26/LICENSE.md
--rw-r--r--   0 val       (1000) val       (1000)      117 2024-05-05 15:42:57.000000 limnoria-2024.4.26/MANIFEST.in
--rw-r--r--   0 val       (1000) val       (1000)      983 2024-05-05 15:42:57.000000 limnoria-2024.4.26/Makefile
--rw-r--r--   0 val       (1000) val       (1000)     1848 2024-05-05 15:43:06.326961 limnoria-2024.4.26/PKG-INFO
--rw-r--r--   0 val       (1000) val       (1000)     2292 2024-05-05 15:42:57.000000 limnoria-2024.4.26/README.md
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.282961 limnoria-2024.4.26/limnoria.egg-info/
--rw-r--r--   0 val       (1000) val       (1000)     1848 2024-05-05 15:43:06.000000 limnoria-2024.4.26/limnoria.egg-info/PKG-INFO
--rw-r--r--   0 val       (1000) val       (1000)    16256 2024-05-05 15:43:06.000000 limnoria-2024.4.26/limnoria.egg-info/SOURCES.txt
--rw-r--r--   0 val       (1000) val       (1000)        1 2024-05-05 15:43:06.000000 limnoria-2024.4.26/limnoria.egg-info/dependency_links.txt
--rw-r--r--   0 val       (1000) val       (1000)      934 2024-05-05 15:43:06.000000 limnoria-2024.4.26/limnoria.egg-info/entry_points.txt
--rw-r--r--   0 val       (1000) val       (1000)        8 2024-05-05 15:43:06.000000 limnoria-2024.4.26/limnoria.egg-info/top_level.txt
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.282961 limnoria-2024.4.26/locales/
--rw-r--r--   0 val       (1000) val       (1000)        0 2024-05-05 15:42:57.000000 limnoria-2024.4.26/locales/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)    54113 2024-05-05 15:42:57.000000 limnoria-2024.4.26/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    76337 2024-05-05 15:42:57.000000 limnoria-2024.4.26/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    77441 2024-05-05 15:42:57.000000 limnoria-2024.4.26/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     3749 2024-05-05 15:42:57.000000 limnoria-2024.4.26/locales/fr.py
--rw-r--r--   0 val       (1000) val       (1000)    69991 2024-05-05 15:42:57.000000 limnoria-2024.4.26/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    42399 2024-05-05 15:42:57.000000 limnoria-2024.4.26/locales/messages.pot
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.282961 limnoria-2024.4.26/man/
--rw-r--r--   0 val       (1000) val       (1000)     1196 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria-adduser.1
--rw-r--r--   0 val       (1000) val       (1000)     1487 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria-botchk.1
--rw-r--r--   0 val       (1000) val       (1000)     1125 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria-plugin-create.1
--rw-r--r--   0 val       (1000) val       (1000)     1378 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria-plugin-doc.1
--rw-r--r--   0 val       (1000) val       (1000)     1026 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria-reset-password.1
--rw-r--r--   0 val       (1000) val       (1000)     1499 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria-test.1
--rw-r--r--   0 val       (1000) val       (1000)     1191 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria-wizard.1
--rw-r--r--   0 val       (1000) val       (1000)     1970 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/limnoria.1
--rw-r--r--   0 val       (1000) val       (1000)     1196 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot-adduser.1
--rw-r--r--   0 val       (1000) val       (1000)     1487 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot-botchk.1
--rw-r--r--   0 val       (1000) val       (1000)     1125 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot-plugin-create.1
--rw-r--r--   0 val       (1000) val       (1000)     1378 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot-plugin-doc.1
--rw-r--r--   0 val       (1000) val       (1000)     1026 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot-reset-password.1
--rw-r--r--   0 val       (1000) val       (1000)     1499 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot-test.1
--rw-r--r--   0 val       (1000) val       (1000)     1191 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot-wizard.1
--rw-r--r--   0 val       (1000) val       (1000)     1970 2024-05-05 15:42:57.000000 limnoria-2024.4.26/man/supybot.1
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Admin/
--rw-r--r--   0 val       (1000) val       (1000)     2422 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2312 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Admin/locales/
--rw-r--r--   0 val       (1000) val       (1000)     8064 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     8857 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7809 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     8112 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    15152 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6275 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Admin/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Aka/
--rw-r--r--   0 val       (1000) val       (1000)     2788 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Aka/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2979 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Aka/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Aka/locales/
--rw-r--r--   0 val       (1000) val       (1000)    11022 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Aka/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    39586 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Aka/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    14785 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Aka/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Alias/
--rw-r--r--   0 val       (1000) val       (1000)     2655 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2539 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Alias/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4716 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5751 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5059 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5176 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     4919 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    19130 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     8039 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Alias/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Anonymous/
--rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3516 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Anonymous/locales/
--rw-r--r--   0 val       (1000) val       (1000)     6558 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     7384 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5903 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6893 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     6535 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     9054 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6882 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Anonymous/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/AutoMode/
--rw-r--r--   0 val       (1000) val       (1000)     2697 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4521 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/AutoMode/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4202 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5058 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4512 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4131 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     8029 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1787 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/AutoMode/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/Autocomplete/
--rw-r--r--   0 val       (1000) val       (1000)     2946 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Autocomplete/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2808 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Autocomplete/config.py
--rw-r--r--   0 val       (1000) val       (1000)     6158 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Autocomplete/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6635 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Autocomplete/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/BadWords/
--rw-r--r--   0 val       (1000) val       (1000)     2695 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/BadWords/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     6163 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/BadWords/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.286961 limnoria-2024.4.26/plugins/BadWords/locales/
--rw-r--r--   0 val       (1000) val       (1000)     6862 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/BadWords/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6112 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/BadWords/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6277 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/BadWords/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7475 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/BadWords/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3943 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/BadWords/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Channel/
--rw-r--r--   0 val       (1000) val       (1000)     2480 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3497 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Channel/locales/
--rw-r--r--   0 val       (1000) val       (1000)    32456 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    35277 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    32166 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    32899 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)    33333 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    44679 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    13344 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Channel/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/ChannelLogger/
--rw-r--r--   0 val       (1000) val       (1000)     2531 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5994 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/ChannelLogger/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5491 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5340 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5607 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     5183 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    13745 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9242 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelLogger/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/ChannelStats/
--rw-r--r--   0 val       (1000) val       (1000)     2682 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelStats/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3449 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelStats/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/ChannelStats/locales/
--rw-r--r--   0 val       (1000) val       (1000)     6426 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelStats/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6640 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelStats/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6242 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelStats/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    15391 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelStats/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4870 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ChannelStats/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Conditional/
--rw-r--r--   0 val       (1000) val       (1000)     2907 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Conditional/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2763 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Conditional/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Conditional/locales/
--rw-r--r--   0 val       (1000) val       (1000)     8160 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Conditional/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7180 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Conditional/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7493 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Conditional/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    11342 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Conditional/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6497 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Conditional/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Config/
--rw-r--r--   0 val       (1000) val       (1000)     2325 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Config/locales/
--rw-r--r--   0 val       (1000) val       (1000)     9209 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     9329 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     9333 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     9333 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     9265 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    21747 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    25531 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Config/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Ctcp/
--rw-r--r--   0 val       (1000) val       (1000)     2420 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3652 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/Ctcp/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2084 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     2196 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2072 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2073 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     1911 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7136 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1785 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Ctcp/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.290961 limnoria-2024.4.26/plugins/DDG/
--rw-r--r--   0 val       (1000) val       (1000)     2670 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/DDG/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3332 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/DDG/config.py
--rw-r--r--   0 val       (1000) val       (1000)     6037 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/DDG/parser.py
--rw-r--r--   0 val       (1000) val       (1000)     6988 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/DDG/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2389 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/DDG/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Debug/
--rw-r--r--   0 val       (1000) val       (1000)     2377 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Debug/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2399 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Debug/config.py
--rw-r--r--   0 val       (1000) val       (1000)     7253 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Debug/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2648 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Debug/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Dict/
--rw-r--r--   0 val       (1000) val       (1000)     2559 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2877 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Dict/local/
--rw-r--r--   0 val       (1000) val       (1000)       58 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/local/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)    12308 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/local/dictclient.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Dict/locales/
--rw-r--r--   0 val       (1000) val       (1000)     3731 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     3433 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     3365 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     6458 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2548 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dict/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Dunno/
--rw-r--r--   0 val       (1000) val       (1000)     2817 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2511 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Dunno/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1414 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     1637 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1557 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1441 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3095 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3446 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Dunno/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Factoids/
--rw-r--r--   0 val       (1000) val       (1000)     2738 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Factoids/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4867 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Factoids/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Factoids/locales/
--rw-r--r--   0 val       (1000) val       (1000)    14672 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Factoids/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    14207 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Factoids/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    13986 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Factoids/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    37539 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Factoids/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    10544 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Factoids/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Fediverse/
--rw-r--r--   0 val       (1000) val       (1000)     2506 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Fediverse/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     9206 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Fediverse/activitypub.py
--rw-r--r--   0 val       (1000) val       (1000)     3583 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Fediverse/config.py
--rw-r--r--   0 val       (1000) val       (1000)    16853 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Fediverse/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    21650 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Fediverse/test.py
--rw-r--r--   0 val       (1000) val       (1000)    21570 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Fediverse/test_data.py
--rw-r--r--   0 val       (1000) val       (1000)     2553 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Fediverse/utils.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Filter/
--rw-r--r--   0 val       (1000) val       (1000)     2691 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Filter/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3118 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Filter/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Filter/locales/
--rw-r--r--   0 val       (1000) val       (1000)    14523 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Filter/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    13736 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Filter/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    14301 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Filter/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    27294 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Filter/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     7848 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Filter/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Format/
--rw-r--r--   0 val       (1000) val       (1000)     2559 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Format/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2522 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Format/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/Format/locales/
--rw-r--r--   0 val       (1000) val       (1000)     6742 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Format/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5998 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Format/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6115 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Format/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7452 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Format/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4078 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Format/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.294961 limnoria-2024.4.26/plugins/GPG/
--rw-r--r--   0 val       (1000) val       (1000)     2606 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/GPG/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2996 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/GPG/config.py
--rw-r--r--   0 val       (1000) val       (1000)     9566 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/GPG/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5817 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/GPG/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Games/
--rw-r--r--   0 val       (1000) val       (1000)     2660 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2313 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Games/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4801 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5274 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4968 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4732 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7248 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2854 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Games/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Geography/
--rw-r--r--   0 val       (1000) val       (1000)     2578 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Geography/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     1936 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Geography/common.py
--rw-r--r--   0 val       (1000) val       (1000)     2441 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Geography/config.py
--rw-r--r--   0 val       (1000) val       (1000)     2924 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Geography/nominatim.py
--rw-r--r--   0 val       (1000) val       (1000)     6528 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Geography/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    10325 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Geography/test.py
--rw-r--r--   0 val       (1000) val       (1000)     5514 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Geography/wikidata.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Google/
--rw-r--r--   0 val       (1000) val       (1000)     2507 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     7042 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Google/locales/
--rw-r--r--   0 val       (1000) val       (1000)     9595 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     9003 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     9000 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     4460 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/parser.py
--rw-r--r--   0 val       (1000) val       (1000)    11693 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3095 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Google/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Hashes/
--rw-r--r--   0 val       (1000) val       (1000)     2585 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Hashes/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2244 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Hashes/config.py
--rw-r--r--   0 val       (1000) val       (1000)     4049 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Hashes/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2754 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Hashes/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Herald/
--rw-r--r--   0 val       (1000) val       (1000)     2423 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Herald/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3907 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Herald/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Herald/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7333 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Herald/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6711 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Herald/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6615 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Herald/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    10794 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Herald/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1789 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Herald/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Internet/
--rw-r--r--   0 val       (1000) val       (1000)     2676 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Internet/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2541 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Internet/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Internet/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2313 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Internet/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1791 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Internet/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1769 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Internet/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     8888 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Internet/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2420 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Internet/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Karma/
--rw-r--r--   0 val       (1000) val       (1000)     2540 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Karma/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3929 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Karma/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Karma/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7837 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Karma/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7070 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Karma/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7143 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Karma/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    18303 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Karma/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9962 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Karma/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Lart/
--rw-r--r--   0 val       (1000) val       (1000)     2571 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Lart/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2679 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Lart/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Lart/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2427 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Lart/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2027 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Lart/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1956 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Lart/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     4264 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Lart/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2583 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Lart/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.298961 limnoria-2024.4.26/plugins/Later/
--rw-r--r--   0 val       (1000) val       (1000)     2650 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3413 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Later/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7371 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     7908 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6739 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7370 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    11043 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6360 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Later/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Limiter/
--rw-r--r--   0 val       (1000) val       (1000)     2662 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3141 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Limiter/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2685 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2688 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2724 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     2573 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3657 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2871 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Limiter/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/LogToIrc/
--rw-r--r--   0 val       (1000) val       (1000)     2457 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/LogToIrc/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5627 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/LogToIrc/config.py
--rw-r--r--   0 val       (1000) val       (1000)     6213 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/LogToIrc/handler.py
--rw-r--r--   0 val       (1000) val       (1000)     2710 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/LogToIrc/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1781 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/LogToIrc/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Math/
--rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2516 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Math/local/
--rw-r--r--   0 val       (1000) val       (1000)       58 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/local/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)    46378 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/local/convertcore.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Math/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5920 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5424 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5331 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     5325 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    11324 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9441 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Math/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/MessageParser/
--rw-r--r--   0 val       (1000) val       (1000)     3026 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MessageParser/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4464 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MessageParser/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/MessageParser/locales/
--rw-r--r--   0 val       (1000) val       (1000)    11282 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MessageParser/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    10121 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MessageParser/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    10440 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MessageParser/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    20338 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MessageParser/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    11746 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MessageParser/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Misc/
--rw-r--r--   0 val       (1000) val       (1000)     2299 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4131 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Misc/locales/
--rw-r--r--   0 val       (1000) val       (1000)    13201 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    14554 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    13747 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    13209 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)    13537 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    29646 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    17530 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Misc/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/MoobotFactoids/
--rw-r--r--   0 val       (1000) val       (1000)     2648 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MoobotFactoids/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2740 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MoobotFactoids/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/MoobotFactoids/locales/
--rw-r--r--   0 val       (1000) val       (1000)    11225 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MoobotFactoids/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    10014 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MoobotFactoids/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    10059 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MoobotFactoids/locales/it.po
--rwxr-xr-x   0 val       (1000) val       (1000)    29418 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MoobotFactoids/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    16971 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/MoobotFactoids/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Network/
--rw-r--r--   0 val       (1000) val       (1000)     2514 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.302961 limnoria-2024.4.26/plugins/Network/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7181 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     8612 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7289 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7472 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    12972 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3097 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Network/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/News/
--rw-r--r--   0 val       (1000) val       (1000)     2777 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/News/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2519 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/News/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/News/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4608 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/News/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4221 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/News/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4314 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/News/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     8659 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/News/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3616 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/News/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/NickAuth/
--rw-r--r--   0 val       (1000) val       (1000)     2574 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickAuth/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2495 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickAuth/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/NickAuth/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4837 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickAuth/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     4838 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickAuth/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     9213 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickAuth/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6306 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickAuth/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/NickCapture/
--rw-r--r--   0 val       (1000) val       (1000)     2582 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2738 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/NickCapture/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1598 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     1716 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1592 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1500 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     5415 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1799 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/NickCapture/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Nickometer/
--rw-r--r--   0 val       (1000) val       (1000)     3249 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Nickometer/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2616 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Nickometer/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Nickometer/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1338 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Nickometer/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1027 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Nickometer/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)      952 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Nickometer/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     9695 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Nickometer/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2183 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Nickometer/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Note/
--rw-r--r--   0 val       (1000) val       (1000)     2645 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Note/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3477 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Note/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Note/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4033 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Note/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     3453 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Note/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     3399 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Note/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    16493 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Note/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4040 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Note/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Owner/
--rw-r--r--   0 val       (1000) val       (1000)     2427 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3252 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Owner/locales/
--rw-r--r--   0 val       (1000) val       (1000)     8724 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5600 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     8546 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     9038 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     8811 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    33701 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9690 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Owner/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Plugin/
--rw-r--r--   0 val       (1000) val       (1000)     2666 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2523 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/Plugin/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7234 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     7937 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6377 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7290 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     9985 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4272 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Plugin/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/PluginDownloader/
--rw-r--r--   0 val       (1000) val       (1000)     2670 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2535 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.306961 limnoria-2024.4.26/plugins/PluginDownloader/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4570 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     6726 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6327 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5727 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    16307 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3847 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/PluginDownloader/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Poll/
--rw-r--r--   0 val       (1000) val       (1000)     2516 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Poll/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2922 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Poll/config.py
--rw-r--r--   0 val       (1000) val       (1000)     8542 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Poll/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6858 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Poll/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Praise/
--rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Praise/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2695 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Praise/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Praise/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2548 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Praise/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2424 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Praise/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2352 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Praise/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     4348 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Praise/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1953 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Praise/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Protector/
--rw-r--r--   0 val       (1000) val       (1000)     2594 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Protector/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2901 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Protector/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Protector/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1626 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Protector/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1245 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Protector/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1153 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Protector/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7598 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Protector/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1789 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Protector/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Quote/
--rw-r--r--   0 val       (1000) val       (1000)     2524 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Quote/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2519 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Quote/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Quote/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1700 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Quote/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1418 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Quote/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1372 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Quote/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3106 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Quote/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2541 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Quote/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/QuoteGrabs/
--rw-r--r--   0 val       (1000) val       (1000)     2675 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/QuoteGrabs/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3670 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/QuoteGrabs/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/QuoteGrabs/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7337 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/QuoteGrabs/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6529 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/QuoteGrabs/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     6636 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/QuoteGrabs/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    17122 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/QuoteGrabs/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     8560 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/QuoteGrabs/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/RSS/
--rw-r--r--   0 val       (1000) val       (1000)     2706 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     6867 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/RSS/locales/
--rw-r--r--   0 val       (1000) val       (1000)    12451 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    15597 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    13213 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    13001 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)    12728 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    30557 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    25475 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/RSS/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Relay/
--rw-r--r--   0 val       (1000) val       (1000)     2517 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Relay/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4744 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Relay/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Relay/locales/
--rw-r--r--   0 val       (1000) val       (1000)     8274 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Relay/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7545 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Relay/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7487 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Relay/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    19682 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Relay/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     1787 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Relay/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Reply/
--rw-r--r--   0 val       (1000) val       (1000)     2572 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2519 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Reply/locales/
--rw-r--r--   0 val       (1000) val       (1000)     2384 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     2630 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2331 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2669 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     2433 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3694 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3051 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Reply/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.310961 limnoria-2024.4.26/plugins/Scheduler/
--rw-r--r--   0 val       (1000) val       (1000)     2757 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Scheduler/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2541 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Scheduler/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/Scheduler/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4116 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Scheduler/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     3797 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Scheduler/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     3850 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Scheduler/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    12852 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Scheduler/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     8402 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Scheduler/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/SedRegex/
--rw-r--r--   0 val       (1000) val       (1000)     2709 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/SedRegex/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4356 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/SedRegex/config.py
--rwxr-xr-x   0 val       (1000) val       (1000)      874 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/SedRegex/constants.py
--rw-r--r--   0 val       (1000) val       (1000)    10523 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/SedRegex/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    13147 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/SedRegex/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/Seen/
--rw-r--r--   0 val       (1000) val       (1000)     2637 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2979 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/Seen/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5779 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     6954 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     6235 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5812 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    16735 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6414 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Seen/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/Services/
--rw-r--r--   0 val       (1000) val       (1000)     2607 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5658 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/Services/locales/
--rw-r--r--   0 val       (1000) val       (1000)    11466 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    11843 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    11294 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    11525 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    35273 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    14436 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Services/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/ShrinkUrl/
--rw-r--r--   0 val       (1000) val       (1000)     2542 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ShrinkUrl/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5035 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ShrinkUrl/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/ShrinkUrl/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5983 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ShrinkUrl/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5213 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ShrinkUrl/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5243 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ShrinkUrl/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    10186 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ShrinkUrl/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5286 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/ShrinkUrl/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/Status/
--rw-r--r--   0 val       (1000) val       (1000)     2457 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2901 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/Status/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5435 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     6124 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5481 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5563 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    11461 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3180 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Status/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/String/
--rw-r--r--   0 val       (1000) val       (1000)     2551 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/String/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3429 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/String/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.314961 limnoria-2024.4.26/plugins/String/locales/
--rw-r--r--   0 val       (1000) val       (1000)     9469 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/String/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     8780 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/String/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     8557 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/String/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     9911 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/String/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     7585 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/String/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Success/
--rw-r--r--   0 val       (1000) val       (1000)     2646 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Success/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2751 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Success/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Success/locales/
--rw-r--r--   0 val       (1000) val       (1000)     1578 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Success/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     1435 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Success/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     1323 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Success/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     3471 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Success/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     2272 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Success/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Time/
--rw-r--r--   0 val       (1000) val       (1000)     2673 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2640 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Time/locales/
--rw-r--r--   0 val       (1000) val       (1000)     5480 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     6313 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     5483 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     5849 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)     5574 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    10127 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5071 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Time/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Todo/
--rw-r--r--   0 val       (1000) val       (1000)     2607 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2683 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Todo/locales/
--rw-r--r--   0 val       (1000) val       (1000)     4575 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     5089 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4595 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4664 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    10596 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     6654 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Todo/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Topic/
--rw-r--r--   0 val       (1000) val       (1000)     2583 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Topic/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     4776 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Topic/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Topic/locales/
--rw-r--r--   0 val       (1000) val       (1000)    18502 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Topic/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    16877 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Topic/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    17231 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Topic/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    25153 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Topic/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)    13078 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Topic/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/URL/
--rw-r--r--   0 val       (1000) val       (1000)     2661 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/URL/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2629 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/URL/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/URL/locales/
--rw-r--r--   0 val       (1000) val       (1000)     3421 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/URL/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     2907 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/URL/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     2841 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/URL/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     6765 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/URL/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4241 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/URL/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Unix/
--rw-r--r--   0 val       (1000) val       (1000)     2669 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Unix/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     6252 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Unix/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.318961 limnoria-2024.4.26/plugins/Unix/locales/
--rw-r--r--   0 val       (1000) val       (1000)    13680 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Unix/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    11967 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Unix/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    12075 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Unix/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    20048 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Unix/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     7736 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Unix/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/plugins/User/
--rw-r--r--   0 val       (1000) val       (1000)     2355 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2728 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/plugins/User/locales/
--rw-r--r--   0 val       (1000) val       (1000)    15416 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)    21068 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)    19566 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)    10856 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/locales/hu.po
--rw-r--r--   0 val       (1000) val       (1000)    15349 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    23217 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9203 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/User/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/plugins/Utilities/
--rw-r--r--   0 val       (1000) val       (1000)     2407 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2541 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/plugins/Utilities/locales/
--rw-r--r--   0 val       (1000) val       (1000)     3623 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     4827 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     4250 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     4335 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)     7065 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     3958 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Utilities/test.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/plugins/Web/
--rw-r--r--   0 val       (1000) val       (1000)     2446 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     5246 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/config.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/plugins/Web/locales/
--rw-r--r--   0 val       (1000) val       (1000)     7308 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/locales/de.po
--rw-r--r--   0 val       (1000) val       (1000)     8904 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/locales/fi.po
--rw-r--r--   0 val       (1000) val       (1000)     7488 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/locales/fr.po
--rw-r--r--   0 val       (1000) val       (1000)     7113 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/locales/it.po
--rw-r--r--   0 val       (1000) val       (1000)    17047 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     9430 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/Web/test.py
--rw-r--r--   0 val       (1000) val       (1000)    23695 2024-05-05 15:42:57.000000 limnoria-2024.4.26/plugins/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)      192 2024-05-05 15:42:57.000000 limnoria-2024.4.26/pyproject.toml
--rw-r--r--   0 val       (1000) val       (1000)      946 2024-05-05 15:42:57.000000 limnoria-2024.4.26/requirements.txt
--rw-r--r--   0 val       (1000) val       (1000)       38 2024-05-05 15:43:06.326961 limnoria-2024.4.26/setup.cfg
--rw-r--r--   0 val       (1000) val       (1000)     8446 2024-05-05 15:42:57.000000 limnoria-2024.4.26/setup.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/src/
--rw-r--r--   0 val       (1000) val       (1000)     4117 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     3548 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/ansi.py
--rw-r--r--   0 val       (1000) val       (1000)    75220 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/callbacks.py
--rw-r--r--   0 val       (1000) val       (1000)    14986 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/cdb.py
--rw-r--r--   0 val       (1000) val       (1000)    41479 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/commands.py
--rw-r--r--   0 val       (1000) val       (1000)    67015 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/conf.py
--rw-r--r--   0 val       (1000) val       (1000)    14165 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/dbi.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.322961 limnoria-2024.4.26/src/drivers/
--rw-r--r--   0 val       (1000) val       (1000)    19591 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/drivers/Socket.py
--rw-r--r--   0 val       (1000) val       (1000)     9696 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/drivers/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2350 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/dynamicScope.py
--rw-r--r--   0 val       (1000) val       (1000)     2997 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/gpg.py
--rw-r--r--   0 val       (1000) val       (1000)    17964 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/httpserver.py
--rw-r--r--   0 val       (1000) val       (1000)    13332 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/i18n.py
--rw-r--r--   0 val       (1000) val       (1000)    52151 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/ircdb.py
--rw-r--r--   0 val       (1000) val       (1000)    98073 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/irclib.py
--rw-r--r--   0 val       (1000) val       (1000)    38939 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/ircmsgs.py
--rw-r--r--   0 val       (1000) val       (1000)    43234 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/ircutils.py
--rw-r--r--   0 val       (1000) val       (1000)    16573 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/log.py
--rw-r--r--   0 val       (1000) val       (1000)     8379 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     5342 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/questions.py
--rw-r--r--   0 val       (1000) val       (1000)    34261 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/registry.py
--rw-r--r--   0 val       (1000) val       (1000)     6156 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/schedule.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.326961 limnoria-2024.4.26/src/scripts/
--rw-r--r--   0 val       (1000) val       (1000)        0 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)    15886 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria.py
--rw-r--r--   0 val       (1000) val       (1000)     5258 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria_adduser.py
--rw-r--r--   0 val       (1000) val       (1000)     5455 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria_botchk.py
--rw-r--r--   0 val       (1000) val       (1000)    10536 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria_plugin_create.py
--rw-r--r--   0 val       (1000) val       (1000)    14353 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria_plugin_doc.py
--rw-r--r--   0 val       (1000) val       (1000)     4454 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria_reset_password.py
--rw-r--r--   0 val       (1000) val       (1000)    10443 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria_test.py
--rw-r--r--   0 val       (1000) val       (1000)    37750 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/scripts/limnoria_wizard.py
--rw-r--r--   0 val       (1000) val       (1000)     4790 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/setup.py
--rw-r--r--   0 val       (1000) val       (1000)     8198 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/shlex.py
--rw-r--r--   0 val       (1000) val       (1000)    25444 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/test.py
--rw-r--r--   0 val       (1000) val       (1000)     3869 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/unpreserve.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.326961 limnoria-2024.4.26/src/utils/
--rw-r--r--   0 val       (1000) val       (1000)     2575 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     1741 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/crypt.py
--rw-r--r--   0 val       (1000) val       (1000)     1992 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/error.py
--rw-r--r--   0 val       (1000) val       (1000)     9475 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/file.py
--rw-r--r--   0 val       (1000) val       (1000)    11587 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/gen.py
--rw-r--r--   0 val       (1000) val       (1000)     5210 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/iter.py
--rw-r--r--   0 val       (1000) val       (1000)     6195 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/math_evaluator.py
--rw-r--r--   0 val       (1000) val       (1000)     3914 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/minisix.py
--rw-r--r--   0 val       (1000) val       (1000)     6526 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/net.py
--rw-r--r--   0 val       (1000) val       (1000)     7726 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/python.py
--rw-r--r--   0 val       (1000) val       (1000)     4169 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/seq.py
--rw-r--r--   0 val       (1000) val       (1000)    21873 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/str.py
--rw-r--r--   0 val       (1000) val       (1000)    19840 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/structures.py
--rw-r--r--   0 val       (1000) val       (1000)     2838 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/time.py
--rw-r--r--   0 val       (1000) val       (1000)     8826 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/transaction.py
--rw-r--r--   0 val       (1000) val       (1000)    10662 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/utils/web.py
--rw-r--r--   0 val       (1000) val       (1000)      175 2024-05-05 15:43:05.000000 limnoria-2024.4.26/src/version.py
--rw-r--r--   0 val       (1000) val       (1000)     7660 2024-05-05 15:42:57.000000 limnoria-2024.4.26/src/world.py
-drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-05 15:43:06.326961 limnoria-2024.4.26/test/
--rw-r--r--   0 val       (1000) val       (1000)     1754 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/__init__.py
--rw-r--r--   0 val       (1000) val       (1000)     2265 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test.py
--rw-r--r--   0 val       (1000) val       (1000)    49856 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_callbacks.py
--rw-r--r--   0 val       (1000) val       (1000)     9002 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_commands.py
--rw-r--r--   0 val       (1000) val       (1000)     2813 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_conf.py
--rw-r--r--   0 val       (1000) val       (1000)     4122 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_drivers.py
--rw-r--r--   0 val       (1000) val       (1000)     2458 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_dynamicScope.py
--rw-r--r--   0 val       (1000) val       (1000)     3225 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_firewall.py
--rw-r--r--   0 val       (1000) val       (1000)     1925 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_format.py
--rw-r--r--   0 val       (1000) val       (1000)     2832 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_i18n.py
--rw-r--r--   0 val       (1000) val       (1000)    29200 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_ircdb.py
--rw-r--r--   0 val       (1000) val       (1000)    67775 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_irclib.py
--rw-r--r--   0 val       (1000) val       (1000)    14083 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_ircmsgs.py
--rw-r--r--   0 val       (1000) val       (1000)    22829 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_ircutils.py
--rw-r--r--   0 val       (1000) val       (1000)     3341 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_misc.py
--rw-r--r--   0 val       (1000) val       (1000)     2016 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_plugin.py
--rw-r--r--   0 val       (1000) val       (1000)     4832 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_plugin_create.py
--rw-r--r--   0 val       (1000) val       (1000)     2430 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_plugins.py
--rw-r--r--   0 val       (1000) val       (1000)    13283 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_registry.py
--rw-r--r--   0 val       (1000) val       (1000)     4575 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_schedule.py
--rw-r--r--   0 val       (1000) val       (1000)     3759 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_standardSubstitute.py
--rw-r--r--   0 val       (1000) val       (1000)    49349 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_utils.py
--rw-r--r--   0 val       (1000) val       (1000)     3672 2024-05-05 15:42:57.000000 limnoria-2024.4.26/test/test_yn.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.974829 limnoria-2024.5.30/
+-rw-r--r--   0 val       (1000) val       (1000)     1654 2024-05-31 21:10:49.000000 limnoria-2024.5.30/LICENSE.md
+-rw-r--r--   0 val       (1000) val       (1000)      117 2024-05-31 21:10:49.000000 limnoria-2024.5.30/MANIFEST.in
+-rw-r--r--   0 val       (1000) val       (1000)      983 2024-05-31 21:10:49.000000 limnoria-2024.5.30/Makefile
+-rw-r--r--   0 val       (1000) val       (1000)     1848 2024-05-31 21:10:53.974829 limnoria-2024.5.30/PKG-INFO
+-rw-r--r--   0 val       (1000) val       (1000)     2292 2024-05-31 21:10:49.000000 limnoria-2024.5.30/README.md
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.914829 limnoria-2024.5.30/limnoria.egg-info/
+-rw-r--r--   0 val       (1000) val       (1000)     1848 2024-05-31 21:10:53.000000 limnoria-2024.5.30/limnoria.egg-info/PKG-INFO
+-rw-r--r--   0 val       (1000) val       (1000)    16256 2024-05-31 21:10:53.000000 limnoria-2024.5.30/limnoria.egg-info/SOURCES.txt
+-rw-r--r--   0 val       (1000) val       (1000)        1 2024-05-31 21:10:53.000000 limnoria-2024.5.30/limnoria.egg-info/dependency_links.txt
+-rw-r--r--   0 val       (1000) val       (1000)      934 2024-05-31 21:10:53.000000 limnoria-2024.5.30/limnoria.egg-info/entry_points.txt
+-rw-r--r--   0 val       (1000) val       (1000)        8 2024-05-31 21:10:53.000000 limnoria-2024.5.30/limnoria.egg-info/top_level.txt
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.918829 limnoria-2024.5.30/locales/
+-rw-r--r--   0 val       (1000) val       (1000)        0 2024-05-31 21:10:49.000000 limnoria-2024.5.30/locales/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)    54113 2024-05-31 21:10:49.000000 limnoria-2024.5.30/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    76337 2024-05-31 21:10:49.000000 limnoria-2024.5.30/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    77441 2024-05-31 21:10:49.000000 limnoria-2024.5.30/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     3749 2024-05-31 21:10:49.000000 limnoria-2024.5.30/locales/fr.py
+-rw-r--r--   0 val       (1000) val       (1000)    69991 2024-05-31 21:10:49.000000 limnoria-2024.5.30/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    42399 2024-05-31 21:10:49.000000 limnoria-2024.5.30/locales/messages.pot
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.918829 limnoria-2024.5.30/man/
+-rw-r--r--   0 val       (1000) val       (1000)     1196 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/limnoria-adduser.1
+-rw-r--r--   0 val       (1000) val       (1000)     1487 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/limnoria-botchk.1
+-rw-r--r--   0 val       (1000) val       (1000)     1125 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/limnoria-plugin-create.1
+-rw-r--r--   0 val       (1000) val       (1000)     1378 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/limnoria-plugin-doc.1
+-rw-r--r--   0 val       (1000) val       (1000)     1026 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/limnoria-reset-password.1
+-rw-r--r--   0 val       (1000) val       (1000)     1499 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/limnoria-test.1
+-rw-r--r--   0 val       (1000) val       (1000)     1191 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/limnoria-wizard.1
+-rw-r--r--   0 val       (1000) val       (1000)     1970 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/limnoria.1
+-rw-r--r--   0 val       (1000) val       (1000)     1196 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/supybot-adduser.1
+-rw-r--r--   0 val       (1000) val       (1000)     1487 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/supybot-botchk.1
+-rw-r--r--   0 val       (1000) val       (1000)     1125 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/supybot-plugin-create.1
+-rw-r--r--   0 val       (1000) val       (1000)     1378 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/supybot-plugin-doc.1
+-rw-r--r--   0 val       (1000) val       (1000)     1026 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/supybot-reset-password.1
+-rw-r--r--   0 val       (1000) val       (1000)     1499 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/supybot-test.1
+-rw-r--r--   0 val       (1000) val       (1000)     1191 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/supybot-wizard.1
+-rw-r--r--   0 val       (1000) val       (1000)     1970 2024-05-31 21:10:49.000000 limnoria-2024.5.30/man/supybot.1
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.918829 limnoria-2024.5.30/plugins/
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.918829 limnoria-2024.5.30/plugins/Admin/
+-rw-r--r--   0 val       (1000) val       (1000)     2422 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Admin/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2312 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Admin/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.918829 limnoria-2024.5.30/plugins/Admin/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     8064 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Admin/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     8857 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Admin/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7809 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Admin/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     8112 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Admin/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    15152 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Admin/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6275 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Admin/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.918829 limnoria-2024.5.30/plugins/Aka/
+-rw-r--r--   0 val       (1000) val       (1000)     2788 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Aka/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2979 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Aka/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.918829 limnoria-2024.5.30/plugins/Aka/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    11022 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Aka/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    39586 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Aka/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    14785 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Aka/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.918829 limnoria-2024.5.30/plugins/Alias/
+-rw-r--r--   0 val       (1000) val       (1000)     2655 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Alias/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2539 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Alias/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.918829 limnoria-2024.5.30/plugins/Alias/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4716 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Alias/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5751 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Alias/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5059 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Alias/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5176 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Alias/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     4919 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Alias/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    19130 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Alias/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     8039 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Alias/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.922829 limnoria-2024.5.30/plugins/Anonymous/
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Anonymous/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3516 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Anonymous/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.922829 limnoria-2024.5.30/plugins/Anonymous/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     6558 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Anonymous/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     7384 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Anonymous/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5903 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Anonymous/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6893 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Anonymous/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     6535 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Anonymous/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     9054 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Anonymous/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6882 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Anonymous/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.922829 limnoria-2024.5.30/plugins/AutoMode/
+-rw-r--r--   0 val       (1000) val       (1000)     2697 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/AutoMode/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4521 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/AutoMode/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.922829 limnoria-2024.5.30/plugins/AutoMode/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4202 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/AutoMode/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5058 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/AutoMode/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4512 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/AutoMode/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4131 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/AutoMode/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     8029 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/AutoMode/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1787 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/AutoMode/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.922829 limnoria-2024.5.30/plugins/Autocomplete/
+-rw-r--r--   0 val       (1000) val       (1000)     2946 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Autocomplete/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2808 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Autocomplete/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     6158 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Autocomplete/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6635 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Autocomplete/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.922829 limnoria-2024.5.30/plugins/BadWords/
+-rw-r--r--   0 val       (1000) val       (1000)     2695 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/BadWords/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     6163 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/BadWords/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.926829 limnoria-2024.5.30/plugins/BadWords/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     6862 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/BadWords/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6112 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/BadWords/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6277 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/BadWords/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7475 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/BadWords/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3943 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/BadWords/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.926829 limnoria-2024.5.30/plugins/Channel/
+-rw-r--r--   0 val       (1000) val       (1000)     2480 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Channel/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3497 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Channel/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.926829 limnoria-2024.5.30/plugins/Channel/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    32456 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Channel/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    35277 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Channel/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    32166 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Channel/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    32899 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Channel/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)    33333 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Channel/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    44679 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Channel/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    13344 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Channel/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.926829 limnoria-2024.5.30/plugins/ChannelLogger/
+-rw-r--r--   0 val       (1000) val       (1000)     2531 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelLogger/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5994 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelLogger/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.926829 limnoria-2024.5.30/plugins/ChannelLogger/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5491 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelLogger/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5340 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelLogger/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5607 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelLogger/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     5183 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelLogger/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    13745 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelLogger/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9242 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelLogger/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.926829 limnoria-2024.5.30/plugins/ChannelStats/
+-rw-r--r--   0 val       (1000) val       (1000)     2682 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelStats/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3449 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelStats/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.926829 limnoria-2024.5.30/plugins/ChannelStats/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     6426 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelStats/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6640 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelStats/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6242 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelStats/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    15391 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelStats/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4870 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ChannelStats/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.926829 limnoria-2024.5.30/plugins/Conditional/
+-rw-r--r--   0 val       (1000) val       (1000)     2907 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Conditional/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2763 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Conditional/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.926829 limnoria-2024.5.30/plugins/Conditional/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     8160 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Conditional/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7180 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Conditional/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7493 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Conditional/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    11342 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Conditional/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6497 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Conditional/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.926829 limnoria-2024.5.30/plugins/Config/
+-rw-r--r--   0 val       (1000) val       (1000)     2325 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Config/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Config/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.926829 limnoria-2024.5.30/plugins/Config/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     9209 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Config/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     9329 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Config/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     9333 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Config/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     9333 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Config/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     9265 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Config/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    21747 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Config/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    25531 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Config/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.926829 limnoria-2024.5.30/plugins/Ctcp/
+-rw-r--r--   0 val       (1000) val       (1000)     2420 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Ctcp/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3652 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Ctcp/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.930829 limnoria-2024.5.30/plugins/Ctcp/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2084 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Ctcp/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     2196 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Ctcp/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2072 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Ctcp/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2073 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Ctcp/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     1911 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Ctcp/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7136 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Ctcp/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1785 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Ctcp/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.930829 limnoria-2024.5.30/plugins/DDG/
+-rw-r--r--   0 val       (1000) val       (1000)     2670 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/DDG/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3332 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/DDG/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     6037 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/DDG/parser.py
+-rw-r--r--   0 val       (1000) val       (1000)     6988 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/DDG/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2391 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/DDG/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.930829 limnoria-2024.5.30/plugins/Debug/
+-rw-r--r--   0 val       (1000) val       (1000)     2377 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Debug/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2399 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Debug/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     7253 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Debug/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2648 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Debug/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.930829 limnoria-2024.5.30/plugins/Dict/
+-rw-r--r--   0 val       (1000) val       (1000)     2559 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dict/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2877 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dict/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.930829 limnoria-2024.5.30/plugins/Dict/local/
+-rw-r--r--   0 val       (1000) val       (1000)       58 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dict/local/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)    12309 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dict/local/dictclient.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.930829 limnoria-2024.5.30/plugins/Dict/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     3731 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dict/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     3433 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dict/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     3365 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dict/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     6458 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dict/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2548 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dict/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.930829 limnoria-2024.5.30/plugins/Dunno/
+-rw-r--r--   0 val       (1000) val       (1000)     2817 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dunno/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2511 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dunno/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.930829 limnoria-2024.5.30/plugins/Dunno/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1414 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dunno/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     1637 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dunno/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1557 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dunno/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1441 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dunno/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3095 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dunno/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3446 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Dunno/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.930829 limnoria-2024.5.30/plugins/Factoids/
+-rw-r--r--   0 val       (1000) val       (1000)     2738 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Factoids/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4867 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Factoids/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.930829 limnoria-2024.5.30/plugins/Factoids/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    14672 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Factoids/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    14207 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Factoids/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    13986 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Factoids/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    37539 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Factoids/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    10544 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Factoids/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.930829 limnoria-2024.5.30/plugins/Fediverse/
+-rw-r--r--   0 val       (1000) val       (1000)     2506 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Fediverse/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     9206 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Fediverse/activitypub.py
+-rw-r--r--   0 val       (1000) val       (1000)     3583 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Fediverse/config.py
+-rw-r--r--   0 val       (1000) val       (1000)    16853 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Fediverse/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    21650 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Fediverse/test.py
+-rw-r--r--   0 val       (1000) val       (1000)    21570 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Fediverse/test_data.py
+-rw-r--r--   0 val       (1000) val       (1000)     2558 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Fediverse/utils.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.930829 limnoria-2024.5.30/plugins/Filter/
+-rw-r--r--   0 val       (1000) val       (1000)     2691 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Filter/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3118 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Filter/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.930829 limnoria-2024.5.30/plugins/Filter/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    14523 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Filter/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    13736 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Filter/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    14301 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Filter/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    27294 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Filter/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     7848 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Filter/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.934829 limnoria-2024.5.30/plugins/Format/
+-rw-r--r--   0 val       (1000) val       (1000)     2559 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Format/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2522 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Format/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.934829 limnoria-2024.5.30/plugins/Format/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     6742 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Format/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5998 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Format/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6115 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Format/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7452 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Format/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4078 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Format/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.934829 limnoria-2024.5.30/plugins/GPG/
+-rw-r--r--   0 val       (1000) val       (1000)     2606 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/GPG/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2996 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/GPG/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     9566 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/GPG/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     5817 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/GPG/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.934829 limnoria-2024.5.30/plugins/Games/
+-rw-r--r--   0 val       (1000) val       (1000)     2660 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Games/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2313 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Games/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.934829 limnoria-2024.5.30/plugins/Games/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4801 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Games/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5274 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Games/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4968 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Games/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4732 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Games/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7248 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Games/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2854 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Games/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.934829 limnoria-2024.5.30/plugins/Geography/
+-rw-r--r--   0 val       (1000) val       (1000)     2578 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Geography/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     1936 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Geography/common.py
+-rw-r--r--   0 val       (1000) val       (1000)     2441 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Geography/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     2924 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Geography/nominatim.py
+-rw-r--r--   0 val       (1000) val       (1000)     6528 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Geography/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    10325 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Geography/test.py
+-rw-r--r--   0 val       (1000) val       (1000)     5514 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Geography/wikidata.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.934829 limnoria-2024.5.30/plugins/Google/
+-rw-r--r--   0 val       (1000) val       (1000)     2507 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Google/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     7042 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Google/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.934829 limnoria-2024.5.30/plugins/Google/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     9595 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Google/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     9003 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Google/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     9000 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Google/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     4460 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Google/parser.py
+-rw-r--r--   0 val       (1000) val       (1000)    11693 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Google/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3095 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Google/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.934829 limnoria-2024.5.30/plugins/Hashes/
+-rw-r--r--   0 val       (1000) val       (1000)     2585 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Hashes/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2244 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Hashes/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     4049 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Hashes/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2754 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Hashes/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.934829 limnoria-2024.5.30/plugins/Herald/
+-rw-r--r--   0 val       (1000) val       (1000)     2423 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Herald/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3907 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Herald/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.934829 limnoria-2024.5.30/plugins/Herald/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7333 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Herald/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6711 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Herald/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6615 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Herald/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    10794 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Herald/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1789 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Herald/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.934829 limnoria-2024.5.30/plugins/Internet/
+-rw-r--r--   0 val       (1000) val       (1000)     2676 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Internet/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2541 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Internet/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.934829 limnoria-2024.5.30/plugins/Internet/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2313 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Internet/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1791 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Internet/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1769 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Internet/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     8904 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Internet/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2355 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Internet/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/Karma/
+-rw-r--r--   0 val       (1000) val       (1000)     2540 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Karma/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3929 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Karma/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/Karma/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7837 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Karma/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7070 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Karma/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7143 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Karma/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    18303 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Karma/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9962 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Karma/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/Lart/
+-rw-r--r--   0 val       (1000) val       (1000)     2571 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Lart/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2679 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Lart/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/Lart/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2427 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Lart/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2027 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Lart/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1956 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Lart/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     4264 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Lart/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2583 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Lart/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/Later/
+-rw-r--r--   0 val       (1000) val       (1000)     2650 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Later/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3413 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Later/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/Later/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7371 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Later/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     7908 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Later/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6739 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Later/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7370 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Later/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    11043 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Later/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6360 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Later/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/Limiter/
+-rw-r--r--   0 val       (1000) val       (1000)     2662 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Limiter/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3141 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Limiter/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/Limiter/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2685 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Limiter/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2688 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Limiter/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2724 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Limiter/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     2573 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Limiter/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3657 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Limiter/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2871 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Limiter/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/LogToIrc/
+-rw-r--r--   0 val       (1000) val       (1000)     2457 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/LogToIrc/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5627 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/LogToIrc/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     6213 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/LogToIrc/handler.py
+-rw-r--r--   0 val       (1000) val       (1000)     2710 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/LogToIrc/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1781 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/LogToIrc/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/Math/
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Math/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2516 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Math/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/Math/local/
+-rw-r--r--   0 val       (1000) val       (1000)       58 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Math/local/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)    46382 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Math/local/convertcore.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/Math/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5920 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Math/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5424 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Math/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5331 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Math/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     5325 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Math/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    11324 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Math/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9441 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Math/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/MessageParser/
+-rw-r--r--   0 val       (1000) val       (1000)     3026 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/MessageParser/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4464 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/MessageParser/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/MessageParser/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    11282 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/MessageParser/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    10121 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/MessageParser/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    10440 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/MessageParser/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    20338 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/MessageParser/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    11746 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/MessageParser/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.938829 limnoria-2024.5.30/plugins/Misc/
+-rw-r--r--   0 val       (1000) val       (1000)     2299 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Misc/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4131 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Misc/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/Misc/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    13201 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Misc/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    14554 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Misc/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    13747 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Misc/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    13209 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Misc/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)    13537 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Misc/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    29848 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Misc/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    17530 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Misc/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/MoobotFactoids/
+-rw-r--r--   0 val       (1000) val       (1000)     2648 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/MoobotFactoids/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2740 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/MoobotFactoids/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/MoobotFactoids/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    11225 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/MoobotFactoids/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    10014 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/MoobotFactoids/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    10059 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/MoobotFactoids/locales/it.po
+-rwxr-xr-x   0 val       (1000) val       (1000)    29418 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/MoobotFactoids/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    16971 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/MoobotFactoids/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/Network/
+-rw-r--r--   0 val       (1000) val       (1000)     2514 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Network/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Network/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/Network/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7181 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Network/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     8612 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Network/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7289 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Network/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7472 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Network/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    12972 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Network/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3097 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Network/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/News/
+-rw-r--r--   0 val       (1000) val       (1000)     2777 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/News/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2519 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/News/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/News/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4608 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/News/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4221 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/News/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4314 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/News/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     8659 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/News/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3616 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/News/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/NickAuth/
+-rw-r--r--   0 val       (1000) val       (1000)     2574 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/NickAuth/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2495 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/NickAuth/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/NickAuth/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4837 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/NickAuth/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     4838 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/NickAuth/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     9213 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/NickAuth/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6306 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/NickAuth/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/NickCapture/
+-rw-r--r--   0 val       (1000) val       (1000)     2582 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/NickCapture/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2738 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/NickCapture/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/NickCapture/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1598 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/NickCapture/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     1716 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/NickCapture/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1592 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/NickCapture/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1500 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/NickCapture/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     5415 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/NickCapture/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1799 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/NickCapture/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/Nickometer/
+-rw-r--r--   0 val       (1000) val       (1000)     3249 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Nickometer/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2616 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Nickometer/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/Nickometer/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1338 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Nickometer/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1027 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Nickometer/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)      952 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Nickometer/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     9695 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Nickometer/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2183 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Nickometer/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/Note/
+-rw-r--r--   0 val       (1000) val       (1000)     2645 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Note/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3477 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Note/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/Note/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4033 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Note/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     3453 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Note/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     3399 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Note/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    16493 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Note/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4040 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Note/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.942829 limnoria-2024.5.30/plugins/Owner/
+-rw-r--r--   0 val       (1000) val       (1000)     2427 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Owner/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3252 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Owner/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.946829 limnoria-2024.5.30/plugins/Owner/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     8724 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Owner/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5600 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Owner/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     8546 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Owner/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     9038 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Owner/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     8811 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Owner/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    33701 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Owner/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9690 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Owner/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.946829 limnoria-2024.5.30/plugins/Plugin/
+-rw-r--r--   0 val       (1000) val       (1000)     2666 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Plugin/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2523 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Plugin/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.946829 limnoria-2024.5.30/plugins/Plugin/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7234 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Plugin/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     7937 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Plugin/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6377 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Plugin/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7290 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Plugin/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     9985 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Plugin/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4272 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Plugin/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.946829 limnoria-2024.5.30/plugins/PluginDownloader/
+-rw-r--r--   0 val       (1000) val       (1000)     2670 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/PluginDownloader/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2535 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/PluginDownloader/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.946829 limnoria-2024.5.30/plugins/PluginDownloader/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4570 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/PluginDownloader/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     6726 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/PluginDownloader/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6327 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/PluginDownloader/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5727 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/PluginDownloader/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    16307 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/PluginDownloader/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3847 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/PluginDownloader/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.946829 limnoria-2024.5.30/plugins/Poll/
+-rw-r--r--   0 val       (1000) val       (1000)     2516 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Poll/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2922 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Poll/config.py
+-rw-r--r--   0 val       (1000) val       (1000)     8542 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Poll/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6858 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Poll/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.946829 limnoria-2024.5.30/plugins/Praise/
+-rw-r--r--   0 val       (1000) val       (1000)     2528 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Praise/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2695 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Praise/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.946829 limnoria-2024.5.30/plugins/Praise/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2548 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Praise/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2424 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Praise/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2352 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Praise/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     4348 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Praise/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1953 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Praise/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.946829 limnoria-2024.5.30/plugins/Protector/
+-rw-r--r--   0 val       (1000) val       (1000)     2594 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Protector/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2901 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Protector/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.946829 limnoria-2024.5.30/plugins/Protector/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1626 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Protector/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1245 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Protector/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1153 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Protector/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7598 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Protector/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1789 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Protector/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.946829 limnoria-2024.5.30/plugins/Quote/
+-rw-r--r--   0 val       (1000) val       (1000)     2524 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Quote/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2519 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Quote/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.946829 limnoria-2024.5.30/plugins/Quote/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1700 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Quote/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1418 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Quote/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1372 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Quote/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3106 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Quote/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2541 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Quote/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.946829 limnoria-2024.5.30/plugins/QuoteGrabs/
+-rw-r--r--   0 val       (1000) val       (1000)     2675 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/QuoteGrabs/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3670 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/QuoteGrabs/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.946829 limnoria-2024.5.30/plugins/QuoteGrabs/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7337 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/QuoteGrabs/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6529 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/QuoteGrabs/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     6636 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/QuoteGrabs/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    17122 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/QuoteGrabs/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     8560 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/QuoteGrabs/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.950829 limnoria-2024.5.30/plugins/RSS/
+-rw-r--r--   0 val       (1000) val       (1000)     2706 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/RSS/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     6867 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/RSS/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.950829 limnoria-2024.5.30/plugins/RSS/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    12451 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/RSS/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    15597 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/RSS/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    13213 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/RSS/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    13001 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/RSS/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)    12728 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/RSS/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    30590 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/RSS/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    26289 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/RSS/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.950829 limnoria-2024.5.30/plugins/Relay/
+-rw-r--r--   0 val       (1000) val       (1000)     2517 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Relay/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4744 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Relay/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.950829 limnoria-2024.5.30/plugins/Relay/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     8274 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Relay/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7545 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Relay/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7487 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Relay/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    19682 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Relay/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     1787 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Relay/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.954829 limnoria-2024.5.30/plugins/Reply/
+-rw-r--r--   0 val       (1000) val       (1000)     2572 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Reply/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2519 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Reply/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.954829 limnoria-2024.5.30/plugins/Reply/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     2384 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Reply/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     2630 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Reply/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2331 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Reply/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2669 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Reply/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     2433 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Reply/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3694 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Reply/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3051 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Reply/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.954829 limnoria-2024.5.30/plugins/Scheduler/
+-rw-r--r--   0 val       (1000) val       (1000)     2757 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Scheduler/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2541 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Scheduler/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.954829 limnoria-2024.5.30/plugins/Scheduler/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4116 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Scheduler/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     3797 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Scheduler/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     3850 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Scheduler/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    12852 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Scheduler/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     8402 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Scheduler/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.958829 limnoria-2024.5.30/plugins/SedRegex/
+-rw-r--r--   0 val       (1000) val       (1000)     2709 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/SedRegex/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4356 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/SedRegex/config.py
+-rwxr-xr-x   0 val       (1000) val       (1000)      874 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/SedRegex/constants.py
+-rw-r--r--   0 val       (1000) val       (1000)    10523 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/SedRegex/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    13147 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/SedRegex/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.958829 limnoria-2024.5.30/plugins/Seen/
+-rw-r--r--   0 val       (1000) val       (1000)     2637 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Seen/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2979 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Seen/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.958829 limnoria-2024.5.30/plugins/Seen/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5779 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Seen/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     6954 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Seen/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     6235 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Seen/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5812 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Seen/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    16735 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Seen/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6414 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Seen/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.958829 limnoria-2024.5.30/plugins/Services/
+-rw-r--r--   0 val       (1000) val       (1000)     2607 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Services/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5658 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Services/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.958829 limnoria-2024.5.30/plugins/Services/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    11466 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Services/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    11843 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Services/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    11294 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Services/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    11525 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Services/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    35273 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Services/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    14436 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Services/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.958829 limnoria-2024.5.30/plugins/ShrinkUrl/
+-rw-r--r--   0 val       (1000) val       (1000)     2542 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ShrinkUrl/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5035 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ShrinkUrl/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.958829 limnoria-2024.5.30/plugins/ShrinkUrl/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5983 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ShrinkUrl/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5213 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ShrinkUrl/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5243 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ShrinkUrl/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    10186 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ShrinkUrl/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     5286 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/ShrinkUrl/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.958829 limnoria-2024.5.30/plugins/Status/
+-rw-r--r--   0 val       (1000) val       (1000)     2457 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Status/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2901 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Status/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.958829 limnoria-2024.5.30/plugins/Status/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5435 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Status/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     6124 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Status/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5481 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Status/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5563 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Status/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    11461 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Status/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3180 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Status/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/String/
+-rw-r--r--   0 val       (1000) val       (1000)     2551 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/String/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3429 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/String/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/String/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     9469 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/String/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     8780 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/String/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     8557 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/String/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     9911 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/String/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     7585 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/String/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/Success/
+-rw-r--r--   0 val       (1000) val       (1000)     2646 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Success/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2751 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Success/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/Success/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     1578 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Success/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     1435 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Success/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     1323 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Success/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     3471 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Success/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     2272 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Success/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/Time/
+-rw-r--r--   0 val       (1000) val       (1000)     2673 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Time/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2640 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Time/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/Time/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     5480 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Time/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     6313 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Time/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     5483 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Time/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     5849 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Time/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)     5574 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Time/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    10127 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Time/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     5071 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Time/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/Todo/
+-rw-r--r--   0 val       (1000) val       (1000)     2607 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Todo/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2683 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Todo/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/Todo/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     4575 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Todo/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     5089 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Todo/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4595 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Todo/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4664 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Todo/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    10596 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Todo/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     6654 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Todo/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/Topic/
+-rw-r--r--   0 val       (1000) val       (1000)     2583 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Topic/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     4776 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Topic/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/Topic/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    18502 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Topic/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    16877 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Topic/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    17231 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Topic/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    25153 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Topic/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)    13078 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Topic/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/URL/
+-rw-r--r--   0 val       (1000) val       (1000)     2661 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/URL/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2629 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/URL/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/URL/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     3421 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/URL/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     2907 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/URL/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     2841 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/URL/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     6765 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/URL/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4241 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/URL/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/Unix/
+-rw-r--r--   0 val       (1000) val       (1000)     2669 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Unix/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     6252 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Unix/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/Unix/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    13680 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Unix/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    11967 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Unix/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    12075 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Unix/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    20231 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Unix/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     7851 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Unix/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.962829 limnoria-2024.5.30/plugins/User/
+-rw-r--r--   0 val       (1000) val       (1000)     2355 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/User/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2728 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/User/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.966829 limnoria-2024.5.30/plugins/User/locales/
+-rw-r--r--   0 val       (1000) val       (1000)    15416 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/User/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)    21068 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/User/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)    19566 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/User/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)    10856 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/User/locales/hu.po
+-rw-r--r--   0 val       (1000) val       (1000)    15349 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/User/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    23217 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/User/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9203 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/User/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.966829 limnoria-2024.5.30/plugins/Utilities/
+-rw-r--r--   0 val       (1000) val       (1000)     2407 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Utilities/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2541 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Utilities/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.966829 limnoria-2024.5.30/plugins/Utilities/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     3623 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Utilities/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     4827 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Utilities/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     4250 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Utilities/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     4335 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Utilities/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)     7065 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Utilities/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     3958 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Utilities/test.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.966829 limnoria-2024.5.30/plugins/Web/
+-rw-r--r--   0 val       (1000) val       (1000)     2446 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Web/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     5246 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Web/config.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.966829 limnoria-2024.5.30/plugins/Web/locales/
+-rw-r--r--   0 val       (1000) val       (1000)     7308 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Web/locales/de.po
+-rw-r--r--   0 val       (1000) val       (1000)     8904 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Web/locales/fi.po
+-rw-r--r--   0 val       (1000) val       (1000)     7488 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Web/locales/fr.po
+-rw-r--r--   0 val       (1000) val       (1000)     7113 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Web/locales/it.po
+-rw-r--r--   0 val       (1000) val       (1000)    17047 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Web/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     9430 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/Web/test.py
+-rw-r--r--   0 val       (1000) val       (1000)    23695 2024-05-31 21:10:49.000000 limnoria-2024.5.30/plugins/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)      192 2024-05-31 21:10:49.000000 limnoria-2024.5.30/pyproject.toml
+-rw-r--r--   0 val       (1000) val       (1000)      946 2024-05-31 21:10:49.000000 limnoria-2024.5.30/requirements.txt
+-rw-r--r--   0 val       (1000) val       (1000)       38 2024-05-31 21:10:53.974829 limnoria-2024.5.30/setup.cfg
+-rw-r--r--   0 val       (1000) val       (1000)     8511 2024-05-31 21:10:49.000000 limnoria-2024.5.30/setup.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.970829 limnoria-2024.5.30/src/
+-rw-r--r--   0 val       (1000) val       (1000)     4117 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     3548 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/ansi.py
+-rw-r--r--   0 val       (1000) val       (1000)    75220 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/callbacks.py
+-rw-r--r--   0 val       (1000) val       (1000)    14986 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/cdb.py
+-rw-r--r--   0 val       (1000) val       (1000)    41479 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/commands.py
+-rw-r--r--   0 val       (1000) val       (1000)    67508 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/conf.py
+-rw-r--r--   0 val       (1000) val       (1000)    14165 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/dbi.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.970829 limnoria-2024.5.30/src/drivers/
+-rw-r--r--   0 val       (1000) val       (1000)    19713 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/drivers/Socket.py
+-rw-r--r--   0 val       (1000) val       (1000)     9696 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/drivers/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2350 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/dynamicScope.py
+-rw-r--r--   0 val       (1000) val       (1000)     2997 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/gpg.py
+-rw-r--r--   0 val       (1000) val       (1000)    21040 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/httpserver.py
+-rw-r--r--   0 val       (1000) val       (1000)    13332 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/i18n.py
+-rw-r--r--   0 val       (1000) val       (1000)    52151 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/ircdb.py
+-rw-r--r--   0 val       (1000) val       (1000)    98073 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/irclib.py
+-rw-r--r--   0 val       (1000) val       (1000)    38939 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/ircmsgs.py
+-rw-r--r--   0 val       (1000) val       (1000)    43234 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/ircutils.py
+-rw-r--r--   0 val       (1000) val       (1000)    16573 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/log.py
+-rw-r--r--   0 val       (1000) val       (1000)     8379 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     5342 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/questions.py
+-rw-r--r--   0 val       (1000) val       (1000)    34261 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/registry.py
+-rw-r--r--   0 val       (1000) val       (1000)     6156 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/schedule.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.970829 limnoria-2024.5.30/src/scripts/
+-rw-r--r--   0 val       (1000) val       (1000)        0 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/scripts/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)    15886 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/scripts/limnoria.py
+-rw-r--r--   0 val       (1000) val       (1000)     5258 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/scripts/limnoria_adduser.py
+-rw-r--r--   0 val       (1000) val       (1000)     5455 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/scripts/limnoria_botchk.py
+-rw-r--r--   0 val       (1000) val       (1000)    10536 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/scripts/limnoria_plugin_create.py
+-rw-r--r--   0 val       (1000) val       (1000)    14353 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/scripts/limnoria_plugin_doc.py
+-rw-r--r--   0 val       (1000) val       (1000)     4454 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/scripts/limnoria_reset_password.py
+-rw-r--r--   0 val       (1000) val       (1000)    10443 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/scripts/limnoria_test.py
+-rw-r--r--   0 val       (1000) val       (1000)    37750 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/scripts/limnoria_wizard.py
+-rw-r--r--   0 val       (1000) val       (1000)     4790 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/setup.py
+-rw-r--r--   0 val       (1000) val       (1000)     8198 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/shlex.py
+-rw-r--r--   0 val       (1000) val       (1000)    25444 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/test.py
+-rw-r--r--   0 val       (1000) val       (1000)     3869 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/unpreserve.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.970829 limnoria-2024.5.30/src/utils/
+-rw-r--r--   0 val       (1000) val       (1000)     2575 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     1741 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/crypt.py
+-rw-r--r--   0 val       (1000) val       (1000)     1992 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/error.py
+-rw-r--r--   0 val       (1000) val       (1000)     9475 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/file.py
+-rw-r--r--   0 val       (1000) val       (1000)    11742 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/gen.py
+-rw-r--r--   0 val       (1000) val       (1000)     5210 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/iter.py
+-rw-r--r--   0 val       (1000) val       (1000)     6195 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/math_evaluator.py
+-rw-r--r--   0 val       (1000) val       (1000)     3914 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/minisix.py
+-rw-r--r--   0 val       (1000) val       (1000)     6526 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/net.py
+-rw-r--r--   0 val       (1000) val       (1000)     7726 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/python.py
+-rw-r--r--   0 val       (1000) val       (1000)     4169 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/seq.py
+-rw-r--r--   0 val       (1000) val       (1000)    21873 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/str.py
+-rw-r--r--   0 val       (1000) val       (1000)    19840 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/structures.py
+-rw-r--r--   0 val       (1000) val       (1000)     2838 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/time.py
+-rw-r--r--   0 val       (1000) val       (1000)     8826 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/transaction.py
+-rw-r--r--   0 val       (1000) val       (1000)    10662 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/utils/web.py
+-rw-r--r--   0 val       (1000) val       (1000)      175 2024-05-31 21:10:53.000000 limnoria-2024.5.30/src/version.py
+-rw-r--r--   0 val       (1000) val       (1000)     7660 2024-05-31 21:10:49.000000 limnoria-2024.5.30/src/world.py
+drwxr-xr-x   0 val       (1000) val       (1000)        0 2024-05-31 21:10:53.974829 limnoria-2024.5.30/test/
+-rw-r--r--   0 val       (1000) val       (1000)     1754 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/__init__.py
+-rw-r--r--   0 val       (1000) val       (1000)     2265 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test.py
+-rw-r--r--   0 val       (1000) val       (1000)    49856 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_callbacks.py
+-rw-r--r--   0 val       (1000) val       (1000)     9002 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_commands.py
+-rw-r--r--   0 val       (1000) val       (1000)     2813 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_conf.py
+-rw-r--r--   0 val       (1000) val       (1000)     4122 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_drivers.py
+-rw-r--r--   0 val       (1000) val       (1000)     2458 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_dynamicScope.py
+-rw-r--r--   0 val       (1000) val       (1000)     3225 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_firewall.py
+-rw-r--r--   0 val       (1000) val       (1000)     1925 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_format.py
+-rw-r--r--   0 val       (1000) val       (1000)     2832 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_i18n.py
+-rw-r--r--   0 val       (1000) val       (1000)    29200 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_ircdb.py
+-rw-r--r--   0 val       (1000) val       (1000)    67775 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_irclib.py
+-rw-r--r--   0 val       (1000) val       (1000)    14083 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_ircmsgs.py
+-rw-r--r--   0 val       (1000) val       (1000)    22829 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_ircutils.py
+-rw-r--r--   0 val       (1000) val       (1000)     3341 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_misc.py
+-rw-r--r--   0 val       (1000) val       (1000)     2016 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_plugin.py
+-rw-r--r--   0 val       (1000) val       (1000)     4832 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_plugin_create.py
+-rw-r--r--   0 val       (1000) val       (1000)     2430 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_plugins.py
+-rw-r--r--   0 val       (1000) val       (1000)    13283 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_registry.py
+-rw-r--r--   0 val       (1000) val       (1000)     4575 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_schedule.py
+-rw-r--r--   0 val       (1000) val       (1000)     3759 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_standardSubstitute.py
+-rw-r--r--   0 val       (1000) val       (1000)    49349 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_utils.py
+-rw-r--r--   0 val       (1000) val       (1000)     3672 2024-05-31 21:10:49.000000 limnoria-2024.5.30/test/test_yn.py
```

### Comparing `limnoria-2024.4.26/LICENSE.md` & `limnoria-2024.5.30/LICENSE.md`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/Makefile` & `limnoria-2024.5.30/Makefile`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/PKG-INFO` & `limnoria-2024.5.30/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limnoria
-Version: 2024.4.26
+Version: 2024.5.30
 Summary: A multipurpose Python IRC bot, designed for flexibility and robustness , while being easy to install, set up, and maintain.
 Home-page: https://limnoria.net/
 Download-URL: https://pypi.python.org/pypi/limnoria
 Author: Valentin Lorentz
 Author-email: progval+limnoria@progval.net
 Platform: linux
 Platform: linux2
```

### Comparing `limnoria-2024.4.26/README.md` & `limnoria-2024.5.30/README.md`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/limnoria.egg-info/PKG-INFO` & `limnoria-2024.5.30/limnoria.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: limnoria
-Version: 2024.4.26
+Version: 2024.5.30
 Summary: A multipurpose Python IRC bot, designed for flexibility and robustness , while being easy to install, set up, and maintain.
 Home-page: https://limnoria.net/
 Download-URL: https://pypi.python.org/pypi/limnoria
 Author: Valentin Lorentz
 Author-email: progval+limnoria@progval.net
 Platform: linux
 Platform: linux2
```

### Comparing `limnoria-2024.4.26/limnoria.egg-info/SOURCES.txt` & `limnoria-2024.5.30/limnoria.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/limnoria.egg-info/entry_points.txt` & `limnoria-2024.5.30/limnoria.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/locales/de.po` & `limnoria-2024.5.30/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/locales/fi.po` & `limnoria-2024.5.30/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/locales/fr.po` & `limnoria-2024.5.30/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/locales/fr.py` & `limnoria-2024.5.30/locales/fr.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/locales/it.po` & `limnoria-2024.5.30/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/locales/messages.pot` & `limnoria-2024.5.30/locales/messages.pot`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/limnoria-adduser.1` & `limnoria-2024.5.30/man/limnoria-adduser.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/limnoria-botchk.1` & `limnoria-2024.5.30/man/limnoria-botchk.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/limnoria-plugin-create.1` & `limnoria-2024.5.30/man/limnoria-plugin-create.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/limnoria-plugin-doc.1` & `limnoria-2024.5.30/man/limnoria-plugin-doc.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/limnoria-reset-password.1` & `limnoria-2024.5.30/man/limnoria-reset-password.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/limnoria-test.1` & `limnoria-2024.5.30/man/limnoria-test.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/limnoria-wizard.1` & `limnoria-2024.5.30/man/limnoria-wizard.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/limnoria.1` & `limnoria-2024.5.30/man/limnoria.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/supybot-adduser.1` & `limnoria-2024.5.30/man/supybot-adduser.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/supybot-botchk.1` & `limnoria-2024.5.30/man/supybot-botchk.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/supybot-plugin-create.1` & `limnoria-2024.5.30/man/supybot-plugin-create.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/supybot-plugin-doc.1` & `limnoria-2024.5.30/man/supybot-plugin-doc.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/supybot-reset-password.1` & `limnoria-2024.5.30/man/supybot-reset-password.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/supybot-test.1` & `limnoria-2024.5.30/man/supybot-test.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/supybot-wizard.1` & `limnoria-2024.5.30/man/supybot-wizard.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/man/supybot.1` & `limnoria-2024.5.30/man/supybot.1`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Admin/__init__.py` & `limnoria-2024.5.30/plugins/Admin/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Admin/config.py` & `limnoria-2024.5.30/plugins/Admin/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Admin/locales/de.po` & `limnoria-2024.5.30/plugins/Admin/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Admin/locales/fi.po` & `limnoria-2024.5.30/plugins/Admin/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Admin/locales/fr.po` & `limnoria-2024.5.30/plugins/Admin/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Admin/locales/it.po` & `limnoria-2024.5.30/plugins/Admin/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Admin/plugin.py` & `limnoria-2024.5.30/plugins/Admin/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Admin/test.py` & `limnoria-2024.5.30/plugins/Admin/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Aka/__init__.py` & `limnoria-2024.5.30/plugins/Aka/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Aka/config.py` & `limnoria-2024.5.30/plugins/Aka/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Aka/locales/fi.po` & `limnoria-2024.5.30/plugins/Aka/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Aka/plugin.py` & `limnoria-2024.5.30/plugins/Aka/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Aka/test.py` & `limnoria-2024.5.30/plugins/Aka/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Alias/__init__.py` & `limnoria-2024.5.30/plugins/Alias/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Alias/config.py` & `limnoria-2024.5.30/plugins/Alias/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Alias/locales/de.po` & `limnoria-2024.5.30/plugins/Alias/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Alias/locales/fi.po` & `limnoria-2024.5.30/plugins/Alias/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Alias/locales/fr.po` & `limnoria-2024.5.30/plugins/Alias/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Alias/locales/hu.po` & `limnoria-2024.5.30/plugins/Alias/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Alias/locales/it.po` & `limnoria-2024.5.30/plugins/Alias/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Alias/plugin.py` & `limnoria-2024.5.30/plugins/Alias/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Alias/test.py` & `limnoria-2024.5.30/plugins/Alias/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Anonymous/__init__.py` & `limnoria-2024.5.30/plugins/Anonymous/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Anonymous/config.py` & `limnoria-2024.5.30/plugins/Anonymous/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Anonymous/locales/de.po` & `limnoria-2024.5.30/plugins/Anonymous/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Anonymous/locales/fi.po` & `limnoria-2024.5.30/plugins/Anonymous/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Anonymous/locales/fr.po` & `limnoria-2024.5.30/plugins/Anonymous/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Anonymous/locales/hu.po` & `limnoria-2024.5.30/plugins/Anonymous/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Anonymous/locales/it.po` & `limnoria-2024.5.30/plugins/Anonymous/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Anonymous/plugin.py` & `limnoria-2024.5.30/plugins/Anonymous/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Anonymous/test.py` & `limnoria-2024.5.30/plugins/Anonymous/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/AutoMode/__init__.py` & `limnoria-2024.5.30/plugins/AutoMode/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/AutoMode/config.py` & `limnoria-2024.5.30/plugins/AutoMode/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/AutoMode/locales/de.po` & `limnoria-2024.5.30/plugins/AutoMode/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/AutoMode/locales/fi.po` & `limnoria-2024.5.30/plugins/AutoMode/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/AutoMode/locales/fr.po` & `limnoria-2024.5.30/plugins/AutoMode/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/AutoMode/locales/it.po` & `limnoria-2024.5.30/plugins/AutoMode/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/AutoMode/plugin.py` & `limnoria-2024.5.30/plugins/AutoMode/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/AutoMode/test.py` & `limnoria-2024.5.30/plugins/AutoMode/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Autocomplete/__init__.py` & `limnoria-2024.5.30/plugins/Autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Autocomplete/config.py` & `limnoria-2024.5.30/plugins/Autocomplete/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Autocomplete/plugin.py` & `limnoria-2024.5.30/plugins/Autocomplete/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Autocomplete/test.py` & `limnoria-2024.5.30/plugins/Autocomplete/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/BadWords/__init__.py` & `limnoria-2024.5.30/plugins/BadWords/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/BadWords/config.py` & `limnoria-2024.5.30/plugins/BadWords/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/BadWords/locales/fi.po` & `limnoria-2024.5.30/plugins/BadWords/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/BadWords/locales/fr.po` & `limnoria-2024.5.30/plugins/BadWords/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/BadWords/locales/it.po` & `limnoria-2024.5.30/plugins/BadWords/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/BadWords/plugin.py` & `limnoria-2024.5.30/plugins/BadWords/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/BadWords/test.py` & `limnoria-2024.5.30/plugins/BadWords/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Channel/__init__.py` & `limnoria-2024.5.30/plugins/Channel/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Channel/config.py` & `limnoria-2024.5.30/plugins/Channel/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Channel/locales/de.po` & `limnoria-2024.5.30/plugins/Channel/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Channel/locales/fi.po` & `limnoria-2024.5.30/plugins/Channel/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Channel/locales/fr.po` & `limnoria-2024.5.30/plugins/Channel/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Channel/locales/hu.po` & `limnoria-2024.5.30/plugins/Channel/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Channel/locales/it.po` & `limnoria-2024.5.30/plugins/Channel/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Channel/plugin.py` & `limnoria-2024.5.30/plugins/Channel/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Channel/test.py` & `limnoria-2024.5.30/plugins/Channel/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelLogger/__init__.py` & `limnoria-2024.5.30/plugins/ChannelLogger/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelLogger/config.py` & `limnoria-2024.5.30/plugins/ChannelLogger/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelLogger/locales/fi.po` & `limnoria-2024.5.30/plugins/ChannelLogger/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelLogger/locales/fr.po` & `limnoria-2024.5.30/plugins/ChannelLogger/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelLogger/locales/hu.po` & `limnoria-2024.5.30/plugins/ChannelLogger/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelLogger/locales/it.po` & `limnoria-2024.5.30/plugins/ChannelLogger/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelLogger/plugin.py` & `limnoria-2024.5.30/plugins/ChannelLogger/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelLogger/test.py` & `limnoria-2024.5.30/plugins/ChannelLogger/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelStats/__init__.py` & `limnoria-2024.5.30/plugins/ChannelStats/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelStats/config.py` & `limnoria-2024.5.30/plugins/ChannelStats/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelStats/locales/fi.po` & `limnoria-2024.5.30/plugins/ChannelStats/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelStats/locales/fr.po` & `limnoria-2024.5.30/plugins/ChannelStats/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelStats/locales/it.po` & `limnoria-2024.5.30/plugins/ChannelStats/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelStats/plugin.py` & `limnoria-2024.5.30/plugins/ChannelStats/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ChannelStats/test.py` & `limnoria-2024.5.30/plugins/ChannelStats/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Conditional/__init__.py` & `limnoria-2024.5.30/plugins/Conditional/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Conditional/config.py` & `limnoria-2024.5.30/plugins/Conditional/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Conditional/locales/fi.po` & `limnoria-2024.5.30/plugins/Conditional/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Conditional/locales/fr.po` & `limnoria-2024.5.30/plugins/Conditional/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Conditional/locales/it.po` & `limnoria-2024.5.30/plugins/Conditional/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Conditional/plugin.py` & `limnoria-2024.5.30/plugins/Conditional/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Conditional/test.py` & `limnoria-2024.5.30/plugins/Conditional/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Config/__init__.py` & `limnoria-2024.5.30/plugins/Config/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Config/config.py` & `limnoria-2024.5.30/plugins/Config/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Config/locales/de.po` & `limnoria-2024.5.30/plugins/Config/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Config/locales/fi.po` & `limnoria-2024.5.30/plugins/Config/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Config/locales/fr.po` & `limnoria-2024.5.30/plugins/Config/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Config/locales/hu.po` & `limnoria-2024.5.30/plugins/Config/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Config/locales/it.po` & `limnoria-2024.5.30/plugins/Config/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Config/plugin.py` & `limnoria-2024.5.30/plugins/Config/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Config/test.py` & `limnoria-2024.5.30/plugins/Config/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Ctcp/__init__.py` & `limnoria-2024.5.30/plugins/Ctcp/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Ctcp/config.py` & `limnoria-2024.5.30/plugins/Ctcp/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Ctcp/locales/de.po` & `limnoria-2024.5.30/plugins/Ctcp/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Ctcp/locales/fi.po` & `limnoria-2024.5.30/plugins/Ctcp/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Ctcp/locales/fr.po` & `limnoria-2024.5.30/plugins/Ctcp/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Ctcp/locales/hu.po` & `limnoria-2024.5.30/plugins/Ctcp/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Ctcp/locales/it.po` & `limnoria-2024.5.30/plugins/Ctcp/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Ctcp/plugin.py` & `limnoria-2024.5.30/plugins/Ctcp/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Ctcp/test.py` & `limnoria-2024.5.30/plugins/Ctcp/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/DDG/__init__.py` & `limnoria-2024.5.30/plugins/DDG/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/DDG/config.py` & `limnoria-2024.5.30/plugins/DDG/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/DDG/parser.py` & `limnoria-2024.5.30/plugins/DDG/parser.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/DDG/plugin.py` & `limnoria-2024.5.30/plugins/DDG/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/DDG/test.py` & `limnoria-2024.5.30/plugins/DDG/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,18 +35,18 @@
 class DDGTestCase(PluginTestCase):
     plugins = ('DDG',)
 
     if network:
 
         def testSearch(self):
             self.assertRegexp(
-                'ddg search wikipedia', 'Wikipedia.*? - .*?https?\:\/\/')
+                'ddg search wikipedia', r'Wikipedia.*? - .*?https?\:\/\/')
             self.assertRegexp(
                 'ddg search en.wikipedia.org',
                 'Wikipedia, the free encyclopedia\x02 - '
                 '.* <https://en.wikipedia.org/>')
             with conf.supybot.plugins.DDG.region.context('fr-fr'):
                 self.assertRegexp(
                     'ddg search wikipedia',
-                    'Wikipédia, l\'encyclopédie libre - .*?https?\:\/\/')
+                    r'Wikipédia, l\'encyclopédie libre - .*?https?\:\/\/')
 
 # vim:set shiftwidth=4 tabstop=4 expandtab textwidth=79:
```

### Comparing `limnoria-2024.4.26/plugins/Debug/__init__.py` & `limnoria-2024.5.30/plugins/Debug/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Debug/config.py` & `limnoria-2024.5.30/plugins/Debug/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Debug/plugin.py` & `limnoria-2024.5.30/plugins/Debug/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Debug/test.py` & `limnoria-2024.5.30/plugins/Debug/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dict/__init__.py` & `limnoria-2024.5.30/plugins/Dict/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dict/config.py` & `limnoria-2024.5.30/plugins/Dict/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dict/local/dictclient.py` & `limnoria-2024.5.30/plugins/Dict/local/dictclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,15 @@
             raise Exception("Unknown code %d" % code)
 
         while True:
             code, text = self.getresultcode()
             if code != 151 or code is None:
                 break
 
-            resultword, resultdb = re.search('^"(.+)" (\S+)', text).groups()
+            resultword, resultdb = re.search(r'^"(.+)" (\S+)', text).groups()
             defstr = self.get100block()
             retval.append(Definition(self, self.getdbobj(resultdb),
                                      resultword, defstr))
         return retval
 
     def match(self, database, strategy, word):
         """Gets matches for a query.  Arguments are database name,
```

### Comparing `limnoria-2024.4.26/plugins/Dict/locales/fi.po` & `limnoria-2024.5.30/plugins/Dict/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dict/locales/fr.po` & `limnoria-2024.5.30/plugins/Dict/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dict/locales/it.po` & `limnoria-2024.5.30/plugins/Dict/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dict/plugin.py` & `limnoria-2024.5.30/plugins/Dict/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dict/test.py` & `limnoria-2024.5.30/plugins/Dict/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dunno/__init__.py` & `limnoria-2024.5.30/plugins/Dunno/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dunno/config.py` & `limnoria-2024.5.30/plugins/Dunno/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dunno/locales/de.po` & `limnoria-2024.5.30/plugins/Dunno/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dunno/locales/fi.po` & `limnoria-2024.5.30/plugins/Dunno/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dunno/locales/fr.po` & `limnoria-2024.5.30/plugins/Dunno/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dunno/locales/it.po` & `limnoria-2024.5.30/plugins/Dunno/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dunno/plugin.py` & `limnoria-2024.5.30/plugins/Dunno/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Dunno/test.py` & `limnoria-2024.5.30/plugins/Dunno/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Factoids/__init__.py` & `limnoria-2024.5.30/plugins/Factoids/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Factoids/config.py` & `limnoria-2024.5.30/plugins/Factoids/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Factoids/locales/fi.po` & `limnoria-2024.5.30/plugins/Factoids/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Factoids/locales/fr.po` & `limnoria-2024.5.30/plugins/Factoids/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Factoids/locales/it.po` & `limnoria-2024.5.30/plugins/Factoids/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Factoids/plugin.py` & `limnoria-2024.5.30/plugins/Factoids/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Factoids/test.py` & `limnoria-2024.5.30/plugins/Factoids/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Fediverse/__init__.py` & `limnoria-2024.5.30/plugins/Fediverse/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Fediverse/activitypub.py` & `limnoria-2024.5.30/plugins/Fediverse/activitypub.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Fediverse/config.py` & `limnoria-2024.5.30/plugins/Fediverse/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Fediverse/plugin.py` & `limnoria-2024.5.30/plugins/Fediverse/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Fediverse/test.py` & `limnoria-2024.5.30/plugins/Fediverse/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Fediverse/test_data.py` & `limnoria-2024.5.30/plugins/Fediverse/test_data.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Fediverse/utils.py` & `limnoria-2024.5.30/plugins/Fediverse/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 ###
 
 import re
 import datetime
 
 # Credits for the regexp and function: https://stackoverflow.com/a/2765366/539465
 _XSD_DURATION_RE = re.compile(
-    "(?P<sign>-?)P"
-    "(?:(?P<years>\d+)Y)?"
-    "(?:(?P<months>\d+)M)?"
-    "(?:(?P<days>\d+)D)?"
-    "(?:T(?:(?P<hours>\d+)H)?(?:(?P<minutes>\d+)M)?(?:(?P<seconds>\d+)S)?)?"
+    r"(?P<sign>-?)P"
+    r"(?:(?P<years>\d+)Y)?"
+    r"(?:(?P<months>\d+)M)?"
+    r"(?:(?P<days>\d+)D)?"
+    r"(?:T(?:(?P<hours>\d+)H)?(?:(?P<minutes>\d+)M)?(?:(?P<seconds>\d+)S)?)?"
 )
 
 
 def parse_xsd_duration(s):
     """Parses this format to a timedelta:
     https://www.w3.org/TR/xmlschema11-2/#duration"""
     # Fetch the match groups with default value of 0 (not None)
```

### Comparing `limnoria-2024.4.26/plugins/Filter/__init__.py` & `limnoria-2024.5.30/plugins/Filter/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Filter/config.py` & `limnoria-2024.5.30/plugins/Filter/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Filter/locales/fi.po` & `limnoria-2024.5.30/plugins/Filter/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Filter/locales/fr.po` & `limnoria-2024.5.30/plugins/Filter/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Filter/locales/it.po` & `limnoria-2024.5.30/plugins/Filter/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Filter/plugin.py` & `limnoria-2024.5.30/plugins/Filter/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Filter/test.py` & `limnoria-2024.5.30/plugins/Filter/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Format/__init__.py` & `limnoria-2024.5.30/plugins/Format/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Format/config.py` & `limnoria-2024.5.30/plugins/Format/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Format/locales/fi.po` & `limnoria-2024.5.30/plugins/Format/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Format/locales/fr.po` & `limnoria-2024.5.30/plugins/Format/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Format/locales/it.po` & `limnoria-2024.5.30/plugins/Format/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Format/plugin.py` & `limnoria-2024.5.30/plugins/Format/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Format/test.py` & `limnoria-2024.5.30/plugins/Format/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/GPG/__init__.py` & `limnoria-2024.5.30/plugins/GPG/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/GPG/config.py` & `limnoria-2024.5.30/plugins/GPG/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/GPG/plugin.py` & `limnoria-2024.5.30/plugins/GPG/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/GPG/test.py` & `limnoria-2024.5.30/plugins/GPG/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Games/__init__.py` & `limnoria-2024.5.30/plugins/Games/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Games/config.py` & `limnoria-2024.5.30/plugins/Games/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Games/locales/de.po` & `limnoria-2024.5.30/plugins/Games/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Games/locales/fi.po` & `limnoria-2024.5.30/plugins/Games/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Games/locales/fr.po` & `limnoria-2024.5.30/plugins/Games/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Games/locales/it.po` & `limnoria-2024.5.30/plugins/Games/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Games/plugin.py` & `limnoria-2024.5.30/plugins/Games/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Games/test.py` & `limnoria-2024.5.30/plugins/Games/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Geography/__init__.py` & `limnoria-2024.5.30/plugins/Geography/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Geography/common.py` & `limnoria-2024.5.30/plugins/Geography/common.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Geography/config.py` & `limnoria-2024.5.30/plugins/Geography/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Geography/nominatim.py` & `limnoria-2024.5.30/plugins/Geography/nominatim.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Geography/plugin.py` & `limnoria-2024.5.30/plugins/Geography/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Geography/test.py` & `limnoria-2024.5.30/plugins/Geography/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Geography/wikidata.py` & `limnoria-2024.5.30/plugins/Geography/wikidata.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Google/__init__.py` & `limnoria-2024.5.30/plugins/Google/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Google/config.py` & `limnoria-2024.5.30/plugins/Google/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Google/locales/fi.po` & `limnoria-2024.5.30/plugins/Google/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Google/locales/fr.po` & `limnoria-2024.5.30/plugins/Google/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Google/locales/it.po` & `limnoria-2024.5.30/plugins/Google/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Google/parser.py` & `limnoria-2024.5.30/plugins/Google/parser.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Google/plugin.py` & `limnoria-2024.5.30/plugins/Google/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Google/test.py` & `limnoria-2024.5.30/plugins/Google/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Hashes/__init__.py` & `limnoria-2024.5.30/plugins/Hashes/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Hashes/config.py` & `limnoria-2024.5.30/plugins/Hashes/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Hashes/plugin.py` & `limnoria-2024.5.30/plugins/Hashes/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Hashes/test.py` & `limnoria-2024.5.30/plugins/Hashes/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Herald/__init__.py` & `limnoria-2024.5.30/plugins/Herald/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Herald/config.py` & `limnoria-2024.5.30/plugins/Herald/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Herald/locales/fi.po` & `limnoria-2024.5.30/plugins/Herald/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Herald/locales/fr.po` & `limnoria-2024.5.30/plugins/Herald/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Herald/locales/it.po` & `limnoria-2024.5.30/plugins/Herald/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Herald/plugin.py` & `limnoria-2024.5.30/plugins/Herald/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Herald/test.py` & `limnoria-2024.5.30/plugins/Herald/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Internet/__init__.py` & `limnoria-2024.5.30/plugins/Internet/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Internet/config.py` & `limnoria-2024.5.30/plugins/Internet/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Internet/locales/fi.po` & `limnoria-2024.5.30/plugins/Internet/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Internet/locales/fr.po` & `limnoria-2024.5.30/plugins/Internet/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Internet/locales/it.po` & `limnoria-2024.5.30/plugins/Internet/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Internet/plugin.py` & `limnoria-2024.5.30/plugins/Internet/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 ###
 
 import time
 import socket
-import telnetlib
 
 import supybot.conf as conf
 import supybot.utils as utils
 from supybot.commands import *
 from supybot.utils.iter import any
 import supybot.callbacks as callbacks
 from supybot.i18n import PluginInternationalization, internationalizeDocstring
@@ -154,22 +153,22 @@
                 s = ':'.join(line.split(':')[1:]).strip()
                 expires = _('expires %s') % s
             elif not status and any(line.startswith, self._status):
                 status = ':'.join(line.split(':')[1:]).strip().lower()
         if not status:
             status = 'unknown'
         try:
-            t = telnetlib.Telnet('whois.iana.org', 43)
+            sock = socket.create_connection(('whois.iana.org', 43))
         except socket.error as e:
             irc.error(str(e))
             return
-        t.write(b'registrar ')
-        t.write(registrar.split('(')[0].strip().encode('ascii'))
-        t.write(b'\n')
-        s = t.read_all()
+        sock.sendall(b'registrar ')
+        sock.sendall(registrar.split('(')[0].strip().encode('ascii'))
+        sock.sendall(b'\n')
+        s = sock.recv(100000)
         url = ''
         for line in s.splitlines():
             line = line.decode('ascii').strip()
             if not line:
                 continue
             if line.startswith('Email'):
                 url = _(' <registered at %s>') % line.split('@')[-1]
```

### Comparing `limnoria-2024.4.26/plugins/Internet/test.py` & `limnoria-2024.5.30/plugins/Internet/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
     if network:
         def testDns(self):
             self.assertNotError('dns slashdot.org')
             self.assertResponse('dns does.not.exist.',
                                 'Host not found.')
 
         def testWhois(self):
-            self.assertNotError('internet whois ohio-state.edu')
             self.assertNotError('internet whois microsoft.com')
             self.assertNotError('internet whois inria.fr')
             self.assertNotError('internet whois slime.com.au')
             self.assertNotError('internet whois 8.8.8.8')
             self.assertNotError('internet whois net')
```

### Comparing `limnoria-2024.4.26/plugins/Karma/__init__.py` & `limnoria-2024.5.30/plugins/Karma/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Karma/config.py` & `limnoria-2024.5.30/plugins/Karma/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Karma/locales/fi.po` & `limnoria-2024.5.30/plugins/Karma/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Karma/locales/fr.po` & `limnoria-2024.5.30/plugins/Karma/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Karma/locales/it.po` & `limnoria-2024.5.30/plugins/Karma/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Karma/plugin.py` & `limnoria-2024.5.30/plugins/Karma/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Karma/test.py` & `limnoria-2024.5.30/plugins/Karma/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Lart/__init__.py` & `limnoria-2024.5.30/plugins/Lart/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Lart/config.py` & `limnoria-2024.5.30/plugins/Lart/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Lart/locales/fi.po` & `limnoria-2024.5.30/plugins/Lart/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Lart/locales/fr.po` & `limnoria-2024.5.30/plugins/Lart/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Lart/locales/it.po` & `limnoria-2024.5.30/plugins/Lart/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Lart/plugin.py` & `limnoria-2024.5.30/plugins/Lart/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Lart/test.py` & `limnoria-2024.5.30/plugins/Lart/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Later/__init__.py` & `limnoria-2024.5.30/plugins/Later/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Later/config.py` & `limnoria-2024.5.30/plugins/Later/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Later/locales/de.po` & `limnoria-2024.5.30/plugins/Later/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Later/locales/fi.po` & `limnoria-2024.5.30/plugins/Later/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Later/locales/fr.po` & `limnoria-2024.5.30/plugins/Later/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Later/locales/it.po` & `limnoria-2024.5.30/plugins/Later/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Later/plugin.py` & `limnoria-2024.5.30/plugins/Later/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Later/test.py` & `limnoria-2024.5.30/plugins/Later/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Limiter/__init__.py` & `limnoria-2024.5.30/plugins/Limiter/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Limiter/config.py` & `limnoria-2024.5.30/plugins/Limiter/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Limiter/locales/fi.po` & `limnoria-2024.5.30/plugins/Limiter/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Limiter/locales/fr.po` & `limnoria-2024.5.30/plugins/Limiter/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Limiter/locales/hu.po` & `limnoria-2024.5.30/plugins/Limiter/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Limiter/locales/it.po` & `limnoria-2024.5.30/plugins/Limiter/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Limiter/plugin.py` & `limnoria-2024.5.30/plugins/Limiter/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Limiter/test.py` & `limnoria-2024.5.30/plugins/Limiter/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/LogToIrc/__init__.py` & `limnoria-2024.5.30/plugins/LogToIrc/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/LogToIrc/config.py` & `limnoria-2024.5.30/plugins/LogToIrc/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/LogToIrc/handler.py` & `limnoria-2024.5.30/plugins/LogToIrc/handler.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/LogToIrc/plugin.py` & `limnoria-2024.5.30/plugins/LogToIrc/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/LogToIrc/test.py` & `limnoria-2024.5.30/plugins/LogToIrc/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Math/__init__.py` & `limnoria-2024.5.30/plugins/Math/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Math/config.py` & `limnoria-2024.5.30/plugins/Math/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Math/local/convertcore.py` & `limnoria-2024.5.30/plugins/Math/local/convertcore.py`

 * *Files 0% similar despite different names*

```diff
@@ -845,15 +845,15 @@
         if cursorPos != None:
             self.updateCurrentUnit(text, cursorPos)
         else:
             self.currentNum = len(self.unitList) - 1
 
     def updateCurrentUnit(self, text, cursorPos):
         "Set current unit number"
-        self.currentNum = len(re.findall('[\*/]', text[:cursorPos]))
+        self.currentNum = len(re.findall(r'[\*/]', text[:cursorPos]))
 
     def currentUnit(self):
         "Return current unit if its a full match, o/w None"
         if self.unitList and self.unitList[self.currentNum].equiv:
             return self.unitList[self.currentNum]
         return None
 
@@ -921,15 +921,15 @@
     def clearUnit(self):
         "Remove units"
         self.unitList = []
 
     def parseGroup(self, text):
         "Return list of units from text string"
         unitList = []
-        parts = [part.strip() for part in re.split('([\*/])', text)]
+        parts = [part.strip() for part in re.split(r'([\*/])', text)]
         numerator = 1
         while parts:
             unit = self.parseUnit(parts.pop(0))
             if not numerator:
                 unit.exp = -unit.exp
             if parts and parts.pop(0) == '/':
                 numerator = not numerator
@@ -1176,25 +1176,25 @@
         self.factor = 1.0
         self.fromEqn = ''   # used only for non-linear units
         self.toEqn = ''     # used only for non-linear units
         if unitList:
             self.equiv = unitList[0].strip()
             if self.equiv[0] == '[':   # used only for non-linear units
                 try:
-                    self.equiv, self.fromEqn = re.match('\[(.*?)\](.*)', \
+                    self.equiv, self.fromEqn = re.match(r'\[(.*?)\](.*)', \
                                                         self.equiv).groups()
                     if ';' in self.fromEqn:
                         self.fromEqn, self.toEqn = self.fromEqn.split(';', 1)
                         self.toEqn = self.toEqn.strip()
                     self.fromEqn = self.fromEqn.strip()
                 except AttributeError:
                     raise UnitDataError('Bad equation for "%s"' % self.name)
             else:                # split factor and equiv unit for linear
                 parts = self.equiv.split(None, 1)
-                if len(parts) > 1 and re.search('[^\d\.eE\+\-\*/]', parts[0]) \
+                if len(parts) > 1 and re.search(r'[^\d\.eE\+\-\*/]', parts[0]) \
                    == None:       # only allowed digits and operators
                     try:
                         self.factor = float(eval(parts[0]))
                         self.equiv = parts[1]
                     except:
                         pass
         self.comments = [comm.strip() for comm in dataList]
```

### Comparing `limnoria-2024.4.26/plugins/Math/locales/fi.po` & `limnoria-2024.5.30/plugins/Math/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Math/locales/fr.po` & `limnoria-2024.5.30/plugins/Math/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Math/locales/hu.po` & `limnoria-2024.5.30/plugins/Math/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Math/locales/it.po` & `limnoria-2024.5.30/plugins/Math/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Math/plugin.py` & `limnoria-2024.5.30/plugins/Math/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Math/test.py` & `limnoria-2024.5.30/plugins/Math/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/MessageParser/__init__.py` & `limnoria-2024.5.30/plugins/MessageParser/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/MessageParser/config.py` & `limnoria-2024.5.30/plugins/MessageParser/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/MessageParser/locales/fi.po` & `limnoria-2024.5.30/plugins/MessageParser/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/MessageParser/locales/fr.po` & `limnoria-2024.5.30/plugins/MessageParser/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/MessageParser/locales/it.po` & `limnoria-2024.5.30/plugins/MessageParser/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/MessageParser/plugin.py` & `limnoria-2024.5.30/plugins/MessageParser/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/MessageParser/test.py` & `limnoria-2024.5.30/plugins/MessageParser/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Misc/__init__.py` & `limnoria-2024.5.30/plugins/Misc/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Misc/config.py` & `limnoria-2024.5.30/plugins/Misc/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Misc/locales/de.po` & `limnoria-2024.5.30/plugins/Misc/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Misc/locales/fi.po` & `limnoria-2024.5.30/plugins/Misc/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Misc/locales/fr.po` & `limnoria-2024.5.30/plugins/Misc/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Misc/locales/hu.po` & `limnoria-2024.5.30/plugins/Misc/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Misc/locales/it.po` & `limnoria-2024.5.30/plugins/Misc/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Misc/plugin.py` & `limnoria-2024.5.30/plugins/Misc/plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -338,29 +338,39 @@
     @internationalizeDocstring
     def version(self, irc, msg, args):
         """takes no arguments
 
         Returns the version of the current bot.
         """
         try:
-            newestUrl = 'https://api.github.com/repos/progval/Limnoria/' + \
-                    'commits/%s'
-            versions = {}
-            for branch in ('master', 'testing'):
-                data = json.loads(utils.web.getUrl(newestUrl % branch)
-                        .decode('utf8'))
-                version = data['commit']['committer']['date']
-                # Strip the last 'Z':
-                version = version.rsplit('T', 1)[0].replace('-', '.')
-                if minisix.PY2 and isinstance(version, unicode):
-                    version = version.encode('utf8')
-                versions[branch] = version
-            newest = _('The newest versions available online are %s.') % \
-                    ', '.join([_('%s (in %s)') % (y,x)
-                               for x,y in versions.items()])
+            versions = []
+
+            # fetch from PyPI
+            data = json.loads(utils.web.getUrl(
+                'https://pypi.org/pypi/limnoria/json'
+            ).decode('utf8'))
+            release_version = data['info']['version']
+            # zero-left-pad months and days
+            release_version = re.sub(
+                r'\.([0-9])\b', lambda m: '.0' + m.group(1), release_version
+            )
+
+            # fetch from Git
+            data = json.loads(utils.web.getUrl(
+                'https://api.github.com/repos/progval/Limnoria/'
+                'commits/master'
+            ).decode('utf8'))
+            git_version = data['commit']['committer']['date']
+            # Strip the last 'Z':
+            git_version = git_version.rsplit('T', 1)[0].replace('-', '.')
+
+            newest = _(
+                'The newest version available online is %(release_version)s, '
+                'or %(git_version)s in Git'
+            ) % {'release_version': release_version, 'git_version': git_version}
         except utils.web.Error as e:
             self.log.info('Couldn\'t get website version: %s', e)
             newest = _('I couldn\'t fetch the newest version '
                      'from the Limnoria repository.')
         s = _('The current (running) version of this Limnoria is %s, '
               'running on Python %s.  %s') % \
             (conf.version, sys.version.replace('\n', ' '), newest)
```

### Comparing `limnoria-2024.4.26/plugins/Misc/test.py` & `limnoria-2024.5.30/plugins/Misc/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/MoobotFactoids/__init__.py` & `limnoria-2024.5.30/plugins/MoobotFactoids/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/MoobotFactoids/config.py` & `limnoria-2024.5.30/plugins/MoobotFactoids/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/MoobotFactoids/locales/fi.po` & `limnoria-2024.5.30/plugins/MoobotFactoids/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/MoobotFactoids/locales/fr.po` & `limnoria-2024.5.30/plugins/MoobotFactoids/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/MoobotFactoids/locales/it.po` & `limnoria-2024.5.30/plugins/MoobotFactoids/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/MoobotFactoids/plugin.py` & `limnoria-2024.5.30/plugins/MoobotFactoids/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/MoobotFactoids/test.py` & `limnoria-2024.5.30/plugins/MoobotFactoids/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Network/__init__.py` & `limnoria-2024.5.30/plugins/Network/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Network/config.py` & `limnoria-2024.5.30/plugins/Network/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Network/locales/de.po` & `limnoria-2024.5.30/plugins/Network/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Network/locales/fi.po` & `limnoria-2024.5.30/plugins/Network/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Network/locales/fr.po` & `limnoria-2024.5.30/plugins/Network/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Network/locales/it.po` & `limnoria-2024.5.30/plugins/Network/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Network/plugin.py` & `limnoria-2024.5.30/plugins/Network/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Network/test.py` & `limnoria-2024.5.30/plugins/Network/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/News/__init__.py` & `limnoria-2024.5.30/plugins/News/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/News/config.py` & `limnoria-2024.5.30/plugins/News/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/News/locales/fi.po` & `limnoria-2024.5.30/plugins/News/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/News/locales/fr.po` & `limnoria-2024.5.30/plugins/News/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/News/locales/it.po` & `limnoria-2024.5.30/plugins/News/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/News/plugin.py` & `limnoria-2024.5.30/plugins/News/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/News/test.py` & `limnoria-2024.5.30/plugins/News/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/NickAuth/__init__.py` & `limnoria-2024.5.30/plugins/NickAuth/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/NickAuth/config.py` & `limnoria-2024.5.30/plugins/NickAuth/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/NickAuth/locales/de.po` & `limnoria-2024.5.30/plugins/NickAuth/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/NickAuth/locales/fi.po` & `limnoria-2024.5.30/plugins/NickAuth/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/NickAuth/plugin.py` & `limnoria-2024.5.30/plugins/NickAuth/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/NickAuth/test.py` & `limnoria-2024.5.30/plugins/NickAuth/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/NickCapture/__init__.py` & `limnoria-2024.5.30/plugins/NickCapture/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/NickCapture/config.py` & `limnoria-2024.5.30/plugins/NickCapture/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/NickCapture/locales/de.po` & `limnoria-2024.5.30/plugins/NickCapture/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/NickCapture/locales/fi.po` & `limnoria-2024.5.30/plugins/NickCapture/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/NickCapture/locales/fr.po` & `limnoria-2024.5.30/plugins/NickCapture/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/NickCapture/locales/it.po` & `limnoria-2024.5.30/plugins/NickCapture/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/NickCapture/plugin.py` & `limnoria-2024.5.30/plugins/NickCapture/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/NickCapture/test.py` & `limnoria-2024.5.30/plugins/NickCapture/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Nickometer/__init__.py` & `limnoria-2024.5.30/plugins/Nickometer/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Nickometer/config.py` & `limnoria-2024.5.30/plugins/Nickometer/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Nickometer/locales/fi.po` & `limnoria-2024.5.30/plugins/Nickometer/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Nickometer/locales/fr.po` & `limnoria-2024.5.30/plugins/Nickometer/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Nickometer/locales/it.po` & `limnoria-2024.5.30/plugins/Nickometer/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Nickometer/plugin.py` & `limnoria-2024.5.30/plugins/Nickometer/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Nickometer/test.py` & `limnoria-2024.5.30/plugins/Nickometer/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Note/__init__.py` & `limnoria-2024.5.30/plugins/Note/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Note/config.py` & `limnoria-2024.5.30/plugins/Note/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Note/locales/fi.po` & `limnoria-2024.5.30/plugins/Note/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Note/locales/fr.po` & `limnoria-2024.5.30/plugins/Note/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Note/locales/it.po` & `limnoria-2024.5.30/plugins/Note/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Note/plugin.py` & `limnoria-2024.5.30/plugins/Note/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Note/test.py` & `limnoria-2024.5.30/plugins/Note/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Owner/__init__.py` & `limnoria-2024.5.30/plugins/Owner/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Owner/config.py` & `limnoria-2024.5.30/plugins/Owner/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Owner/locales/de.po` & `limnoria-2024.5.30/plugins/Owner/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Owner/locales/fi.po` & `limnoria-2024.5.30/plugins/Owner/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Owner/locales/fr.po` & `limnoria-2024.5.30/plugins/Owner/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Owner/locales/hu.po` & `limnoria-2024.5.30/plugins/Owner/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Owner/locales/it.po` & `limnoria-2024.5.30/plugins/Owner/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Owner/plugin.py` & `limnoria-2024.5.30/plugins/Owner/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Owner/test.py` & `limnoria-2024.5.30/plugins/Owner/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Plugin/__init__.py` & `limnoria-2024.5.30/plugins/Plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Plugin/config.py` & `limnoria-2024.5.30/plugins/Plugin/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Plugin/locales/de.po` & `limnoria-2024.5.30/plugins/Plugin/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Plugin/locales/fi.po` & `limnoria-2024.5.30/plugins/Plugin/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Plugin/locales/fr.po` & `limnoria-2024.5.30/plugins/Plugin/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Plugin/locales/it.po` & `limnoria-2024.5.30/plugins/Plugin/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Plugin/plugin.py` & `limnoria-2024.5.30/plugins/Plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Plugin/test.py` & `limnoria-2024.5.30/plugins/Plugin/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/PluginDownloader/__init__.py` & `limnoria-2024.5.30/plugins/PluginDownloader/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/PluginDownloader/config.py` & `limnoria-2024.5.30/plugins/PluginDownloader/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/PluginDownloader/locales/de.po` & `limnoria-2024.5.30/plugins/PluginDownloader/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/PluginDownloader/locales/fi.po` & `limnoria-2024.5.30/plugins/PluginDownloader/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/PluginDownloader/locales/fr.po` & `limnoria-2024.5.30/plugins/PluginDownloader/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/PluginDownloader/locales/it.po` & `limnoria-2024.5.30/plugins/PluginDownloader/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/PluginDownloader/plugin.py` & `limnoria-2024.5.30/plugins/PluginDownloader/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/PluginDownloader/test.py` & `limnoria-2024.5.30/plugins/PluginDownloader/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Poll/__init__.py` & `limnoria-2024.5.30/plugins/Poll/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Poll/config.py` & `limnoria-2024.5.30/plugins/Poll/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Poll/plugin.py` & `limnoria-2024.5.30/plugins/Poll/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Poll/test.py` & `limnoria-2024.5.30/plugins/Poll/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Praise/__init__.py` & `limnoria-2024.5.30/plugins/Praise/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Praise/config.py` & `limnoria-2024.5.30/plugins/Praise/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Praise/locales/fi.po` & `limnoria-2024.5.30/plugins/Praise/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Praise/locales/fr.po` & `limnoria-2024.5.30/plugins/Praise/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Praise/locales/it.po` & `limnoria-2024.5.30/plugins/Praise/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Praise/plugin.py` & `limnoria-2024.5.30/plugins/Praise/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Praise/test.py` & `limnoria-2024.5.30/plugins/Praise/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Protector/__init__.py` & `limnoria-2024.5.30/plugins/Protector/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Protector/config.py` & `limnoria-2024.5.30/plugins/Protector/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Protector/locales/fi.po` & `limnoria-2024.5.30/plugins/Protector/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Protector/locales/fr.po` & `limnoria-2024.5.30/plugins/Protector/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Protector/locales/it.po` & `limnoria-2024.5.30/plugins/Protector/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Protector/plugin.py` & `limnoria-2024.5.30/plugins/Protector/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Protector/test.py` & `limnoria-2024.5.30/plugins/Protector/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Quote/__init__.py` & `limnoria-2024.5.30/plugins/Quote/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Quote/config.py` & `limnoria-2024.5.30/plugins/Quote/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Quote/locales/fi.po` & `limnoria-2024.5.30/plugins/Quote/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Quote/locales/fr.po` & `limnoria-2024.5.30/plugins/Quote/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Quote/locales/it.po` & `limnoria-2024.5.30/plugins/Quote/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Quote/plugin.py` & `limnoria-2024.5.30/plugins/Quote/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Quote/test.py` & `limnoria-2024.5.30/plugins/Quote/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/QuoteGrabs/__init__.py` & `limnoria-2024.5.30/plugins/QuoteGrabs/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/QuoteGrabs/config.py` & `limnoria-2024.5.30/plugins/QuoteGrabs/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/QuoteGrabs/locales/fi.po` & `limnoria-2024.5.30/plugins/QuoteGrabs/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/QuoteGrabs/locales/fr.po` & `limnoria-2024.5.30/plugins/QuoteGrabs/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/QuoteGrabs/locales/it.po` & `limnoria-2024.5.30/plugins/QuoteGrabs/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/QuoteGrabs/plugin.py` & `limnoria-2024.5.30/plugins/QuoteGrabs/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/QuoteGrabs/test.py` & `limnoria-2024.5.30/plugins/QuoteGrabs/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/RSS/__init__.py` & `limnoria-2024.5.30/plugins/RSS/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/RSS/config.py` & `limnoria-2024.5.30/plugins/RSS/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/RSS/locales/de.po` & `limnoria-2024.5.30/plugins/RSS/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/RSS/locales/fi.po` & `limnoria-2024.5.30/plugins/RSS/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/RSS/locales/fr.po` & `limnoria-2024.5.30/plugins/RSS/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/RSS/locales/hu.po` & `limnoria-2024.5.30/plugins/RSS/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/RSS/locales/it.po` & `limnoria-2024.5.30/plugins/RSS/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/RSS/plugin.py` & `limnoria-2024.5.30/plugins/RSS/plugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,15 @@
     def assert_feed_does_not_exist(self, name, url=None):
         if self.isCommandMethod(name):
             s = format(_('I already have a command in this plugin named %s.'),
                     name)
             raise callbacks.Error(s)
         if url:
             feed = self.feeds.get(url)
-            if feed and feed.name != feed.url:
+            if feed and feed.name != feed.url and feed.name in self.feed_names:
                 s = format(_('I already have a feed with that URL named %s.'),
                         feed.name)
                 raise callbacks.Error(s)
 
     def register_feed(self, name, url, initial,
             plugin_is_loading, announced=None):
         if name != url:
```

### Comparing `limnoria-2024.4.26/plugins/RSS/test.py` & `limnoria-2024.5.30/plugins/RSS/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
             f(self, mock)
 
     return newf
 
 
 url = 'http://www.advogato.org/rss/articles.xml'
 class RSSTestCase(ChannelPluginTestCase):
-    plugins = ('RSS','Plugin')
+    plugins = ('RSS', 'Plugin')
 
     timeout = 1
 
     def testRssAddBadName(self):
         self.assertError('rss add "foo bar" %s' % url)
 
     def testCantAddFeedNamedRss(self):
@@ -118,14 +118,35 @@
         finally:
             self.assertNotError('rss announce remove http://xkcd.com/rss.xml')
             self.assertNotError('rss remove xkcd')
         self.assertEqual(self.irc.getCallback('RSS').feed_names, {})
         self.assertTrue(self.irc.getCallback('RSS').get_feed('http://xkcd.com/rss.xml'))
 
     @mock_urllib
+    def testChangeUrl(self, mock):
+        try:
+            self.assertNotError('rss add xkcd http://xkcd.com/rss.xml')
+            self.assertNotError('rss remove xkcd')
+            self.assertNotError('rss add xkcd https://xkcd.com/rss.xml')
+            self.assertRegexp('help xkcd', 'https://')
+        finally:
+            self._feedMsg('rss remove xkcd')
+
+    @mock_urllib
+    def testChangeName(self, mock):
+        try:
+            self.assertNotError('rss add xkcd http://xkcd.com/rss.xml')
+            self.assertNotError('rss remove xkcd')
+            self.assertNotError('rss add xkcd2 http://xkcd.com/rss.xml')
+            self.assertRegexp('help xkcd2', 'http://xkcd.com')
+        finally:
+            self._feedMsg('rss remove xkcd')
+            self._feedMsg('rss remove xkcd2')
+
+    @mock_urllib
     def testInitialAnnounceNewest(self, mock):
         mock._data = xkcd_new
         timeFastForward(1.1)
         try:
             with conf.supybot.plugins.RSS.sortFeedItems.context('newestFirst'):
                 with conf.supybot.plugins.RSS.initialAnnounceHeadlines.context(1):
                     self.assertNotError('rss add xkcd http://xkcd.com/rss.xml')
```

### Comparing `limnoria-2024.4.26/plugins/Relay/__init__.py` & `limnoria-2024.5.30/plugins/Relay/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Relay/config.py` & `limnoria-2024.5.30/plugins/Relay/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Relay/locales/fi.po` & `limnoria-2024.5.30/plugins/Relay/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Relay/locales/fr.po` & `limnoria-2024.5.30/plugins/Relay/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Relay/locales/it.po` & `limnoria-2024.5.30/plugins/Relay/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Relay/plugin.py` & `limnoria-2024.5.30/plugins/Relay/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Relay/test.py` & `limnoria-2024.5.30/plugins/Relay/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Reply/__init__.py` & `limnoria-2024.5.30/plugins/Reply/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Reply/config.py` & `limnoria-2024.5.30/plugins/Reply/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Reply/locales/de.po` & `limnoria-2024.5.30/plugins/Reply/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Reply/locales/fi.po` & `limnoria-2024.5.30/plugins/Reply/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Reply/locales/fr.po` & `limnoria-2024.5.30/plugins/Reply/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Reply/locales/hu.po` & `limnoria-2024.5.30/plugins/Reply/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Reply/locales/it.po` & `limnoria-2024.5.30/plugins/Reply/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Reply/plugin.py` & `limnoria-2024.5.30/plugins/Reply/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Reply/test.py` & `limnoria-2024.5.30/plugins/Reply/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Scheduler/__init__.py` & `limnoria-2024.5.30/plugins/Scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Scheduler/config.py` & `limnoria-2024.5.30/plugins/Scheduler/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Scheduler/locales/fi.po` & `limnoria-2024.5.30/plugins/Scheduler/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Scheduler/locales/fr.po` & `limnoria-2024.5.30/plugins/Scheduler/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Scheduler/locales/it.po` & `limnoria-2024.5.30/plugins/Scheduler/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Scheduler/plugin.py` & `limnoria-2024.5.30/plugins/Scheduler/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Scheduler/test.py` & `limnoria-2024.5.30/plugins/Scheduler/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/SedRegex/__init__.py` & `limnoria-2024.5.30/plugins/SedRegex/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/SedRegex/config.py` & `limnoria-2024.5.30/plugins/SedRegex/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/SedRegex/constants.py` & `limnoria-2024.5.30/plugins/SedRegex/constants.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/SedRegex/plugin.py` & `limnoria-2024.5.30/plugins/SedRegex/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/SedRegex/test.py` & `limnoria-2024.5.30/plugins/SedRegex/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Seen/__init__.py` & `limnoria-2024.5.30/plugins/Seen/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Seen/config.py` & `limnoria-2024.5.30/plugins/Seen/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Seen/locales/de.po` & `limnoria-2024.5.30/plugins/Seen/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Seen/locales/fi.po` & `limnoria-2024.5.30/plugins/Seen/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Seen/locales/fr.po` & `limnoria-2024.5.30/plugins/Seen/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Seen/locales/it.po` & `limnoria-2024.5.30/plugins/Seen/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Seen/plugin.py` & `limnoria-2024.5.30/plugins/Seen/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Seen/test.py` & `limnoria-2024.5.30/plugins/Seen/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Services/__init__.py` & `limnoria-2024.5.30/plugins/Services/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Services/config.py` & `limnoria-2024.5.30/plugins/Services/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Services/locales/de.po` & `limnoria-2024.5.30/plugins/Services/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Services/locales/fi.po` & `limnoria-2024.5.30/plugins/Services/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Services/locales/fr.po` & `limnoria-2024.5.30/plugins/Services/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Services/locales/it.po` & `limnoria-2024.5.30/plugins/Services/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Services/plugin.py` & `limnoria-2024.5.30/plugins/Services/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Services/test.py` & `limnoria-2024.5.30/plugins/Services/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ShrinkUrl/__init__.py` & `limnoria-2024.5.30/plugins/ShrinkUrl/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ShrinkUrl/config.py` & `limnoria-2024.5.30/plugins/ShrinkUrl/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ShrinkUrl/locales/fi.po` & `limnoria-2024.5.30/plugins/ShrinkUrl/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ShrinkUrl/locales/fr.po` & `limnoria-2024.5.30/plugins/ShrinkUrl/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ShrinkUrl/locales/it.po` & `limnoria-2024.5.30/plugins/ShrinkUrl/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ShrinkUrl/plugin.py` & `limnoria-2024.5.30/plugins/ShrinkUrl/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/ShrinkUrl/test.py` & `limnoria-2024.5.30/plugins/ShrinkUrl/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Status/__init__.py` & `limnoria-2024.5.30/plugins/Status/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Status/config.py` & `limnoria-2024.5.30/plugins/Status/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Status/locales/de.po` & `limnoria-2024.5.30/plugins/Status/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Status/locales/fi.po` & `limnoria-2024.5.30/plugins/Status/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Status/locales/fr.po` & `limnoria-2024.5.30/plugins/Status/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Status/locales/it.po` & `limnoria-2024.5.30/plugins/Status/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Status/plugin.py` & `limnoria-2024.5.30/plugins/Status/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Status/test.py` & `limnoria-2024.5.30/plugins/Status/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/String/__init__.py` & `limnoria-2024.5.30/plugins/String/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/String/config.py` & `limnoria-2024.5.30/plugins/String/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/String/locales/fi.po` & `limnoria-2024.5.30/plugins/String/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/String/locales/fr.po` & `limnoria-2024.5.30/plugins/String/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/String/locales/it.po` & `limnoria-2024.5.30/plugins/String/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/String/plugin.py` & `limnoria-2024.5.30/plugins/String/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/String/test.py` & `limnoria-2024.5.30/plugins/String/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Success/__init__.py` & `limnoria-2024.5.30/plugins/Success/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Success/config.py` & `limnoria-2024.5.30/plugins/Success/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Success/locales/fi.po` & `limnoria-2024.5.30/plugins/Success/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Success/locales/fr.po` & `limnoria-2024.5.30/plugins/Success/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Success/locales/it.po` & `limnoria-2024.5.30/plugins/Success/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Success/plugin.py` & `limnoria-2024.5.30/plugins/Success/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Success/test.py` & `limnoria-2024.5.30/plugins/Success/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Time/__init__.py` & `limnoria-2024.5.30/plugins/Time/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Time/config.py` & `limnoria-2024.5.30/plugins/Time/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Time/locales/de.po` & `limnoria-2024.5.30/plugins/Time/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Time/locales/fi.po` & `limnoria-2024.5.30/plugins/Time/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Time/locales/fr.po` & `limnoria-2024.5.30/plugins/Time/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Time/locales/hu.po` & `limnoria-2024.5.30/plugins/Time/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Time/locales/it.po` & `limnoria-2024.5.30/plugins/Time/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Time/plugin.py` & `limnoria-2024.5.30/plugins/Time/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Time/test.py` & `limnoria-2024.5.30/plugins/Time/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Todo/__init__.py` & `limnoria-2024.5.30/plugins/Todo/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Todo/config.py` & `limnoria-2024.5.30/plugins/Todo/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Todo/locales/de.po` & `limnoria-2024.5.30/plugins/Todo/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Todo/locales/fi.po` & `limnoria-2024.5.30/plugins/Todo/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Todo/locales/fr.po` & `limnoria-2024.5.30/plugins/Todo/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Todo/locales/it.po` & `limnoria-2024.5.30/plugins/Todo/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Todo/plugin.py` & `limnoria-2024.5.30/plugins/Todo/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Todo/test.py` & `limnoria-2024.5.30/plugins/Todo/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Topic/__init__.py` & `limnoria-2024.5.30/plugins/Topic/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Topic/config.py` & `limnoria-2024.5.30/plugins/Topic/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Topic/locales/fi.po` & `limnoria-2024.5.30/plugins/Topic/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Topic/locales/fr.po` & `limnoria-2024.5.30/plugins/Topic/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Topic/locales/it.po` & `limnoria-2024.5.30/plugins/Topic/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Topic/plugin.py` & `limnoria-2024.5.30/plugins/Topic/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Topic/test.py` & `limnoria-2024.5.30/plugins/Topic/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/URL/__init__.py` & `limnoria-2024.5.30/plugins/URL/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/URL/config.py` & `limnoria-2024.5.30/plugins/URL/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/URL/locales/fi.po` & `limnoria-2024.5.30/plugins/URL/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/URL/locales/fr.po` & `limnoria-2024.5.30/plugins/URL/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/URL/locales/it.po` & `limnoria-2024.5.30/plugins/URL/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/URL/plugin.py` & `limnoria-2024.5.30/plugins/URL/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/URL/test.py` & `limnoria-2024.5.30/plugins/URL/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Unix/__init__.py` & `limnoria-2024.5.30/plugins/Unix/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Unix/config.py` & `limnoria-2024.5.30/plugins/Unix/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Unix/locales/fi.po` & `limnoria-2024.5.30/plugins/Unix/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Unix/locales/fr.po` & `limnoria-2024.5.30/plugins/Unix/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Unix/locales/it.po` & `limnoria-2024.5.30/plugins/Unix/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Unix/plugin.py` & `limnoria-2024.5.30/plugins/Unix/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,22 +29,27 @@
 # POSSIBILITY OF SUCH DAMAGE.
 ###
 
 import os
 import re
 import pwd
 import sys
-import crypt
 import errno
 import random
 import select
 import struct
 import subprocess
 import shlex
 
+try:
+    import crypt
+except ImportError:
+    # Python >= 3.13
+    crypt = None
+
 import supybot.conf as conf
 import supybot.utils as utils
 from supybot.commands import *
 import supybot.utils.minisix as minisix
 import supybot.plugins as plugins
 import supybot.ircutils as ircutils
 import supybot.registry as registry
@@ -115,33 +120,34 @@
         """takes no arguments
 
         Returns the current pid of the process for this Supybot.
         """
         irc.reply(format('%i', os.getpid()), private=True)
     pid = wrap(pid, [('checkCapability', 'owner')])
 
-    _cryptre = re.compile(b'[./0-9A-Za-z]')
-    @internationalizeDocstring
-    def crypt(self, irc, msg, args, password, salt):
-        """<password> [<salt>]
-
-        Returns the resulting of doing a crypt() on <password>.  If <salt> is
-        not given, uses a random salt.  If running on a glibc2 system,
-        prepending '$1$' to your salt will cause crypt to return an MD5sum
-        based crypt rather than the standard DES based crypt.
-        """
-        def makeSalt():
-            s = b'\x00'
-            while self._cryptre.sub(b'', s) != b'':
-                s = struct.pack('<h', random.randrange(-(2**15), 2**15))
-            return s
-        if not salt:
-            salt = makeSalt().decode()
-        irc.reply(crypt.crypt(password, salt))
-    crypt = wrap(crypt, ['something', additional('something')])
+    if crypt is not None:  # Python < 3.13
+        _cryptre = re.compile(b'[./0-9A-Za-z]')
+        @internationalizeDocstring
+        def crypt(self, irc, msg, args, password, salt):
+            """<password> [<salt>]
+
+            Returns the resulting of doing a crypt() on <password>.  If <salt> is
+            not given, uses a random salt.  If running on a glibc2 system,
+            prepending '$1$' to your salt will cause crypt to return an MD5sum
+            based crypt rather than the standard DES based crypt.
+            """
+            def makeSalt():
+                s = b'\x00'
+                while self._cryptre.sub(b'', s) != b'':
+                    s = struct.pack('<h', random.randrange(-(2**15), 2**15))
+                return s
+            if not salt:
+                salt = makeSalt().decode()
+            irc.reply(crypt.crypt(password, salt))
+        crypt = wrap(crypt, ['something', additional('something')])
 
     @internationalizeDocstring
     def spell(self, irc, msg, args, word):
         """<word>
 
         Returns the result of passing <word> to aspell/ispell.  The results
         shown are sorted from best to worst in terms of being a likely match
```

### Comparing `limnoria-2024.4.26/plugins/Unix/test.py` & `limnoria-2024.5.30/plugins/Unix/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,19 @@
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 ###
 
 import os
 import socket
 
+try:
+    import crypt
+except ImportError:
+    crypt = None
+
 from supybot.test import *
 
 try:
     from unittest import skip, skipIf
 except ImportError:
     def skipUnlessSpell(f):
         return None
@@ -102,16 +107,17 @@
         def testErrno(self):
             self.assertRegexp('errno 12', '^ENOMEM')
             self.assertRegexp('errno ENOMEM', '#12')
 
         def testProgstats(self):
             self.assertNotError('progstats')
 
-        def testCrypt(self):
-            self.assertNotError('crypt jemfinch')
+        if crypt is not None:  # Python < 3.13
+            def testCrypt(self):
+                self.assertNotError('crypt jemfinch')
 
         @skipUnlessFortune
         def testFortune(self):
             self.assertNotError('fortune')
 
         @skipUnlessPing
         def testPing(self):
```

### Comparing `limnoria-2024.4.26/plugins/User/__init__.py` & `limnoria-2024.5.30/plugins/User/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/User/config.py` & `limnoria-2024.5.30/plugins/User/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/User/locales/de.po` & `limnoria-2024.5.30/plugins/User/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/User/locales/fi.po` & `limnoria-2024.5.30/plugins/User/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/User/locales/fr.po` & `limnoria-2024.5.30/plugins/User/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/User/locales/hu.po` & `limnoria-2024.5.30/plugins/User/locales/hu.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/User/locales/it.po` & `limnoria-2024.5.30/plugins/User/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/User/plugin.py` & `limnoria-2024.5.30/plugins/User/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/User/test.py` & `limnoria-2024.5.30/plugins/User/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Utilities/__init__.py` & `limnoria-2024.5.30/plugins/Utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Utilities/config.py` & `limnoria-2024.5.30/plugins/Utilities/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Utilities/locales/de.po` & `limnoria-2024.5.30/plugins/Utilities/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Utilities/locales/fi.po` & `limnoria-2024.5.30/plugins/Utilities/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Utilities/locales/fr.po` & `limnoria-2024.5.30/plugins/Utilities/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Utilities/locales/it.po` & `limnoria-2024.5.30/plugins/Utilities/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Utilities/plugin.py` & `limnoria-2024.5.30/plugins/Utilities/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Utilities/test.py` & `limnoria-2024.5.30/plugins/Utilities/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Web/__init__.py` & `limnoria-2024.5.30/plugins/Web/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Web/config.py` & `limnoria-2024.5.30/plugins/Web/config.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Web/locales/de.po` & `limnoria-2024.5.30/plugins/Web/locales/de.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Web/locales/fi.po` & `limnoria-2024.5.30/plugins/Web/locales/fi.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Web/locales/fr.po` & `limnoria-2024.5.30/plugins/Web/locales/fr.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Web/locales/it.po` & `limnoria-2024.5.30/plugins/Web/locales/it.po`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Web/plugin.py` & `limnoria-2024.5.30/plugins/Web/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/Web/test.py` & `limnoria-2024.5.30/plugins/Web/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/plugins/__init__.py` & `limnoria-2024.5.30/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/requirements.txt` & `limnoria-2024.5.30/requirements.txt`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/setup.py` & `limnoria-2024.5.30/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,18 +45,20 @@
 try:
     from setuptools import setup
 except ImportError:
     s = normalizeWhitespace("""Limnoria requires the setuptools package to
     install. This package is pretty standard, and often installed alongside
     Python, but it is missing on your system.
     Try installing it with your package manager, it is usually called
-    'python3-setuptools'. If that does not work, try installing python3-pip
+    'python3-setuptools'; or with '%s -m pip install setuptools'.
+    If that does not work, try installing python3-pip
     instead, either with your package manager or by following these
     instructions: https://pip.pypa.io/en/stable/installation/ (replace
-    'python' with 'python3' in all the commands)""")
+    'python' with 'python3' in all the commands)"""
+    % sys.executable)
     sys.stderr.write(os.linesep*2)
     sys.stderr.write(textwrap.fill(s))
     sys.stderr.write(os.linesep*2)
     sys.exit(-1)
 
 warnings.filterwarnings('always', category=DeprecationWarning)
```

### Comparing `limnoria-2024.4.26/src/__init__.py` & `limnoria-2024.5.30/src/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/ansi.py` & `limnoria-2024.5.30/src/ansi.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/callbacks.py` & `limnoria-2024.5.30/src/callbacks.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/cdb.py` & `limnoria-2024.5.30/src/cdb.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/commands.py` & `limnoria-2024.5.30/src/commands.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/conf.py` & `limnoria-2024.5.30/src/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,14 +415,23 @@
     registerGlobalValue(network, 'user', registry.String('', _("""Determines
         the real name which the bot sends to the server. If empty, defaults to
         supybot.user""")))
     registerGlobalValue(network, 'umodes',
         registry.String('', _("""Determines what user modes the bot will request
         from the server when it first connects. If empty, defaults to
         supybot.protocols.irc.umodes""")))
+    registerGlobalValue(network, 'vhost',
+        registry.String('', _("""Determines what vhost the bot will bind to before
+        connecting a server (IRC, HTTP, ...) via IPv4. If empty, defaults to
+        supybot.protocols.irc.vhost""")))
+    registerGlobalValue(network, 'vhostv6',
+        registry.String('', _("""Determines what vhost the bot will bind to before
+        connecting a server (IRC, HTTP, ...) via IPv6. If empty, defaults to
+        supybot.protocols.irc.vhostv6""")))
+
     sasl = registerGroup(network, 'sasl')
     registerGlobalValue(sasl, 'username', registry.String(sasl_username,
         _("""Determines what SASL username will be used on %s. This should
         be the bot's account name.""") % name, private=False))
     registerGlobalValue(sasl, 'password', registry.String(sasl_password,
         _("""Determines what SASL password will be used on %s.""") \
         % name, private=True))
```

### Comparing `limnoria-2024.4.26/src/dbi.py` & `limnoria-2024.5.30/src/dbi.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/drivers/Socket.py` & `limnoria-2024.5.30/src/drivers/Socket.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,16 +308,18 @@
                 return
         drivers.log.connect(self.currentServer, socks_proxy=socks_proxy)
         try:
             self.conn = utils.net.getSocket(
                     address,
                     port=self.currentServer.port,
                     socks_proxy=socks_proxy,
-                    vhost=conf.supybot.protocols.irc.vhost(),
-                    vhostv6=conf.supybot.protocols.irc.vhostv6(),
+                    vhost=self.networkGroup.get('vhost')()
+                        or conf.supybot.protocols.irc.vhost(),
+                    vhostv6=self.networkGroup.get('vhostv6')()
+                        or conf.supybot.protocols.irc.vhostv6(),
                     )
         except socket.error as e:
             drivers.log.connectError(self.currentServer, e)
             self.scheduleReconnect()
             return
         # We allow more time for the connect here, since it might take longer.
         # At least 10 seconds.
```

### Comparing `limnoria-2024.4.26/src/drivers/__init__.py` & `limnoria-2024.5.30/src/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/dynamicScope.py` & `limnoria-2024.5.30/src/dynamicScope.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/gpg.py` & `limnoria-2024.5.30/src/gpg.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/httpserver.py` & `limnoria-2024.5.30/src/httpserver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###
-# Copyright (c) 2011-2021, Valentin Lorentz
+# Copyright (c) 2011-2024, Valentin Lorentz
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 #   * Redistributions of source code must retain the above copyright notice,
 #     this list of conditions, and the following disclaimer.
@@ -28,16 +28,16 @@
 ###
 
 """
 An embedded and centralized HTTP server for Supybot's plugins.
 """
 
 import os
-import cgi
 import socket
+import urllib.parse
 from threading import Thread
 
 import supybot.log as log
 import supybot.conf as conf
 import supybot.world as world
 import supybot.utils.minisix as minisix
 from supybot.i18n import PluginInternationalization
@@ -160,14 +160,122 @@
         with open(path, 'r') as fd:
             return fd.read()
     else:
         assert os.path.isfile(path + '.example'), path + '.example'
         with open(path + '.example', 'r') as fd:
             return fd.read()
 
+class HttpHeader:
+    __slots__ = ('name', 'value')
+
+    def __init__(self, name, value):
+        self.name = name
+        self.value = value
+
+    def __repr__(self):
+        """Return printable representation."""
+        return "HttpHeader(%r, %r)" % (self.name, self.value)
+
+class HttpHeaders:
+    """Copy of `cgi.FieldStorage
+    <https://github.com/python/cpython/blob/v3.12.3/Lib/cgi.py#L512-L594>`
+    before it was removed from the stdlib.
+    """
+    __slots__ = ('list',)
+    def __init__(self, headers):
+        self.list = headers
+
+    def __repr__(self):
+        return 'HttpHeaders(%r)' % self.list
+
+    def __iter__(self):
+        return iter(self.keys())
+
+    def __getattr__(self, name):
+        if name != 'value':
+            raise AttributeError(name)
+        if self.file:
+            self.file.seek(0)
+            value = self.file.read()
+            self.file.seek(0)
+        elif self.list is not None:
+            value = self.list
+        else:
+            value = None
+        return value
+
+    def __getitem__(self, key):
+        """Dictionary style indexing."""
+        if self.list is None:
+            raise TypeError("not indexable")
+        found = []
+        for item in self.list:
+            if item.name == key: found.append(item)
+        if not found:
+            raise KeyError(key)
+        if len(found) == 1:
+            return found[0]
+        else:
+            return found
+
+    def getvalue(self, key, default=None):
+        """Dictionary style get() method, including 'value' lookup."""
+        if key in self:
+            value = self[key]
+            if isinstance(value, list):
+                return [x.value for x in value]
+            else:
+                return value.value
+        else:
+            return default
+
+    def getfirst(self, key, default=None):
+        """ Return the first value received."""
+        if key in self:
+            value = self[key]
+            if isinstance(value, list):
+                return value[0].value
+            else:
+                return value.value
+        else:
+            return default
+
+    def getlist(self, key):
+        """ Return list of received values."""
+        if key in self:
+            value = self[key]
+            if isinstance(value, list):
+                return [x.value for x in value]
+            else:
+                return [value.value]
+        else:
+            return []
+
+    def keys(self):
+        """Dictionary style keys() method."""
+        if self.list is None:
+            raise TypeError("not indexable")
+        return list(set(item.name for item in self.list))
+
+    def __contains__(self, key):
+        """Dictionary style __contains__ method."""
+        if self.list is None:
+            raise TypeError("not indexable")
+        return any(item.name == key for item in self.list)
+
+    def __len__(self):
+        """Dictionary style len(x) support."""
+        return len(self.keys())
+
+    def __bool__(self):
+        if self.list is None:
+            raise TypeError("Cannot be converted to bool.")
+        return bool(self.list)
+
+
 class SupyHTTPRequestHandler(BaseHTTPRequestHandler):
     def do_X(self, callbackMethod, *args, **kwargs):
         if self.path == '/':
             callback = SupyIndex()
         elif self.path in ('/robots.txt',):
             callback = Static('text/plain; charset=utf-8')
         elif self.path in ('/default.css',):
@@ -195,20 +303,19 @@
     def do_GET(self):
         self.do_X('doGet')
 
     def do_POST(self):
         if 'Content-Type' not in self.headers:
             self.headers['Content-Type'] = 'application/x-www-form-urlencoded'
         if self.headers['Content-Type'] == 'application/x-www-form-urlencoded':
-            form = cgi.FieldStorage(
-                fp=self.rfile,
-                headers=self.headers,
-                environ={'REQUEST_METHOD':'POST',
-                         'CONTENT_TYPE':self.headers['Content-Type'],
-                         })
+            length = min(100000, int(self.headers.get('Content-Length', '100000')))
+            qs = self.rfile.read(length).decode()
+            form = HttpHeaders([
+                HttpHeader(k, v) for (k, v) in urllib.parse.parse_qsl(qs)
+            ])
         else:
             content_length = int(self.headers.get('Content-Length', '0'))
             form = self.rfile.read(content_length)
         self.do_X('doPost', form=form)
 
     def do_HEAD(self):
         self.do_X('doHead')
```

### Comparing `limnoria-2024.4.26/src/i18n.py` & `limnoria-2024.5.30/src/i18n.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/ircdb.py` & `limnoria-2024.5.30/src/ircdb.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/irclib.py` & `limnoria-2024.5.30/src/irclib.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/ircmsgs.py` & `limnoria-2024.5.30/src/ircmsgs.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/ircutils.py` & `limnoria-2024.5.30/src/ircutils.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/log.py` & `limnoria-2024.5.30/src/log.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/plugin.py` & `limnoria-2024.5.30/src/plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/questions.py` & `limnoria-2024.5.30/src/questions.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/registry.py` & `limnoria-2024.5.30/src/registry.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/schedule.py` & `limnoria-2024.5.30/src/schedule.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/scripts/limnoria.py` & `limnoria-2024.5.30/src/scripts/limnoria.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/scripts/limnoria_adduser.py` & `limnoria-2024.5.30/src/scripts/limnoria_adduser.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/scripts/limnoria_botchk.py` & `limnoria-2024.5.30/src/scripts/limnoria_botchk.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/scripts/limnoria_plugin_create.py` & `limnoria-2024.5.30/src/scripts/limnoria_plugin_create.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/scripts/limnoria_plugin_doc.py` & `limnoria-2024.5.30/src/scripts/limnoria_plugin_doc.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/scripts/limnoria_reset_password.py` & `limnoria-2024.5.30/src/scripts/limnoria_reset_password.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/scripts/limnoria_test.py` & `limnoria-2024.5.30/src/scripts/limnoria_test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/scripts/limnoria_wizard.py` & `limnoria-2024.5.30/src/scripts/limnoria_wizard.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/setup.py` & `limnoria-2024.5.30/src/setup.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/shlex.py` & `limnoria-2024.5.30/src/shlex.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/test.py` & `limnoria-2024.5.30/src/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/unpreserve.py` & `limnoria-2024.5.30/src/unpreserve.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/__init__.py` & `limnoria-2024.5.30/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/crypt.py` & `limnoria-2024.5.30/src/utils/crypt.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/error.py` & `limnoria-2024.5.30/src/utils/error.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/file.py` & `limnoria-2024.5.30/src/utils/file.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/gen.py` & `limnoria-2024.5.30/src/utils/gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,28 +163,29 @@
         salt = mktemp()[:8]
     if hash == 'sha':
         hasher = crypt.sha
     elif hash == 'md5':
         hasher = crypt.md5
     return '|'.join([salt, hasher((salt + password).encode('utf8')).hexdigest()])
 
-_astStr2 = ast.Str if minisix.PY2 else ast.Bytes
+_OLD_AST = sys.version_info[0:2] < (3, 8)
+"""Whether the AST classes predate the python 3.8 API changes"""
+
 def safeEval(s, namespace=None):
     """Evaluates s, safely.  Useful for turning strings into tuples/lists/etc.
     without unsafely using eval()."""
     try:
         node = ast.parse(s, mode='eval').body
     except SyntaxError as e:
         raise ValueError('Invalid string: %s.' % e)
+
     def checkNode(node):
         if node.__class__ is ast.Expr:
             node = node.value
-        if node.__class__ in (ast.Num,
-                              ast.Str,
-                              _astStr2):
+        if not _OLD_AST and node.__class__ is ast.Constant:
             return True
         elif node.__class__ in (ast.List,
                               ast.Tuple):
             return all([checkNode(x) for x in node.elts])
         elif node.__class__ is ast.Dict:
             return all([checkNode(x) for x in node.values]) and \
                     all([checkNode(x) for x in node.values])
@@ -192,18 +193,20 @@
             if namespace is None and node.id in ('True', 'False', 'None'):
                 # For Python < 3.4, which does not have NameConstant.
                 return True
             elif namespace is not None and node.id in namespace:
                 return True
             else:
                 return False
-        elif node.__class__ is ast.NameConstant:
+        elif _OLD_AST and node.__class__ in (ast.Num, ast.Str, ast.Bytes):
+            # ast.Num, ast.Str, ast.Bytes are deprecated since Python 3.8
+            # and removed since Python 3.14; replaced by ast.Constant.
             return True
-        elif sys.version_info[0:2] >= (3, 8) and \
-                node.__class__ is ast.Constant:
+        elif _OLD_AST and node.__class__ is ast.NameConstant:
+            # ditto
             return True
         else:
             return False
     if checkNode(node):
         # Probably equivalent to eval() because checkNode(node) is True,
         # but it's an extra security.
         return ast.literal_eval(node)
```

### Comparing `limnoria-2024.4.26/src/utils/iter.py` & `limnoria-2024.5.30/src/utils/iter.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/math_evaluator.py` & `limnoria-2024.5.30/src/utils/math_evaluator.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/minisix.py` & `limnoria-2024.5.30/src/utils/minisix.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/net.py` & `limnoria-2024.5.30/src/utils/net.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/python.py` & `limnoria-2024.5.30/src/utils/python.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/seq.py` & `limnoria-2024.5.30/src/utils/seq.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/str.py` & `limnoria-2024.5.30/src/utils/str.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/structures.py` & `limnoria-2024.5.30/src/utils/structures.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/time.py` & `limnoria-2024.5.30/src/utils/time.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/transaction.py` & `limnoria-2024.5.30/src/utils/transaction.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/utils/web.py` & `limnoria-2024.5.30/src/utils/web.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/src/world.py` & `limnoria-2024.5.30/src/world.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/__init__.py` & `limnoria-2024.5.30/test/__init__.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test.py` & `limnoria-2024.5.30/test/test.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_callbacks.py` & `limnoria-2024.5.30/test/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_commands.py` & `limnoria-2024.5.30/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_conf.py` & `limnoria-2024.5.30/test/test_conf.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_drivers.py` & `limnoria-2024.5.30/test/test_drivers.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_dynamicScope.py` & `limnoria-2024.5.30/test/test_dynamicScope.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_firewall.py` & `limnoria-2024.5.30/test/test_firewall.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_format.py` & `limnoria-2024.5.30/test/test_format.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_i18n.py` & `limnoria-2024.5.30/test/test_i18n.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_ircdb.py` & `limnoria-2024.5.30/test/test_ircdb.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_irclib.py` & `limnoria-2024.5.30/test/test_irclib.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_ircmsgs.py` & `limnoria-2024.5.30/test/test_ircmsgs.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_ircutils.py` & `limnoria-2024.5.30/test/test_ircutils.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_misc.py` & `limnoria-2024.5.30/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_plugin.py` & `limnoria-2024.5.30/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_plugin_create.py` & `limnoria-2024.5.30/test/test_plugin_create.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_plugins.py` & `limnoria-2024.5.30/test/test_plugins.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_registry.py` & `limnoria-2024.5.30/test/test_registry.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_schedule.py` & `limnoria-2024.5.30/test/test_schedule.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_standardSubstitute.py` & `limnoria-2024.5.30/test/test_standardSubstitute.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_utils.py` & `limnoria-2024.5.30/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `limnoria-2024.4.26/test/test_yn.py` & `limnoria-2024.5.30/test/test_yn.py`

 * *Files identical despite different names*

