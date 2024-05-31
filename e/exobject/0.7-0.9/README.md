# Comparing `tmp/exobject-0.7.tar.gz` & `tmp/exobject-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\exobject-0.7.tar", last modified: Wed Jan  5 05:27:49 2022, max compression
+gzip compressed data, was "exobject-0.9.tar", last modified: Fri May 31 06:37:42 2024, max compression
```

## Comparing `exobject-0.7.tar` & `exobject-0.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-01-05 05:27:49.000000 exobject-0.7/
-drwxrwxrwx   0        0        0        0 2022-01-05 05:27:49.000000 exobject-0.7/ExObject/
--rw-rw-rw-   0        0        0    14881 2021-11-18 08:14:57.000000 exobject-0.7/ExObject/DateTime.py
--rw-rw-rw-   0        0        0     6384 2020-08-24 10:03:58.000000 exobject-0.7/ExObject/ExObject.py
--rw-rw-rw-   0        0        0     2564 2022-01-05 05:27:35.000000 exobject-0.7/ExObject/ExRedis.py
--rw-rw-rw-   0        0        0     8636 2021-11-19 09:24:39.000000 exobject-0.7/ExObject/ExStock.py
--rw-rw-rw-   0        0        0     6412 2020-08-24 10:01:46.000000 exobject-0.7/ExObject/TimeSpan.py
--rw-rw-rw-   0        0        0       60 2020-08-24 10:01:46.000000 exobject-0.7/ExObject/__init__.py
--rw-rw-rw-   0        0        0     1811 2022-01-05 05:27:49.000000 exobject-0.7/PKG-INFO
--rw-rw-rw-   0        0        0      907 2020-08-24 10:01:46.000000 exobject-0.7/README.rst
-drwxrwxrwx   0        0        0        0 2022-01-05 05:27:49.000000 exobject-0.7/exobject.egg-info/
--rw-rw-rw-   0        0        0     1811 2022-01-05 05:27:49.000000 exobject-0.7/exobject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2022-01-05 05:27:49.000000 exobject-0.7/exobject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-05 05:27:49.000000 exobject-0.7/exobject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-01-05 05:27:49.000000 exobject-0.7/exobject.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-01-05 05:27:49.000000 exobject-0.7/exobject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-01-05 05:27:49.000000 exobject-0.7/setup.cfg
--rw-rw-rw-   0        0        0     1193 2022-01-05 05:27:11.000000 exobject-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 06:37:42.456085 exobject-0.9/
+drwxrwxrwx   0        0        0        0 2024-05-31 06:37:42.441088 exobject-0.9/ExObject/
+-rw-rw-rw-   0        0        0    14881 2021-11-18 08:14:57.000000 exobject-0.9/ExObject/DateTime.py
+-rw-rw-rw-   0        0        0     6384 2020-08-24 10:03:58.000000 exobject-0.9/ExObject/ExObject.py
+-rw-rw-rw-   0        0        0     3166 2024-05-31 06:31:23.000000 exobject-0.9/ExObject/ExParsel.py
+-rw-rw-rw-   0        0        0     3741 2022-01-05 06:06:16.000000 exobject-0.9/ExObject/ExRedis.py
+-rw-rw-rw-   0        0        0     9092 2024-05-31 03:59:36.000000 exobject-0.9/ExObject/ExStock.py
+-rw-rw-rw-   0        0        0     6412 2020-08-24 10:01:46.000000 exobject-0.9/ExObject/TimeSpan.py
+-rw-rw-rw-   0        0        0       60 2020-08-24 10:01:46.000000 exobject-0.9/ExObject/__init__.py
+-rw-rw-rw-   0        0        0     1202 2024-05-31 06:37:42.454087 exobject-0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      907 2020-08-24 10:01:46.000000 exobject-0.9/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-31 06:37:42.453085 exobject-0.9/exobject.egg-info/
+-rw-rw-rw-   0        0        0     1202 2024-05-31 06:37:42.000000 exobject-0.9/exobject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-05-31 06:37:42.000000 exobject-0.9/exobject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 06:37:42.000000 exobject-0.9/exobject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2024-05-31 06:37:42.000000 exobject-0.9/exobject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 06:37:42.000000 exobject-0.9/exobject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-31 06:37:42.457086 exobject-0.9/setup.cfg
+-rw-rw-rw-   0        0        0      508 2024-05-31 06:34:16.000000 exobject-0.9/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `exobject-0.7/ExObject/DateTime.py` & `exobject-0.9/ExObject/DateTime.py`

 * *Files identical despite different names*

