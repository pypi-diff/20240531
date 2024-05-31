# Comparing `tmp/wxhandler-0.1.1.3.tar.gz` & `tmp/wxhandler-0.1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wxhandler-0.1.1.3.tar", last modified: Fri May 31 00:22:14 2024, max compression
+gzip compressed data, was "wxhandler-0.1.1.5.tar", last modified: Fri May 31 03:07:43 2024, max compression
```

## Comparing `wxhandler-0.1.1.3.tar` & `wxhandler-0.1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 00:22:14.058710 wxhandler-0.1.1.3/
--rw-rw-rw-   0        0        0     1055 2024-05-30 23:10:26.000000 wxhandler-0.1.1.3/LICENSE
--rw-rw-rw-   0        0        0      890 2024-05-31 00:22:14.057710 wxhandler-0.1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      402 2024-05-31 00:22:08.000000 wxhandler-0.1.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-31 00:22:14.059709 wxhandler-0.1.1.3/setup.cfg
--rw-rw-rw-   0        0        0      680 2024-05-31 00:20:58.000000 wxhandler-0.1.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:22:14.042839 wxhandler-0.1.1.3/wxhandler/
--rw-rw-rw-   0        0        0       61 2024-05-31 00:11:00.000000 wxhandler-0.1.1.3/wxhandler/__init__.py
--rw-rw-rw-   0        0        0    23197 2024-05-30 15:38:25.000000 wxhandler-0.1.1.3/wxhandler/wxhandler.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:22:14.055713 wxhandler-0.1.1.3/wxhandler.egg-info/
--rw-rw-rw-   0        0        0      890 2024-05-31 00:22:13.000000 wxhandler-0.1.1.3/wxhandler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-05-31 00:22:13.000000 wxhandler-0.1.1.3/wxhandler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 00:22:13.000000 wxhandler-0.1.1.3/wxhandler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-31 00:22:13.000000 wxhandler-0.1.1.3/wxhandler.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-31 00:22:13.000000 wxhandler-0.1.1.3/wxhandler.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 03:07:43.550536 wxhandler-0.1.1.5/
+-rw-rw-rw-   0        0        0     1055 2024-05-30 23:10:26.000000 wxhandler-0.1.1.5/LICENSE
+-rw-rw-rw-   0        0        0     1008 2024-05-31 03:07:43.548536 wxhandler-0.1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      520 2024-05-31 03:05:48.000000 wxhandler-0.1.1.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-31 03:07:43.550536 wxhandler-0.1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      680 2024-05-31 03:06:23.000000 wxhandler-0.1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:07:43.532635 wxhandler-0.1.1.5/wxhandler/
+-rw-rw-rw-   0        0        0       73 2024-05-31 02:02:03.000000 wxhandler-0.1.1.5/wxhandler/__init__.py
+-rw-rw-rw-   0        0        0    43310 2024-05-31 03:01:47.000000 wxhandler-0.1.1.5/wxhandler/wxhandler.py
+drwxrwxrwx   0        0        0        0 2024-05-31 03:07:43.547536 wxhandler-0.1.1.5/wxhandler.egg-info/
+-rw-rw-rw-   0        0        0     1008 2024-05-31 03:07:43.000000 wxhandler-0.1.1.5/wxhandler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2024-05-31 03:07:43.000000 wxhandler-0.1.1.5/wxhandler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 03:07:43.000000 wxhandler-0.1.1.5/wxhandler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-31 03:07:43.000000 wxhandler-0.1.1.5/wxhandler.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-31 03:07:43.000000 wxhandler-0.1.1.5/wxhandler.egg-info/top_level.txt
```

### Comparing `wxhandler-0.1.1.3/LICENSE` & `wxhandler-0.1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wxhandler-0.1.1.3/setup.py` & `wxhandler-0.1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="wxhandler",
-    version="0.1.1.3",
+    version="0.1.1.5",
     packages=find_packages(),
     install_requires=[
         "requests",
     ],
     author="chenbifu",
     author_email="pythonaaa@gmail.com",
     description="A Python package for handling wxHandler operations.",
```

### Comparing `wxhandler-0.1.1.3/wxhandler/wxhandler.py` & `wxhandler-0.1.1.5/wxhandler/wxhandler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ﻿import requests
 import json
 
