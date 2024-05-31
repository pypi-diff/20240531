# Comparing `tmp/personal_knowledge_library-2.1.2.tar.gz` & `tmp/personal_knowledge_library-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "personal_knowledge_library-2.1.2.tar", last modified: Tue Feb 27 05:13:50 2024, max compression
+gzip compressed data, was "personal_knowledge_library-2.1.3.tar", last modified: Mon Apr  8 09:20:38 2024, max compression
```

## Comparing `personal_knowledge_library-2.1.2.tar` & `personal_knowledge_library-2.1.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:13:50.624683 personal_knowledge_library-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    61168 2024-02-27 05:13:50.624683 personal_knowledge_library-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    60298 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:13:50.616683 personal_knowledge_library-2.1.2/knowledge/
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:13:50.616683 personal_knowledge_library-2.1.2/knowledge/base/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/base/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/base/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/base/language.py
--rw-r--r--   0 runner    (1001) docker     (127)    86340 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/base/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)    15780 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/base/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:13:50.616683 personal_knowledge_library-2.1.2/knowledge/nel/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/nel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14921 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/nel/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/nel/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:13:50.616683 personal_knowledge_library-2.1.2/knowledge/ontomapping/
--rw-r--r--   0 runner    (1001) docker     (127)    17327 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/ontomapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/ontomapping/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:13:50.620683 personal_knowledge_library-2.1.2/knowledge/public/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/public/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/public/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/public/relations.py
--rw-r--r--   0 runner    (1001) docker     (127)    44949 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/public/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:13:50.620683 personal_knowledge_library-2.1.2/knowledge/services/
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:13:50.620683 personal_knowledge_library-2.1.2/knowledge/services/asyncio/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15273 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/asyncio/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    55589 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/asyncio/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    17743 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/asyncio/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/asyncio/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/asyncio/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    16330 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    53034 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    21954 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    32189 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/ontology.py
--rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    13947 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/services/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:13:50.620683 personal_knowledge_library-2.1.2/knowledge/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/utils/wikidata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/knowledge/utils/wikipedia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 05:13:50.624683 personal_knowledge_library-2.1.2/personal_knowledge_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    61168 2024-02-27 05:13:50.000000 personal_knowledge_library-2.1.2/personal_knowledge_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-02-27 05:13:50.000000 personal_knowledge_library-2.1.2/personal_knowledge_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 05:13:50.000000 personal_knowledge_library-2.1.2/personal_knowledge_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-27 05:13:50.000000 personal_knowledge_library-2.1.2/personal_knowledge_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-27 05:13:50.000000 personal_knowledge_library-2.1.2/personal_knowledge_library.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-27 05:13:50.624683 personal_knowledge_library-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2508 2024-02-27 05:13:34.000000 personal_knowledge_library-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:38.457588 personal_knowledge_library-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    61168 2024-04-08 09:20:38.457588 personal_knowledge_library-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    60298 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:38.453588 personal_knowledge_library-2.1.3/knowledge/
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:38.453588 personal_knowledge_library-2.1.3/knowledge/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4405 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/base/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7887 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/base/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/base/language.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86318 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/base/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/base/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:38.453588 personal_knowledge_library-2.1.3/knowledge/nel/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/nel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14921 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/nel/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/nel/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:38.453588 personal_knowledge_library-2.1.3/knowledge/ontomapping/
+-rw-r--r--   0 runner    (1001) docker     (127)    17327 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/ontomapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/ontomapping/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:38.453588 personal_knowledge_library-2.1.3/knowledge/public/
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/public/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12382 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/public/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/public/relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44949 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/public/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:38.457588 personal_knowledge_library-2.1.3/knowledge/services/
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:38.457588 personal_knowledge_library-2.1.3/knowledge/services/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15273 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/asyncio/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55589 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/asyncio/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17743 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/asyncio/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/asyncio/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10024 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/asyncio/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16330 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53034 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21954 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32189 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15183 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13947 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12469 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/services/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:38.457588 personal_knowledge_library-2.1.3/knowledge/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12608 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5477 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/utils/wikidata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/knowledge/utils/wikipedia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:20:38.457588 personal_knowledge_library-2.1.3/personal_knowledge_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    61168 2024-04-08 09:20:38.000000 personal_knowledge_library-2.1.3/personal_knowledge_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-08 09:20:38.000000 personal_knowledge_library-2.1.3/personal_knowledge_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:20:38.000000 personal_knowledge_library-2.1.3/personal_knowledge_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 09:20:38.000000 personal_knowledge_library-2.1.3/personal_knowledge_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 09:20:38.000000 personal_knowledge_library-2.1.3/personal_knowledge_library.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 09:20:38.457588 personal_knowledge_library-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-08 09:20:25.000000 personal_knowledge_library-2.1.3/setup.py
```

### Comparing `personal_knowledge_library-2.1.2/LICENSE` & `personal_knowledge_library-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/PKG-INFO` & `personal_knowledge_library-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal_knowledge_library
-Version: 2.1.2
+Version: 2.1.3
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
```

### Comparing `personal_knowledge_library-2.1.2/README.md` & `personal_knowledge_library-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/__init__.py` & `personal_knowledge_library-2.1.3/knowledge/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright © 2021-23 Wacom. All rights reserved.
+# Copyright © 2021-present Wacom. All rights reserved.
 """
 Personal knowledge Library
 --------------------------
 This library provides a set of tools to manage Wacom private knowledge graph API.
 All services are wrapped in a pythonic way to make it easy to use.
 Additionally, the library provides a set of tools to utilise Wikidata.
 """
