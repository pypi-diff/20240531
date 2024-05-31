# Comparing `tmp/blockmango-1.4.7.tar.gz` & `tmp/blockmango-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockmango-1.4.7.tar", last modified: Wed May 29 08:14:30 2024, max compression
+gzip compressed data, was "blockmango-1.4.8.tar", last modified: Fri May 31 21:20:42 2024, max compression
```

## Comparing `blockmango-1.4.7.tar` & `blockmango-1.4.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-29 08:14:30.769675 blockmango-1.4.7/
--rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.7/LICENSE.md
--rw-------   0 userland  (2000) userland  (2000)     1703 2024-05-29 08:14:30.765675 blockmango-1.4.7/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      571 2024-05-28 23:52:58.000000 blockmango-1.4.7/README.md
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-29 08:14:30.749675 blockmango-1.4.7/blockmango/
--rw-------   0 userland  (2000) userland  (2000)      200 2024-05-17 15:51:17.000000 blockmango-1.4.7/blockmango/__init__.py
--rw-------   0 userland  (2000) userland  (2000)     4177 2024-05-28 20:15:07.000000 blockmango-1.4.7/blockmango/clan.py
--rw-------   0 userland  (2000) userland  (2000)     1336 2024-05-28 20:16:13.000000 blockmango-1.4.7/blockmango/decoration.py
--rw-------   0 userland  (2000) userland  (2000)     2231 2024-05-28 20:15:48.000000 blockmango-1.4.7/blockmango/friends.py
--rw-------   0 userland  (2000) userland  (2000)     3520 2024-05-28 20:20:04.000000 blockmango-1.4.7/blockmango/groupchat.py
--rw-------   0 userland  (2000) userland  (2000)     1225 2024-05-28 20:20:42.000000 blockmango-1.4.7/blockmango/http.py
--rw-------   0 userland  (2000) userland  (2000)     2105 2024-05-28 20:19:37.000000 blockmango-1.4.7/blockmango/user.py
-drwx------   0 userland  (2000) userland  (2000)        0 2024-05-29 08:14:30.765675 blockmango-1.4.7/blockmango.egg-info/
--rw-------   0 userland  (2000) userland  (2000)     1703 2024-05-29 08:14:30.000000 blockmango-1.4.7/blockmango.egg-info/PKG-INFO
--rw-------   0 userland  (2000) userland  (2000)      349 2024-05-29 08:14:30.000000 blockmango-1.4.7/blockmango.egg-info/SOURCES.txt
--rw-------   0 userland  (2000) userland  (2000)        1 2024-05-29 08:14:30.000000 blockmango-1.4.7/blockmango.egg-info/dependency_links.txt
--rw-------   0 userland  (2000) userland  (2000)        9 2024-05-29 08:14:30.000000 blockmango-1.4.7/blockmango.egg-info/requires.txt
--rw-------   0 userland  (2000) userland  (2000)       11 2024-05-29 08:14:30.000000 blockmango-1.4.7/blockmango.egg-info/top_level.txt
--rw-------   0 userland  (2000) userland  (2000)       38 2024-05-29 08:14:30.769675 blockmango-1.4.7/setup.cfg
--rw-------   0 userland  (2000) userland  (2000)     1474 2024-05-29 08:14:07.000000 blockmango-1.4.7/setup.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-31 21:20:42.706502 blockmango-1.4.8/
+-rw-------   0 userland  (2000) userland  (2000)     1061 2024-05-16 17:46:17.000000 blockmango-1.4.8/LICENSE.md
+-rw-------   0 userland  (2000) userland  (2000)     1703 2024-05-31 21:20:42.706502 blockmango-1.4.8/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      571 2024-05-28 23:52:58.000000 blockmango-1.4.8/README.md
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-31 21:20:42.682502 blockmango-1.4.8/blockmango/
+-rw-------   0 userland  (2000) userland  (2000)      200 2024-05-17 15:51:17.000000 blockmango-1.4.8/blockmango/__init__.py
+-rw-------   0 userland  (2000) userland  (2000)     4610 2024-05-31 21:16:46.000000 blockmango-1.4.8/blockmango/clan.py
+-rw-------   0 userland  (2000) userland  (2000)      690 2024-05-31 21:17:43.000000 blockmango-1.4.8/blockmango/config.py
+-rw-------   0 userland  (2000) userland  (2000)     1325 2024-05-31 21:14:55.000000 blockmango-1.4.8/blockmango/decoration.py
+-rw-------   0 userland  (2000) userland  (2000)     2443 2024-05-31 21:15:54.000000 blockmango-1.4.8/blockmango/friends.py
+-rw-------   0 userland  (2000) userland  (2000)     3520 2024-05-28 20:20:04.000000 blockmango-1.4.8/blockmango/groupchat.py
+-rw-------   0 userland  (2000) userland  (2000)     1225 2024-05-28 20:20:42.000000 blockmango-1.4.8/blockmango/http.py
+-rw-------   0 userland  (2000) userland  (2000)     2036 2024-05-31 21:12:48.000000 blockmango-1.4.8/blockmango/user.py
+drwx------   0 userland  (2000) userland  (2000)        0 2024-05-31 21:20:42.698502 blockmango-1.4.8/blockmango.egg-info/
+-rw-------   0 userland  (2000) userland  (2000)     1703 2024-05-31 21:20:42.000000 blockmango-1.4.8/blockmango.egg-info/PKG-INFO
+-rw-------   0 userland  (2000) userland  (2000)      370 2024-05-31 21:20:42.000000 blockmango-1.4.8/blockmango.egg-info/SOURCES.txt
+-rw-------   0 userland  (2000) userland  (2000)        1 2024-05-31 21:20:42.000000 blockmango-1.4.8/blockmango.egg-info/dependency_links.txt
+-rw-------   0 userland  (2000) userland  (2000)        9 2024-05-31 21:20:42.000000 blockmango-1.4.8/blockmango.egg-info/requires.txt
+-rw-------   0 userland  (2000) userland  (2000)       11 2024-05-31 21:20:42.000000 blockmango-1.4.8/blockmango.egg-info/top_level.txt
+-rw-------   0 userland  (2000) userland  (2000)       38 2024-05-31 21:20:42.706502 blockmango-1.4.8/setup.cfg
+-rw-------   0 userland  (2000) userland  (2000)     1474 2024-05-31 21:20:14.000000 blockmango-1.4.8/setup.py
```

### Comparing `blockmango-1.4.7/LICENSE.md` & `blockmango-1.4.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.7/PKG-INFO` & `blockmango-1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockmango
-Version: 1.4.7
+Version: 1.4.8
 Summary: Blockman Go API package
 Home-page: https://github.com/darkkpy/blockmango
 Author: Dark
 Author-email: darkness0777@proton.me
 License: MIT
 Project-URL: Documentation, https://github.com/darkkpy/blockmango/tree/main/docs
 Project-URL: Source, https://github.com/darkkpy/blockmango
