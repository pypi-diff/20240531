# Comparing `tmp/erp_apis-1.0.8-py3-none-any.whl.zip` & `tmp/erp_apis-1.2.11-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,21 @@
-Zip file size: 11298 bytes, number of entries: 15
--rw-rw-rw-  2.0 fat      403 b- defN 24-May-06 06:32 erp_apis/config.py
--rw-rw-rw-  2.0 fat     3577 b- defN 24-May-08 03:10 erp_apis/erpRequest.py
+Zip file size: 18995 bytes, number of entries: 19
+-rw-rw-rw-  2.0 fat     2374 b- defN 24-May-31 11:05 erp_apis/config.py
+-rw-rw-rw-  2.0 fat     5734 b- defN 24-May-30 09:48 erp_apis/erpRequest.py
+-rw-rw-rw-  2.0 fat     1062 b- defN 24-May-31 11:06 erp_apis/apis/ItemApi.py
+-rw-rw-rw-  2.0 fat     4597 b- defN 24-May-29 08:53 erp_apis/apis/Print.py
 -rw-rw-rw-  2.0 fat      143 b- defN 24-May-07 03:26 erp_apis/apis/__init__.py
--rw-rw-rw-  2.0 fat     2587 b- defN 24-May-07 06:09 erp_apis/apis/afterSales.py
+-rw-rw-rw-  2.0 fat     4743 b- defN 24-May-21 08:17 erp_apis/apis/afterSales.py
 -rw-rw-rw-  2.0 fat     1538 b- defN 24-May-07 06:09 erp_apis/apis/goods.py
 -rw-rw-rw-  2.0 fat     1013 b- defN 24-May-07 03:18 erp_apis/apis/inventory.py
--rw-rw-rw-  2.0 fat     4346 b- defN 24-May-08 06:17 erp_apis/apis/order.py
--rw-rw-rw-  2.0 fat     2091 b- defN 24-May-08 06:19 erp_apis/apis/test.py
+-rw-rw-rw-  2.0 fat     4841 b- defN 24-May-28 05:28 erp_apis/apis/order.py
+-rw-rw-rw-  2.0 fat     3093 b- defN 24-May-13 02:08 erp_apis/apis/refund.py
+-rw-rw-rw-  2.0 fat     3094 b- defN 24-May-28 01:06 erp_apis/apis/shopData.py
+-rw-rw-rw-  2.0 fat     2057 b- defN 24-May-31 12:15 erp_apis/apis/test.py
 -rw-rw-rw-  2.0 fat     1139 b- defN 24-May-07 12:41 erp_apis/apis/user.py
 -rw-rw-rw-  2.0 fat      141 b- defN 24-Apr-30 10:11 erp_apis/utils/__init__.py
--rw-rw-rw-  2.0 fat     2063 b- defN 24-May-08 06:18 erp_apis/utils/util.py
--rw-rw-rw-  2.0 fat     1580 b- defN 24-May-09 01:52 erp_apis-1.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-09 01:52 erp_apis-1.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       38 b- defN 24-May-09 01:52 erp_apis-1.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1178 b- defN 24-May-09 01:52 erp_apis-1.0.8.dist-info/RECORD
-15 files, 21929 bytes uncompressed, 9368 bytes compressed:  57.3%
+-rw-rw-rw-  2.0 fat     2137 b- defN 24-May-28 05:28 erp_apis/utils/util.py
+-rw-rw-rw-  2.0 fat     1581 b- defN 24-May-31 12:16 erp_apis-1.2.11.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-31 12:16 erp_apis-1.2.11.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       38 b- defN 24-May-31 12:16 erp_apis-1.2.11.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1505 b- defN 24-May-31 12:16 erp_apis-1.2.11.dist-info/RECORD
+19 files, 40922 bytes uncompressed, 16565 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -1,13 +1,19 @@
 Filename: erp_apis/config.py
 Comment: 
 
 Filename: erp_apis/erpRequest.py
 Comment: 
 
+Filename: erp_apis/apis/ItemApi.py
+Comment: 
+
+Filename: erp_apis/apis/Print.py
+Comment: 
+
 Filename: erp_apis/apis/__init__.py
 Comment: 
 
 Filename: erp_apis/apis/afterSales.py
 Comment: 
 
 Filename: erp_apis/apis/goods.py