@@ -13,15 +13,15 @@
 __author__ = "Markus Weber"
 __copyright__ = "Copyright 2021-2024 Wacom. All rights reserved."
 __credits__ = ["Markus Weber"]
 __license__ = "Wacom"
 __maintainer__ = ["Markus Weber"]
 __email__ = "markus.weber@wacom.com"
 __status__ = "beta"
-__version__ = "2.1.1"
+__version__ = "2.1.3"
 
 # Create the Logger
 logger: Union[logging.Logger, None] = None
 
 if logger is None:
     logger = logging.getLogger(__name__)
     logger.setLevel(logging.DEBUG)
```

### Comparing `personal_knowledge_library-2.1.2/knowledge/base/__init__.py` & `personal_knowledge_library-2.1.3/knowledge/base/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/base/access.py` & `personal_knowledge_library-2.1.3/knowledge/base/access.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/base/entity.py` & `personal_knowledge_library-2.1.3/knowledge/base/entity.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/base/language.py` & `personal_knowledge_library-2.1.3/knowledge/base/language.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/base/ontology.py` & `personal_knowledge_library-2.1.3/knowledge/base/ontology.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,20 @@
 from typing import Union, Optional, Any, List, Dict, Tuple, Set
 
 from rdflib import Literal, RDFS, OWL, URIRef, RDF, Graph
 
 from knowledge.base.access import TenantAccessRight
 from knowledge.base.entity import EntityStatus, Label, Description, URI_TAG, IMAGE_TAG, DESCRIPTIONS_TAG, \
     LABELS_TAG, TYPE_TAG, STATUS_FLAG_TAG, DATA_PROPERTIES_TAG, OBJECT_PROPERTIES_TAG, GROUP_IDS, OWNER_TAG, \
-    OWNER_ID_TAG, SOURCE_REFERENCE_ID_TAG, SOURCE_SYSTEM_TAG, TENANT_RIGHTS_TAG, SEND_TO_NEL_TAG, LOCALE_TAG, \
+    OWNER_ID_TAG, SOURCE_REFERENCE_ID_TAG, SOURCE_SYSTEM_TAG, TENANT_RIGHTS_TAG, LOCALE_TAG, \
     IS_MAIN_TAG, USE_NEL_TAG, VALUE_TAG, DATA_PROPERTY_TAG, VISIBILITY_TAG, INFLECTION_CASE_SENSITIVE, \
     INFLECTION_SETTING, INFLECTION_CONCEPT_CLASS, LANGUAGE_TAG, CONTENT_TAG, DATA_TYPE_TAG, RELATION_TAG, \
     INCOMING_TAG, OUTGOING_TAG, COMMENT_TAG, LocalizedContent, COMMENTS_TAG
 from knowledge.base.language import EN_US, SUPPORTED_LOCALES, EN, LanguageCode, LocaleCode
 
