# Comparing `tmp/duckduckgo_search-6.1.3.tar.gz` & `tmp/duckduckgo_search-6.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-6.1.3.tar", last modified: Thu May 30 21:06:53 2024, max compression
+gzip compressed data, was "duckduckgo_search-6.1.4.tar", last modified: Thu May 30 22:24:46 2024, max compression
```

## Comparing `duckduckgo_search-6.1.3.tar` & `duckduckgo_search-6.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:06:53.578731 duckduckgo_search-6.1.3/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-30 21:06:53.578731 duckduckgo_search-6.1.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    17467 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:06:53.574731 duckduckgo_search-6.1.3/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18277 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    42430 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/duckduckgo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/duckduckgo_search_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:06:53.574731 duckduckgo_search-6.1.3/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-30 21:06:53.000000 duckduckgo_search-6.1.3/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-30 21:06:53.000000 duckduckgo_search-6.1.3/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:06:53.000000 duckduckgo_search-6.1.3/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 21:06:53.000000 duckduckgo_search-6.1.3/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 21:06:53.000000 duckduckgo_search-6.1.3/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 21:06:53.000000 duckduckgo_search-6.1.3/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 21:06:53.578731 duckduckgo_search-6.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:06:53.574731 duckduckgo_search-6.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/tests/test_duckduckgo_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-30 21:06:42.000000 duckduckgo_search-6.1.3/tests/test_duckduckgo_search_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:24:46.968030 duckduckgo_search-6.1.4/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-30 22:24:46.968030 duckduckgo_search-6.1.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    17467 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:24:46.964030 duckduckgo_search-6.1.4/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      797 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      140 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18277 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42433 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/duckduckgo_search/duckduckgo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14132 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/duckduckgo_search/duckduckgo_search_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/duckduckgo_search/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/duckduckgo_search/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/duckduckgo_search/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)       22 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:24:46.968030 duckduckgo_search-6.1.4/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18956 2024-05-30 22:24:46.000000 duckduckgo_search-6.1.4/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-30 22:24:46.000000 duckduckgo_search-6.1.4/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 22:24:46.000000 duckduckgo_search-6.1.4/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-30 22:24:46.000000 duckduckgo_search-6.1.4/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 22:24:46.000000 duckduckgo_search-6.1.4/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-30 22:24:46.000000 duckduckgo_search-6.1.4/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 22:24:46.968030 duckduckgo_search-6.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 22:24:46.964030 duckduckgo_search-6.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/tests/test_duckduckgo_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-30 22:24:36.000000 duckduckgo_search-6.1.4/tests/test_duckduckgo_search_async.py
```

### Comparing `duckduckgo_search-6.1.3/LICENSE.md` & `duckduckgo_search-6.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.3/PKG-INFO` & `duckduckgo_search-6.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 6.1.3
+Version: 6.1.4
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-6.1.3/README.md` & `duckduckgo_search-6.1.4/README.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.3/duckduckgo_search/__init__.py` & `duckduckgo_search-6.1.4/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.3/duckduckgo_search/cli.py` & `duckduckgo_search-6.1.4/duckduckgo_search/cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.3/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-6.1.4/duckduckgo_search/duckduckgo_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,15 +270,15 @@
                             "body": body,
                         }
                         page_results.append(result)
             return page_results
 
         slist = [0]
         if max_results:
-            max_results = min(max_results, 500)
+            max_results = min(max_results, 2023)
             slist.extend(range(23, max_results, 50))
         try:
             for r in self._executor.map(_text_api_page, slist):
                 results.extend(r)
         except Exception as e:
             raise e
 
@@ -360,15 +360,15 @@
                             "body": _normalize(body),
                         }
                         page_results.append(result)
             return page_results
 
         slist = [0]
         if max_results:
-            max_results = min(max_results, 500)
+            max_results = min(max_results, 2023)
             slist.extend(range(23, max_results, 50))
         try:
             for r in self._executor.map(_text_html_page, slist):
                 results.extend(r)
         except Exception as e:
             raise e
 