@@ -15,32 +21,38 @@
 
 Filename: erp_apis/apis/inventory.py
 Comment: 
 
 Filename: erp_apis/apis/order.py
 Comment: 
 
+Filename: erp_apis/apis/refund.py
+Comment: 
+
+Filename: erp_apis/apis/shopData.py
+Comment: 
+
 Filename: erp_apis/apis/test.py
 Comment: 
 
 Filename: erp_apis/apis/user.py
 Comment: 
 
 Filename: erp_apis/utils/__init__.py
 Comment: 
 
 Filename: erp_apis/utils/util.py
 Comment: 
 
-Filename: erp_apis-1.0.8.dist-info/METADATA
+Filename: erp_apis-1.2.11.dist-info/METADATA
 Comment: 
 
-Filename: erp_apis-1.0.8.dist-info/WHEEL
+Filename: erp_apis-1.2.11.dist-info/WHEEL
 Comment: 
 
-Filename: erp_apis-1.0.8.dist-info/top_level.txt
+Filename: erp_apis-1.2.11.dist-info/top_level.txt
 Comment: 
 
-Filename: erp_apis-1.0.8.dist-info/RECORD
+Filename: erp_apis-1.2.11.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## erp_apis/config.py

```diff
@@ -3,13 +3,26 @@
 # File：config.py
 # Author：李福成
 # Date ：2024-04-29 10:04
 # IDE：PyCharm
 
 Erp321BaseUrl = 'https://www.erp321.com'
 ErpApiBaseUrl = 'https://api.erp321.com'
+ErpGoodsBaseUrl = 'https://goods.scm121.com'
+
+
 
 
 
 DEFAULT_HEADERS = {
-    'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/237.84.2.178 Safari/537.36 Edg/109.0.1518.78',
-}
+    'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36',    # 'cookie': 'acw_tc=2760779b17154951601776467e2eaae3707f13160901b36135bd350c5c0636; _ati=2632320813015; j_d_3=3ZEUHZ3LD6TF2GRXTWSSJ6LVEZIAKQE7XTZO5II3AI23TRQYIQ2RLBFPPHLVXCO7YVXQXAL36AGJ2C5RQMV7RAGT74; u_ssi=; u_drp=; u_r=12%2c13%2c14%2c15%2c17%2c18%2c22%2c23%2c27%2c28%2c29%2c30%2c31%2c32%2c33%2c34%2c35%2c36%2c39%2c40%2c41%2c52%2c53%2c54%2c61%2c62%2c101%2c1001%2c109; u_shop=-1; u_lastLoginType=ap; tfstk=fP2koMDya7lSpJ-dr-D53zgD_v1xFUMI1ypKJv3FgquXyUp8YpcUADiE4k77-J0qUXN-J43nKkaGDNBOBuZSdx7OWOIUOX6jd2WKLiurgfDFWNBxX-cS2vPd8MOQmoujxUuETyWqgqir4vurTERqbquELvze0Iotb2orT4-qMARrWJPa3GEdPKE0TP2mqb5Y4qJEc-moZVrzEpJUb0co7uucWF37yjrItJtBKfEz1yiazU7tNkP0o0DhHQkamWzic8W9rmN80ygqgHJQmX0ug8lDYpr4m4cgtzbkN4P8ofiqgHXsDP34V8PcAErzW4Dr0jBNjolUM8G_eZJoQ5Z-eWzC6IMuY7kc4fO2_so6dmSLnBOIamim5gRoxaMJO6PPmiATAbojfVIcmBMjamimUijD1DlrccyC.; 3AB9D23F7A4B3C9B=3ZEUHZ3LD6TF2GRXTWSSJ6LVEZIAKQE7XTZO5II3AI23TRQYIQ2RLBFPPHLVXCO7YVXQXAL36AGJ2C5RQMV7RAGT74; u_name=%e6%9d%8e%e7%a6%8f%e6%88%90; u_lid=18986680202; u_json=%7b%22t%22%3a%222024-5-12+14%3a49%3a03%22%2c%22co_type%22%3a%22%e6%a0%87%e5%87%86%e5%95%86%e5%ae%b6%22%2c%22proxy%22%3anull%2c%22ug_id%22%3a%2211003725%22%2c%22dbc%22%3a%221149%22%2c%22tt%22%3a%2295%22%2c%22apps%22%3a%221.4.7.150.152.168.169%22%2c%22pwd_valid%22%3a%220%22%2c%22ssi%22%3anull%2c%22sign%22%3a%224001967.1EA70FE2D4EB480D859D91A98D86E11F%2cd566f976b2c825e4ca410ee0754bcf2b%22%7d; u_co_name=%e6%ad%a6%e6%b1%89%e5%b0%8f%e5%b8%83%e7%94%b5%e5%ad%90%e5%95%86%e5%8a%a1%e6%9c%89%e9%99%90%e5%85%ac%e5%8f%b8; v_d_144=1715496538498_f488932826196e289944b013be36a727; u_cid=133599701439643594; u_sso_token=CS@e1903f92c5c7459fbbe381ba85d75c00; u_id=15424700; u_co_id=10174711; p_50=5DA09A8DA5EF6EC4DE5BE6D6A0231599638511221439646836%7c10174711; u_env=www'
+}
+'''
+  //生成唯一SessionCode
+  if (!$.cookie('SessionCode')) {
+    let guid = newJstTraceGuid();
+    $.cookie('SessionCode', guid);
+    params.SessionCode = guid;
+  }
+
+
+'''
```

