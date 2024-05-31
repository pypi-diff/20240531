# Comparing `tmp/aiosteampy-0.4.1.tar.gz` & `tmp/aiosteampy-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiosteampy-0.4.1.tar", max compression
+gzip compressed data, was "aiosteampy-0.5.0.tar", max compression
```

## Comparing `aiosteampy-0.4.1.tar` & `aiosteampy-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0     1088 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/LICENSE
--rw-r--r--   0        0        0     4985 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/README.md
--rw-r--r--   0        0        0      309 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/__init__.py
--rw-r--r--   0        0        0    10637 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/client.py
--rw-r--r--   0        0        0    10180 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/confirmation.py
--rw-r--r--   0        0        0     6695 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/constants.py
--rw-r--r--   0        0        0     4428 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/converter.py
--rw-r--r--   0        0        0      701 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/exceptions.py
--rw-r--r--   0        0        0      933 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/guard.py
--rw-r--r--   0        0        0      942 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/http.py
--rw-r--r--   0        0        0    10384 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/login.py
--rw-r--r--   0        0        0    21582 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/market.py
--rw-r--r--   0        0        0    11350 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/models.py
--rw-r--r--   0        0        0    16132 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/public.py
--rw-r--r--   0        0        0    22283 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/trade.py
--rw-r--r--   0        0        0     2287 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/typed.py
--rw-r--r--   0        0        0    12464 2024-04-06 19:51:46.486327 aiosteampy-0.4.1/aiosteampy/utils.py
--rw-r--r--   0        0        0     1791 2024-04-06 19:51:46.490327 aiosteampy-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     6268 1970-01-01 00:00:00.000000 aiosteampy-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5196 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/README.md
+-rw-r--r--   0        0        0      291 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/__init__.py
+-rw-r--r--   0        0        0    10748 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/client.py
+-rw-r--r--   0        0        0    10180 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/confirmation.py
+-rw-r--r--   0        0        0     6695 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/constants.py
+-rw-r--r--   0        0        0     4359 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/converter.py
+-rw-r--r--   0        0        0      701 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/exceptions.py
+-rw-r--r--   0        0        0      933 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/guard.py
+-rw-r--r--   0        0        0     2192 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/http.py
+-rw-r--r--   0        0        0    10384 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/login.py
+-rw-r--r--   0        0        0    21582 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/market.py
+-rw-r--r--   0        0        0    11350 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/models.py
+-rw-r--r--   0        0        0    16132 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/public.py
+-rw-r--r--   0        0        0    22633 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/trade.py
+-rw-r--r--   0        0        0     2287 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/typed.py
+-rw-r--r--   0        0        0     1018 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/user_agents.py
+-rw-r--r--   0        0        0    12761 2024-05-31 20:15:36.119938 aiosteampy-0.5.0/aiosteampy/utils.py
+-rw-r--r--   0        0        0     1891 2024-05-31 20:15:36.123938 aiosteampy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6604 1970-01-01 00:00:00.000000 aiosteampy-0.5.0/PKG-INFO
```

### Comparing `aiosteampy-0.4.1/LICENSE` & `aiosteampy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.1/README.md` & `aiosteampy-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -39,25 +39,27 @@
 pipenv install aiosteampy
 ```
 
 ```shell
 poetry add aiosteampy
 ```
 
-Project have extra [currencies converter](https://aiosteampy.somespecial.one/ext/converter/) with
-target dependency `aiosteampy[converter]`. For instance:
+Project have some extras [currencies converter](https://aiosteampy.somespecial.one/ext/converter/),
+[socks proxies](https://aiosteampy.somespecial.one/proxies).
+To install them all, please, use `aiosteampy[all]` install target:
 
 ```shell