-# 微信版本大于或等于3.9.5.81
+# 微信版本3.9.2.23
 class wxHandler:
     def __init__(self, base_url):
         self.base_url = base_url
 
     # 0.检查微信登录**
     def checkLogin(self):
         url = f"{self.base_url}/api/?type=0"
@@ -31,15 +31,15 @@
             "wxid": wxid,
             "msg": msg
         })
         headers = {
             'Content-Type': 'application/json'
         }
         response = requests.request("POST", url, headers=headers, data=payload)
-        print(response.text)
+        # print(response.text)
         return response.json()
    
     # 3.发送@文本消息**
     def sendAtText(self, wxids, chatRoomId, msg):
         print("modify wxids  chatRoomId")
         raise RuntimeError("modify wxids   chatRoomId then deleted me")
         url = f"{self.base_url}/api/?type=3"
@@ -88,32 +88,16 @@
         headers = {
             'Content-Type': 'application/json'
         }
         response = requests.request("POST", url, headers=headers, data=payload)
         print(response.text)
         return response.json()
 
-    # 9.hook消息** 
-    def hookSyncMsg(self, port="19099", ip="127.0.0.1"):
-        url = f"{self.base_url}/api/?type=9"
-        print("modify ip port url ")
-        raise RuntimeError("modify ip port url then deleted me")
-        payload = {
-            "port": port, # 本地服务端端口，用来接收消息内容
-            "ip": ip # 服务端ip地址，用来接收消息内容，可以是任意ip,即tcp客户端连接的服务端的ip (3.8.1.26版本)
-        }
-        headers = {
-            'Content-Type': 'application/json'
-        }
-        response = requests.request("POST", url, headers=headers, data=payload)
-        print(response.text)
-        return response.json()
-    
     # 9.hook消息** (新特性)