## erp_apis/erpRequest.py

```diff
@@ -4,74 +4,105 @@
 # Author：李福成
 # Date ：2024-04-09 11:20
 # IDE：PyCharm
 import os
 from dataclasses import dataclass
 from typing import Optional
 from urllib.parse import urljoin
+
+import requests
 from lxml import etree
 from requests import Session as S, Request as Req, Response as Res
 import time, json as j
-from erp_apis.config import DEFAULT_HEADERS, Erp321BaseUrl, ErpApiBaseUrl
+from erp_apis.config import DEFAULT_HEADERS, Erp321BaseUrl, ErpApiBaseUrl, ErpGoodsBaseUrl
 
 
 @dataclass
 class UserInfoType:
     u_cid: Optional[str]
     u_co_id: Optional[str]
     u_co_name: Optional[str]
     u_id: Optional[str]
     u_name: Optional[str]
     u_lid: Optional[str]
-    def __init__(self, **kwargs):pass
 
+    def __init__(self, **kwargs): pass
 
 
 class Session(S):
     def __init__(self):
         super().__init__()
         self.headers.update(DEFAULT_HEADERS)
         self.proxies = {'http': "", 'https': ""}
         self.viewstateItems = dict()
-        self.userInfo : Optional[UserInfoType]
-
+        self.userInfo: Optional[UserInfoType]
+        self.authorization = None
 
-
-    def erpSend(self, request:Req, **kwargs) -> Res:
-        if not request.headers: request.headers = self.headers
+    def erpSend(self, request: Req, **kwargs) -> Res:
+        if not request.headers: request.headers.update(self.headers)
         hostType = getattr(request, 'hostType', None)
         if hostType:
             resp = getattr(self, hostType + "Send", None)(request, **kwargs)
             if resp is None:
                 raise Exception(f"{hostType}没有这个域的send方法")
             return resp
         raise Exception('hostType is None')
 
-
     def erp321Send(self, request, **kwargs):
         request.url = urljoin(Erp321BaseUrl, request.url)
         if request.method == 'POST':
             request.headers.update({'Content-Type': 'application/x-www-form-urlencoded; charset=UTF-8'})
             request.data.update({k: v for k, v in self.get_viewstate(request.url).items() if k and k != "updateTime"})
+
         res = super().send(self.prepare_request(request), **kwargs)
+
         if request.callback:
             return request.callback(res)
         return res
 
-    def erpApiSend(self, request, **kwargs) :
+    def erpApiSend(self, request, **kwargs):
         request.url = urljoin(ErpApiBaseUrl, request.url)
         res = super().send(self.prepare_request(request), **kwargs)
         if request.callback:
             if request.callback == 'login':
                 if res.json().get('code') == 0:
                     self.userInfo = UserInfoType(**res.json().get('cookie'))
+                    # self.authorization = self.epaasJointLoginGyl().get('data').get('access_token')
+                else:
+                    raise Exception(res.json().get('msg'))
             else:
                 return request.callback(res)
         return res
 
+    def erpGoodsSend(self, request, **kwargs):
+        request.headers.update({
+             'accept': 'application/json',
+            'accept-language': 'zh-CN,zh;q=0.9',
+            'content-type': 'application/json',
+            'origin': 'https://goods.scm121.com',
+            'priority': 'u=1, i',
+            'referer': 'https://goods.scm121.com/manage/goods/goodsManage/index?eTicket=JQing6&f=erp&m=n&y=20220701&_c=jst-epaas&epaas=true&serviceKey=shop_goods',
+            'sec-ch-ua': '"Chromium";v="124", "Google Chrome";v="124", "Not-A.Brand";v="99"',
+            'sec-ch-ua-mobile': '?0',
+            'sec-ch-ua-platform': '"Windows"',
+            'sec-fetch-dest': 'empty',
+            'sec-fetch-mode': 'cors',
+            'sec-fetch-site': 'same-origin',
+            'source': 'SUPPLIER',
+            'user-agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36',
+
+        })
+        request.url = urljoin(ErpGoodsBaseUrl, request.url)
+        if self.authorization:
+            request.headers['Authorization'] = self.authorization
+
+
+        res = super().send(self.prepare_request(request), **kwargs)
+        return res
+
     def get_viewstate(self, url):
         if self.viewstateItems.get(url) and self.viewstateItems.get(url).get("updateTime") > time.time() - 60 * 5:
             return self.viewstateItems.get(url)
         if not self.viewstateItems.get(url):
             self.viewstateItems.update({url: {"updateTime": time.time()}})
         res = self.get(url)
         etree_xpath = etree.HTML(res.text)
@@ -85,18 +116,40 @@
                 "__VIEWSTATE": extract_first("//*[@id='__VIEWSTATE']/@value"),
                 "__VIEWSTATEGENERATOR": extract_first("//*[@id='__VIEWSTATEGENERATOR']/@value"),
                 "__EVENTVALIDATION": extract_first("//*[@id='__EVENTVALIDATION']/@value"),
             }
         )
         return self.viewstateItems.get(url)
 
+    # 获取Authorization
+    def epaasJointLoginGyl(self):
+        res = self.erpSend(Request(
+            method='post',
+            hostType='erpGoods',
+            url="/api/auth/open/epaasJointLoginGyl",
+            json={
+                "eTicket": "JQing6",
+                "serviceKey": "shop_goods"
+            }
+        ))
+        res = self.erpSend(Request(
+            method='post',
+            hostType='erpGoods',
+            url="/api/auth/open/epaasJointLoginGyl",
+            json={
+                "eTicket": "JQing6",
+                "serviceKey": "shop_goods"
+            }
+        ))
+        return res.json()
+
 
 class Request(Req):
 
     def __init__(self,
                  hostType: str = 'erp321',
-                 callback: callable=None,
+                 callback: callable = None,
                  **kwargs
-        ):
+                 ):
         self.hostType = hostType
         self.callback = callback
-        super().__init__(**kwargs)
+        super().__init__(**kwargs)
```