```

### Comparing `blockmango-1.4.7/README.md` & `blockmango-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.7/blockmango/clan.py` & `blockmango-1.4.8/blockmango/clan.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,81 +1,84 @@
+# clan.py
 from .http import HTTPMixin
-
-BASE_URL = "http://modsgs.sandboxol.com/clan/api/v1/clan"
-BASE_URL_V2 = "http://modsgs.sandboxol.com/clan/api/v2/clan"
-BASE_URL_V3 = "http://modsgs.sandboxol.com/clan/api/v3/clan"
+from .config import BASE_URL_CLAN, BASE_URL_CLAN_V2, BASE_URL_CLAN_V3
 
 class Clan(HTTPMixin):
-  def __init__(self, user_id, access_token):
-    self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1"}
+    __slots__ = ("headers",)
+    base_url_clan = BASE_URL_CLAN
+    base_url_clan_v2 = BASE_URL_CLAN_V2
+    base_url_clan_v3 = BASE_URL_CLAN_V3
+
+    def __init__(self, user_id, access_token):
+        self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1"}
 
-  def user_clan(self):
-    return self._get(f"{BASE_URL}/tribe/base", headers=self.headers)
+    def user_clan(self):
+        return self._get(f"{self.base_url_clan}/tribe/base", headers=self.headers)
 
