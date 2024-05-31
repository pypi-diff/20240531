# Comparing `tmp/dub-0.0.6.tar.gz` & `tmp/dub-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dub-0.0.6.tar", last modified: Wed May 29 17:13:44 2024, max compression
+gzip compressed data, was "dub-0.0.7.tar", last modified: Fri May 31 18:48:26 2024, max compression
```

## Comparing `dub-0.0.6.tar` & `dub-0.0.7.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.638980 dub-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-29 17:13:29.000000 dub-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14630 2024-05-29 17:13:44.638980 dub-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-29 17:13:29.000000 dub-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:13:44.638980 dub-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-29 17:13:29.000000 dub-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.622979 dub-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.626979 dub-0.0.6/src/dub/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.626979 dub-0.0.6/src/dub/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/analytics.py
--rw-r--r--   0 runner    (1001) docker     (127)    52378 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/domains.py
--rw-r--r--   0 runner    (1001) docker     (127)    69591 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/metatags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.626979 dub-0.0.6/src/dub/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.634980 dub-0.0.6/src/dub/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clicksbrowsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clickscities.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clickscount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clickscountries.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clicksdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clicksos.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clicksreferers.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clickstimeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clickstoplinks.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/clickstopurls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/countrycode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/domainschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/httpmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadsbrowsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadscities.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadscount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadscountries.py
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadsdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadsos.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadsreferers.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadstimeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadstoplinks.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/leadstopurls.py
--rw-r--r--   0 runner    (1001) docker     (127)    41946 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/linkgeotargeting.py
--rw-r--r--   0 runner    (1001) docker     (127)    50627 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/linkschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salesbrowsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salescities.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salescount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salescountries.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salesdevices.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salesos.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salesreferers.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salestimeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salestoplinks.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/salestopurls.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/tagschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/components/workspaceschema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.634980 dub-0.0.6/src/dub/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/badrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/conflict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/forbidden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/internalservererror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/inviteexpired.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/notfound.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/ratelimitexceeded.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/sdkerror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/unauthorized.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/errors/unprocessableentity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.634980 dub-0.0.6/src/dub/models/internal/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/internal/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.638980 dub-0.0.6/src/dub/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/adddomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     8107 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/bulkcreatelinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/createlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/createtag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/createworkspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/deletedomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/deletelink.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/getlinkinfo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/getlinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/getlinkscount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/getmetatags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/getqrcode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/gettags.py
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/getworkspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/getworkspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/listdomains.py
--rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/retrieveanalytics.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/setprimarydomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/trackcustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/tracklead.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/tracksale.py
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/transferdomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/updatedomain.py
--rw-r--r--   0 runner    (1001) docker     (127)     8671 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/updatelink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/models/operations/upsertlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/qr_codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    17702 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    25415 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/track.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.638980 dub-0.0.6/src/dub/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32701 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24895 2024-05-29 17:13:29.000000 dub-0.0.6/src/dub/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:13:44.626979 dub-0.0.6/src/dub.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14630 2024-05-29 17:13:44.000000 dub-0.0.6/src/dub.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-29 17:13:44.000000 dub-0.0.6/src/dub.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:13:44.000000 dub-0.0.6/src/dub.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-29 17:13:44.000000 dub-0.0.6/src/dub.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-29 17:13:44.000000 dub-0.0.6/src/dub.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:26.125946 dub-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-31 18:48:17.000000 dub-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-05-31 18:48:26.125946 dub-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-05-31 18:48:17.000000 dub-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:48:26.125946 dub-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-31 18:48:17.000000 dub-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:26.105945 dub-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:26.109945 dub-0.0.7/src/dub/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:26.113946 dub-0.0.7/src/dub/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/analytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52378 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/domains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69591 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/metatags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:26.113946 dub-0.0.7/src/dub/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:26.121946 dub-0.0.7/src/dub/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/clicksbrowsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4448 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/clickscities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/clickscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/clickscountries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/clicksdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/clicksos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/clicksreferers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/clickstimeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/clickstoplinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/clickstopurls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/countrycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/domainschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/httpmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/leadsbrowsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/leadscities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/leadscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4284 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/leadscountries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/leadsdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/leadsos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/leadsreferers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/leadstimeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/leadstoplinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/leadstopurls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41946 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/linkgeotargeting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50627 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/linkschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/salesbrowsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/salescities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/salescount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/salescountries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/salesdevices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/salesos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/salesreferers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/salestimeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/salestoplinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/salestopurls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/tagschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/components/workspaceschema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:26.121946 dub-0.0.7/src/dub/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/errors/badrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/errors/conflict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/errors/forbidden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/errors/internalservererror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/errors/inviteexpired.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/errors/notfound.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/errors/ratelimitexceeded.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/errors/sdkerror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/errors/unauthorized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/errors/unprocessableentity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:26.121946 dub-0.0.7/src/dub/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:26.125946 dub-0.0.7/src/dub/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/adddomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8107 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/bulkcreatelinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8159 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/createlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/createtag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/createworkspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/deletedomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/deletelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/getlinkinfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/getlinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/getlinkscount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/getmetatags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/getqrcode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/gettags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/getworkspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/getworkspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/listdomains.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10285 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/retrieveanalytics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/setprimarydomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/trackcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/tracklead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/tracksale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/transferdomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/updatedomain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8671 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/updatelink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8200 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/models/operations/upsertlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8384 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/qr_codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17702 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25415 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/track.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:26.125946 dub-0.0.7/src/dub/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32701 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24895 2024-05-31 18:48:17.000000 dub-0.0.7/src/dub/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:48:26.113946 dub-0.0.7/src/dub.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-05-31 18:48:25.000000 dub-0.0.7/src/dub.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-31 18:48:26.000000 dub-0.0.7/src/dub.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:48:25.000000 dub-0.0.7/src/dub.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-31 18:48:25.000000 dub-0.0.7/src/dub.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 18:48:25.000000 dub-0.0.7/src/dub.egg-info/top_level.txt
```

### Comparing `dub-0.0.6/LICENSE` & `dub-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/PKG-INFO` & `dub-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 Metadata-Version: 2.1
 Name: dub
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/dubinc/dub-python.git
 Author: Speakeasy
 License: UNKNOWN