@@ -454,15 +454,15 @@
                                 "body": _normalize(body),
                             }
                             page_results.append(result)
             return page_results
 
         slist = [0]
         if max_results:
-            max_results = min(max_results, 500)
+            max_results = min(max_results, 2023)
             slist.extend(range(23, max_results, 50))
         try:
             for r in self._executor.map(_text_lite_page, slist):
                 results.extend(r)
         except Exception as e:
             raise e
 
@@ -630,15 +630,15 @@
                     cache.add(row["content"])
                     page_results.append(row)
             return page_results
 
         slist = [0]
         if max_results:
             max_results = min(max_results, 400)
-            slist.extend(range(59, max_results, 59))
+            slist.extend(range(60, max_results, 60))
         try:
             for r in self._executor.map(_videos_page, slist):
                 results.extend(r)
         except Exception as e:
             raise e
 
         return list(islice(results, max_results))
@@ -706,16 +706,16 @@
                         "source": row["source"],
                     }
                     page_results.append(result)
             return page_results
 
         slist = [0]
         if max_results:
-            max_results = min(max_results, 200)
-            slist.extend(range(29, max_results, 29))
+            max_results = min(max_results, 120)
+            slist.extend(range(30, max_results, 30))
         try:
             for r in self._executor.map(_news_page, slist):
                 results.extend(r)
         except Exception as e:
             raise e
 
         return list(islice(results, max_results))
```

### Comparing `duckduckgo_search-6.1.3/duckduckgo_search/duckduckgo_search_async.py` & `duckduckgo_search-6.1.4/duckduckgo_search/duckduckgo_search_async.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.3/duckduckgo_search/utils.py` & `duckduckgo_search-6.1.4/duckduckgo_search/utils.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.3/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-6.1.4/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duckduckgo_search
-Version: 6.1.3
+Version: 6.1.4
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duckduckgo_search-6.1.3/duckduckgo_search.egg-info/SOURCES.txt` & `duckduckgo_search-6.1.4/duckduckgo_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.3/pyproject.toml` & `duckduckgo_search-6.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.3/tests/test_cli.py` & `duckduckgo_search-6.1.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-6.1.3/tests/test_duckduckgo_search.py` & `duckduckgo_search-6.1.4/tests/test_duckduckgo_search.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def pause_between_tests():
     time.sleep(0.5)
 
 
 def test_context_manager():
     with DDGS() as ddgs:
         results = ddgs.news("cars", max_results=30)
-        assert 27 <= len(results) <= 30
+        assert 20 <= len(results) <= 30
 
 def test_chat():
     results = DDGS().chat("cat")
     assert  len(results) >= 1
 
 def test_text():
     results = DDGS().text("cat", safesearch="off", timelimit="m", max_results=30)
@@ -41,15 +41,15 @@
 def test_videos():
     results = DDGS().videos("sea", max_results=40)
     assert 37 <= len(results) <= 40
 
 
 def test_news():
     results = DDGS().news("tesla", max_results=30)
-    assert 27 <= len(results) <= 30
+    assert 20 <= len(results) <= 30
 
 
 def test_maps():
     results = DDGS().maps("school", place="London", max_results=30)
     assert 27 <= len(results) <= 30
```

### Comparing `duckduckgo_search-6.1.3/tests/test_duckduckgo_search_async.py` & `duckduckgo_search-6.1.4/tests/test_duckduckgo_search_async.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 async def test_async_videos():
     results = await AsyncDDGS().avideos("sea", max_results=40)
     assert 37 <= len(results) <= 40
 
 @pytest.mark.asyncio
 async def test_async_news():
     results = await AsyncDDGS().anews("tesla", max_results=30)
-    assert 27 <= len(results) <= 30
+    assert 20 <= len(results) <= 30
 
 @pytest.mark.asyncio
 async def test_async_maps():
     results = await AsyncDDGS().amaps("school", place="London", max_results=30)
     assert 27 <= len(results) <= 30
 
 @pytest.mark.asyncio
```