-  def join(self, clan_id):
-    return self._post(f"{BASE_URL}/tribe/member", headers=self.headers, json={"clanId": clan_id, "msg": ""})
+    def join(self, clan_id):
+        return self._post(f"{self.base_url_clan}/tribe/member", headers=self.headers, json={"clanId": clan_id, "msg": ""})
 
-  def leave(self, clan_id):
-    return self._delete(f"{BASE_URL}/tribe/member", headers=self.headers, params={"clanId": clan_id})
+    def leave(self, clan_id):
+        return self._delete(f"{self.base_url_clan}/tribe/member", headers=self.headers, params={"clanId": clan_id})
 
-  def search(self, clan_name, page_no=0, page_size=20):
-    return self._get(f"{BASE_URL}/tribe/blurry/info", headers=self.headers, params={"clanName": clan_name, "pageNo": page_no, "pageSize": page_size})
+    def search(self, clan_name, page_no=0, page_size=20):
+        return self._get(f"{self.base_url_clan}/tribe/blurry/info", headers=self.headers, params={"clanName": clan_name, "pageNo": page_no, "pageSize": page_size})
 
-  def info(self, clan_id):
-    return self._get(f"{BASE_URL_V2}/tribe", headers=self.headers, params={"clanId": clan_id})
+    def info(self, clan_id):
+        return self._get(f"{self.base_url_clan_v2}/tribe", headers=self.headers, params={"clanId": clan_id})
 
-  def invite(self, friend_ids, message=""):
-    return self._post(f"{BASE_URL}/tribe/member/invite", headers=self.headers, json={"friendIds": friend_ids, "msg": message})
+    def invite(self, friend_ids, message=""):
+        return self._post(f"{self.base_url_clan}/tribe/member/invite", headers=self.headers, json={"friendIds": friend_ids, "msg": message})
 
-  def agreement_user(self, other_id):
-    return self._put(f"{BASE_URL}/tribe/member/agreement", headers=self.headers, params={"otherId": other_id})
+    def agreement_user(self, other_id):
+        return self._put(f"{self.base_url_clan}/tribe/member/agreement", headers=self.headers, params={"otherId": other_id})
 
-  def reject_user(self, other_id):
-    return self._put(f"{BASE_URL}/tribe/member/rejection", headers=self.headers, params={"otherId": other_id})
+    def reject_user(self, other_id):
+        return self._put(f"{self.base_url_clan}/tribe/member/rejection", headers=self.headers, params={"otherId": other_id})
 
-  def mute_member(self, member_id, minutes):
-    return self._post(f"{BASE_URL}/tribe/mute/member", headers=self.headers, params={"memberId": member_id, "minute": minutes})
+    def mute_member(self, member_id, minutes):
+        return self._post(f"{self.base_url_clan}/tribe/mute/member", headers=self.headers, params={"memberId": member_id, "minute": minutes})
 
-  def unmute_member(self, member_id):
-    return self._delete(f"{BASE_URL}/tribe/mute/member", headers=self.headers, params={"memberId": member_id})
+    def unmute_member(self, member_id):
+        return self._delete(f"{self.base_url_clan}/tribe/mute/member", headers=self.headers, params={"memberId": member_id})
 
-  def mute_all(self):
-    return self._put(f"{BASE_URL}/tribe/mute", headers=self.headers, params={"muteStatus": 1})
+    def mute_all(self):
+        return self._put(f"{self.base_url_clan}/tribe/mute", headers=self.headers, params={"muteStatus": 1})
 
-  def unmute_all(self):
-    return self._put(f"{BASE_URL}/tribe/mute", headers=self.headers, params={"muteStatus": 0})
+    def unmute_all(self):
+        return self._put(f"{self.base_url_clan}/tribe/mute", headers=self.headers, params={"muteStatus": 0})
 