-Description: # dub
-        
-        <div align="left">
-            <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
-            <a href="https://opensource.org/licenses/MIT">
-                <img src="https://img.shields.io/badge/License-MIT-blue.svg" style="width: 100px; height: 28px;" />
-            </a>
+Description: <div align="center">
+          <img src="https://github.com/dubinc/dub/assets/28986134/3815d859-afaa-48f9-a9b3-c09964e4d404" alt="Dub.co Python SDK to interact with APIs.">
+          <h3>Dub.co Python SDK</h3>
+          <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
+          <a href="https://opensource.org/licenses/MIT">
+            <img src="https://img.shields.io/badge/License-MIT-blue.svg" style="width: 100px; height: 28px;" />
+          </a>
         </div>
         
+        <br/>
         
-        ## 🏗 **Welcome to your new SDK!** 🏗
-        
-        It has been generated successfully based on your OpenAPI spec. However, it is not yet ready for production use. Here are some next steps:
-        - [ ] 🛠 Make your SDK feel handcrafted by [customizing it](https://www.speakeasyapi.dev/docs/customize-sdks)
-        - [ ] ♻️ Refine your SDK quickly by iterating locally with the [Speakeasy CLI](https://github.com/speakeasy-api/speakeasy)
-        - [ ] 🎁 Publish your SDK to package managers by [configuring automatic publishing](https://www.speakeasyapi.dev/docs/advanced-setup/publish-sdks)
-        - [ ] ✨ When ready to productionize, delete this section from the README
+        Learn more about the Dub.co Python SDK in the [official documentation](https://dub.co/docs/sdks/python/overview).
         
         <!-- Start SDK Installation [installation] -->
         ## SDK Installation
         
         ```bash
         pip install dub
         ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,24 +1,20 @@
-Metadata-Version: 2.1 Name: dub Version: 0.0.6 Summary: Python Client SDK
+Metadata-Version: 2.1 Name: dub Version: 0.0.7 Summary: Python Client SDK
 Generated by Speakeasy Home-page: https://github.com/dubinc/dub-python.git
-Author: Speakeasy License: UNKNOWN Description: # dub
-_[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
-_2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
-## ð **Welcome to your new SDK!** ð It has been generated successfully
-based on your OpenAPI spec. However, it is not yet ready for production use.
-Here are some next steps: - [ ] ð  Make your SDK feel handcrafted by
-[customizing it](https://www.speakeasyapi.dev/docs/customize-sdks) - [ ] â»ï¸
-Refine your SDK quickly by iterating locally with the [Speakeasy CLI](https://
-github.com/speakeasy-api/speakeasy) - [ ] ð Publish your SDK to package
-managers by [configuring automatic publishing](https://www.speakeasyapi.dev/
-docs/advanced-setup/publish-sdks) - [ ] â¨ When ready to productionize, delete
-this section from the README ## SDK Installation ```bash pip install dub ``` ##
-SDK Example Usage ### Example 1 ```python import dub from dub.models import
-operations s = dub.Dub( token="DUB_API_KEY", workspace_id='', ) res =
+Author: Speakeasy License: UNKNOWN Description:
+                  [Dub.co Python SDK to interact with APIs.]
+                          ******** DDuubb..ccoo PPyytthhoonn SSDDKK ********
+    _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
+ _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
+              _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
+
+Learn more about the Dub.co Python SDK in the [official documentation](https://
+dub.co/docs/sdks/python/overview). ## SDK Installation ```bash pip install dub
+``` ## SDK Example Usage ### Example 1 ```python import dub from dub.models
+import operations s = dub.Dub( token="DUB_API_KEY", workspace_id='', ) res =
 s.links.create(request=operations.CreateLinkRequestBody( url='https://google/
 com', external_id='123456', tag_ids=[ 'clux0rgak00011...', ], )) if
 res.link_schema is not None: # handle response pass ``` ### Example 2 ```python
 import dub from dub.models import operations s = dub.Dub( token="DUB_API_KEY",
 workspace_id='', ) res = s.links.upsert
 (request=operations.UpsertLinkRequestBody( url='https://google/com',
 external_id='123456', tag_ids=[ 'clux0rgak00011...', ], )) if res.link_schema
```

### Comparing `dub-0.0.6/README.md` & `dub-0.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-# dub
-
-<div align="left">
-    <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
-    <a href="https://opensource.org/licenses/MIT">
-        <img src="https://img.shields.io/badge/License-MIT-blue.svg" style="width: 100px; height: 28px;" />
-    </a>
+<div align="center">
+  <img src="https://github.com/dubinc/dub/assets/28986134/3815d859-afaa-48f9-a9b3-c09964e4d404" alt="Dub.co Python SDK to interact with APIs.">
+  <h3>Dub.co Python SDK</h3>
+  <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
+  <a href="https://opensource.org/licenses/MIT">
+    <img src="https://img.shields.io/badge/License-MIT-blue.svg" style="width: 100px; height: 28px;" />
+  </a>
 </div>
 
+<br/>
 
-## 🏗 **Welcome to your new SDK!** 🏗
-
-It has been generated successfully based on your OpenAPI spec. However, it is not yet ready for production use. Here are some next steps:
-- [ ] 🛠 Make your SDK feel handcrafted by [customizing it](https://www.speakeasyapi.dev/docs/customize-sdks)
-- [ ] ♻️ Refine your SDK quickly by iterating locally with the [Speakeasy CLI](https://github.com/speakeasy-api/speakeasy)
-- [ ] 🎁 Publish your SDK to package managers by [configuring automatic publishing](https://www.speakeasyapi.dev/docs/advanced-setup/publish-sdks)
-- [ ] ✨ When ready to productionize, delete this section from the README
+Learn more about the Dub.co Python SDK in the [official documentation](https://dub.co/docs/sdks/python/overview).
 
 <!-- Start SDK Installation [installation] -->
 ## SDK Installation
 
 ```bash
 pip install dub
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,22 +1,17 @@
-# dub
-_[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
-_2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
-## ð **Welcome to your new SDK!** ð It has been generated successfully
-based on your OpenAPI spec. However, it is not yet ready for production use.
-Here are some next steps: - [ ] ð  Make your SDK feel handcrafted by
-[customizing it](https://www.speakeasyapi.dev/docs/customize-sdks) - [ ] â»ï¸
-Refine your SDK quickly by iterating locally with the [Speakeasy CLI](https://
-github.com/speakeasy-api/speakeasy) - [ ] ð Publish your SDK to package
-managers by [configuring automatic publishing](https://www.speakeasyapi.dev/
-docs/advanced-setup/publish-sdks) - [ ] â¨ When ready to productionize, delete
-this section from the README ## SDK Installation ```bash pip install dub ``` ##
-SDK Example Usage ### Example 1 ```python import dub from dub.models import
-operations s = dub.Dub( token="DUB_API_KEY", workspace_id='', ) res =
+                  [Dub.co Python SDK to interact with APIs.]
+                          ******** DDuubb..ccoo PPyytthhoonn SSDDKK ********
+    _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
+ _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
+              _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
+
+Learn more about the Dub.co Python SDK in the [official documentation](https://
+dub.co/docs/sdks/python/overview). ## SDK Installation ```bash pip install dub
+``` ## SDK Example Usage ### Example 1 ```python import dub from dub.models
+import operations s = dub.Dub( token="DUB_API_KEY", workspace_id='', ) res =
 s.links.create(request=operations.CreateLinkRequestBody( url='https://google/
 com', external_id='123456', tag_ids=[ 'clux0rgak00011...', ], )) if
 res.link_schema is not None: # handle response pass ``` ### Example 2 ```python
 import dub from dub.models import operations s = dub.Dub( token="DUB_API_KEY",
 workspace_id='', ) res = s.links.upsert
 (request=operations.UpsertLinkRequestBody( url='https://google/com',
 external_id='123456', tag_ids=[ 'clux0rgak00011...', ], )) if res.link_schema
```

### Comparing `dub-0.0.6/setup.py` & `dub-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='dub',
-    version='0.0.6',
+    version='0.0.7',
     author='Speakeasy',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/dubinc/dub-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `dub-0.0.6/src/dub/_hooks/registration.py` & `dub-0.0.7/src/dub/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/_hooks/sdkhooks.py` & `dub-0.0.7/src/dub/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/_hooks/types.py` & `dub-0.0.7/src/dub/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/analytics.py` & `dub-0.0.7/src/dub/analytics.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/domains.py` & `dub-0.0.7/src/dub/domains.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/links.py` & `dub-0.0.7/src/dub/links.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/metatags.py` & `dub-0.0.7/src/dub/metatags.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/__init__.py` & `dub-0.0.7/src/dub/models/components/__init__.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/clicksbrowsers.py` & `dub-0.0.7/src/dub/models/components/clicksbrowsers.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/clickscities.py` & `dub-0.0.7/src/dub/models/components/clickscities.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/clickscountries.py` & `dub-0.0.7/src/dub/models/components/clickscountries.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/clicksdevices.py` & `dub-0.0.7/src/dub/models/components/clicksdevices.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/clicksos.py` & `dub-0.0.7/src/dub/models/components/clicksos.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/clicksreferers.py` & `dub-0.0.7/src/dub/models/components/clicksreferers.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/clickstimeseries.py` & `dub-0.0.7/src/dub/models/components/clickstimeseries.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/clickstoplinks.py` & `dub-0.0.7/src/dub/models/components/clickstoplinks.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/clickstopurls.py` & `dub-0.0.7/src/dub/models/components/clickstopurls.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/countrycode.py` & `dub-0.0.7/src/dub/models/components/countrycode.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/domainschema.py` & `dub-0.0.7/src/dub/models/components/domainschema.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/httpmetadata.py` & `dub-0.0.7/src/dub/models/components/httpmetadata.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/leadsbrowsers.py` & `dub-0.0.7/src/dub/models/components/leadsbrowsers.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/leadscities.py` & `dub-0.0.7/src/dub/models/components/leadscities.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/leadscountries.py` & `dub-0.0.7/src/dub/models/components/leadscountries.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/leadsdevices.py` & `dub-0.0.7/src/dub/models/components/leadsdevices.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/leadsos.py` & `dub-0.0.7/src/dub/models/components/leadsos.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/leadsreferers.py` & `dub-0.0.7/src/dub/models/components/leadsreferers.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/leadstimeseries.py` & `dub-0.0.7/src/dub/models/components/leadstimeseries.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/leadstoplinks.py` & `dub-0.0.7/src/dub/models/components/leadstoplinks.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/leadstopurls.py` & `dub-0.0.7/src/dub/models/components/leadstopurls.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/linkgeotargeting.py` & `dub-0.0.7/src/dub/models/components/linkgeotargeting.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/linkschema.py` & `dub-0.0.7/src/dub/models/components/linkschema.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/salesbrowsers.py` & `dub-0.0.7/src/dub/models/components/salesbrowsers.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/salescities.py` & `dub-0.0.7/src/dub/models/components/salescities.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/salescount.py` & `dub-0.0.7/src/dub/models/components/salescount.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/salescountries.py` & `dub-0.0.7/src/dub/models/components/salescountries.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/salesdevices.py` & `dub-0.0.7/src/dub/models/components/salesdevices.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/salesos.py` & `dub-0.0.7/src/dub/models/components/salesos.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/salesreferers.py` & `dub-0.0.7/src/dub/models/components/salesreferers.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/salestimeseries.py` & `dub-0.0.7/src/dub/models/components/salestimeseries.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/salestoplinks.py` & `dub-0.0.7/src/dub/models/components/salestoplinks.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/salestopurls.py` & `dub-0.0.7/src/dub/models/components/salestopurls.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/tagschema.py` & `dub-0.0.7/src/dub/models/components/tagschema.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/components/workspaceschema.py` & `dub-0.0.7/src/dub/models/components/workspaceschema.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/errors/__init__.py` & `dub-0.0.7/src/dub/models/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/errors/badrequest.py` & `dub-0.0.7/src/dub/models/errors/badrequest.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/errors/conflict.py` & `dub-0.0.7/src/dub/models/errors/conflict.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/errors/forbidden.py` & `dub-0.0.7/src/dub/models/errors/forbidden.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/errors/internalservererror.py` & `dub-0.0.7/src/dub/models/errors/internalservererror.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/errors/inviteexpired.py` & `dub-0.0.7/src/dub/models/errors/inviteexpired.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/errors/notfound.py` & `dub-0.0.7/src/dub/models/errors/notfound.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/errors/ratelimitexceeded.py` & `dub-0.0.7/src/dub/models/errors/ratelimitexceeded.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/errors/sdkerror.py` & `dub-0.0.7/src/dub/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/errors/unauthorized.py` & `dub-0.0.7/src/dub/models/errors/unauthorized.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/errors/unprocessableentity.py` & `dub-0.0.7/src/dub/models/errors/unprocessableentity.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/internal/globals.py` & `dub-0.0.7/src/dub/models/internal/globals.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/__init__.py` & `dub-0.0.7/src/dub/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/adddomain.py` & `dub-0.0.7/src/dub/models/operations/adddomain.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/bulkcreatelinks.py` & `dub-0.0.7/src/dub/models/operations/bulkcreatelinks.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/createlink.py` & `dub-0.0.7/src/dub/models/operations/createlink.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/createtag.py` & `dub-0.0.7/src/dub/models/operations/createtag.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/createworkspace.py` & `dub-0.0.7/src/dub/models/operations/createworkspace.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/deletedomain.py` & `dub-0.0.7/src/dub/models/operations/deletedomain.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/deletelink.py` & `dub-0.0.7/src/dub/models/operations/deletelink.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/getlinkinfo.py` & `dub-0.0.7/src/dub/models/operations/getlinkinfo.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/getlinks.py` & `dub-0.0.7/src/dub/models/operations/getlinks.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/getlinkscount.py` & `dub-0.0.7/src/dub/models/operations/getlinkscount.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/getmetatags.py` & `dub-0.0.7/src/dub/models/operations/getmetatags.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/getqrcode.py` & `dub-0.0.7/src/dub/models/operations/getqrcode.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/gettags.py` & `dub-0.0.7/src/dub/models/operations/gettags.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/getworkspace.py` & `dub-0.0.7/src/dub/models/operations/getworkspace.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/getworkspaces.py` & `dub-0.0.7/src/dub/models/operations/getworkspaces.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/listdomains.py` & `dub-0.0.7/src/dub/models/operations/listdomains.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/retrieveanalytics.py` & `dub-0.0.7/src/dub/models/operations/retrieveanalytics.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/setprimarydomain.py` & `dub-0.0.7/src/dub/models/operations/setprimarydomain.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/trackcustomer.py` & `dub-0.0.7/src/dub/models/operations/trackcustomer.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/tracklead.py` & `dub-0.0.7/src/dub/models/operations/tracklead.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 from dub import utils
 from typing import Any, Dict, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TrackLeadRequestBody:
+    UNSET='__SPEAKEASY_UNSET__'
     click_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('clickId') }})
     r"""The ID of the click in th Dub. You can read this value from `dclid` cookie."""
     event_name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('eventName') }})
     r"""The name of the event to track."""
     customer_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerId') }})
     r"""This is the unique identifier for the customer in the client's app. This is used to track the customer's journey."""
-    customer_name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerName'), 'exclude': lambda f: f is None }})
+    customer_name: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerName'), 'exclude': lambda f: f is TrackLeadRequestBody.UNSET }})
     r"""Name of the customer in the client's app."""
-    customer_email: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerEmail'), 'exclude': lambda f: f is None }})
+    customer_email: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerEmail'), 'exclude': lambda f: f is TrackLeadRequestBody.UNSET }})
     r"""Email of the customer in the client's app."""
-    customer_avatar: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerAvatar'), 'exclude': lambda f: f is None }})
+    customer_avatar: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('customerAvatar'), 'exclude': lambda f: f is TrackLeadRequestBody.UNSET }})
     r"""Avatar of the customer in the client's app."""
-    metadata: Optional[Dict[str, Any]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is None }})
+    metadata: Optional[Dict[str, Any]] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('metadata'), 'exclude': lambda f: f is TrackLeadRequestBody.UNSET }})
     r"""Additional metadata to be stored with the lead event"""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `dub-0.0.6/src/dub/models/operations/tracksale.py` & `dub-0.0.7/src/dub/models/operations/tracksale.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/transferdomain.py` & `dub-0.0.7/src/dub/models/operations/transferdomain.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/updatedomain.py` & `dub-0.0.7/src/dub/models/operations/updatedomain.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/updatelink.py` & `dub-0.0.7/src/dub/models/operations/updatelink.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/models/operations/upsertlink.py` & `dub-0.0.7/src/dub/models/operations/upsertlink.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/qr_codes.py` & `dub-0.0.7/src/dub/qr_codes.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/sdk.py` & `dub-0.0.7/src/dub/sdk.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/sdkconfiguration.py` & `dub-0.0.7/src/dub/sdkconfiguration.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,17 +21,17 @@
     client: requests_http.Session
     globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '0.0.1'
-    sdk_version: str = '0.0.6'
-    gen_version: str = '2.338.1'
-    user_agent: str = 'speakeasy-sdk/python 0.0.6 2.338.1 0.0.1 dub'
+    sdk_version: str = '0.0.7'
+    gen_version: str = '2.338.7'
+    user_agent: str = 'speakeasy-sdk/python 0.0.7 2.338.7 0.0.1 dub'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `dub-0.0.6/src/dub/tags.py` & `dub-0.0.7/src/dub/tags.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/track.py` & `dub-0.0.7/src/dub/track.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/utils/retries.py` & `dub-0.0.7/src/dub/utils/retries.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/utils/utils.py` & `dub-0.0.7/src/dub/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub/workspaces.py` & `dub-0.0.7/src/dub/workspaces.py`

 * *Files identical despite different names*

### Comparing `dub-0.0.6/src/dub.egg-info/PKG-INFO` & `dub-0.0.7/src/dub.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 Metadata-Version: 2.1
 Name: dub
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/dubinc/dub-python.git
 Author: Speakeasy
 License: UNKNOWN
-Description: # dub
-        
-        <div align="left">
-            <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
-            <a href="https://opensource.org/licenses/MIT">
-                <img src="https://img.shields.io/badge/License-MIT-blue.svg" style="width: 100px; height: 28px;" />
-            </a>
+Description: <div align="center">
+          <img src="https://github.com/dubinc/dub/assets/28986134/3815d859-afaa-48f9-a9b3-c09964e4d404" alt="Dub.co Python SDK to interact with APIs.">
+          <h3>Dub.co Python SDK</h3>
+          <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
+          <a href="https://opensource.org/licenses/MIT">
+            <img src="https://img.shields.io/badge/License-MIT-blue.svg" style="width: 100px; height: 28px;" />
+          </a>
         </div>
         
+        <br/>
         
-        ## 🏗 **Welcome to your new SDK!** 🏗
-        
-        It has been generated successfully based on your OpenAPI spec. However, it is not yet ready for production use. Here are some next steps:
-        - [ ] 🛠 Make your SDK feel handcrafted by [customizing it](https://www.speakeasyapi.dev/docs/customize-sdks)
-        - [ ] ♻️ Refine your SDK quickly by iterating locally with the [Speakeasy CLI](https://github.com/speakeasy-api/speakeasy)
-        - [ ] 🎁 Publish your SDK to package managers by [configuring automatic publishing](https://www.speakeasyapi.dev/docs/advanced-setup/publish-sdks)
-        - [ ] ✨ When ready to productionize, delete this section from the README
+        Learn more about the Dub.co Python SDK in the [official documentation](https://dub.co/docs/sdks/python/overview).
         
         <!-- Start SDK Installation [installation] -->
         ## SDK Installation
         
         ```bash
         pip install dub
         ```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

#### html2text {}

```diff
@@ -1,24 +1,20 @@
-Metadata-Version: 2.1 Name: dub Version: 0.0.6 Summary: Python Client SDK
+Metadata-Version: 2.1 Name: dub Version: 0.0.7 Summary: Python Client SDK
 Generated by Speakeasy Home-page: https://github.com/dubinc/dub-python.git
-Author: Speakeasy License: UNKNOWN Description: # dub
-_[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
-_2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
-_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
-## ð **Welcome to your new SDK!** ð It has been generated successfully
-based on your OpenAPI spec. However, it is not yet ready for production use.
-Here are some next steps: - [ ] ð  Make your SDK feel handcrafted by
-[customizing it](https://www.speakeasyapi.dev/docs/customize-sdks) - [ ] â»ï¸
-Refine your SDK quickly by iterating locally with the [Speakeasy CLI](https://
-github.com/speakeasy-api/speakeasy) - [ ] ð Publish your SDK to package
-managers by [configuring automatic publishing](https://www.speakeasyapi.dev/
-docs/advanced-setup/publish-sdks) - [ ] â¨ When ready to productionize, delete
-this section from the README ## SDK Installation ```bash pip install dub ``` ##
-SDK Example Usage ### Example 1 ```python import dub from dub.models import
-operations s = dub.Dub( token="DUB_API_KEY", workspace_id='', ) res =
+Author: Speakeasy License: UNKNOWN Description:
+                  [Dub.co Python SDK to interact with APIs.]
+                          ******** DDuubb..ccoo PPyytthhoonn SSDDKK ********
+    _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
+ _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
+              _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_b_l_u_e_._s_v_g_]
+
+Learn more about the Dub.co Python SDK in the [official documentation](https://
+dub.co/docs/sdks/python/overview). ## SDK Installation ```bash pip install dub
+``` ## SDK Example Usage ### Example 1 ```python import dub from dub.models
+import operations s = dub.Dub( token="DUB_API_KEY", workspace_id='', ) res =
 s.links.create(request=operations.CreateLinkRequestBody( url='https://google/
 com', external_id='123456', tag_ids=[ 'clux0rgak00011...', ], )) if
 res.link_schema is not None: # handle response pass ``` ### Example 2 ```python
 import dub from dub.models import operations s = dub.Dub( token="DUB_API_KEY",
 workspace_id='', ) res = s.links.upsert
 (request=operations.UpsertLinkRequestBody( url='https://google/com',
 external_id='123456', tag_ids=[ 'clux0rgak00011...', ], )) if res.link_schema
```

### Comparing `dub-0.0.6/src/dub.egg-info/SOURCES.txt` & `dub-0.0.7/src/dub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