## erp_apis/apis/afterSales.py

```diff
@@ -73,20 +73,110 @@
             }
         ),
     },
         method='Confirms',
         url='/app/Service/aftersale/aftersale_common.aspx'
     )
 
+# 反确认售后订单
+def unconfirms(afterId):
+    '''
+    反确认售后订单
+    :param oid:  内部订单号
+    :return: 执行结果
+    '''
+    return AftersaleRequest({
+        'isCB': '0',
+        '__CALLBACKID': 'ACall1',
+        '__CALLBACKPARAM': dumps(
+            {
+                "Method": "UnConfirms",
+                "Args": [afterId],
+             "CallControl": "{page}"
+            }
+        ),
+    },
+        method='UnConfirms',
+        url='/app/Service/aftersale/aftersale_common.aspx'
+    )
+
+# 确认收到退货
+def confirmReturnQty(afterId):
+    '''
+    反确认售后订单
+    :param oid:  内部订单号
+    :return: 执行结果
+    '''
+    return AftersaleRequest({
+        'isCB': '0',
+        '__CALLBACKID': 'ACall1',
+        '__CALLBACKPARAM': dumps(
+            {
+                "Method": "ConfirmReturnQty",
+                "Args": [afterId],
+             "CallControl": "{page}"
+            }
+        ),
+    },
+        method='ConfirmReturnQty',
+        url='/app/Service/aftersale/aftersale_common.aspx'
+    )
+
+# 确认收到货物
+def confirmGoods(afterId):
+    '''
+    反确认售后订单
+    :param oid:  内部订单号
+    :return: 执行结果
+    '''
+    return AftersaleRequest({
+        'isCB': '0',
+        '__CALLBACKID': 'ACall1',
+        '__CALLBACKPARAM': dumps(
+            {
+                "Method": "ConfirmGoods",
+                "Args": [afterId],
+             "CallControl": "{page}"
+            }
+        ),
+    },
+        method='ConfirmGoods',
+        url='/app/Service/aftersale/aftersale_common.aspx'
+    )
+
+
+# 更新售后单 售后类型
+def save(update_order):
+    '''
+    反确认售后订单
+    :param oid:  内部订单号
+    :return: 执行结果
+    '''
+    return AftersaleRequest({
+        'isCB': '0',
+        '__CALLBACKID': 'JTable1',
+        '__CALLBACKPARAM': dumps(
+            {
+                "Method": "Save",
+                "Args": [update_order]
+            }
+        ),
+    },
+        method='Save',
+        url='/app/Service/aftersale/aftersale.aspx'
+    )
+
 
 # 售后单转转成
 def clearException(afterId: Union[str, int]):
     '''
     售后单转转成
     :param oid:  内部订单号
     :return: 执行结果
     '''
     return AftersaleRequest({
         '__CALLBACKID': 'JTable1',
         '__CALLBACKPARAM': dumps({"Method":"ClearException","Args":[afterId],"CallControl":"{page}"}),
     },
-        method='ClearException')
+        method='ClearException')
+
+
```

