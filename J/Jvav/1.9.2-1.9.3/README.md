# Comparing `tmp/Jvav-1.9.2.tar.gz` & `tmp/Jvav-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-qc07b9l0/Jvav-1.9.2.tar", last modified: Fri May 24 08:30:18 2024, max compression
+gzip compressed data, was "/Users/zh/Codes/jvav/dist/.tmp-zkxb_j_j/Jvav-1.9.3.tar", last modified: Fri May 31 16:50:52 2024, max compression
```

## Comparing `Jvav-1.9.2.tar` & `Jvav-1.9.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-05-24 08:30:18.000000 Jvav-1.9.2/
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-05-24 08:30:18.000000 Jvav-1.9.2/Jvav.egg-info/
--rw-r--r--   0 zh         (501) staff       (20)     4311 2024-05-24 08:30:18.000000 Jvav-1.9.2/Jvav.egg-info/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)      295 2024-05-24 08:30:18.000000 Jvav-1.9.2/Jvav.egg-info/SOURCES.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2024-05-24 08:30:18.000000 Jvav-1.9.2/Jvav.egg-info/dependency_links.txt
--rw-r--r--   0 zh         (501) staff       (20)       39 2024-05-24 08:30:18.000000 Jvav-1.9.2/Jvav.egg-info/entry_points.txt
--rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-1.9.2/Jvav.egg-info/not-zip-safe
--rw-r--r--   0 zh         (501) staff       (20)      495 2024-05-24 08:30:18.000000 Jvav-1.9.2/Jvav.egg-info/requires.txt
--rw-r--r--   0 zh         (501) staff       (20)       11 2024-05-24 08:30:18.000000 Jvav-1.9.2/Jvav.egg-info/top_level.txt
--rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-1.9.2/LICENSE
--rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-1.9.2/MANIFEST.in
--rw-r--r--   0 zh         (501) staff       (20)     4311 2024-05-24 08:30:18.000000 Jvav-1.9.2/PKG-INFO
--rw-r--r--   0 zh         (501) staff       (20)     3581 2024-04-21 15:00:39.000000 Jvav-1.9.2/README.md
-drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-05-24 08:30:18.000000 Jvav-1.9.2/jvav/
--rw-r--r--   0 zh         (501) staff       (20)      481 2024-05-24 08:29:24.000000 Jvav-1.9.2/jvav/__init__.py
--rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-1.9.2/jvav/cmd.py
--rw-r--r--   0 zh         (501) staff       (20)    74172 2024-05-24 08:28:05.000000 Jvav-1.9.2/jvav/utils.py
--rw-r--r--   0 zh         (501) staff       (20)      495 2024-04-22 03:22:14.000000 Jvav-1.9.2/requirements.txt
--rw-r--r--   0 zh         (501) staff       (20)       38 2024-05-24 08:30:18.000000 Jvav-1.9.2/setup.cfg
--rw-r--r--   0 zh         (501) staff       (20)     1345 2024-05-24 08:29:19.000000 Jvav-1.9.2/setup.py
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-05-31 16:50:52.000000 Jvav-1.9.3/
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-05-31 16:50:52.000000 Jvav-1.9.3/Jvav.egg-info/
+-rw-r--r--   0 zh         (501) staff       (20)     4311 2024-05-31 16:50:52.000000 Jvav-1.9.3/Jvav.egg-info/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)      295 2024-05-31 16:50:52.000000 Jvav-1.9.3/Jvav.egg-info/SOURCES.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2024-05-31 16:50:52.000000 Jvav-1.9.3/Jvav.egg-info/dependency_links.txt
+-rw-r--r--   0 zh         (501) staff       (20)       39 2024-05-31 16:50:52.000000 Jvav-1.9.3/Jvav.egg-info/entry_points.txt
+-rw-r--r--   0 zh         (501) staff       (20)        1 2023-07-18 10:13:18.000000 Jvav-1.9.3/Jvav.egg-info/not-zip-safe
+-rw-r--r--   0 zh         (501) staff       (20)      579 2024-05-31 16:50:52.000000 Jvav-1.9.3/Jvav.egg-info/requires.txt
+-rw-r--r--   0 zh         (501) staff       (20)       11 2024-05-31 16:50:52.000000 Jvav-1.9.3/Jvav.egg-info/top_level.txt
+-rw-r--r--   0 zh         (501) staff       (20)    35149 2023-07-16 04:15:06.000000 Jvav-1.9.3/LICENSE
+-rw-r--r--   0 zh         (501) staff       (20)      108 2023-07-16 04:15:06.000000 Jvav-1.9.3/MANIFEST.in
+-rw-r--r--   0 zh         (501) staff       (20)     4311 2024-05-31 16:50:52.000000 Jvav-1.9.3/PKG-INFO
+-rw-r--r--   0 zh         (501) staff       (20)     3581 2024-04-21 15:00:39.000000 Jvav-1.9.3/README.md
+drwxr-xr-x   0 zh         (501) staff       (20)        0 2024-05-31 16:50:52.000000 Jvav-1.9.3/jvav/
+-rw-r--r--   0 zh         (501) staff       (20)      481 2024-05-31 16:50:21.000000 Jvav-1.9.3/jvav/__init__.py
+-rw-r--r--   0 zh         (501) staff       (20)     7578 2024-02-16 02:42:42.000000 Jvav-1.9.3/jvav/cmd.py
+-rw-r--r--   0 zh         (501) staff       (20)    76532 2024-05-31 16:49:02.000000 Jvav-1.9.3/jvav/utils.py
+-rw-r--r--   0 zh         (501) staff       (20)      579 2024-05-31 16:49:11.000000 Jvav-1.9.3/requirements.txt
+-rw-r--r--   0 zh         (501) staff       (20)       38 2024-05-31 16:50:52.000000 Jvav-1.9.3/setup.cfg
+-rw-r--r--   0 zh         (501) staff       (20)     1345 2024-05-31 16:50:22.000000 Jvav-1.9.3/setup.py
```

### Comparing `Jvav-1.9.2/Jvav.egg-info/PKG-INFO` & `Jvav-1.9.3/Jvav.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.9.2
+Version: 1.9.3
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jvav Version: 1.9.2 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 1.9.3 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `Jvav-1.9.2/LICENSE` & `Jvav-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.2/PKG-INFO` & `Jvav-1.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jvav
-Version: 1.9.2
+Version: 1.9.3
 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav
 Download-URL: https://github.com/akynazh/jvav/releases/latest
 Author: akynazh
 Author-email: akynazh@gmail.com
 License: GPLv3
 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jvav Version: 1.9.2 Summary: Useful tools for Jav.
+Metadata-Version: 2.1 Name: Jvav Version: 1.9.3 Summary: Useful tools for Jav.
 Home-page: https://github.com/akynazh/jvav Download-URL: https://github.com/
 akynazh/jvav/releases/latest Author: akynazh Author-email: akynazh@gmail.com
 License: GPLv3 Project-URL: Tracker, https://github.com/akynazh/jvav/issues
 Project-URL: Source, https://github.com/akynazh/jvav Keywords: jav japan av api
 library python spider Classifier: License :: OSI Approved :: GNU General Public
 License v3 (GPLv3) Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Topic :: Internet :: WWW/HTTP
```