-
 # ---------------------------------------------- Vocabulary base URI ---------------------------------------------------
 PREFIX: str = "xsd"
 BASE_URI: str = "http://www.w3.org/2001/XMLSchema#"
 # ---------------------------------------------------- Constants -------------------------------------------------------
 SUB_CLASS_OF_TAG: str = 'subClassOf'
 TENANT_ID: str = 'tenantId'
 NAME_TAG: str = "name"
@@ -1957,15 +1956,15 @@
             LABELS_TAG: labels,
             DESCRIPTIONS_TAG: [desc.__dict__() for desc in self.description],
             TYPE_TAG: self.concept_type.iri,
             DATA_PROPERTIES_TAG: [],
             OBJECT_PROPERTIES_TAG: [],
             TENANT_RIGHTS_TAG: self.tenant_access_right.to_list(),
             GROUP_IDS: group_ids if group_ids else [],
-            SEND_TO_NEL_TAG: self.use_for_nel
+            USE_NEL_TAG: self.use_for_nel
         }
         for _, items in self.data_properties.items():
             dict_object[DATA_PROPERTIES_TAG].extend([i.__dict__() for i in items])
         for _, item in self.object_properties.items():
             dict_object[OBJECT_PROPERTIES_TAG].append(item.__dict__())
         return dict_object
```

### Comparing `personal_knowledge_library-2.1.2/knowledge/base/search.py` & `personal_knowledge_library-2.1.3/knowledge/base/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,14 +221,15 @@
     def __init__(self, stats: Dict[str, Any]):
         self.__locale: LocaleCode = stats.get('locale')
         self.__model_name: str = stats.get('model-name', "unknown")
         self.__top_k: int = stats.get('top-k', 10)
         self.__loading_time: float = stats.get('loading', 0.0) * 1000
         self.__embedding_time: float = stats.get('embedding', 0.0) * 1000
         self.__vector_db_response_time: float = stats.get('request', 0.0) * 1000
+        self.__overall_time: float = stats.get('overall', 0.0) * 1000
 
     @property
     def locale_code(self) -> LocaleCode:
         """Performance for the model with the given locale."""
         return self.__locale
 
     @property
@@ -252,14 +253,19 @@
         return self.__embedding_time
 
     @property
     def vector_db_response_time(self) -> float:
         """Response time in milliseconds for the vector database."""
         return self.__vector_db_response_time
 
+    @property
+    def overall_time(self) -> float:
+        """Overall time in milliseconds for the search query."""
+        return self.__overall_time
+
     def __repr__(self):
         return f"PerformanceStats(locale_code={self.locale_code}, model_name={self.model_name}, top_k={self.top_k}, " \
                f"model_loading_time={self.model_loading_time}, embedding_time={self.embedding_time}, " \
                f"vector_db_response_time={self.vector_db_response_time})"
 
 
 class DocumentSearchStats(PerformanceStats):
