# Comparing `tmp/jsz-2024.5.19.tar.gz` & `tmp/jsz-2024.5.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsz-2024.5.19.tar", last modified: Sat May 18 20:42:05 2024, max compression
+gzip compressed data, was "jsz-2024.5.31.tar", last modified: Fri May 31 11:56:18 2024, max compression
```

## Comparing `jsz-2024.5.19.tar` & `jsz-2024.5.31.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      128 2024-05-09 15:00:28.691669 jsz-2024.5.19/README.md
--rw-r--r--   0        0        0      734 2024-05-18 20:42:05.865001 jsz-2024.5.19/pyproject.toml
--rw-r--r--   0        0        0      304 2024-05-18 20:33:48.507696 jsz-2024.5.19/src/jsz/__init__.py
--rw-r--r--   0        0        0     4396 2024-05-18 20:33:49.720446 jsz-2024.5.19/src/jsz/newpool.py
--rw-r--r--   0        0        0    21920 2024-05-18 20:33:50.819403 jsz-2024.5.19/src/jsz/tools.py
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 jsz-2024.5.19/PKG-INFO
+-rw-r--r--   0        0        0      128 2024-05-09 15:00:28.691669 jsz-2024.5.31/README.md
+-rw-r--r--   0        0        0      734 2024-05-31 11:56:18.263586 jsz-2024.5.31/pyproject.toml
+-rw-r--r--   0        0        0      308 2024-05-24 09:19:50.656331 jsz-2024.5.31/src/jsz/__init__.py
+-rw-r--r--   0        0        0     4406 2024-05-24 09:22:59.788359 jsz-2024.5.31/src/jsz/newpool.py
+-rw-r--r--   0        0        0    24197 2024-05-31 06:50:12.826409 jsz-2024.5.31/src/jsz/tools.py
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 jsz-2024.5.31/PKG-INFO
```

### Comparing `jsz-2024.5.19/pyproject.toml` & `jsz-2024.5.31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "jsz"
-version = "2024.5.19"
+version = "2024.5.31"
 description = "金手指"
 authors = [
     { name = "jiaosenvip" },
     { name = "jiaosenvip", email = "jiaosenvip@163.com" },
 ]
 dependencies = [
     "beautifulsoup4",
```

### Comparing `jsz-2024.5.19/src/jsz/newpool.py` & `jsz-2024.5.31/src/jsz/newpool.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,21 +22,21 @@
 """
 
 import multiprocessing
 import concurrent.futures
 from functools import wraps
 import time
 from rich.panel import Panel
-from rich import print
 
 
 class Pool:
     """
     线程池
     """
+
     def __init__(self, n: int = None):
         """
         线程池
 
         n: 线程数。默认为CPU核心数，可以自定义线程数。
         """
         if n:
@@ -147,23 +147,23 @@
             "正在运行": count_running,
             "剩余任务": count_other,
         }
         return state_result
 
     def state(self, extend: dict = None):
         """
-        返回线程池当前运行状态
+        返回线程池当前运行状态, 打印使用 jsz.print 函数.
 
         extend: 拓展字段。
         """
         state_dict = self.state_dict()
         state_result = (
             f"时间:[green]{time.strftime('%F %T')}[/]\n"
             f"总任务:{state_dict['总任务']}\n"
             f"已完成:{state_dict['已完成']} (成功:{state_dict['成功']} 取消:{state_dict['取消']} 报错:{state_dict['报错']})\n"
             f"正在运行:{state_dict['正在运行']}\n"
             f"剩余任务:{state_dict['剩余任务']}"
         )
 
         if extend and isinstance(extend, dict):
             state_result += "\n" + "\n".join([f"{i[0]}:{i[1]}" for i in extend.items()])
-        print(Panel(state_result, expand=False))
+        return Panel(state_result, expand=False)
```

### Comparing `jsz-2024.5.19/src/jsz/tools.py` & `jsz-2024.5.31/src/jsz/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 """
 工具库
 """
 
+import asyncio
 import time
 import datetime
 import calendar
 import os
 import platform
 import json
 import random
 import re
 import hashlib
 import base64
 from functools import wraps
+from typing import Callable
 from threading import Timer
 from urllib.parse import (
     urljoin,
     urlparse,
     urlunparse,
     urlencode,
     urlsplit,
@@ -27,38 +29,39 @@
     quote,
     parse_qs,
     parse_qsl,
 )
 import httpx
 from loguru import logger
 from faker import Faker
-from rich import print, print_json, inspect, load_ipython_extension
+from rich import print, print_json, inspect
 from rich.console import Console, Group
 from rich.progress import Progress, track
 from rich.padding import Padding
 from rich.columns import Columns
 from rich.markdown import Markdown
 from rich.panel import Panel
 from rich.rule import Rule
 from rich.status import Status
 from rich.table import Table
 from rich.pretty import pprint
 from bs4 import BeautifulSoup, element
 import html2text
-from pymongo import MongoClient
 from parsel import Selector
 from dateutil.parser import parse as timeparse
 
 if platform.machine() != "aarch64":
     from dateparser import parse as timeparse2
 else:
     timeparse2 = None
 
 
 __all__ = [
+    "async_httpx",
+    "asyncio",
     "base64_decode",
     "base64_encode",
     "bs_get_text",
     "bs_get_text2",
     "bs_html",
     "console",
     "clear",
@@ -74,14 +77,16 @@
     "inspect",
     "httpx",
     "listdir",
     "logger",
     "load_ipython_extension",
     "Markdown",
     "md5",
+    "mongodb",
+    "mongo_tongji",
     "now",
     "os",
     "oss2_find_file",
     "Panel",
     "parse_qs",
     "parse_qsl",
     "Padding",
@@ -107,14 +112,15 @@
     "Table",
     "time_next",
     "timeit",
     "timeparse",
     "timestamp",
     "to_excel",
     "to_json",
+    "to_async",
     "today",
     "tongji_content",
     "track",
     "ua",
     "unquote",
     "unquote_plus",
     "unwrap",
@@ -204,84 +210,303 @@
     "thead",
     "tbody",
     "tfoot",
     "form",
 ]
 
 fake = Faker()
-fake.zh = Faker("zh")
+fake.zh = Faker("zh")  # type: ignore
 console = Console()
 print_exception = console.print_exception
 
 
-def clear():
+def to_async(func: Callable) -> Callable:
     """
-    清屏
+    同步函数转异步，装饰器或直接调用
+
+    func: 函数
     """
-    if os.name == "nt":
-        os.system("cls")
-    else:
-        os.system("clear")
 
+    @wraps(func)
+    def async_func(*args, **kwargs):
+        return asyncio.to_thread(func, *args, **kwargs)
 
-def ua(version_from=101, version_to=125):
+    return async_func
+
+
+class async_httpx:
+    """
+    简化httpx异步调用
     """
-    随机ua
 
-    chrome 版本101-125
+    get = to_async(httpx.get)
+    post = to_async(httpx.post)
+    put = to_async(httpx.put)
+    head = to_async(httpx.head)
+    patch = to_async(httpx.patch)
+    delete = to_async(httpx.delete)
+    options = to_async(httpx.options)
+
+
+def bs_html(
+    markup: str = "",
+    features: str = "lxml",
+    builder=None,
+    parse_only=None,
+    from_encoding=None,
+    exclude_encodings=None,
+    element_classes=None,
+):
     """
-    return fake.chrome(
-        version_from=version_from,
-        version_to=version_to,
-        build_from=0,
-        build_to=0,
+    使用 BeautifulSoup 解析网页
+
+    markup: 网页源码
+    features: 默认使用 lxml 解析
+    """
+    return BeautifulSoup(
+        markup=markup,
+        features=features,
+        builder=builder,
+        parse_only=parse_only,
+        from_encoding=from_encoding,
+        exclude_encodings=exclude_encodings,
+        element_classes=element_classes,
     )
 
 
-def printx(*objects, sep: str = " ", end: str = "\n"):
+def load_ipython_extension(ip=None):
+    from rich.pretty import install
+    from rich.traceback import install as tr_install
+
+    install()
+    tr_install()
+
+
+def bs_get_text(
+    soup,
+    strip_tags: list = ["style", "script", "code"],
+) -> str:
     """
-    增加随机颜色的print
+    基于 BeautifulSoup 提取网页文本v1
+
+    soup: BeautifulSoup 对象或html文本
+    strip_tags: 需要删除的节点
     """
-    for i in objects[:-1]:
-        print(f"[{fake.color()}]{i}[/]" if isinstance(i, str) else i, sep=sep, end=sep)
-    print(
-        f"[{fake.color()}]{objects[-1]}[/]"
-        if isinstance(objects[-1], str)
-        else objects[-1],
-        sep=sep,
-        end=end,
+    if isinstance(soup, str):
+        soup = bs_html(soup)
+    for node in soup(strip_tags):
+        node.extract()
+    for node in soup.find_all():
+        if node.name not in NON_BREAKING_ELEMENTS:
+            node.append("\n") if node.name == "br" else node.append("\n\n")
+    return (
+        re.sub("\n\n+", "\n\n", soup.get_text())
+        .strip()
+        .replace("\xa0", " ")
+        .replace("\u3000", " ")
     )
 
 
-def md5(string: bytes):
-    if isinstance(string, str):
-        string = string.encode()
-    result = hashlib.md5(string).hexdigest()
-    return result
+def bs_get_text2(
+    soup,
+    strip_tags: list = ["style", "script", "code"],
+):
+    """
+    基于 BeautifulSoup 提取网页文本v2
 
+    soup: BeautifulSoup 对象或html文本
+    """
+    if isinstance(soup, str):
+        soup = bs_html(soup)
+    for node in soup(strip_tags):
+        node.extract()
 
-def base64_encode(string: bytes):
+    def traverse(node):
+        if isinstance(node, element.NavigableString):
+            if node.strip():
+                yield node.strip()
+        else:
+            if node.name in BLOCK_TAGS:
+                yield "\n"
+            for child in node.children:
+                yield from traverse(child)
+            if node.name in BLOCK_TAGS:
+                yield "\n"
+
+    parsed = "".join(traverse(soup)).strip().replace("\xa0", " ").replace("\u3000", " ")
+    return parsed
+
+
+def base64_encode(string: bytes | str):
     """
     base64编码
     """
     if isinstance(string, str):
         string = string.encode()
     return base64.b64encode(string).decode()
 
 
-def base64_decode(string: bytes):
+def base64_decode(string: bytes | str):
     """
     base64解码
     """
     if isinstance(string, str):
         string = string.encode()
     return base64.b64decode(string).decode()
 
 
-def now(fmt_type: int = None, fmt: str = None):
+def mongodb(
+    host,
+    database,
+    port: int | None = None,
+):
+    """
+    连接 MongoDB
+
+    host: mongo 链接
+    database: 数据库名称
+    port: mongo 端口
+
+    host 有密码格式: "mongodb://username:password@192.168.0.1:27017/"
+    host 无密码格式: "mongodb://192.168.0.1:27017/"
+    """
+    from pymongo import MongoClient
+
+    try:
+        # 连接到 MongoDB
+        client = MongoClient(host, port)
+        db = client[database]
+        db.list_collection_names()
+        logger.success(f"MongoDB 成功连接到 {database}")
+        return db
+    except Exception as e:
+        logger.error("MongoDB 连接失败:", str(e))
+        return None
+
+
+connect_to_mongodb = mongodb
+
+
+def mongo_tongji(
+    mongodb,
+    prefix: str = "",
+    tongji_collection: str = "tongji",
+) -> dict:
+    """
+    统计 mongodb 每个集合的`文档数量`
+
+    mongodb: mongo 库
+    prefix: mongo 表前缀, 默认空字符串可以获取所有表, 字段名称例如 `统计_20240101`。
+    tongji_collection: 统计表名称，默认为 tongji
+    """
+
+    tongji = mongodb[tongji_collection]
+    key = prefix if prefix else f"统计_{now(7)}"
+    collection_count_dict = {
+        **(
+            tongji.find_one({"key": key}).get("count")
+            if tongji.find_one({"key": key})
+            else {}
+        ),
+        **(
+            {
+                i: mongodb[i].estimated_document_count()
+                for i in mongodb.list_collection_names()
+                if i.startswith(prefix)
+            }
+        ),
+    }
+    tongji.update_one(
+        {"key": prefix if prefix else f"统计_{now(7)}"},
+        {"$set": {"count": collection_count_dict}},
+        upsert=True,
+    )
+    return dict(sorted(collection_count_dict.items()))
+
+
+def clear():
+    """
+    清屏
+    """
+    if os.name == "nt":
+        os.system("cls")
+    else:
+        os.system("clear")
+
+
+def get_proxies(n: int = 1, httpx: bool = False):
+    """
+    ## 随机返回代理
+
+    需要先配置环境变量 HTTP_PROXY_DICT,  使用 to_json 将 HTTP_PROXY_DICT 转换成 json
+
+    n: 代理选择，数字或对应的字符串
+    """
+    http_proxy_dict_str = os.getenv("HTTP_PROXY_DICT", "")
+    if not http_proxy_dict_str:
+        print("未配置 HTTP_PROXY_DICT")
+        raise Exception()
+    proxyurl = random.choice(read_json(http_proxy_dict_str).get(str(n)))
+    if httpx:
+        proxies = {
+            "http://": proxyurl,
+            "https://": proxyurl,
+        }
+    else:
+        proxies = {
+            "http": proxyurl,
+            "https": proxyurl,
+        }
+    return proxies
+
+
+def listdir(path=None, key=None, reverse: bool = False):
+    """
+    help(os.listdir)
+
+    path: 目录路径
+    key: 排序方式
+    reverse: 指定是否反转, 默认否。
+    """
+    return sorted(
+        os.listdir(path),
+        key=key,
+        reverse=reverse,
+    )
+
+
+def html2md(
+    string: str,
+    ignore_links: bool = True,
+    ignore_images: bool = True,
+    ignore_tables: bool = True,
+) -> str:
+    """
+    ## HTML 转 Markdown
+
+    默认忽略链接、忽略图像、忽略表格
+    """
+    converter = html2text.HTML2Text()
+    converter.ignore_links = ignore_links  # 忽略链接
+    converter.ignore_images = ignore_images  # 忽略图像
+    converter.ignore_tables = ignore_tables  # 忽略表格
+    if ignore_tables:
+        string = re.sub("<table.*?</table>", "", string)
+    content = converter.handle(string)
+    return content
+
+
+def md5(string: bytes | str):
+    if isinstance(string, str):
+        string = string.encode()
+    result = hashlib.md5(string).hexdigest()
+    return result
+
+
+def now(fmt_type: int | None = None, fmt: str | None = None):
     """
     默认返回当前时间, 精度到秒。
 
     fmt_type: 格式化类型。
     fmt: 通过 strformat 格式化。
 
     - fmt=None -> datetime.datetime(2024, 1, 18, 11, 44, 57)
@@ -309,14 +534,29 @@
         return f"{datetime.date.today():%Y/%m/%d}"
     elif fmt_type == 7:
         return f"{datetime.date.today():%Y%m%d}"
     else:
         return datetime.datetime.now().replace(microsecond=0)
 
 
+def printx(*objects, sep: str = " ", end: str = "\n"):
+    """
+    增加随机颜色的print
+    """
+    for i in objects[:-1]:
+        print(f"[{fake.color()}]{i}[/]" if isinstance(i, str) else i, sep=sep, end=sep)
+    print(
+        f"[{fake.color()}]{objects[-1]}[/]"
+        if isinstance(objects[-1], str)
+        else objects[-1],
+        sep=sep,
+        end=end,
+    )
+
+
 def timestamp(n: int = 10):
     """
     返回时间戳
 
     n 可选 10位和13位。
     """
     if n == 13:
@@ -370,15 +610,15 @@
         )
     ]
 
 
 def date_next(
     days: int = 0,
     weeks: int = 0,
-    date: datetime.date = None,
+    date: datetime.date | None = None,
 ):
     """
     返回下一个的日期, 默认为0, 负数为过去, 正数为未来。
     """
     if not date:
         date = datetime.date.today()
     return date + datetime.timedelta(days=days, weeks=weeks)