### Comparing `exobject-0.7/ExObject/ExObject.py` & `exobject-0.9/ExObject/ExObject.py`

 * *Files identical despite different names*

### Comparing `exobject-0.7/ExObject/ExRedis.py` & `exobject-0.9/ExObject/ExRedis.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,24 +12,40 @@
 
     def getValue(self,key):
         r = self.redis.get(key)
         #self.redis.delete(key)
         if r:
             return r.decode("utf-8")
         return None
-        
+
+    def getValueBytes(self,key):
+        r = self.redis.get(key)
+        #self.redis.delete(key)
+        if r:
+            return r
+        return None
+
     def getValue_wait(self,key,timeout=10):
         c=0
         while c<timeout:
             r=self.getValue(key)
             if r:
                 return r
             c+=1
             time.sleep(1)
 
+    def getValueBytes_wait(self,key,timeout=10):
+        c=0
+        while c<timeout:
+            r=self.getValueBytes(key)
+            if r:
+                return r
+            c+=1
+            time.sleep(1)
+
     def push(self,key,value):
         self.redis.rpush(key,value)
 
     def lpush(self,key,value):
         self.redis.lpush(key,value)
 
     def pop_nowait(self,key):
@@ -40,14 +56,20 @@
 
     def pop_wait(self,key):
         r=self.redis.blpop(key)
         if r:
             return r[1].decode("utf-8")
         return None
 
+    def pop_wait_bytes(self,key):
+        r=self.redis.blpop(key)
+        if r:
+            return r[1]
+        return None
+
     def get_size(self,key):
         return self.redis.llen(key)
 
     def subscriber(self,chennal):
         ps = self.redis.pubsub()
         ps.subscribe(chennal)
         for item in ps.listen():
@@ -70,14 +92,31 @@
         callback_channel=chennal+"_"+callback_id
         _content=callback_id+content
         self.push(chennal,_content)
         r=self.getValue_wait(callback_channel,timeout)
         self.redis.delete(callback_channel)
         return r
 
+    def client_send_bytes(self,chennal,content,timeout=20):
+        callback_id=self._get_uuid()
+        callback_channel=chennal+"_"+callback_id
+        _content=bytes(callback_id,"utf-8")+content
+        self.push(chennal,_content)
+        r=self.getValueBytes_wait(callback_channel,timeout)
+        self.redis.delete(callback_channel)
+        return r
+
+    def server_listen_bytes(self,chennal,callback):
+        while True:
+            item = self.pop_wait_bytes(chennal)
+            callback_id=item[:32].decode("utf-8")
+            content=item[32:]
+            result=callback(content)
+            self.setValue(chennal+"_"+callback_id,result,3600)
+
     def close(self):
         try:
             self.redis.close()
         except:
             pass
 
     def _get_uuid(self):
```

### Comparing `exobject-0.7/ExObject/ExStock.py` & `exobject-0.9/ExObject/ExStock.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,268 +6,284 @@
 import time
 import requests
 import sys
 import os
 import json
 import datetime
 import sqlite3
-data_dict=None
-def _get(url)->Response:
-    response=None
+
+data_dict = None
+
+
+def _get(url) -> Response:
+    response = None
     for i in range(0, 3):
         try:
             # r = requests.post(url,data=json.dumps(params), headers={"Content-Type": "application/json"}, timeout=5)
-            response = requests.get(url,timeout=5)
+            response = requests.get(url, timeout=5)
             break
         except:
             time.sleep(1)
             pass
     return response
 
