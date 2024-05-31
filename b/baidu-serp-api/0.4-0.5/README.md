# Comparing `tmp/baidu_serp_api-0.4.tar.gz` & `tmp/baidu_serp_api-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baidu_serp_api-0.4.tar", last modified: Thu May 30 06:59:39 2024, max compression
+gzip compressed data, was "baidu_serp_api-0.5.tar", last modified: Thu May 30 15:20:37 2024, max compression
```

## Comparing `baidu_serp_api-0.4.tar` & `baidu_serp_api-0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:59:39.087936 baidu_serp_api-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 06:59:39.083936 baidu_serp_api-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:59:39.083936 baidu_serp_api-0.4/baidu_serp_api/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/baidu_serp_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6182 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/baidu_serp_api/baidu_mobile.py
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/baidu_serp_api/baidu_pc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/baidu_serp_api/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:59:39.083936 baidu_serp_api-0.4/baidu_serp_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 06:59:39.000000 baidu_serp_api-0.4/baidu_serp_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 06:59:39.000000 baidu_serp_api-0.4/baidu_serp_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 06:59:39.000000 baidu_serp_api-0.4/baidu_serp_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 06:59:39.000000 baidu_serp_api-0.4/baidu_serp_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 06:59:39.000000 baidu_serp_api-0.4/baidu_serp_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 06:59:39.087936 baidu_serp_api-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 06:59:39.083936 baidu_serp_api-0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-30 06:59:35.000000 baidu_serp_api-0.4/tests/test_baidu_serp_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:20:37.055167 baidu_serp_api-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-30 15:20:33.000000 baidu_serp_api-0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 15:20:37.055167 baidu_serp_api-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-05-30 15:20:33.000000 baidu_serp_api-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:20:37.051167 baidu_serp_api-0.5/baidu_serp_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-30 15:20:33.000000 baidu_serp_api-0.5/baidu_serp_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6143 2024-05-30 15:20:33.000000 baidu_serp_api-0.5/baidu_serp_api/baidu_mobile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-05-30 15:20:33.000000 baidu_serp_api-0.5/baidu_serp_api/baidu_pc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-30 15:20:33.000000 baidu_serp_api-0.5/baidu_serp_api/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:20:37.055167 baidu_serp_api-0.5/baidu_serp_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4435 2024-05-30 15:20:37.000000 baidu_serp_api-0.5/baidu_serp_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 15:20:37.000000 baidu_serp_api-0.5/baidu_serp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:20:37.000000 baidu_serp_api-0.5/baidu_serp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 15:20:37.000000 baidu_serp_api-0.5/baidu_serp_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-30 15:20:37.000000 baidu_serp_api-0.5/baidu_serp_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:20:37.055167 baidu_serp_api-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-30 15:20:33.000000 baidu_serp_api-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:20:37.055167 baidu_serp_api-0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-30 15:20:33.000000 baidu_serp_api-0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-30 15:20:33.000000 baidu_serp_api-0.5/tests/test_baidu_serp_api.py
```

### Comparing `baidu_serp_api-0.4/LICENSE.txt` & `baidu_serp_api-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.4/PKG-INFO` & `baidu_serp_api-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baidu-serp-api
-Version: 0.4
+Version: 0.5
 Summary: A library to extract data from Baidu SERP and output it as JSON objects
 Home-page: https://github.com/ohblue/baidu-serp-api
 Author: Ben Chen
 Author-email: chan@live.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `baidu_serp_api-0.4/README.md` & `baidu_serp_api-0.5/README.md`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.4/baidu_serp_api/baidu_mobile.py` & `baidu_serp_api-0.5/baidu_serp_api/baidu_mobile.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,36 +10,36 @@
         self.random_params = gen_random_params()
         self.keyword = None
         self.recomment_list = []
 
     def extract_baidum_data(self, html_content):
         search_data = []
         soup = BeautifulSoup(html_content, 'html.parser')
-        search_results = soup.find_all(class_='c-result result')
+        search_results = soup.select('div[tpl="www_index"]')
         for result in search_results:
             title_element = result.find('p', class_='cu-title')
 
             url = result.get('data-log')
             if url:
                 url = json.loads(url)['mu']
 
             description = ""
             date_time = ""
             source = ""
 