@@ -388,16 +628,16 @@
     days: int = 0,
     hours: int = 0,
     minutes: int = 0,
     seconds: int = 0,
     weeks: int = 0,
     months: int = 0,
     years: int = 0,
-    start: tuple | datetime.datetime = None,
-    fmt: str = None,
+    start: tuple | datetime.datetime | None = None,
+    fmt: str | None = None,
 ):
     """
     返回下一个的时间, 默认为0, 负数为过去, 正数为未来。先算月份再算年, 然后依次计算。
 
     - days: 偏移天数
     - hours: 偏移小时数
     - minutes: 偏移分钟数
@@ -409,15 +649,14 @@
     - fmt: 指定输出格式。
     """
     if start:
         if not isinstance(start, datetime.datetime):
             start = datetime.datetime(*start)
     else:
         start = datetime.datetime.now().replace(microsecond=0)
-    start: datetime.datetime
     if months:
         # 获取下个时间的年份和月份
         next_year = start.year + (start.month == 12)
         next_month = start.month + months
         if next_month > 12:
             next_year += next_month // 12
             next_month = next_month % 12
@@ -475,15 +714,15 @@
 def fromtimestamp(t: int):
     """
     从时间戳返回 datetime 格式, 自动判断字符串和数字, 不符合格式要求会原样返回。
     """
     _t = t
     if isinstance(t, str) and t.isdigit():
         t = int(t[:10])