### Comparing `Jvav-1.9.2/README.md` & `Jvav-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.2/jvav/cmd.py` & `Jvav-1.9.3/jvav/cmd.py`

 * *Files identical despite different names*

### Comparing `Jvav-1.9.2/jvav/utils.py` & `Jvav-1.9.3/jvav/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         """随机返回 UserAgent
 
         :return str: UserAgent
         """
         return UserAgent().random
 
     def _inner_send_req(
-        self, url: str, session, headers={}, proxies={}, m=0, **args
+            self, url: str, session, headers={}, proxies={}, m=0, **args
     ) -> typing.Tuple[int, requests.Response]:
         if headers == {}:
             headers = {"user-agent": self.ua()}
         if proxies == {}:
             proxies = self.proxy_json
         try:
             if m == 0:
@@ -75,15 +75,15 @@
                 return 404, None
             return 200, resp
         except Exception as e:
             self.log.error(f"BaseUtil: 访问 {url}: {e}")
             return 502, None
 
     def send_req(
-        self, url: str, headers={}, proxies={}, m=0, **args
+            self, url: str, headers={}, proxies={}, m=0, **args
     ) -> typing.Tuple[int, requests.Response]:
         """发送请求
 
         :param str url: 地址
         :param dict headers: 请求头, 默认使用随机请求头
         :param dict proxies: 代理字典, 默认使用类初始化时指定的代理进行配置
         :param int m: 请求方法, 默认为 get(0), 其他为 post(1), delete(2), put(3)