```

### Comparing `personal_knowledge_library-2.1.2/knowledge/nel/base.py` & `personal_knowledge_library-2.1.3/knowledge/nel/base.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/nel/engine.py` & `personal_knowledge_library-2.1.3/knowledge/nel/engine.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/ontomapping/__init__.py` & `personal_knowledge_library-2.1.3/knowledge/ontomapping/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/ontomapping/manager.py` & `personal_knowledge_library-2.1.3/knowledge/ontomapping/manager.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/public/__init__.py` & `personal_knowledge_library-2.1.3/knowledge/public/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/public/cache.py` & `personal_knowledge_library-2.1.3/knowledge/public/cache.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/public/helper.py` & `personal_knowledge_library-2.1.3/knowledge/public/helper.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/public/relations.py` & `personal_knowledge_library-2.1.3/knowledge/public/relations.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/public/wikidata.py` & `personal_knowledge_library-2.1.3/knowledge/public/wikidata.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/services/__init__.py` & `personal_knowledge_library-2.1.3/knowledge/services/__init__.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/services/asyncio/base.py` & `personal_knowledge_library-2.1.3/knowledge/services/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/services/asyncio/graph.py` & `personal_knowledge_library-2.1.3/knowledge/services/asyncio/graph.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/services/asyncio/group.py` & `personal_knowledge_library-2.1.3/knowledge/services/asyncio/group.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/services/asyncio/search.py` & `personal_knowledge_library-2.1.3/knowledge/services/asyncio/search.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/services/asyncio/users.py` & `personal_knowledge_library-2.1.3/knowledge/services/asyncio/users.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/services/base.py` & `personal_knowledge_library-2.1.3/knowledge/services/base.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/services/graph.py` & `personal_knowledge_library-2.1.3/knowledge/services/graph.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/services/group.py` & `personal_knowledge_library-2.1.3/knowledge/services/group.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/services/ontology.py` & `personal_knowledge_library-2.1.3/knowledge/services/ontology.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/services/search.py` & `personal_knowledge_library-2.1.3/knowledge/services/search.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/services/session.py` & `personal_knowledge_library-2.1.3/knowledge/services/session.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/services/tenant.py` & `personal_knowledge_library-2.1.3/knowledge/services/tenant.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/services/users.py` & `personal_knowledge_library-2.1.3/knowledge/services/users.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/utils/graph.py` & `personal_knowledge_library-2.1.3/knowledge/utils/graph.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/utils/wikidata.py` & `personal_knowledge_library-2.1.3/knowledge/utils/wikidata.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/knowledge/utils/wikipedia.py` & `personal_knowledge_library-2.1.3/knowledge/utils/wikipedia.py`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/personal_knowledge_library.egg-info/PKG-INFO` & `personal_knowledge_library-2.1.3/personal_knowledge_library.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: personal-knowledge-library
-Version: 2.1.2
+Version: 2.1.3
 Summary: Library to access Wacom's Personal Knowledge graph.
 Home-page: https://github.com/Wacom-Developer/personal-knowledge-library
 Author: Markus Weber
 Author-email: markus.weber@wacom.com
 License: Apache 2.0 License
 Keywords: semantic-knowledge;knowledge-graph
 Platform: UNKNOWN
```

### Comparing `personal_knowledge_library-2.1.2/personal_knowledge_library.egg-info/SOURCES.txt` & `personal_knowledge_library-2.1.3/personal_knowledge_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `personal_knowledge_library-2.1.2/setup.py` & `personal_knowledge_library-2.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,40 +4,40 @@
 from setuptools import setup, find_packages
 
 CURRENT_PYTHON = sys.version_info[:2]
 REQUIRED_PYTHON = (3, 7)
 
 if CURRENT_PYTHON < REQUIRED_PYTHON:
     sys.stderr.write(f"""
-==========================
-Unsupported Python version
-==========================
-This version of personal knowledge lib requires Python {REQUIRED_PYTHON}.
-
-This may be because you are using a version of pip that doesn't
-understand the python_requires classifier. Make sure you
-have pip >= 9.0 and setuptools >= 24.2, then try again:
-    $ python -m pip install --upgrade pip setuptools
-This will install the latest version of personal-knowledge-library which works on your
-version of Python. If you can't upgrade your pip (or Python), request
-an older version of knowledge-service-lib :
-    $ python -m pip install personal-knowledge-library
-""")
+    ==========================
+    Unsupported Python version
+    ==========================
+    This version of personal knowledge lib requires Python {REQUIRED_PYTHON}.
+    
+    This may be because you are using a version of pip that doesn't
+    understand the python_requires classifier. Make sure you
+    have pip >= 9.0 and setuptools >= 24.2, then try again:
+        $ python -m pip install --upgrade pip setuptools
+    This will install the latest version of personal-knowledge-library which works on your
+    version of Python. If you can't upgrade your pip (or Python), request
+    an older version of knowledge-service-lib :
+        $ python -m pip install personal-knowledge-library
+    """)
     sys.exit(1)
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # the setup
 setup(
     name='personal_knowledge_library',
-    version="2.1.2",
+    version="2.1.3",
     description="Library to access Wacom's Personal Knowledge graph.",
     long_description=README,
     long_description_content_type="text/markdown",
     url='https://github.com/Wacom-Developer/personal-knowledge-library',
     author='Markus Weber',
     author_email='markus.weber@wacom.com',
     license='Apache 2.0 License',
```