-  def remove_member(self, member_ids):
-    return self._delete(f"{BASE_URL}/tribe/member/remove/batch", headers=self.headers, json=member_ids)
+    def remove_member(self, member_ids):
+        return self._delete(f"{self.base_url_clan}/tribe/member/remove/batch", headers=self.headers, json=member_ids)
 
-  def edit(self, clan_id, currency=0, details="", head_pic="", name="", tags=None):
-    return self._put(f"{BASE_URL}/tribe", headers=self.headers, json={"clanId": clan_id, "currency": currency, "details": details, "headPic": head_pic, "name": name, "tags": tags or []})
+    def edit(self, clan_id, currency=0, details="", head_pic="", name="", tags=None):
+        return self._put(f"{self.base_url_clan}/tribe", headers=self.headers, json={"clanId": clan_id, "currency": currency, "details": details, "headPic": head_pic, "name": name, "tags": tags or []})
 
-  def edit_elders(self, type_, elder_ids):
-    return self._put(f"{BASE_URL}/tribe/members", headers=self.headers, params={"type": type_, "otherIds": elder_ids})
+    def edit_elders(self, type_, elder_ids):
+        return self._put(f"{self.base_url_clan}/tribe/members", headers=self.headers, params={"type": type_, "otherIds": elder_ids})
 
-  def authentication(self, type_):
-    return self._put(f"{BASE_URL}/free/verification", headers=self.headers, params={"freeVerify": 1 if type_ == "on" else 0})
+    def authentication(self, type_):
+        return self._put(f"{self.base_url_clan}/free/verification", headers=self.headers, params={"freeVerify": 1 if type_ == "on" else 0})
 
-  def buy_decoration(self, decoration_id):
-    return self._put(f"{BASE_URL}/decorations/purchase", headers=self.headers, params={"decorationId": decoration_id})
+    def buy_decoration(self, decoration_id):
+        return self._put(f"{self.base_url_clan}/decorations/purchase", headers=self.headers, params={"decorationId": decoration_id})
 
-  def task_accept(self, task_id, is_team_task):
-    return self._put(f"{BASE_URL}/tasks/accept", headers=self.headers, params={"id": task_id, "type": 0 if is_team_task else 1})
+    def task_accept(self, task_id, is_team_task):
+        return self._put(f"{self.base_url_clan}/tasks/accept", headers=self.headers, params={"id": task_id, "type": 0 if is_team_task else 1})
 
-  def self_task_refresh(self):
-    return self._get(f"{BASE_URL_V3}/personal/tasks", headers=self.headers, params={"type": 1})
+    def self_task_refresh(self):
+        return self._get(f"{self.base_url_clan_v3}/personal/tasks", headers=self.headers, params={"type": 1})
 
-  def task_claim(self, task_id, is_team_task):
-    return self._put(f"{BASE_URL}/tasks", headers=self.headers, params={"id": task_id, "type": 0 if is_team_task else 1})
+    def task_claim(self, task_id, is_team_task):
+        return self._put(f"{self.base_url_clan}/tasks", headers=self.headers, params={"id": task_id, "type": 0 if is_team_task else 1})
 
-  def notice(self, content):
-    return self._post(f"{BASE_URL}/tribe/bulletin", headers=self.headers, json={"content": content})
+    def notice(self, content):
+        return self._post(f"{self.base_url_clan}/tribe/bulletin", headers=self.headers, json={"content": content})
 
-  def transfer_chief(self, new_chief_id):
-    return self._put(f"{BASE_URL}/tribe/member", headers=self.headers, params={"otherId": new_chief_id, "type": 3})
+    def transfer_chief(self, new_chief_id):
+        return self._put(f"{self.base_url_clan}/tribe/member", headers=self.headers, params={"otherId": new_chief_id, "type": 3})
 
-  def create(self, clan_id=0, currency=2, details="", head_pic="", name="", tags=None):
-    return self._post(f"{BASE_URL_V3}/tribe", headers=self.headers, json={"clanId": clan_id, "currency": currency, "details": details, "headPic": head_pic, "name": name, "tags": tags or []})
+    def create(self, clan_id=0, currency=2, details="", head_pic="", name="", tags=None):
+        return self._post(f"{self.base_url_clan_v3}/tribe", headers=self.headers, json={"clanId": clan_id, "currency": currency, "details": details, "headPic": head_pic, "name": name, "tags": tags or []})
 