@@ -151,19 +151,19 @@
     BASE_URL_VIDEO = BASE_URL + "/v/"
     BASE_URL_ACTOR = BASE_URL + "/actors/"
     BASE_URL_SEARCH_STAR = BASE_URL + "/search?f=actor&q="
     BASE_PARAM_NICE_AVS_OF_STAR = "?sort_type=1"
     PAT_SCORE = re.compile(r"(\d+\.?\d+)分")
 
     def __init__(
-        self,
-        proxy_addr="",
-        use_cache=True,
-        max_home_page_count=100,
-        max_new_avs_count=8,
+            self,
+            proxy_addr="",
+            use_cache=True,
+            max_home_page_count=100,
+            max_new_avs_count=8,
     ):
         """初始化
 
         :param str proxy_addr: 代理服务器地址, 默认为 ''
         :param bool use_cache: 是否使用缓存, 默认为 True
         :param int max_home_page_count: 主页最大爬取页数, 默认为 100 页
         :param int max_new_avs_count: 获取最新 AV 数量, 默认为 8 部
@@ -232,14 +232,34 @@
             if not url:
                 return 404, None
             return 200, f"{self.BASE_URL}{url}"
         except Exception as e:
             self.log.error(f"JavDbUtil: 获取预览图片: {e}")
             return 404, None
 
+    def fuzzy_search_stars(self, text) -> typing.Tuple[int, list]:
+        """模糊搜索演员
+
+        :param str text: 演员名称
+        :return typing.Tuple[int, list]: 状态码和演员列表
+        """
+        code, resp = self.send_req(url=JavDbUtil.BASE_URL_SEARCH_STAR + text)
+        if code != 200:
+            return code, None
+        try:
+            soup = self.get_soup(resp)
+            actor_boxs = soup.find_all(class_="actor-box")
+            names = [box.find("a")["title"] for box in actor_boxs]
+            if not names:
+                return 404, None
+            return 200, names
+        except Exception as e:
+            self.log.error(f"JavDbUtil: 模糊搜索演员: {e}")
+            return 404, None
+
     def get_id_by_star_name(self, star_name: str, page=-1) -> typing.Tuple[int, str]:
         """根据演员名称获取一个番号
 
         :param str star_name: 演员名称
         :param int page: 用于指定爬取哪一页的数据, 默认值为 -1, 表示随机获取某一页
         :return tuple[int, str]: 状态码和番号
         """
@@ -289,15 +309,15 @@
                 return code, None
             return 200, ids[: self.max_new_avs_count]
         except Exception as e:
             self.log.error(f"JavDbUtil: 根据演员名字获取最新番号列表: {e}")
             return 404, None
 
     def get_nice_avs_by_star_name(
-        self, star_name: str, cookie: str
+            self, star_name: str, cookie: str
     ) -> typing.Tuple[int, list]:
         """根据演员名字获取高分番号列表(需要登录)
 
         :param str star_name: 演员名字
         :param str cookie: 该方法需要登录，cookie 中的 _jdb_session 为必须值
         :return typing.Tuple[int, list]: 状态码和番号列表
         番号列表单个对象结构:
@@ -513,20 +533,20 @@
                 return 404, None
             return 200, [t.attrs["href"] for t in img_tags]
         except Exception as e:
             self.log.error(f"JavDbUtil: 获取预览图片: {e}")
             return 404, None
 
     def get_av_by_javdb_id(
-        self,
-        javdb_id: str,
-        is_nice: bool,
-        is_uncensored: bool,
-        sex_limit: bool = False,
-        magnet_max_count=10,
+            self,
+            javdb_id: str,
+            is_nice: bool,
+            is_uncensored: bool,
+            sex_limit: bool = False,
+            magnet_max_count=10,
     ) -> typing.Tuple[int, dict]:
         """通过 JavDB ID 获取 av
 
         :param javdb_id: JavDB 内部 ID
         :param bool is_nice: 是否过滤出高清，有字幕磁链
         :param bool is_uncensored: 是否过滤出无码磁链
         :param bool sex_limit: 是否只获取女优信息
@@ -649,26 +669,26 @@
                 # 获取大小
                 size = link.find("span", {"class": "meta"})
                 if size:
                     magnet["size"] = size.text.strip().split(",")[0]
                 # 检查是否为uc
                 title = link.find("span", {"class": "name"}).text
                 if any(
-                    k in title
-                    for k in [
-                        "-U",
-                        "无码",
-                        "無碼",
-                        "无码流出",
-                        "無碼流出",
-                        "无码破解",
-                        "無碼破解",
-                        "uncensored",
-                        "Uncensored",
-                    ]
+                        k in title
+                        for k in [
+                            "-U",
+                            "无码",
+                            "無碼",
+                            "无码流出",
+                            "無碼流出",
+                            "无码破解",
+                            "無碼破解",
+                            "uncensored",
+                            "Uncensored",
+                        ]
                 ):
                     magnet["uc"] = "1"
                 # 检查tag
                 tags_elements = link.find("div", {"class": "tags"})
                 if tags_elements:
                     tags_contents = tags_elements.findAll("span")
                     for i in tags_contents:
@@ -694,20 +714,20 @@
                 av["magnets"] = magnets
             return 200, av
         except Exception as e:
             self.log.error(f"JavDbUtil: 获取av信息: {e}")
             return 404, None
 
     def get_av_by_id(
-        self,
-        id: str,
-        is_nice: bool,
-        is_uncensored: bool,
-        sex_limit: bool = False,
-        magnet_max_count=10,
+            self,
+            id: str,
+            is_nice: bool,
+            is_uncensored: bool,
+            sex_limit: bool = False,
+            magnet_max_count=10,
     ) -> typing.Tuple[int, dict]:
         """通过 javdb 获取番号对应 av
 
         :param str id: 番号
         :param bool is_nice: 是否过滤出高清，有字幕磁链
         :param bool is_uncensored: 是否过滤出无码磁链
         :param int magnet_max_count: 过滤后磁链的最大数目, 默认为 10
@@ -783,15 +803,15 @@
     BASE_URL_COMMENT = BASE_URL + "/cn/videocomments.php?v="
     # review 最佳评论
     BASE_URL_REVIEW = BASE_URL + "/cn/videoreviews.php?v="
     # 排行榜最大页数
     MAX_RANK_PAGE = 25
 
     def get_random_ids_from_rank_by_page(
-        self, page: int, list_type: int
+            self, page: int, list_type: int
     ) -> typing.Tuple[int, str]:
         """从排行榜某页中获取该页番号列表
 
         :param int page: 第几页
         :param int list_type: 排行榜类型 0 nice | 1 new
         :return typing.Tuple[int, list]: 状态码和番号列表
         """