-    if isinstance(t, int):
+    if isinstance(t, (int, float)):
         return datetime.datetime.fromtimestamp(int(str(t)[:10]))
     return _t
 
 
 def read_json(filepath, encoding="utf-8"):
     """
     JSON 反序列化, 读取 JSON 文件
@@ -498,16 +737,16 @@
 
 
 def to_json(
     obj,
     filename=None,
     encoding="utf-8",
     ensure_ascii: bool = False,
-    indent: int = None,
-    separators: tuple = None,
+    indent: int | None = None,
+    separators: tuple | None = None,
 ):
     """
     JSON 序列化, 将Python 对象写入文件或转换为字符串。
 
     filename: JSON 文件路径
     indent: 缩进
     ensure_ascii: 默认不转为unicode
@@ -528,50 +767,50 @@
                 indent=indent,
                 ensure_ascii=ensure_ascii,
                 separators=separators,
             )
 
 
 def to_excel(
-    df,
-    path,
+    df,  # type: ignore
+    path: str,
     mode: str = "w",
     index: bool = False,
     engine: str = "xlsxwriter",
 ):
     """
     ## 导出 excel
 
-    - df: dataframe 对象, 多个sheet可以通过字典传入, 键为sheet名称。`{"sheet_name1":df1, "sheet_name2":df2}`
+    - df: dataframe 对象, 多个sheet可以通过字典传入, 键为sheet名称。`{"sheet_name1": df1, "sheet_name2": df2}`
     - path: 文件保存路径
     - mode: 默认 `w` 为全新写入; 如果为 `a` 则为插入, 引擎会改为 openpyxl。
     - strings_to_urls: 默认不转换url
     - index: 默认不导出索引
     - engine: 默认引擎使用xlsxwriter, 其他选项有 'auto'、'openpyxl'、'odf'
     """
     import pandas as pd
 