-poetry add aiosteampy[converter]
+poetry add aiosteampy[all]
 ```
 
 <!--install-end-->
 
 > [!TIP]
-> [aiohttp docs](https://docs.aiohttp.org/en/stable/#installing-all-speedups-in-one-command) recommends installing speedups (`aiodns`, `cchardet`, ...)
+> [aiohttp docs](https://docs.aiohttp.org/en/stable/#installing-all-speedups-in-one-command) recommends installing
+> speedups (`aiodns`, `cchardet`, ...)
 
 <!--intro-start-->
 
 AIOSTEAMPY use [aiohttp](https://github.com/aio-libs/aiohttp) underneath to do asynchronous requests to steam servers,
 with modern async/await syntax.
 
 > Generally, project inspired most
@@ -67,14 +69,15 @@
 
 - Stateless: the main idea was a low-middle layer API wrapper of some steam services and methods like market,
   tradeoffers, confirmations, steamguard, etc. But if you want to cache your entities data (listings, confirmations,
   ...) [there is some methods to help](https://aiosteampy.somespecial.one/examples/states/).
 - Declarative: there is models almost for every data.
 - Typed: for editor support most things are typed.
 - Short: I really tried to fit most important for steam trading methods.
+- Connection behind web proxy.
 
 ## What can I do with this
 
 - Operate with steam trade offers for any manner.
 - Sell, buy items on market. Place, cancel orders.
 - Login trough steam to 3rd party sites.
 - Fetch data from market.
@@ -103,14 +106,16 @@
 
 There is no rules or requirements to contribute. Feedbacks, suggests, other are welcome.
 I will be very grateful for helping me get the things right.
 
 ## Credits
 
 - [bukson/steampy](https://github.com/bukson/steampy)
+- [aiohttp-socks](https://github.com/romis2012/aiohttp-socks)
+- [croniter](https://github.com/kiorky/croniter)
 - [DoctorMcKay/node-steamcommunity](https://github.com/DoctorMcKay/node-steamcommunity)
 - [Identifying Steam items](https://dev.doctormckay.com/topic/332-identifying-steam-items/)
 - [Revadike/InternalSteamWebAPI](https://github.com/Revadike/InternalSteamWebAPI)
 - [Gobot1234/steam.py](https://github.com/Gobot1234/steam.py)
 - [Steam Market id's storage repo](https://github.com/somespecialone/steam-item-name-ids)
 - [steamapi.xpaw.me](https://steamapi.xpaw.me/)
 - [Steam Exchange Rate Tracker](https://github.com/somespecialone/sert)
```

### Comparing `aiosteampy-0.4.1/aiosteampy/client.py` & `aiosteampy-0.5.0/aiosteampy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,29 +66,36 @@
         api_key: str = None,
         trade_token: str = None,
         wallet_currency: Currency = None,
         wallet_country=DEF_COUNTRY,
         lang=Language.ENGLISH,
         tz_offset=0.0,
         session: ClientSession = None,
+        proxy: str = None,
         user_agent: str = None,
     ):
         self.username = username
         self.steam_id = account_id_to_steam_id(steam_id) if steam_id < 4294967296 else steam_id  # steam id64
         self.trade_token = trade_token
 
         self._password = password
         self._shared_secret = shared_secret
         self._identity_secret = identity_secret
         self._api_key = api_key
         self._wallet_currency = wallet_currency
 
         self._wallet_country = wallet_country
 
-        super().__init__(session=session, user_agent=user_agent, access_token=access_token, refresh_token=refresh_token)
+        super().__init__(
+            session=session,
+            user_agent=user_agent,
+            access_token=access_token,
+            refresh_token=refresh_token,
+            proxy=proxy,
+        )
 
         self._set_init_cookies(lang, tz_offset)
 
     @property
     def account_id(self) -> int:
         """Steam id32."""
         return steam_id_to_account_id(self.steam_id)
```

### Comparing `aiosteampy-0.4.1/aiosteampy/confirmation.py` & `aiosteampy-0.5.0/aiosteampy/confirmation.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.1/aiosteampy/constants.py` & `aiosteampy-0.5.0/aiosteampy/constants.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.1/aiosteampy/converter.py` & `aiosteampy-0.5.0/aiosteampy/converter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Currency converter extension."""
+
 import asyncio
 from collections import UserDict
 from datetime import datetime, timedelta
 
 from yarl import URL
 from aiohttp import ClientSession
 
@@ -11,18 +13,15 @@
 except ImportError:
     from warnings import warn
 
     warn(
         """
         The `aiosteampy.converter` module requires the `croniter` library to be installed
         to make the rates synchronization with backend service work.