@@ -845,21 +865,21 @@
             return code, None
         javlib_av_id = ""
         if resp.url == url:
             try:
                 soup = self.get_soup(resp)
                 videos = soup.find_all(class_="video")
                 video_href = videos[0].a["href"]
-                javlib_av_id = video_href[video_href.find("v=") + 2 :]
+                javlib_av_id = video_href[video_href.find("v=") + 2:]
             except Exception as e:
                 self.log.error(f"JavLibUtil: 根据番号 {id} 获取评论失败: {e}")
                 return 404, None
         else:
             r_url = resp.url
-            javlib_av_id = r_url[r_url.find("v=") + 2 :]
+            javlib_av_id = r_url[r_url.find("v=") + 2:]
         comment_url = JavLibUtil.BASE_URL_REVIEW + javlib_av_id
         code, resp = self.send_req(url=comment_url)
         if code != 200:
             return code, None
         try:
             soup = self.get_soup(resp)
             comment_tags = soup.find_all(class_="t")
@@ -874,18 +894,18 @@
             return 404, None
 
 
 class DmmUtil(BaseUtil):
     BASE_URL = "https://www.dmm.co.jp"
     BASE_URL_SEARCH_AV = BASE_URL + "/digital/-/list/search/=/sort=ranking/?searchstr="
     BASE_URL_SEARCH_AV_MONTHLY = (
-        BASE_URL + "/monthly/dream/-/list/search/=/sort=ranking/?searchstr="
+            BASE_URL + "/monthly/dream/-/list/search/=/sort=ranking/?searchstr="
     )
     BASE_URL_SEARCH_STAR = (
-        BASE_URL + "/digital/videoa/-/list/search/=/device=tv/sort=ranking/?searchstr="
+            BASE_URL + "/digital/videoa/-/list/search/=/device=tv/sort=ranking/?searchstr="
     )
     BASE_URL_TOP_STARS = BASE_URL + "/digital/videoa/-/ranking/=/type=actress"
     PAT_CID = re.compile(r"/cid=.+/")
     PAT_CID_REAL = re.compile(r"[A-Za-z]+0+[0-9]+")
     PAT_AV = re.compile(r"[a-z]+\d+")
 
     def get_pv_by_id(self, id: str) -> typing.Tuple[int, str]:
@@ -1115,31 +1135,42 @@
     BASE_URL_SEARCH_BY_STAR_NAME = f"{BASE_URL}/search"
     BASE_URL_SEARCH_BY_STAR_ID = f"{BASE_URL}/star"
     BASE_URL_SEARCH_STAR = f"{BASE_URL}/searchstar"
     BASE_URL_MAGNET = f"{BASE_URL}/ajax/uncledatoolsbyajax.php?lang=zh"
     BASE_URL_GENRE = f"{BASE_URL}/genre"
 
     def get_headers(self):