-    df: pd.DataFrame
+    df: dict[str, pd.DataFrame] | pd.DataFrame
 
     if engine == "xlsxwriter":
         engine_kwargs = {"options": {"strings_to_urls": False}}
 
     if mode == "a":
         engine = "openpyxl"
         engine_kwargs = None
 
     with pd.ExcelWriter(
         path,
-        engine=engine,
-        mode=mode,
+        engine=engine,  # type: ignore
+        mode=mode,  # type: ignore
         engine_kwargs=engine_kwargs,
     ) as writer:
         if isinstance(df, dict):
             for sheet in df:
-                df.get(sheet).to_excel(writer, index=index, sheet_name=sheet)
+                df.get(sheet).to_excel(writer, index=index, sheet_name=sheet)  # type: ignore
         else:
             df.to_excel(writer, index=index)
 
 
 def retry(
     num: int = 3,
     log: bool = False,
@@ -612,65 +851,19 @@
                 raise error_list[-1]
 
         return func
 
     return wrap
 
 
-def html2md(
-    string: str,
-    ignore_links: bool = True,
-    ignore_images: bool = True,
-    ignore_tables: bool = True,
-) -> str:
-    """
-    ## HTML 转 Markdown
-
-    默认忽略链接、忽略图像、忽略表格
-    """
-    converter = html2text.HTML2Text()
-    converter.ignore_links = ignore_links  # 忽略链接
-    converter.ignore_images = ignore_images  # 忽略图像
-    converter.ignore_tables = ignore_tables  # 忽略表格
-    if ignore_tables:
-        string = re.sub("<table.*?</table>", "", string)
-    content = converter.handle(string)
-    return content
-
-
-def wait(n: int = 0, log: bool = False):
-    """
-    后台运行, 异步不阻塞。
-
-    n: 等待秒数
-    log: 启动后打印日志。
-
-    @wait(2)
-    def hello():
-        print('运行完毕')
-    """
-
-    def wrap(f):
-        @wraps(f)
-        def func(*args, **kwargs):
-            if log:
-                logger.info(f"{f.__name__} 函数将于 {n} 秒后运行")
-            t = Timer(n, f, args=args, kwargs=kwargs)
-            t.start()
-
-        return func
-
-    return wrap
-
-
 def send_bot(
     content: str = "测试",
     bot_key: str = "",
     msgtype: str = "markdown",
-    filepath: str = None,
+    filepath: str | None = None,
     mentioned_list: list = [],
 ):
     """
     企业微信群机器人, 基础的 Mardkown 语法。
 
     <font color="info">绿色</font>
     <font color="comment">灰色</font>
@@ -681,201 +874,41 @@
     msgtype: 类型, 包括 markdown, text, file, voice, image
     filepath: 文件路径，非文本类型使用。
     mentioned_list: 提醒用户列表, 填入手机号或 "@all", 仅支持 text 类型。
     """
     if msgtype not in ["markdown", "text", "file", "voice", "image"]:
         raise NameError('类型仅支持 "markdown", "text", "file", "voice", "image"')
     if not bot_key:
-        bot_key = os.environ.get("BOT_KEY")
+        bot_key = os.getenv("BOT_KEY", "")
         if not bot_key:
             print("未全局配置 BOT_KEY，也未填写参数 bot_key")
             raise Exception("请填写 bot_key")
     if "key=" in bot_key:
         raise Exception("bot_key 只需要填入 `key=` 后面的部分")
     if msgtype == "file" or msgtype == "voice":
         file_upload_url = f"https://qyapi.weixin.qq.com/cgi-bin/webhook/upload_media?key={bot_key}&type=file"
-        files = {filepath.rsplit(".", 1)[0]: open(filepath, "rb")}
+        files = {filepath.rsplit(".", 1)[0]: open(filepath, "rb")}  # type: ignore
         resp = httpx.post(file_upload_url, files=files)
         msg = {"media_id": resp.json().get("media_id")}
     elif msgtype == "image":
-        content = open(filepath, "rb").read()
+        content = open(filepath, "rb").read()  # type: ignore
         msg = {"base64": base64_encode(content), "md5": md5(content)}
     elif msgtype == "text":
         msg = {"content": content, "mentioned_mobile_list": mentioned_list}
     else:
         msg = {"content": content}
     url = f"https://qyapi.weixin.qq.com/cgi-bin/webhook/send?key={bot_key}"
     json_data = {
         "msgtype": msgtype,
         msgtype: msg,
     }
     response = httpx.post(url, json=json_data)
     return response
 
 
-def get_proxies(n: int = 1, httpx: bool = False):
-    """
-    ## 随机返回代理
-
-    需要先配置环境变量 HTTP_PROXY_DICT,  使用 to_json 将 HTTP_PROXY_DICT 转换成 json
-
-    n: 代理选择，数字或对应的字符串
-    """
-    http_proxy_dict_str = os.environ.get("HTTP_PROXY_DICT")
-    if not http_proxy_dict_str:
-        print("未配置 HTTP_PROXY_DICT")
-        raise Exception()
-    proxyurl = random.choice(read_json(http_proxy_dict_str).get(str(n)))
-    if httpx:
-        proxies = {
-            "http://": proxyurl,
-            "https://": proxyurl,
-        }
-    else:
-        proxies = {
-            "http": proxyurl,
-            "https": proxyurl,
-        }
-    return proxies
-
-
-def pdf2text(filepath):
-    """
-    从 pdf 提取文本内容
-
-    filepath: 文件路径
-    """
-    from pypdf import PdfReader
-
-    reader = PdfReader(filepath)
-    content = "".join([i.extract_text() for i in reader.pages])
-    return content
-
-
-def listdir(path=None, key=None, reverse: bool = False):
-    """
-    help(os.listdir)
-
-    path: 目录路径
-    key: 排序方式
-    reverse: 指定是否反转, 默认否。
-    """
-    return sorted(os.listdir(path), key=key, reverse=reverse)
-
-
-def randint(a: int, b: int):
-    """
-    返回随机数, [a, b]前后包含。
-    """
-    return random.randint(a, b)
-
-
-def bs_html(
-    markup: str = "",
-    features: str = "lxml",
-    builder=None,
-    parse_only=None,
-    from_encoding=None,
-    exclude_encodings=None,
-    element_classes=None,
-):
-    """
-    使用 BeautifulSoup 解析网页
-
-    markup: 网页源码
-    features: 默认使用 lxml 解析
-    """
-    return BeautifulSoup(
-        markup=markup,
-        features=features,
-        builder=builder,
-        parse_only=parse_only,
-        from_encoding=from_encoding,
-        exclude_encodings=exclude_encodings,
-        element_classes=element_classes,
-    )
-
-
-def bs_get_text(
-    soup,
-    strip_tags: list = ["style", "script", "code"],
-) -> str:
-    """
-    基于 BeautifulSoup 提取网页文本v1
-
-    soup: BeautifulSoup 对象或html文本
-    strip_tags: 需要删除的节点
-    """
-    if isinstance(soup, str):
-        soup = bs_html(soup)
-    for node in soup(strip_tags):
-        node.extract()
-    for node in soup.find_all():
-        if node.name not in NON_BREAKING_ELEMENTS:
-            node.append("\n") if node.name == "br" else node.append("\n\n")
-    return re.sub("\n\n+", "\n\n", soup.get_text()).strip()
-
-
-def bs_get_text2(
-    soup,
-    strip_tags: list = ["style", "script", "code"],
-):
-    """
-    基于 BeautifulSoup 提取网页文本v2
-
-    soup: BeautifulSoup 对象或html文本
-    """
-    if isinstance(soup, str):
-        soup = bs_html(soup)
-    for node in soup(strip_tags):
-        node.extract()
-
-    def traverse(node):
-        if isinstance(node, element.NavigableString):
-            if node.strip():
-                yield node.strip()
-        else:
-            if node.name in BLOCK_TAGS:
-                yield "\n"
-            for child in node.children:
-                yield from traverse(child)
-            if node.name in BLOCK_TAGS:
-                yield "\n"
-
-    parsed = "".join(traverse(soup)).strip()
-    return parsed
-
-
-def connect_to_mongodb(
-    uri,
-    database,
-    port: int = None,
-):
-    """
-    连接 MongoDB
-
-    uri: mongo 链接
-    database: 数据库名称
-    port: mongo 端口
-
-    uri 有密码格式: "mongodb://username:password@192.168.0.1:27017/"
-    uri 无密码格式: "mongodb://192.168.0.1:27017/"
-    """
-    try:
-        # 连接到 MongoDB
-        client = MongoClient(uri, port)
-        db = client[database]
-        db.list_collection_names()
-        logger.success(f"MongoDB 成功连接到 {database}")
-        return db
-    except Exception as e:
-        logger.error("MongoDB 连接失败:", str(e))
-        return None
-
-
 def oss2_find_file(bucket, prefix, size1=0, size2=1048576000):
     """
     寻找 oss 文件, 指定 size1 和 size2 可以筛选特定大小的文件。默认单位为 KB。返回值为字典。
 
     - 可以通过 len 统计文件数量。
     - 可以通过 sum 统计返回值字典的 values 统计文件夹文件的总大小, 单位为KB。
 
@@ -894,14 +927,34 @@
         t = obj.size / 1024
         if size1 < t < size2 and not obj.is_prefix():
             print(f"文件名:{obj.key}  文件大小: {t:.2f} KB")
             d[obj.key] = t
     return d
 
 
+def pdf2text(filepath):
+    """
+    从 pdf 提取文本内容
+
+    filepath: 文件路径
+    """
+    from pypdf import PdfReader
+
+    reader = PdfReader(filepath)
+    content = "".join([i.extract_text() for i in reader.pages])
+    return content
+
+
+def randint(a: int, b: int):
+    """
+    返回随机数, [a, b]前后包含。
+    """
+    return random.randint(a, b)
+
+
 def timeit(function):
     """
     计时器
 
     ```
     @timeit
     def hello():
@@ -913,7 +966,46 @@
     def func(*args, **kwargs):
         t0 = time.time() * 1000
         result = function(*args, **kwargs)
         print(f"运行 {function.__name__} 耗时: {time.time() * 1000 - t0:.2f} ms")
         return result
 
     return func
+
+
+def ua(version_from=101, version_to=125):
+    """
+    随机ua
+
+    chrome 版本101-125
+    """
+    return fake.chrome(
+        version_from=version_from,
+        version_to=version_to,
+        build_from=0,
+        build_to=0,
+    )
+
+
+def wait(n: int = 0, log: bool = False):
+    """
+    后台运行, 异步不阻塞。
+
+    n: 等待秒数
+    log: 启动后打印日志。
+
+    @wait(2)
+    def hello():
+        print('运行完毕')
+    """
+
+    def wrap(f):
+        @wraps(f)
+        def func(*args, **kwargs):
+            if log:
+                logger.info(f"{f.__name__} 函数将于 {n} 秒后运行")
+            t = Timer(n, f, args=args, kwargs=kwargs)
+            t.start()
+
+        return func
+
+    return wrap
```

### Comparing `jsz-2024.5.19/PKG-INFO` & `jsz-2024.5.31/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsz
-Version: 2024.5.19
+Version: 2024.5.31
 Summary: 金手指
 Author: jiaosenvip
 Author-Email: jiaosenvip <jiaosenvip@163.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jiaosenvip/jsz
 Requires-Python: >=3.11
 Requires-Dist: beautifulsoup4
```