-        In order You need this functionality, You can use `aiosteampy[converter]` dependency install target:
-        `pip install aiosteampy[converter]`
-        or
-        `poetry add aiosteampy[converter]`
+        In order You need this functionality, You can use `aiosteampy[converter]` dependency install target.
         """,
         category=RuntimeWarning,
     )
 
     croniter = None
 
 
@@ -129,11 +128,11 @@
         """
 
         source_rate = self[currency][0] if currency is not Currency.USD else 1
         target_rate = self[target][0] if target is not Currency.USD else 1
 
         # direct conversion
         # return round(amount * (target_rate / source_rate))
-        
+
         # with USD in middle step
         usd_amount = round(amount * (1 / source_rate))
         return round(usd_amount * target_rate)
```

### Comparing `aiosteampy-0.4.1/aiosteampy/exceptions.py` & `aiosteampy-0.5.0/aiosteampy/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.1/aiosteampy/guard.py` & `aiosteampy-0.5.0/aiosteampy/guard.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.1/aiosteampy/login.py` & `aiosteampy-0.5.0/aiosteampy/login.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.1/aiosteampy/market.py` & `aiosteampy-0.5.0/aiosteampy/market.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.1/aiosteampy/models.py` & `aiosteampy-0.5.0/aiosteampy/models.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.1/aiosteampy/public.py` & `aiosteampy-0.5.0/aiosteampy/public.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.1/aiosteampy/trade.py` & `aiosteampy-0.5.0/aiosteampy/trade.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, overload, Literal, Type, TypeAlias, Callable
+from typing import TYPE_CHECKING, overload, Literal, Type, TypeAlias, Callable, Iterable, Sequence
 from datetime import datetime
 from json import dumps as jdumps
 
 from yarl import URL
 
 from .exceptions import ApiError
 from .constants import STEAM_URL, CORO, T_KWARGS
@@ -419,15 +419,15 @@
         """
 
         if isinstance(offer, TradeOffer):
             if offer.is_our_offer:
                 raise ValueError("You can't accept your offer! Are you trying to cancel outgoing offer?")
             offer_id = offer.id
             partner = offer.partner_id64
-            to_remove = TradeOffer
+            to_remove = offer
         else:  # int
             if not partner:
                 fetched = await self.get_or_fetch_trade_offer(offer)
                 return await self.accept_trade_offer(fetched)
 
             offer_id = offer
             partner = account_id_to_steam_id(partner) if partner < 4294967296 else partner  # 2**32
@@ -448,62 +448,62 @@
 
         await self.remove_trade_offer(offer_id, to_remove)
 
     @overload
     async def make_trade_offer(
         self,
         obj: int,
-        to_give: list[EconItemType] = ...,
-        to_receive: list[EconItemType] = ...,
+        to_give: Sequence[EconItemType] = ...,
+        to_receive: Sequence[EconItemType] = ...,
         message: str = ...,
         *,
         token: str = ...,
         confirm: bool = ...,
         countered_id: int = ...,
     ) -> int:
         ...
 
     @overload
     async def make_trade_offer(
         self,
         obj: str,
-        to_give: list[EconItemType] = ...,
-        to_receive: list[EconItemType] = ...,
+        to_give: Sequence[EconItemType] = ...,
+        to_receive: Sequence[EconItemType] = ...,
         message: str = ...,
         *,
         confirm: bool = ...,
         countered_id: int = ...,
     ) -> int:
         ...
 
     async def make_trade_offer(
         self: "SteamCommunityMixin",
         obj: int | str,
-        to_give: list[EconItemType] = (),
-        to_receive: list[EconItemType] = (),
+        to_give: Sequence[EconItemType] = (),
+        to_receive: Sequence[EconItemType] = (),
         message="",
         *,
         token: str = None,
         confirm=True,
         countered_id: int = None,
         **kwargs: T_KWARGS,
     ) -> int:
         """
         Make (send) steam trade offer to partner.
 
         .. note:: Make sure that partner is in friends list if you not pass trade url or trade token.
 
         :param obj: partner trade url, partner id(id32 or id64)