-  def dissolve(self, clan_id):
-    return self._delete(f"{BASE_URL}/tribe", headers=self.headers, params={"clanId": clan_id})
+    def dissolve(self, clan_id):
+        return self._delete(f"{self.base_url_clan}/tribe", headers=self.headers, params={"clanId": clan_id})
```

### Comparing `blockmango-1.4.7/blockmango/decoration.py` & `blockmango-1.4.8/blockmango/decoration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,29 @@
+# decoration.py
 from .http import HTTPMixin
-
-BASE_URL_DECORATION = "http://modsgs.sandboxol.com/decoration/api/v1"
-BASE_URL_SHOP = "http://modsgs.sandboxol.com/shop/api/v1"
-BASE_URL_USER = "http://modsgs.sandboxol.com/user/api/v1"
+from .config import BASE_URL_DECORATION, BASE_URL_SHOP
 
 class Decoration(HTTPMixin):
-  def __init__(self, user_id, access_token):
-    self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1"}
+    __slots__ = ("headers",)
+    base_url = BASE_URL_DECORATION
+
+    def __init__(self, user_id, access_token):
+        self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1"}
 
-  def skins(self, uid):
-    params = {"engineVersion": "10105", "os": "android", "showVip": 1}
-    return self._get(f"{BASE_URL_DECORATION}/new/decorations/users/{uid}/classify/all", headers=self.headers, params=params)
-
-  def current_price(self, skin_id, is_suit):
-    payload = [{"id": skin_id, "isSuit": is_suit}]
-    return self._post(f"{BASE_URL_DECORATION}/decoration/current/price", headers=self.headers, json=payload)
-
-  def buy(self, diamond, cloth_voucher, paytype):
-    params = {"diamond": diamond, "gold": 0, "clothVoucher": cloth_voucher, "payType": paytype}
-    return self._post(f"{BASE_URL_SHOP}/new/shop/decorations/buy", headers=self.headers, params=params)
-
-  def shop_info(self):
-    return self._get(f"{BASE_URL_USER}/user/shop/info", headers=self.headers)
-
-  def equip(self, skin_id):
-    params = {"ids": skin_id}
-    return self._post(f"{BASE_URL_DECORATION}/decorations/using/new", headers=self.headers, params=params)
+    def skins(self, uid):
+        params = {"engineVersion": "10105", "os": "android", "showVip": 1}
+        return self._get(f"{self.base_url}/new/decorations/users/{uid}/classify/all", headers=self.headers, params=params)
+
+    def current_price(self, skin_id, is_suit):
+        payload = [{"id": skin_id, "isSuit": is_suit}]
+        return self._post(f"{self.base_url}/decoration/current/price", headers=self.headers, json=payload)
+
+    def buy(self, diamond, cloth_voucher, paytype):
+        params = {"diamond": diamond, "gold": 0, "clothVoucher": cloth_voucher, "payType": paytype}
+        return self._post(f"{BASE_URL_SHOP}/new/shop/decorations/buy", headers=self.headers, params=params)
+
+    def shop_info(self):
+        return self._get(f"{BASE_URL_USER}/user/shop/info", headers=self.headers)
+
+    def equip(self, skin_id):
+        params = {"ids": skin_id}
+        return self._post(f"{BASE_URL_DECORATION}/decorations/using/new", headers=self.headers, params=params)
```

### Comparing `blockmango-1.4.7/blockmango/friends.py` & `blockmango-1.4.8/blockmango/friends.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,53 @@
+# friends.py
 from .http import HTTPMixin
-
-BASE_URL_FRIEND = "http://modsgs.sandboxol.com/friend/api/v1"
-BASE_URL_DECORATION = "http://modsgs.sandboxol.com/decoration/api/v1"
+from .config import BASE_URL_FRIEND, BASE_URL_DECORATION
 
 class Friends(HTTPMixin):