-            summary_element = result.find('div', class_=lambda x: x and 'summary-' in x)
-
+            summary_element = result.select_one('div[class*=summary-]')
             if summary_element:
                 description = clean_html_tags(summary_element.get_text().strip())
 
                 date_time_element = summary_element.find('span', class_='c-gap-right-small c-color-gray')
                 if date_time_element:
                     description = description.replace(date_time_element.get_text().strip(), '')
                     date_time = date_time_element.get_text().strip()
-            source_element = result.find('div', class_=lambda x: x and '_text_' in x)
+
+            source_element = result.select_one('div[class*=_text_]')
             if source_element:
                 source = source_element.get_text().strip()
 
             if title_element and url:
                 title_text = clean_html_tags(title_element.get_text().strip())
                 search_data.append({'title': title_text, 'url': url, 'description': description, 'date_time': date_time, "source": source})
 
@@ -70,24 +70,26 @@
             response = requests.get(url, headers=headers, params=params, proxies=proxies, timeout=10)
             response.raise_for_status()
             response.encoding = 'utf-8'
             json_data = response.json()
             # 获取所有键名为'up'和'down'的值
             up_values = []
             down_values = []
-            for item in json_data['rs']['rcmd']['list']:
-                up_values.extend(item['up'])
-                down_values.extend(item['down'])
-
-            # 排重并合并为新的列表
-            recomment_list = list(set(up_values + down_values))
-            logger.debug(len(recomment_list))
-            return recomment_list
+            if json_data['errcode'] != 0:
+                return []
+            else: 
+                for item in json_data['rs']['rcmd']['list']:
+                    up_values.extend(item['up'])
+                    down_values.extend(item['down'])
+
+                # 排重并合并为新的列表
+                recomment_list = list(set(up_values + down_values))
+                return recomment_list
         except requests.exceptions.RequestException as e:
-            return {'code': 500, 'msg': '网络请求错误'}
+            return []
 
     def get_baidum_serp(self, keyword, date_range=None, pn=None, proxies=None):
         url = 'https://m.baidu.com/s'
         params = {
             'word': keyword
         }
         if date_range:
@@ -109,16 +111,15 @@
                 if 'qid' in res_headers:
                     qid = res_headers['qid']
                 self.recomment_list = self.get_recommend(keyword, qid=qid, proxies=proxies)
             response.raise_for_status()
             response.encoding = 'utf-8'
             return response.text
         except requests.exceptions.RequestException as e:
-            logger.error(f'{keyword}相关搜索词获取失败')
-            return []
+            return {'code': 500, 'msg': '网络请求失败'}
 
     def handle_response(self, response):
         if isinstance(response, str):
             if '百度安全验证' in response:
                 return {'code': 501, 'msg': '百度安全验证'}
             elif '未找到相关结果' in response:
                 return {'code': 404, 'msg': '未找到相关结果'}
```

### Comparing `baidu_serp_api-0.4/baidu_serp_api/baidu_pc.py` & `baidu_serp_api-0.5/baidu_serp_api/baidu_pc.py`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.4/baidu_serp_api/util.py` & `baidu_serp_api-0.5/baidu_serp_api/util.py`

 * *Files identical despite different names*

### Comparing `baidu_serp_api-0.4/baidu_serp_api.egg-info/PKG-INFO` & `baidu_serp_api-0.5/baidu_serp_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baidu-serp-api
-Version: 0.4
+Version: 0.5
 Summary: A library to extract data from Baidu SERP and output it as JSON objects
 Home-page: https://github.com/ohblue/baidu-serp-api
 Author: Ben Chen
 Author-email: chan@live.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `baidu_serp_api-0.4/setup.py` & `baidu_serp_api-0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='baidu-serp-api',
-    version='0.4',
+    version='0.5',
     packages=find_packages(),
     install_requires=[
         'requests',
         'beautifulsoup4',
     ],
     entry_points={
         'console_scripts': [
```

### Comparing `baidu_serp_api-0.4/tests/test_baidu_serp_api.py` & `baidu_serp_api-0.5/tests/test_baidu_serp_api.py`

 * *Files identical despite different names*