-        :param token:
-        :param to_give:
-        :param to_receive:
-        :param message:
-        :param confirm:
-        :param countered_id:
-        :param kwargs:
+        :param token: trade token (mandatory if `obj` is partner id)
+        :param to_give: sequence of items that you want to give
+        :param to_receive: sequence of items that you want to receive
+        :param message: message to the partner
+        :param confirm: auto-confirm offer
+        :param countered_id: id of offer that you want to counter. Use `counter_trade_offer` method for this
+        :param kwargs: additional data to send in payload
         :return: trade offer id
         :raises ValueError: trade is empty
         """
 
         if not to_give and not to_receive:
             raise ValueError("You can't make empty trade offer!")
 
@@ -567,40 +567,40 @@
 
         return trade_url, partner_id32, partner_id64, token
 
     @overload
     async def counter_trade_offer(
         self,
         obj: TradeOffer,
-        to_give: list[EconItemType] = (),
-        to_receive: list[EconItemType] = (),
+        to_give: Sequence[EconItemType] = (),
+        to_receive: Sequence[EconItemType] = (),
         message="",
         *,
         confirm: bool = ...,
     ) -> int:
         ...
 
     @overload
     async def counter_trade_offer(
         self,
         obj: int,
-        to_give: list[EconItemType] = (),
-        to_receive: list[EconItemType] = (),
+        to_give: Sequence[EconItemType] = (),
+        to_receive: Sequence[EconItemType] = (),
         message="",
         *,
         partner_id: int,
         confirm: bool = ...,
     ) -> int:
         ...
 
     def counter_trade_offer(
         self,
         obj: TradeOffer | int,
-        to_give: list[EconItemType] = (),
-        to_receive: list[EconItemType] = (),
+        to_give: Sequence[EconItemType] = (),
+        to_receive: Sequence[EconItemType] = (),
         message="",
         *,
         partner_id: int = None,
         confirm=True,
         **kwargs: T_KWARGS,
     ) -> CORO[int]:
         """
```

### Comparing `aiosteampy-0.4.1/aiosteampy/typed.py` & `aiosteampy-0.5.0/aiosteampy/typed.py`

 * *Files identical despite different names*

### Comparing `aiosteampy-0.4.1/aiosteampy/utils.py` & `aiosteampy-0.5.0/aiosteampy/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+"""Useful utils."""
+
 import asyncio
 from base64 import b64decode, b64encode
 from struct import pack, unpack
 from time import time as time_time
 from hmac import new as hmac_new
 from hashlib import sha1
 from functools import wraps
 from typing import Callable, overload, ParamSpec, TypeVar, TYPE_CHECKING, TypeAlias
 from http.cookies import SimpleCookie, Morsel
 from math import floor
 from secrets import token_hex
 from re import search as re_search
 from json import loads as j_loads
 
-from aiohttp import ClientSession
+from aiohttp import ClientSession, ClientResponse
 from yarl import URL
 
 from .typed import JWTToken
 
 if TYPE_CHECKING:
     from .client import SteamCommunityMixin
 
@@ -93,31 +95,32 @@
         "action": re_search(r"id=\"actionInput\"[\w=\"\s]+value=\"(?P<action>\w+)\"", page_text)["action"],
         "openid.mode": re_search(r"name=\"openid\.mode\"[\w=\"\s]+value=\"(?P<mode>\w+)\"", page_text)["mode"],
         "openidparams": re_search(r"name=\"openidparams\"[\w=\"\s]+value=\"(?P<params>[\w=/]+)\"", page_text)["params"],
         "nonce": re_search(r"name=\"nonce\"[\w=\"\s]+value=\"(?P<nonce>\w+)\"", page_text)["nonce"],
     }
 
 