-    def hookSyncMsgNew(self, enableHttp, httpPort):
+    def hookSyncMsg(self, enableHttp, httpPort):
         # 定义要发送的数据
         data = {
             "port": "19099",
             "ip": "127.0.0.1",
             "url": f"http://127.0.0.1:{httpPort}",
             "timeout": "3000",
             "enableHttp": bool(enableHttp) # True HTTP专用 | False TCP专用
@@ -125,14 +109,15 @@
             if data["enableHttp"] == True:
                 notice = f' * hook启动成功。文本消息将转发到http服务：{data["url"]}'
             else:
                 notice = ' * hook启动成功。文本消息将转发到TCP服务'
         else:
             notice = ' * hook启动失败。文本消息转发设置失败'
         print(notice)
+        return notice
     
 
     # 10.取消hook消息**
     def unhookSyncMsg(self):
         url = f"{self.base_url}/api/?type=10"
         payload = {}
         headers = {}
@@ -624,9 +609,626 @@
 
         response = requests.request("POST", url, headers=headers, data=payload)
 
         print(response.text)
         return response.json()
 
     
+ # 微信版本3.9.2.23   
+
+# 微信版本大于或等于3.9.5.81本例使用3.9.8.25
+class wxHandler1:
+    def __init__(self, base_url):
+        self.base_url = base_url
+
+    # 0.检查微信登录**
+    def checkLogin(self):
+        url = f"{self.base_url}/api/checkLogin"
+        payload = {}
+        headers = {}
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 1.获取登录用户信息**
+    def userInfo(self):
+        url = f"{self.base_url}/api/userInfo"
+        payload = {}
+        headers = {}
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 2.发送文本消息**
+    def sendTextMsg(self, wxid, msg):
+        url = f"{self.base_url}/api/sendTextMsg"
+        payload = json.dumps({
+            "wxid": wxid,
+            "msg": msg
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 3.hook消息**
+    def hookSyncMsg(self, enableHttp, httpPort):
+        url = f"{self.base_url}/api/hookSyncMsg"
+        # 定义要发送的数据
+        data = {
+            "port": "19099",
+            "ip": "127.0.0.1",
+            "url": f"http://127.0.0.1:{httpPort}",
+            "timeout": "3000",
+            "enableHttp": bool(enableHttp) # 直接使用转换后的布尔值
+        }
+        
+        # 使用 json 参数传递 JSON 数据
+        response = requests.post(url, json=data)
+        if response.json()["msg"] == "success":  # 使用 .json() 方法来解析响应的 JSON 数据
+            if data["enableHttp"] == True:
+                notice = f'文本消息将转发到http服务：{data["url"]}'
+            else:
+                notice = '文本消息将转发到TCP服务'
+        else:
+            notice = '文本消息转发设置失败'
+        print(f'{notice}\n{response.text}')
+
+    # 4.取消hook消息**
+    def unhookSyncMsg(self):
+        url = f"{self.base_url}/api/unhookSyncMsg"
+        payload = {}
+        headers = {}
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 5.好友列表**
+    def getContactList(self):
+        url = f"{self.base_url}/api/getContactList"
+        payload = {}
+        headers = {}
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 6.获取数据库信息**
+    def getDBInfo(self):
+        url = f"{self.base_url}/api/getDBInfo"
+        payload = {}
+        headers = {}
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 7.查询数据库**
+    def execSql(self, dbHandle:int, sql):
+        url = f"{self.base_url}/api/execSql"
+        print("modify dbHandle ")
+        raise RuntimeError("modify dbHandle then deleted me")
+        payload = json.dumps({
+            "dbHandle": dbHandle,
+            "sql": sql
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 8.发送文件消息**
+    def sendFileMsg(self, wxid, filePath):
+        url = f"{self.base_url}/api/sendFileMsg"
+        print("modify filePath")
+        raise RuntimeError("modify filePath then deleted me")
+        payload = json.dumps({
+            "wxid": wxid,
+            "filePath": filePath
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    #9.获取群详情**
+    def getChatRoomDetailInfo(self, chatRoomId):
+        url = f"{self.base_url}/api/getChatRoomDetailInfo"
+        print("modify chatRoomId ")
+        raise RuntimeError("modify chatRoomId then deleted me")
+        payload = json.dumps({
+            "chatRoomId": chatRoomId
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 10.添加群成员**
+    def addMemberToChatRoom(self, chatRoomId, memberIds):
+        url = f"{self.base_url}/api/addMemberToChatRoom"
+        print("modify chatRoomId  memberIds ")
+        raise RuntimeError("modify chatRoomId memberIds then deleted me")
+        payload = json.dumps({
+            "chatRoomId": chatRoomId,
+            "memberIds": memberIds # string 成员id，多个用,分隔
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()
+
+    # 12.删除群成员**
+    def delMemberFromChatRoom(self, chatRoomId, memberIds):
+        url = f"{self.base_url}/api/delMemberFromChatRoom"
+        print("modify chatRoomId  memberIds ")
+        raise RuntimeError("modify chatRoomId memberIds then deleted me")
+        payload = json.dumps({
+            "chatRoomId": chatRoomId,
+            "memberIds": memberIds # string 成员id，多个用,分隔
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 11.修改群昵称**
+    def modifyNickname(self, chatRoomId, wxid, nickName):
+        url = f"{self.base_url}/api/modifyNickname"
+        print("modify chatRoomId  wxid  nickName")
+        raise RuntimeError("modify chatRoomId  wxid  nickName then deleted me")
+        payload = json.dumps({
+            "chatRoomId": chatRoomId,
+            "wxid": wxid,
+            "nickName": nickName
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 13.获取群成员**
+    def getMemberFromChatRoom(self, chatRoomId):
+        print("modify chatRoomId  ")
+        raise RuntimeError("modify chatRoomId then deleted me")
+        url = f"{self.base_url}/api/getMemberFromChatRoom"
+        payload = json.dumps({
+            "chatRoomId": chatRoomId
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 14.置顶群消息**
+    def topMsg(self, msgId:int):
+        print("modify msgId  ")
+        raise RuntimeError("modify msgId then deleted me")
+        url = f"{self.base_url}/api/topMsg"
+        payload = json.dumps({
+            "msgId": msgId
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 15.移除置顶群消息**
+    def removeTopMsg(self, chatRoomId, msgId:int):
+        print("modify msgId chatRoomId ")
+        raise RuntimeError("modify msgId chatRoomId then deleted me")
+
+        url = f"{self.base_url}/api/removeTopMsg"
+
+        payload = json.dumps({
+            "chatRoomId": chatRoomId,
+            "msgId": msgId
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 16.邀请入群**
+    def InviteMemberToChatRoom(self, chatRoomId, memberIds):
+        print("modify memberIds chatRoomId ")
+        raise RuntimeError("modify memberIds chatRoomId then deleted me")
+
+        url = f"{self.base_url}/api/InviteMemberToChatRoom"
+
+        payload = json.dumps({
+            "chatRoomId": chatRoomId,
+            "memberIds": memberIds # wxid，用,分隔
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 17.hook日志**
+    def hookLog(self):
+        url = f"{self.base_url}/api/hookLog"
+        payload = {}
+        headers = {}
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 18.取消hook日志**
+    def unhookLog(self):
+        url = f"{self.base_url}/api/unhookLog"
+        payload = {}
+        headers = {}
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 19.建群**
+    def createChatRoom(self, memberIds):
+        print("modify memberIds  ")
+        raise RuntimeError("modify memberIds then deleted me")
+        url = f"{self.base_url}/api/createChatRoom"
+
+        payload = json.dumps({
+            "memberIds": memberIds # string 群成员id，以,分割
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 20.退群**
+    def quitChatRoom(self, chatRoomId):
+        print("modify chatRoomId  ")
+        raise RuntimeError("modify chatRoomId then deleted me")
+        url = f"{self.base_url}/api/quitChatRoom"
+
+        payload = json.dumps({
+            "chatRoomId": chatRoomId
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+    
+    # 21.转发消息**
+    def forwardMsg(self, wxid, msgId:str):
+        print("modify msgId  ")
+        raise RuntimeError("modify msgId then deleted me")
+        url = f"{self.base_url}/api/forwardMsg"
+
+        payload = json.dumps({
+            "wxid": wxid,
+            "msgId": msgId
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+    
+    # 22.朋友圈首页**
+    def getSNSFirstPage(self):
+        url = f"{self.base_url}/api/getSNSFirstPage"
+
+        payload = {}
+        headers = {}
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+    
+    # 23.朋友圈下一页**
+    def getSNSNextPage(self, snsId):
+        print("modify snsId  ")
+        raise RuntimeError("modify snsId then deleted me")
+        url = f"{self.base_url}/api/getSNSNextPage"
+
+        payload = json.dumps({
+            "snsId": snsId
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()
+    
+    # 24.收藏消息**
+    def addFavFromMsg(self, msgId):
+        print("modify msgId  ")
+        raise RuntimeError("modify msgId then deleted me")
+        url = f"{self.base_url}/api/addFavFromMsg"
+
+        payload = json.dumps({
+            "msgId": msgId
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()
+        
+    # 24.收藏图片**    
+    def addFavFromImage(self, wxid, imagePath):
+        print("modify wxid imagePath ")
+        raise RuntimeError("modify wxid  imagePath then deleted me")
+        url = f"{self.base_url}/api/addFavFromImage"
+
+        payload = json.dumps({
+            "wxid": wxid,
+            "imagePath": imagePath
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()
+
+    # 26.获取群成员信息**
+    def getContactProfile(self, wxid):
+        print("modify wxid  ")
+        raise RuntimeError("modify wxid   then deleted me")
+        url = f"{self.base_url}/api/getContactProfile"
+
+        payload = json.dumps({
+            "wxid": wxid
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+        print(response.text)
+        return response.json()
+
+    # 25.发送@消息**
+    def sendAtText(self, wxids, chatRoomId, msg):
+        print("modify wxids  chatRoomId")
+        raise RuntimeError("modify wxids   chatRoomId then deleted me")
+        url = f"{self.base_url}/api/sendAtText"
+
+        payload = json.dumps({
+            "wxids": wxids,
+            "chatRoomId": chatRoomId,
+            "msg": msg
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()
+
+    # 27.发送公众号消息**
+    def forwardPublicMsg(self, appName, userName, title, url, thumbUrl, digest, wxid):
+        print("modify param ")
+        raise RuntimeError("modify param then deleted me")
+        url = f"{self.base_url}/api/forwardPublicMsg"
+
+        payload = json.dumps({
+            "appName": appName, # 公众号id，消息内容里的appname
+            "userName": userName, # 公众号昵称，消息内容里的username
+            "title": title, # 链接地址，消息内容里的title
+            "url": url, # 链接地址，消息内容里的url
+            "thumbUrl": thumbUrl, # 缩略图地址，消息内容里的thumburl
+            "digest": digest, # 摘要，消息内容里的digest
+            "wxid": wxid # 	wxid
+        })
+        headers = {
+        'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()
+
+    # 28.转发公众号消息**
+    def forwardPublicMsgByMsgId(self, msgId:int, wxid):
+        print("modify param ")
+        raise RuntimeError("modify param then deleted me")
+        url = f"{self.base_url}/api/forwardPublicMsgByMsgId"
+
+        payload = json.dumps({
+            "msgId": msgId,
+            "wxid": wxid
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()
+
+    # 29.下载附件**
+    def downloadAttach(self, msgId:int):
+        print("modify param ")
+        raise RuntimeError("modify param then deleted me")
+        url = f"{self.base_url}/api/downloadAttach"
+
+        payload = json.dumps({
+            "msgId": msgId
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()
+
+    # 30.解码图片**
+    def decodeImage(self, filePath, storeDir):
+        print("modify param ")
+        raise RuntimeError("modify param then deleted me")
+        url = f"{self.base_url}/api/decodeImage"
+
+        payload = json.dumps({
+            "filePath": filePath, # 待解码图片地址 "C:\\66664816980131.dat",
+            "storeDir": storeDir # 解码后图片的存储目录 "C:\\test"
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()
+
+    # 31.获取语音**
+    def getVoiceByMsgId(self, msgId:int, storeDir):
+        print("modify param ")
+        raise RuntimeError("modify param then deleted me")
+        url = f"{self.base_url}/api/getVoiceByMsgId"
+
+        payload = json.dumps({
+            "msgId": msgId,
+            "storeDir": storeDir # 语音的存储目录 "c:\\test"
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()
+
+    # 32.发送图片**
+    def sendImagesMsg(self, wxid, imagePath):
+        url = f"{self.base_url}/api/sendImagesMsg"
+        print("modify imagePath")
+        raise RuntimeError("modify imagePath then deleted me")
+        payload = json.dumps({
+            "wxid": wxid,
+            "imagePath": imagePath
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()
+
+    # 33.发送自定义表情**
+    def sendCustomEmotion(self, wxid, filePath):
+        url = f"{self.base_url}/api/sendCustomEmotion"
+        print("modify filePath")
+        raise RuntimeError("modify filePath then deleted me")
+        payload = json.dumps({
+            "wxid": wxid,
+            "filePath": filePath
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()
     
+    # 34.发送小程序**
+    def sendApplet(self, wxid, waidConcat, appletWxid, jsonParam, headImgUrl, mainImg, indexPage):
+        url = f"{self.base_url}/api/sendApplet"
+        print("modify sendApplet")
+        raise RuntimeError("modify sendApplet then deleted me")
+        payload = json.dumps({
+            "wxid": wxid, # 接收人wxid
+            "waidConcat": waidConcat, # app的wxid与回调信息之类绑定的拼接字符串，伪造的数据可以随意
+            "appletWxid": appletWxid, # app的wxid
+            "jsonParam": jsonParam, # 相关参数
+            "headImgUrl": headImgUrl, # 头像url
+            "mainImg": mainImg, # 主图的本地路径,需要在小程序的临时目录下
+            "indexPage": indexPage # 小程序的跳转页面
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()
+    
+    # 35.拍一拍**
+    def sendPatMsg(self, wxid, receiver):
+        url = f"{self.base_url}/api/sendPatMsg"
+        print("modify receiver")
+        raise RuntimeError("modify receiver then deleted me")
+        payload = json.dumps({
+            "wxid": wxid,
+            "filePath": receiver # 接收人id，可以是自己wxid，私聊好友wxid，群id
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()
+   
+    # 36.OCR**
+    def ocr(self, imagePath):
+        url = f"{self.base_url}/api/ocr"
+        print("modify receiver")
+        raise RuntimeError("modify receiver then deleted me")
+        payload = json.dumps({
+            "imagePath": imagePath # 图片全路径
+        })
+        headers = {
+            'Content-Type': 'application/json'
+        }
+
+        response = requests.request("POST", url, headers=headers, data=payload)
+
+        print(response.text)
+        return response.json()   
+ 
+
+
```