-def _create_dblite(cursor:Cursor):
-    sql='''
+
+def _create_dblite(cursor: Cursor):
+    sql = """
         CREATE TABLE IF NOT EXISTS stock_price(
         code TEXT NOT NULL,
         dt TEXT NOT NULL,
         open NUMERIC NULL DEFAULT NULL,
         close NUMERIC NULL DEFAULT NULL,
         high NUMERIC NULL DEFAULT NULL,
         low NUMERIC NULL DEFAULT NULL,
         volume NUMERIC NULL DEFAULT NULL,
         amount NUMERIC NULL DEFAULT NULL,
         amplitude NUMERIC NULL DEFAULT NULL,
         zdf NUMERIC NULL DEFAULT NULL,
         zde NUMERIC NULL DEFAULT NULL,
         turnover NUMERIC NULL DEFAULT NULL,
         PRIMARY KEY (code,dt))
-    '''
+    """
     cursor.execute(sql)
 
-def _to_sqlite(cursor,table,data):
-    dbItem=data
-    params=[]
+
+def _to_sqlite(cursor, table, data):
+    dbItem = data
+    params = []
     for key in dbItem:
         params.append(dbItem[key])
-    sql=f"INSERT OR IGNORE INTO {table} ({','.join(dbItem.keys())}) VALUES ({','.join(['?' for i in range(len(dbItem.keys()))])}) "
+    sql = f"INSERT OR IGNORE INTO {table} ({','.join(dbItem.keys())}) VALUES ({','.join(['?' for i in range(len(dbItem.keys()))])}) "
 
     # sql+="ON DUPLICATE KEY UPDATE "
     # for key in dbItem:
     #     if key in ["code","dt"]:
     #         continue
     #     if dbItem[key]:
     #         sql+= key+"=?,"
     #         params.append(dbItem[key])
-    #sql=sql[:-1]+";"
-    cursor.execute(sql,params)
+    # sql=sql[:-1]+";"
+    cursor.execute(sql, params)
+
 
 def get_holiday_from_api(year=None):
     if not year:
-        year=DateTime.Now().Year
-    url="http://timor.tech/api/holiday/year/"+str(year)
-    result=[]
-    data=None
+        year = DateTime.Now().Year
+    url = "https://timor.tech/api/holiday/year/" + str(year)
+    result = []
+    data = None
     for i in range(0, 3):
         try:
             # r = requests.post(url,data=json.dumps(params), headers={"Content-Type": "application/json"}, timeout=5)
-            r = requests.get(url,timeout=5)
-            data=r.json()
+            headers = {
+                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/125.0.0.0 Safari/537.36 Edg/125.0.0.0"
+            }
+            r = requests.get(url, timeout=5, headers=headers)
+            data = r.json()
             break
         except:
             time.sleep(1)
             pass
     for key in data["holiday"]:
         if data["holiday"][key]["holiday"]:
             result.append(data["holiday"][key]["date"])
 
     return result
 
+
 def get_holiday(year=None):
     global data_dict
     if not year:
-        year=DateTime.Now().Year
+        year = DateTime.Now().Year
     if not os.path.exists(".exobj"):
         os.mkdir(".exobj")
     if not os.path.exists(".exobj/exstock.json"):
-        with open(".exobj/exstock.json","w",encoding='utf-8') as file:
+        with open(".exobj/exstock.json", "w", encoding="utf-8") as file:
             file.write("{}")
-    
+
     if not data_dict:
-        data_dict=json.loads(open(".exobj/exstock.json").read())
+        data_dict = json.loads(open(".exobj/exstock.json").read())
 
-    holidays=data_dict.get(str(year))
+    holidays = data_dict.get(str(year))
     if not holidays:
-        holidays=get_holiday_from_api(year)
-        data_dict[str(year)]=holidays
-        with open(".exobj/exstock.json","w+",encoding='utf-8') as file:
+        holidays = get_holiday_from_api(year)
+        data_dict[str(year)] = holidays
+        with open(".exobj/exstock.json", "w+", encoding="utf-8") as file:
             file.write(json.dumps(data_dict))
 
     return holidays
 
-def is_trading_day(dt)->bool:
-    _dt=""
+
+def is_trading_day(dt) -> bool:
+    _dt = ""
     if type(dt) is DateTime:
-        _dt=dt.ToString('yyyy-MM-dd')
+        _dt = dt.ToString("yyyy-MM-dd")
     elif type(dt) is datetime.datetime:
-        _dt=dt.strftime('%Y-%m-%d')
+        _dt = dt.strftime("%Y-%m-%d")
     elif type(dt) is datetime.date:
-        _dt=str(dt)
+        _dt = str(dt)
     elif type(dt) is str:
-        _dt=DateTime.AutoConvert(dt).ToString('yyyy-MM-dd')
+        _dt = DateTime.AutoConvert(dt).ToString("yyyy-MM-dd")
     else:
-        raise Exception("UNSUPPORTED TYPE:"+str(type(dt)))
+        raise Exception("UNSUPPORTED TYPE:" + str(type(dt)))
 
     if _dt in get_holiday():
         return False
-    if DateTime.Convert(_dt,"yyyy-MM-dd").WeekDay>=6:
+    if DateTime.Convert(_dt, "yyyy-MM-dd").WeekDay >= 6:
         return False
     return True
 
-def get_next_trading_day(dt)->DateTime:
-    _dt=None
+
+def get_next_trading_day(dt) -> DateTime:
+    _dt = None
     if type(dt) is DateTime:
-        _dt=dt
+        _dt = dt
     elif type(dt) is datetime.datetime:
-        _dt=DateTime.Convert(dt.strftime('%Y-%m-%d'),"yyyy-MM-dd")
+        _dt = DateTime.Convert(dt.strftime("%Y-%m-%d"), "yyyy-MM-dd")
     elif type(dt) is datetime.date:
-        _dt=DateTime.Convert(str(dt),"yyyy-MM-dd")
+        _dt = DateTime.Convert(str(dt), "yyyy-MM-dd")
     elif type(dt) is str:
-        _dt=DateTime.AutoConvert(dt).ToString('yyyy-MM-dd')
-    
+        _dt = DateTime.AutoConvert(dt).ToString("yyyy-MM-dd")
+
     if not _dt:
         raise Exception("UNSUPPORTED dt")
 
     while True:
-        _dt=_dt.AddDays(1)
-        if(is_trading_day(_dt)):
+        _dt = _dt.AddDays(1)
+        if is_trading_day(_dt):
             return _dt.Date()
 
-def get_last_trading_day(dt)->DateTime:
-    _dt=None
+
+def get_last_trading_day(dt) -> DateTime:
+    _dt = None
     if type(dt) is DateTime:
-        _dt=dt
+        _dt = dt
     elif type(dt) is datetime.datetime:
-        _dt=DateTime.Convert(dt.strftime('%Y-%m-%d'),"yyyy-MM-dd")
+        _dt = DateTime.Convert(dt.strftime("%Y-%m-%d"), "yyyy-MM-dd")
     elif type(dt) is datetime.date:
-        _dt=DateTime.Convert(str(dt),"yyyy-MM-dd")
+        _dt = DateTime.Convert(str(dt), "yyyy-MM-dd")
     elif type(dt) is str:
-        _dt=DateTime.AutoConvert(dt).ToString('yyyy-MM-dd')
-    
+        _dt = DateTime.AutoConvert(dt).ToString("yyyy-MM-dd")
+
     if not _dt:
         raise Exception("UNSUPPORTED dt")
 
     while True:
-        _dt=_dt.AddDays(-1)
-        if(is_trading_day(_dt)):
+        _dt = _dt.AddDays(-1)
+        if is_trading_day(_dt):
             return _dt.Date()
 
-def get_price_from_api(code,date=None):
-    url=f"http://quote.eastmoney.com/{code}.html"
-    _str=_get(url).text
-    sec_id=ExObject.regexOne('nid=([0-9a-zA-Z\.]+)&',_str)
+
+def get_price_from_api(code, date=None):
+    url = f"http://quote.eastmoney.com/{code}.html"
+    _str = _get(url).text
+    sec_id = ExObject.regexOne("nid=([0-9a-zA-Z\.]+)&", _str)
     if not sec_id:
         raise Exception("Get Price Failure!")
-    url=f"http://46.push2his.eastmoney.com/api/qt/stock/kline/get?"
-    params={
-        "secid":sec_id,
-        "fields1":"f1,f2,f3,f4,f5,f6",
-        "fields2":"f51,f52,f53,f54,f55,f56,f57,f58,f59,f60,f61",
-        "klt":"101",
-        "fqt":"0",
-        "end":"20500101" if not date else date.ToString("yyyyMMdd"),
-        "lmt":"120"
+    url = f"http://46.push2his.eastmoney.com/api/qt/stock/kline/get?"
+    params = {
+        "secid": sec_id,
+        "fields1": "f1,f2,f3,f4,f5,f6",
+        "fields2": "f51,f52,f53,f54,f55,f56,f57,f58,f59,f60,f61",
+        "klt": "101",
+        "fqt": "0",
+        "end": "20500101" if not date else date.ToString("yyyyMMdd"),
+        "lmt": "120",
     }
-    url+=urlencode(params)
-    data=_get(url).json()
-    result=[]
+    url += urlencode(params)
+    data = _get(url).json()
+    result = []
     for line in data["data"]["klines"]:
-        items=line.split(",")
+        items = line.split(",")
         result.append(items)
     return result
 
-def get_price_from_sqlite(cursor:Cursor,code:str,date:str,lang="en"):
+
+def get_price_from_sqlite(cursor: Cursor, code: str, date: str, lang="en"):
     cursor.execute(f"SELECT * FROM stock_price WHERE code='{code}' AND dt='{date}' LIMIT 0,1")
-    item=cursor.fetchone()
+    item = cursor.fetchone()
     if not item:
         return None
-    result={}
-    result["code"]=item[0]
-    result["dt"]=item[1]
-    result["open"]=item[2]
-    result["close"]=item[3]
-    result["high"]=item[4]
-    result["low"]=item[5]
-    result["volume"]=item[6]
-    result["amount"]=item[7]
-    result["amplitude"]=str(item[8])+"%"
-    result["zdf"]=str(item[9])+"%"
-    result["zde"]=item[10]
-    result["turnover"]=str(item[11])+"%"
-    
-    if lang=="cn":
-        _result={
-            "代码":result["code"],
-            "日期":result["dt"],
-            "开盘":result["open"],
-            "收盘":result["close"],
-            "最高":result["high"],
-            "最低":result["low"],
-            "成交量":result["volume"],
-            "成交额":result["amount"],
-            "振幅":result["amplitude"],
-            "涨跌幅":result["zdf"],
-            "涨跌额":result["zde"],
-            "换手率":result["turnover"],
+    result = {}
+    result["code"] = item[0]
+    result["dt"] = item[1]
+    result["open"] = item[2]
+    result["close"] = item[3]
+    result["high"] = item[4]
+    result["low"] = item[5]
+    result["volume"] = item[6]
+    result["amount"] = item[7]
+    result["amplitude"] = str(item[8]) + "%"
+    result["zdf"] = str(item[9]) + "%"
+    result["zde"] = item[10]
+    result["turnover"] = str(item[11]) + "%"
+
+    if lang == "cn":
+        _result = {
+            "代码": result["code"],
+            "日期": result["dt"],
+            "开盘": result["open"],
+            "收盘": result["close"],
+            "最高": result["high"],
+            "最低": result["low"],
+            "成交量": result["volume"],
+            "成交额": result["amount"],
+            "振幅": result["amplitude"],
+            "涨跌幅": result["zdf"],
+            "涨跌额": result["zde"],
+            "换手率": result["turnover"],
         }
         return _result
     return result
 
-def get_price(code,dt,lang="en"):
-    _dt=""
+
+def get_price(code, dt, lang="en"):
+    _dt = ""
     if type(dt) is DateTime:
-        _dt=dt.ToString('yyyy-MM-dd')
+        _dt = dt.ToString("yyyy-MM-dd")
     elif type(dt) is datetime.datetime:
-        _dt=dt.strftime('%Y-%m-%d')
+        _dt = dt.strftime("%Y-%m-%d")
     elif type(dt) is datetime.date:
-        _dt=str(dt)
+        _dt = str(dt)
     elif type(dt) is str:
-        _dt=DateTime.AutoConvert(dt).ToString('yyyy-MM-dd')
+        _dt = DateTime.AutoConvert(dt).ToString("yyyy-MM-dd")
     else:
-        raise Exception("UNSUPPORTED TYPE:"+str(type(dt)))
+        raise Exception("UNSUPPORTED TYPE:" + str(type(dt)))
 
-    #判断是否存在SQLITE数据库
+    # 判断是否存在SQLITE数据库
     if not os.path.exists(".exobj"):
         os.mkdir(".exobj")
-    conn=None
-    cursor=None
+    conn = None
+    cursor = None
     if not os.path.exists(".exobj/price.db"):
         conn = sqlite3.connect(".exobj/price.db")
         cursor = conn.cursor()
         _create_dblite(cursor)
     else:
         conn = sqlite3.connect(".exobj/price.db")
         cursor = conn.cursor()
-    
-    result=get_price_from_sqlite(cursor,code,_dt,lang)
+
+    result = get_price_from_sqlite(cursor, code, _dt, lang)
     if not result:
-        code_sp=code.split(".")
-        _datas=get_price_from_api(code_sp[1].lower()+code_sp[0],DateTime.Convert(_dt,"yyyy-MM-dd").AddDays(1))
+        code_sp = code.split(".")
+        _datas = get_price_from_api(code_sp[1].lower() + code_sp[0], DateTime.Convert(_dt, "yyyy-MM-dd").AddDays(1))
         if not _datas:
             raise Exception("Get Price Failure!")
         for _data in _datas:
-            dbItem={
-                "code":code,
-                "dt":_data[0],
-                "open":_data[1],
-                "close":_data[2],
-                "high":_data[3],
-                "low":_data[4],
-                "volume":_data[5],
-                "amount":_data[6],
-                "amplitude":_data[7],
-                "zdf":_data[8],
-                "zde":_data[9],
-                "turnover":_data[10],
+            dbItem = {
+                "code": code,
+                "dt": _data[0],
+                "open": _data[1],
+                "close": _data[2],
+                "high": _data[3],
+                "low": _data[4],
+                "volume": _data[5],
+                "amount": _data[6],
+                "amplitude": _data[7],
+                "zdf": _data[8],
+                "zde": _data[9],
+                "turnover": _data[10],
             }
-            _to_sqlite(cursor,"stock_price",dbItem)
+            _to_sqlite(cursor, "stock_price", dbItem)
         conn.commit()
-        result=get_price_from_sqlite(cursor,code,_dt,lang)
-    return result
+        result = get_price_from_sqlite(cursor, code, _dt, lang)
+    return result
```

### Comparing `exobject-0.7/ExObject/TimeSpan.py` & `exobject-0.9/ExObject/TimeSpan.py`

 * *Files identical despite different names*

### Comparing `exobject-0.7/PKG-INFO` & `exobject-0.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,20 @@
 Metadata-Version: 2.1
 Name: exobject
-Version: 0.7
+Version: 0.9
 Summary: Extend Object Code
-Home-page: UNKNOWN
+Home-page: 
 Author: LenShang
 Author-email: lenshang@qq.com
 Maintainer: LenShang
 Maintainer-email: lenshang@qq.com
 License: BSD License
 Platform: all
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: python-dateutil
+Requires-Dist: parsel
 
 
 Extend Object Code
 ==================
 
 Pip:https://pypi.org/project/exobject
 
@@ -54,9 +43,7 @@
         print(c)
         print(c["?name"].ToString())#print a
         print(c["?nickName"].ToString())#print none
         #====
         date=DateTime.Now()
         date2=DateTime.AutoConvert("2019-02-06")
         print(date2)
-
-
```

### Comparing `exobject-0.7/README.rst` & `exobject-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `exobject-0.7/exobject.egg-info/PKG-INFO` & `exobject-0.9/exobject.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,20 @@
 Metadata-Version: 2.1
 Name: exobject
-Version: 0.7
+Version: 0.9
 Summary: Extend Object Code
-Home-page: UNKNOWN
+Home-page: 
 Author: LenShang
 Author-email: lenshang@qq.com
 Maintainer: LenShang
 Maintainer-email: lenshang@qq.com
 License: BSD License
 Platform: all
-Classifier: Development Status :: 4 - Beta
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: Implementation
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: python-dateutil
+Requires-Dist: parsel
 
 
 Extend Object Code
 ==================
 
 Pip:https://pypi.org/project/exobject
 
@@ -54,9 +43,7 @@
         print(c)
         print(c["?name"].ToString())#print a
         print(c["?nickName"].ToString())#print none
         #====
         date=DateTime.Now()
         date2=DateTime.AutoConvert("2019-02-06")
         print(date2)
-
-
```