-async def do_session_steam_auth(session: ClientSession, auth_url: str | URL):
+async def do_session_steam_auth(session: ClientSession, auth_url: str | URL) -> ClientResponse:
     """
     Request auth page, find specs of steam openid and log in through steam with passed session.
     Use it when you need to log in 3rd party site trough Steam using only cookies.
 
     .. seealso:: https://aiosteampy.somespecial.one/examples/auth_3rd_party_site/
 
     :param session: just session.
     :param auth_url: url to site, which redirect you to steam login page.
+    :return: response with history, headers and data
     """
 
     r = await session.get(auth_url)
     rt = await r.text()
 
     data = extract_openid_payload(rt)
 
-    await session.post("https://steamcommunity.com/openid/login", data=data, allow_redirects=True)
+    return await session.post("https://steamcommunity.com/openid/login", data=data, allow_redirects=True)
 
 
 def get_cookie_value_from_session(session: ClientSession, url: URL, field: str) -> str | None:
     """Just get value from session cookies."""
 
     c = session.cookie_jar.filter_cookies(url)
     return c[field].value if field in c else None
@@ -239,18 +242,19 @@
 
 async def restore_from_cookies(
     cookies: JSONABLE_COOKIE_JAR,
     client: "SteamCommunityMixin",
     *,
     init_data=True,
     **init_kwargs,
-):
+) -> bool:
     """
     Helper func. Restore client session from cookies.
     Login if session is not alive.
+    Return `True` if cookies are valid and not expired.
     """
 
     prepared = []
     for cookie_data in cookies:
         c = SimpleCookie()
         for k, v in cookie_data.items():
             m = Morsel()
@@ -268,17 +272,19 @@
 
         prepared.append(c)
 
     for c in prepared:
         client.session.cookie_jar.update_cookies(c)
     if not (await client.is_session_alive()):
         await client.login(init_data=init_data, **init_kwargs)
+        return False
     else:
         client._is_logged = True
         init_data and await client._init_data()