-  def __init__(self, user_id, access_token):
-    self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1"}
+    __slots__ = ("headers",)
+    base_url_friend = BASE_URL_FRIEND
+    base_url_decoration = BASE_URL_DECORATION
+
+    def __init__(self, user_id, access_token):
+        self.headers = {"userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1"}
 
-  def delete_friend(self, friend_id):
-    return self._delete(f"{BASE_URL_FRIEND}/friends", headers=self.headers, params={"friendId": friend_id})
+    def delete_friend(self, friend_id):
+        return self._delete(f"{self.base_url_friend}/friends", headers=self.headers, params={"friendId": friend_id})
 
-  def request(self, friend_id, msg):
-    payload = {"friendId": friend_id, "msg": msg, "type": 1}
-    headers = {"Content-Type": "application/json", **self.headers}
-    return self._post(f"{BASE_URL_FRIEND}/friends", headers=headers, json=payload)
+    def request(self, friend_id, msg):
+        payload = {"friendId": friend_id, "msg": msg, "type": 1}
+        headers = {"Content-Type": "application/json", **self.headers}
+        return self._post(f"{self.base_url_friend}/friends", headers=headers, json=payload)
 
-  def popularity(self, friend_id):
-    return self._get(f"{BASE_URL_FRIEND}/popularity/{friend_id}", headers=self.headers)
+    def popularity(self, friend_id):
+        return self._get(f"{self.base_url_friend}/popularity/{friend_id}", headers=self.headers)
 
-  def info(self, friend_id):
-    return self._get(f"{BASE_URL_FRIEND}/friends/{friend_id}", headers=self.headers)
+    def info(self, friend_id):
+        return self._get(f"{self.base_url_friend}/friends/{friend_id}", headers=self.headers)
 
-  def decoration(self, friend_id):
-    return self._get(f"{BASE_URL_DECORATION}/decorations-v2/{friend_id}/using", headers=self.headers)
+    def decoration(self, friend_id):
+        return self._get(f"{self.base_url_decoration}/decorations-v2/{friend_id}/using", headers=self.headers)
 
-  def add_popularity(self, friend_id):
-    return self._post(f"{BASE_URL_FRIEND}/popularity", headers=self.headers, params={"friendId": friend_id})
+    def add_popularity(self, friend_id):
+        return self._post(f"{self.base_url_friend}/popularity", headers=self.headers, params={"friendId": friend_id})
 
-  def friend_list(self):
-    headers = {"language": "en_US", **self.headers}
-    return self._get(f"{BASE_URL_FRIEND}/friends/status", headers=headers)
+    def friend_list(self):
+        headers = {"language": "en_US", **self.headers}
+        return self._get(f"{self.base_url_friend}/friends/status", headers=headers)
 
-  def nickname(self, friend_id, alias):
-    return self._post(f"{BASE_URL_FRIEND}/friends/{friend_id}/alias", headers=self.headers, params={"alias": alias})
+    def nickname(self, friend_id, alias):
+        return self._post(f"{self.base_url_friend}/friends/{friend_id}/alias", headers=self.headers, params={"alias": alias})
 
-  def friend_approve(self, friend_id):
-    return self._put(f"{BASE_URL_FRIEND}/friends/{friend_id}/agreement", headers=self.headers)
+    def friend_approve(self, friend_id):
+        return self._put(f"{self.base_url_friend}/friends/{friend_id}/agreement", headers=self.headers)
 
-  def friend_blacklist(self, friend_id):
-    return self._delete(f"{BASE_URL_FRIEND}/friends/black", headers=self.headers, params={"friendId": friend_id})
+    def friend_blacklist(self, friend_id):
+        return self._delete(f"{self.base_url_friend}/friends/black", headers=self.headers, params={"friendId": friend_id})
 
-  def reject_all(self):
-    return self._post(f"{BASE_URL_FRIEND}/friends/requests/reject-all", headers=self.headers)
+    def reject_all(self):
+        return self._post(f"{self.base_url_friend}/friends/requests/reject-all", headers=self.headers)
 
-  def approve_all(self):
-    return self._post(f"{BASE_URL_FRIEND}/friends/requests/approve-all", headers=self.headers)
+    def approve_all(self):
+        return self._post(f"{self.base_url_friend}/friends/requests/approve-all", headers=self.headers)
 