## erp_apis/apis/order.py

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 # Project：erp_out_of_stock
 # File：order.py
 # Author：李福成
 # Date ：2024-04-28 18:23
 # IDE：PyCharm
 # 订单API
-from typing import Optional, Union
+from typing import Optional, Union, List
 from erp_apis.erpRequest import Request
 from erp_apis.utils.util import dumps, getDefaultParams, JTable1, generateChangeBatchItems
 
 
 def OrderRequest(
         data: dict,
         method: str = 'LoadDataToJSON',
@@ -53,14 +53,34 @@
                     "{}"
                 ]
             }
         ),
     }, method='LoadDataToJSON')
 
 
+# 获取订单编码库存
+def OrderPickable(oid: int):
+    '''
+    获取订单
+    :param page_num: 页数
+    :param page_size:  每页条数
+    :param queryData:  查询条件
+    :return: 查询结果
+    '''
+    return OrderRequest({
+        '__CALLBACKPARAM': dumps(
+            {
+                "Method": "LoadOrderPickable",
+                "Args": [oid],
+                "CallControl": "{page}"
+            }
+        ),
+    }, method='LoadOrderPickable')
+
+
 # 修改订单异常类型
 def Questions(questionName: str, questionMsg: str, oid: Union[str, int]):
     '''
     修改订单异常类型
     :param questionName: 异常分类名称
     :param questionMsg:  异常信息
     :param oid:  内部订单号
@@ -113,15 +133,15 @@
             "CallControl": "{page}"
         }),
     },
         method='SaveAppendRemarks')
 
 
 # 换商品
-def ChangeBatchItems(oid: Union[str, int], items: list, newBatchItems: list[dict]):
+def ChangeBatchItems(oid: Union[str, int], items: list, newBatchItems: List[dict]):
     '''
     换商品
     :param oid:  内部订单号
     :param oldBatchItems:  旧商品
     :param newBatchItems:  新商品
     :return: 执行结果
     '''
```

## erp_apis/apis/test.py

```diff
@@ -1,25 +1,22 @@
 # coding: utf-8
 # Project：erp_out_of_stock
 # File：test.py
 # Author：李福成
 # Date ：2024-04-28 18:24
 # IDE：PyCharm
-from apis.inventory import WmsSkuStock
-from apis.order import OrderList, ChangeBatchItems, LogisticsInfo
+from erp_apis.apis.order import LogisticsInfo
 from erp_apis.apis.user import login
-from apis.afterSales import aftersaleList, aftersaleCommon, clearException
-from erp_apis.apis.goods import ItemList
 from erpRequest import Session
 
 if __name__ == '__main__':
     session = Session()
     session.erpSend(login(
-        username="18986660202",
-        password="lfc199968"
+        username="",
+        password=""
     ))
     # 获取分仓库存
     # order = session.erpSend(OrderList(queryData=[{"k": "o_id", "v": "39104496", "c": "@="}])).json()['ReturnValue']['datas'][0]
     # print(order)
     # res = session.erpSend(ChangeBatchItems(
     #     oid = order['o_id'],
     #     items = order['items'],
@@ -39,12 +36,16 @@
     # )
     # res = session.erpSend(aftersaleCommon(1452451077))
     # res = session.erpSend(clearException(1452451077))
 
     res = session.erpSend(LogisticsInfo(
         {
             "from": "aftersale",
-            "l_id": "78791674020636",
+            "l_id": "78795088342441",
             "l_name": "中通速递"
         }
     ))
-    print(res.json())
+    loginslist = [l['detail'] for l in res.json()['ReturnValue']]
+    if '当阳' in str(loginslist) or '宜昌' in str(loginslist):
+        print(loginslist)
+    print(loginslist)
+
```

## erp_apis/utils/util.py

```diff
@@ -4,49 +4,51 @@
 # Author：李福成
 # Date ：2024-04-29 9:35
 # IDE：PyCharm
 import json
 import time
 
 from requests import Response
+from typing import List
 
 
 def dumps(obj, **kwargs):
     return json.dumps(obj, **kwargs, separators=(',', ':'), ensure_ascii=False)
 
 
 def getDefaultParams(params: dict = None) -> dict:
     rand_params = {
         '_c': lambda: 'jst-epaas',
         '_t': lambda: int(time.time() * 1000),
         '_float': lambda: True,
         'ts___': lambda: int(time.time() * 1000),
         'am___': lambda: 'LoadDataToJSON',
-        'owner_co_id' : lambda: 1
+        'owner_co_id' : lambda: 1,
+        'authorize_co_id' : lambda: 1
     }
     if params.get('defaultParams'):
         for k in params.get('defaultParams'):
             params.update({k: rand_params.get(k)()})
     del params['defaultParams']
     return params
 
 
 def JTable1(res: Response):
-    print(res.text)
-    res_data = json.loads(res.text[2:])
+    text = res.text
+    res_data = json.loads(text[text.find('{'):])
     if res_data.get('ReturnValue'):
         try:res_data['ReturnValue'] = json.loads(res_data.get('ReturnValue'))
         except:pass
     res._content = json.dumps(res_data).encode('utf-8')
     return res
 
 
 
 
-def generateChangeBatchItems(items: list, newBatchItems: list[dict]):
+def generateChangeBatchItems(items: list, newBatchItems: List[dict]):
     new_items = []
     newBatchItems_to_dict = {i['oi_id']: i for i in newBatchItems}
     for sku in items:
         if sku['oi_id'] not in newBatchItems_to_dict: continue
         new_items.extend([{
             **{k: sku[k] for k in ['is_gift', 'qty']},
             "price": -99999,
```

## Comparing `erp_apis-1.0.8.dist-info/METADATA` & `erp_apis-1.2.11.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erp-apis
-Version: 1.0.8
+Version: 1.2.11
 Summary: erp_apis
 Home-page: https://gitee.com/li_fucheng/erp_sdk_python
 Author: 李福成
 Author-email: lfct@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://gitee.com/li_fucheng/erp_sdk_python/issues
 Project-URL: Documentation, https://gitee.com/li_fucheng/erp_sdk_python
```

## Comparing `erp_apis-1.0.8.dist-info/RECORD` & `erp_apis-1.2.11.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,19 @@
-erp_apis/config.py,sha256=tXtGQtsW-Wdbhh2X1AKyGx_X8B_ShMvdVF4rOXf8zDg,403
-erp_apis/erpRequest.py,sha256=RDCcdYiW7doHGZBoIRG97WSXg7suuIKoZSlgy9FMCMQ,3577
+erp_apis/config.py,sha256=7AfOc0rdICRcfSmXHOnRrFT4KYA8QgOrTmpgFZ7EEMM,2374
+erp_apis/erpRequest.py,sha256=rerA7L-knMpbuJPDU7xJHgE7jRC66pW-bY9_SYcy3Ek,5734
+erp_apis/apis/ItemApi.py,sha256=poIcNB7Ve2k324InU0Ggf4pidaAkTODGTAoOGBCX5Qg,1062
+erp_apis/apis/Print.py,sha256=3s8B37fT60x2qnKzgmAaO5rgnekVl_fq9pBmX4ShD8k,4597
 erp_apis/apis/__init__.py,sha256=L6HaO-zN2-mMbaZUFJ8YFFgFScFE4aizJCVPed8CluY,143
-erp_apis/apis/afterSales.py,sha256=biTQql3R1JgOS4fluuOT76F40Fu3KA8KggmLYrE68as,2587
+erp_apis/apis/afterSales.py,sha256=gS3Ck9XiYVx9yiXfV2hYEuxJdXo5to1Vl9JsgXNg_qc,4743
 erp_apis/apis/goods.py,sha256=3HplLv-feqNMiV46ANuzhRfL9RDiOovF8RAAvNydmdI,1538
 erp_apis/apis/inventory.py,sha256=ktCBMrKRdHKSOKZIgCCWan0cTYNKm-ddpFNe1hkxgGk,1013
-erp_apis/apis/order.py,sha256=ybUJ8i1oSsu9TfP4HE99HFk8sbiO8qWy4f8ssdBFzM0,4346
-erp_apis/apis/test.py,sha256=ZrR-jcO6S6xGulPVMoVdAr7RAAyuuCux9UhGto2viZc,2091
+erp_apis/apis/order.py,sha256=7-SkxpBRPdmhJVMd1n4jBfg76q9DWgL-ALgbklWVVSE,4841
+erp_apis/apis/refund.py,sha256=oUvhwQ3JOj-0XS2DZDPEfZWtJGVFtXty0CcpRMd9_B4,3093
+erp_apis/apis/shopData.py,sha256=EBhVWQWizQuFmrPumK5r4kc_dlstRWbeS17ongU8Fqo,3094
+erp_apis/apis/test.py,sha256=aRAff6YG0a8GHhJhYUiywmZcvD-IYPP4fUOpARabtw0,2057
 erp_apis/apis/user.py,sha256=vosgBp1QNesLIRMQyafe9y9PDFJyIjpPdmiE1jvVzOA,1139
 erp_apis/utils/__init__.py,sha256=4OS0q-GbgI0b14i4ErUYKUo-t1jzw8wSvtJZu3nXSMM,141
-erp_apis/utils/util.py,sha256=xkmwXqGWbh7Qz_rRtXk5BclnvQz8PgMaS73UpR-Fm4s,2063
-erp_apis-1.0.8.dist-info/METADATA,sha256=7CqHa7TXkoBoLldT-L-MESKiUAJzcD_Vma36fdKt264,1580
-erp_apis-1.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-erp_apis-1.0.8.dist-info/top_level.txt,sha256=vqDQIzqoC9jLUmJwUdHu1qRTGhYD1SxQ5BsetWAnMrs,38
-erp_apis-1.0.8.dist-info/RECORD,,
+erp_apis/utils/util.py,sha256=TMU0DowoXgoEdBjqbxue2Mb7KennGe_n_ZzRpZ23Adg,2137
+erp_apis-1.2.11.dist-info/METADATA,sha256=xQEJbyIhmBOhJzDNMuIy4M7Szq6cMvMtJvLcbEG8YCU,1581
+erp_apis-1.2.11.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+erp_apis-1.2.11.dist-info/top_level.txt,sha256=vqDQIzqoC9jLUmJwUdHu1qRTGhYD1SxQ5BsetWAnMrs,38
+erp_apis-1.2.11.dist-info/RECORD,,
```