+        return True
 
 
 def get_jsonable_cookies(session: ClientSession) -> JSONABLE_COOKIE_JAR:
     """Extract and convert cookies to dict object."""
 
     return [
         {
@@ -395,7 +401,11 @@
 
 def decode_jwt(token: str) -> JWTToken:
     parts = token.split(".")
     if len(parts) != 3:
         raise ValueError("Invalid JWT", parts)
 
     return j_loads(b64decode(parts[1] + "==", altchars="-_"))
+
+
+def patch_session_with_proxy(session: ClientSession, proxy: str):
+    pass
```

### Comparing `aiosteampy-0.4.1/pyproject.toml` & `aiosteampy-0.5.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "aiosteampy"
-version = "0.4.1"
-description = "Simple library to trade and interact with steam market, webapi, guard"
+version = "0.5.0"
+description = "Trade and interact with steam market, webapi, guard"
 license = "MIT"
 authors = ["Dmytro Tkachenko <itsme@somespecial.one>"]
 readme = "README.md"
 homepage = "https://aiosteampy.somespecial.one"
 repository = "https://github.com/somespecialone/aiosteampy"
 documentation = "https://aiosteampy.somespecial.one"
 keywords = ["steam", "trade", "steamguard", "asyncio", "steam-market"]
@@ -25,17 +25,20 @@
 "Bug Tracker" = "https://github.com/somespecialone/aiosteampy/issues"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.9.1"
 rsa = "^4.9"
 croniter = { version = "^2.0.1", optional = true }
+aiohttp-socks = { version = "^0.8.4", optional = true }
 
 [tool.poetry.extras]
 converter = ["croniter"]
+socks = ["aiohttp-socks"]
+all = ["croniter", "aiohttp-socks"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.12.1"
 
 [tool.poetry.group.test]
 optional = true
 [tool.poetry.group.test.dependencies]
```

### Comparing `aiosteampy-0.4.1/PKG-INFO` & `aiosteampy-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: aiosteampy
-Version: 0.4.1
-Summary: Simple library to trade and interact with steam market, webapi, guard
+Version: 0.5.0
+Summary: Trade and interact with steam market, webapi, guard
 Home-page: https://aiosteampy.somespecial.one
 License: MIT
 Keywords: steam,trade,steamguard,asyncio,steam-market
 Author: Dmytro Tkachenko
 Author-email: itsme@somespecial.one
 Requires-Python: >=3.10,<4.0
 Classifier: Framework :: AsyncIO
@@ -15,17 +15,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
+Provides-Extra: all
 Provides-Extra: converter
+Provides-Extra: socks
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
-Requires-Dist: croniter (>=2.0.1,<3.0.0) ; extra == "converter"
+Requires-Dist: aiohttp-socks (>=0.8.4,<0.9.0) ; extra == "socks" or extra == "all"
+Requires-Dist: croniter (>=2.0.1,<3.0.0) ; extra == "converter" or extra == "all"
 Requires-Dist: rsa (>=4.9,<5.0)
 Project-URL: Bug Tracker, https://github.com/somespecialone/aiosteampy/issues
 Project-URL: Documentation, https://aiosteampy.somespecial.one
 Project-URL: Repository, https://github.com/somespecialone/aiosteampy
 Description-Content-Type: text/markdown
 
 <!--header-start-->
@@ -69,25 +72,27 @@
 pipenv install aiosteampy
 ```
 
 ```shell
 poetry add aiosteampy
 ```
 
-Project have extra [currencies converter](https://aiosteampy.somespecial.one/ext/converter/) with
-target dependency `aiosteampy[converter]`. For instance:
+Project have some extras [currencies converter](https://aiosteampy.somespecial.one/ext/converter/),
+[socks proxies](https://aiosteampy.somespecial.one/proxies).
+To install them all, please, use `aiosteampy[all]` install target:
 
 ```shell
-poetry add aiosteampy[converter]
+poetry add aiosteampy[all]
 ```
 
 <!--install-end-->
 
 > [!TIP]
-> [aiohttp docs](https://docs.aiohttp.org/en/stable/#installing-all-speedups-in-one-command) recommends installing speedups (`aiodns`, `cchardet`, ...)
+> [aiohttp docs](https://docs.aiohttp.org/en/stable/#installing-all-speedups-in-one-command) recommends installing
+> speedups (`aiodns`, `cchardet`, ...)
 
 <!--intro-start-->
 
 AIOSTEAMPY use [aiohttp](https://github.com/aio-libs/aiohttp) underneath to do asynchronous requests to steam servers,
 with modern async/await syntax.
 
 > Generally, project inspired most
@@ -97,14 +102,15 @@
 
 - Stateless: the main idea was a low-middle layer API wrapper of some steam services and methods like market,
   tradeoffers, confirmations, steamguard, etc. But if you want to cache your entities data (listings, confirmations,
   ...) [there is some methods to help](https://aiosteampy.somespecial.one/examples/states/).
 - Declarative: there is models almost for every data.
 - Typed: for editor support most things are typed.
 - Short: I really tried to fit most important for steam trading methods.
+- Connection behind web proxy.
 
 ## What can I do with this
 
 - Operate with steam trade offers for any manner.
 - Sell, buy items on market. Place, cancel orders.
 - Login trough steam to 3rd party sites.
 - Fetch data from market.
@@ -133,14 +139,16 @@
 
 There is no rules or requirements to contribute. Feedbacks, suggests, other are welcome.
 I will be very grateful for helping me get the things right.
 
 ## Credits
 
 - [bukson/steampy](https://github.com/bukson/steampy)
+- [aiohttp-socks](https://github.com/romis2012/aiohttp-socks)
+- [croniter](https://github.com/kiorky/croniter)
 - [DoctorMcKay/node-steamcommunity](https://github.com/DoctorMcKay/node-steamcommunity)
 - [Identifying Steam items](https://dev.doctormckay.com/topic/332-identifying-steam-items/)
 - [Revadike/InternalSteamWebAPI](https://github.com/Revadike/InternalSteamWebAPI)
 - [Gobot1234/steam.py](https://github.com/Gobot1234/steam.py)
 - [Steam Market id's storage repo](https://github.com/somespecialone/steam-item-name-ids)
 - [steamapi.xpaw.me](https://steamapi.xpaw.me/)
 - [Steam Exchange Rate Tracker](https://github.com/somespecialone/sert)
```