-  def friend_reject(self, friend_id):
-    return self._put(f"{BASE_URL_FRIEND}/friends/{friend_id}/rejection", headers=self.headers)
+    def friend_reject(self, friend_id):
+        return self._put(f"{self.base_url_friend}/friends/{friend_id}/rejection", headers=self.headers)
```

### Comparing `blockmango-1.4.7/blockmango/groupchat.py` & `blockmango-1.4.8/blockmango/groupchat.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.7/blockmango/http.py` & `blockmango-1.4.8/blockmango/http.py`

 * *Files identical despite different names*

### Comparing `blockmango-1.4.7/blockmango/user.py` & `blockmango-1.4.8/blockmango/user.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
+# user.py
 from .http import HTTPMixin
-
-BASE_URL_USER = "http://modsgs.sandboxol.com/user/api/v1"
-BASE_URL_ROUTE = "http://route.sandboxol.com/user/api"
-BASE_URL_USER_INFO = "http://modsgs.sandboxol.com/user/api"
+from .config import BASE_URL_USER, BASE_URL_ROUTE, BASE_URL_USER_INFO
 
 class User(HTTPMixin):
     __slots__ = ("headers",)
+    base_url = BASE_URL_USER
 
     def __init__(self, user_id, access_token):
         self.headers = { "userId": user_id, "Access-Token": access_token, "User-Agent": "okhttp/3.12.1" }
 
     def get_user_info(self):
-        return self._get(f"{BASE_URL_USER_INFO}/v2/user/details/info", headers=self.headers)
+        return self._get(f"{self.base_url}/v2/user/details/info", headers=self.headers)
 
     def set_birthday(self, birthday):
         return self._put(f"{BASE_URL_USER}/user/info", headers=self.headers, json_data={"birthday": birthday})
 
     def login(self, device_id, device_sign, password, userId):
         headers = { **self.headers, "bmg-sign": device_sign, "bmg-device-id": device_id }
         return self._post(f"{BASE_URL_ROUTE}/v1/app/login", headers=headers, json_data={"password": password, "uid": userId})
@@ -32,8 +31,8 @@
     def modify_password(self, old_password, new_password):
         return self._post(f"{BASE_URL_USER}/user/password/modify", headers=self.headers, json_data={"confirmPassword": "", "newPassword": new_password, "oldPassword": old_password})
 
     def bind_email(self, email, verify_code):
         return self._post(f"{BASE_URL_USER}/users/bind/email", headers=self.headers, json_data={"email": email, "verifyCode": verify_code})
 
     def unbind_email(self, verify_code, email):
-        return self._delete(f"{BASE_URL_USER_INFO}/v2/users/{self.headers['userId']}/emails", headers=self.headers, params={"email": email, "verifyCode": verify_code})
+        return self._delete(f"{BASE_URL_USER_INFO}/v2/users/{self.headers['userId']}/emails", headers=self.headers, params={"email": email, "verifyCode": verify_code})
```

### Comparing `blockmango-1.4.7/blockmango.egg-info/PKG-INFO` & `blockmango-1.4.8/blockmango.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blockmango
-Version: 1.4.7
+Version: 1.4.8
 Summary: Blockman Go API package
 Home-page: https://github.com/darkkpy/blockmango
 Author: Dark
 Author-email: darkness0777@proton.me
 License: MIT
 Project-URL: Documentation, https://github.com/darkkpy/blockmango/tree/main/docs
 Project-URL: Source, https://github.com/darkkpy/blockmango
```

### Comparing `blockmango-1.4.7/setup.py` & `blockmango-1.4.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open(filename, "r", encoding="utf-8") as file:
         return file.read() + "\n\n"
 
 long_description = read_md_file("README.md")
 
 setup(
     name='blockmango',
-    version='1.4.7',
+    version='1.4.8',
     author='Dark',
     author_email='darkness0777@proton.me',
     description='Blockman Go API package',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/darkkpy/blockmango',
     packages=['blockmango'],
```