+        # return {
+        #     "authority": "www.javbus.com",
+        #     "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
+        #     "accept-language": "zh-CN,zh;q=0.9,en;q=0.8,en-US;q=0.7,fr-FR;q=0.6,fr;q=0.5",
+        #     "cookie": f"bus_auth={self.bus_auth};",
+        #     "dnt": "1",
+        #     "sec-ch-ua-platform": '"Windows"',
+        #     "user-agent": self.ua_desktop(),
+        # }
         return {
-            "authority": "www.javbus.com",
-            "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.7",
-            "accept-language": "zh-CN,zh;q=0.9,en;q=0.8,en-US;q=0.7,fr-FR;q=0.6,fr;q=0.5",
-            "cookie": f"bus_auth={self.bus_auth};",
-            "dnt": "1",
-            "sec-ch-ua-platform": '"Windows"',
-            "user-agent": self.ua_desktop(),
+            'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8',
+            'Sec-Fetch-Site': 'none',
+            'Accept-Encoding': 'gzip, deflate, br',
+            'Sec-Fetch-Mode': 'navigate',
+            'Host': 'www.javbus.com',
+            'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/17.5 Safari/605.1.15',
+            'Accept-Language': 'zh-CN,zh-Hans;q=0.9',
+            'Sec-Fetch-Dest': 'document',
+            'Connection': 'keep-alive',
         }
 
     def __init__(
-        self,
-        bus_auth: str,
-        proxy_addr="",
-        use_cache=True,
-        max_home_page_count=100,
-        max_new_avs_count=8,
+            self,
+            bus_auth: str,
+            proxy_addr="",
+            use_cache=True,
+            max_home_page_count=100,
+            max_new_avs_count=8,
     ):
         """初始化
 
         :param str proxy_addr: 代理服务器地址, 默认为 ''
         :param bool use_cache: 是否使用缓存
         :param int max_home_page_count: 主页最大爬取页数, 默认为 100 页
         :param int max_new_avs_count: 获取最新 AV 数量, 默认为 8 部
@@ -1163,15 +1194,15 @@
         try:
             soup = self.get_soup(resp)
             boxes = soup.find_all(class_="row genre-box")
             genres = []
             for box in boxes:
                 tags = box.find_all("a")
                 for tag in tags:
-                    genres.append({tag.text: tag["href"][tag["href"].rfind("/") + 1 :]})
+                    genres.append({tag.text: tag["href"][tag["href"].rfind("/") + 1:]})
             if genres == []:
                 return 404, None
             return 200, genres
         except Exception as e:
             self.log.error(f"JavBusUtil: 获取所有标签失败: {e}")
             return 404, None
 
@@ -1235,15 +1266,15 @@
             return code, None
         try:
             ids = []
             soup = self.get_soup(resp)
             tags = soup.find_all(class_="movie-box")
             for tag in tags:
                 id_link = tag["href"]
-                id = id_link[id_link.rfind("/") + 1 :]
+                id = id_link[id_link.rfind("/") + 1:]
                 ids.append(id)
             if ids == []:
                 return 404, None
             return 200, ids
         except Exception as e:
             self.log.error(
                 f"JavBusUtil: 从 av 列表页面 {base_page_url} 获取该页面全部番号: {e}"
@@ -1388,20 +1419,40 @@
             return 200, {"star_id": star_id, "star_name": res_star_name}
         except Exception as e:
             self.log.error(
                 f"JavBusUtil: 根据演员名称 {star_name} 确认该演员在 javbus 是否存在: {e}"
             )
             return 404, None
 
+    def fuzzy_search_stars(self, text) -> typing.Tuple[int, list]:
+        """模糊搜索演员
+
+        :param str text: 演员名称
+        :return typing.Tuple[int, list]: 状态码和演员列表
+        """
+        code, resp = self.send_req(url=f"{JavBusUtil.BASE_URL_SEARCH_STAR}/{text}", headers=self.get_headers())
+        if code != 200:
+            return code, None
+        try:
+            soup = self.get_soup(resp)
+            actor_boxs = soup.find_all(class_="avatar-box text-center")
+            names = [box.find("img")["title"] for box in actor_boxs]
+            if not names:
+                return 404, None
+            return 200, names
+        except Exception as e:
+            self.log.error(f"JavDbUtil: 模糊搜索演员: {e}")
+            return 404, None
+
     def get_av_by_id(
-        self,
-        id: str,
-        is_nice: bool,
-        is_uncensored: bool,
-        magnet_max_count=10,
+            self,
+            id: str,
+            is_nice: bool,
+            is_uncensored: bool,
+            magnet_max_count=10,
     ) -> typing.Tuple[int, dict]:
         """通过 javbus 获取番号对应 av
 
         :param str id: 番号
         :param bool is_nice: 是否过滤出高清, 有字幕磁链
         :param bool is_uncensored: 是否过滤出无码磁链
         :param int magnet_max_count: 过滤后磁链的最大数目, 默认为 10
@@ -1519,18 +1570,18 @@
                 magnet = {"link": "", "hd": "0", "zm": "0", "uc": "0"}
                 tds = tr.find_all("td")
                 for i, td in enumerate(tds):
                     if i == 0:
                         magnet["link"] = td.a["href"]
                         magnet_title = td.a.text.strip().lower()
                         if (
-                            "uncensor" in magnet_title
-                            or "無修正" in magnet_title
-                            or "无修正" in magnet_title
-                            or "无码" in magnet_title
+                                "uncensor" in magnet_title
+                                or "無修正" in magnet_title
+                                or "无修正" in magnet_title
+                                or "无码" in magnet_title
                         ):
                             magnet["uc"] = "1"
                         links = td.find_all("a")
                         for link in links:
                             text = link.text.strip()
                             if text == "高清":
                                 magnet["hd"] = "1"
@@ -1668,19 +1719,19 @@
         return magnets
 
 
 class SukebeiUtil(BaseUtil):
     BASE_URL = "https://sukebei.nyaa.si"
 
     def get_av_by_id(
-        self,
-        id: str,
-        is_nice: bool,
-        is_uncensored: bool,
-        magnet_max_count=10,
+            self,
+            id: str,
+            is_nice: bool,
+            is_uncensored: bool,
+            magnet_max_count=10,
     ) -> typing.Tuple[int, dict]:
         """通过 sukebei 获取番号对应 av
 
         :param str id: 番号
         :param bool is_nice: 是否过滤出高清, 有字幕磁链
         :param bool is_uncensored: 是否过滤出无码磁链
         :param int magnet_max_count: 过滤后磁链的最大数目, 默认为 10
@@ -1743,18 +1794,18 @@
                     "zm": "0",  # 是否有字幕 0 否 | 1 是
                     "uc": "0",  # 是否未经审查 0 否 | 1 是
                 }
                 for j, td in enumerate(tds):
                     if j == 1:  # 获取标题
                         title = td.a.text
                         if (
-                            "uncensor" in title
-                            or "無修正" in title
-                            or "无修正" in title
-                            or "无码" in title
+                                "uncensor" in title
+                                or "無修正" in title
+                                or "无修正" in title
+                                or "无码" in title
                         ):
                             magnet["uc"] = "1"
                         if i == 0:
                             av["title"] = title
                     if j == 2:  # 获取磁链
                         magnet["link"] = td.find_all("a")[-1]["href"]
                     if j == 3:  # 获取大小
@@ -1924,17 +1975,17 @@
             "sec-ch-ua-platform": '"macOS"',
             "sec-fetch-dest": "empty",
             "sec-fetch-mode": "cors",
             "sec-fetch-site": "cross-site",
             "user-agent": self.ua(),
         }
         data = (
-            '{"conditions": "'
-            + av_id
-            + '", "field": 0, "target": 1, "sort": 1, "userToken": "", "hm": "008-api", "device_id": ""}'
+                '{"conditions": "'
+                + av_id
+                + '", "field": 0, "target": 1, "sort": 1, "userToken": "", "hm": "008-api", "device_id": ""}'
         )
 
         code, resp = self.send_req(
             url=SgpUtil.BASE_URL_SEARCH, headers=headers, m=1, data=data
         )
         if code != 200:
             return code, None
```

### Comparing `Jvav-1.9.2/setup.py` & `Jvav-1.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     requires = [i.strip() for i in r]
 
 with open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setup(
     name="Jvav",
-    version="1.9.2",
+    version="1.9.3",
     description="Useful tools for Jav.",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/akynazh/jvav",
     download_url="https://github.com/akynazh/jvav/releases/latest",
     author="akynazh",
     author_email="akynazh@gmail.com",
```

