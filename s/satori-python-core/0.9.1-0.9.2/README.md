# Comparing `tmp/satori_python_core-0.9.1.tar.gz` & `tmp/satori_python_core-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satori_python_core-0.9.1.tar", last modified: Wed Nov 29 15:18:07 2023, max compression
+gzip compressed data, was "satori_python_core-0.9.2.tar", last modified: Wed Dec  6 07:07:02 2023, max compression
```

## Comparing `satori_python_core-0.9.1.tar` & `satori_python_core-0.9.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      953 2023-11-29 15:17:49.441649 satori_python_core-0.9.1/.mina/core.toml
--rw-r--r--   0        0        0     1069 2023-11-29 15:17:49.441649 satori_python_core-0.9.1/LICENSE
--rw-r--r--   0        0        0     2662 2023-11-29 15:17:49.441649 satori_python_core-0.9.1/README.md
--rw-r--r--   0        0        0     2020 2023-11-29 15:18:07.049725 satori_python_core-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1513 2023-11-29 15:17:49.441649 satori_python_core-0.9.1/src/satori/__init__.py
--rw-r--r--   0        0        0     1627 2023-11-29 15:17:49.445649 satori_python_core-0.9.1/src/satori/config.py
--rw-r--r--   0        0        0     2259 2023-11-29 15:17:49.445649 satori_python_core-0.9.1/src/satori/const.py
--rw-r--r--   0        0        0    11809 2023-11-29 15:17:49.445649 satori_python_core-0.9.1/src/satori/element.py
--rw-r--r--   0        0        0      451 2023-11-29 15:17:49.445649 satori_python_core-0.9.1/src/satori/exception.py
--rw-r--r--   0        0        0     8583 2023-11-29 15:17:49.445649 satori_python_core-0.9.1/src/satori/model.py
--rw-r--r--   0        0        0     3805 2023-11-29 15:17:49.445649 satori_python_core-0.9.1/src/satori/parser.py
--rw-r--r--   0        0        0     3626 1970-01-01 00:00:00.000000 satori_python_core-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      953 2023-12-06 07:06:53.073263 satori_python_core-0.9.2/.mina/core.toml
+-rw-r--r--   0        0        0     1069 2023-12-06 07:06:53.073263 satori_python_core-0.9.2/LICENSE
+-rw-r--r--   0        0        0     2662 2023-12-06 07:06:53.073263 satori_python_core-0.9.2/README.md
+-rw-r--r--   0        0        0     2020 2023-12-06 07:07:02.861142 satori_python_core-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1563 2023-12-06 07:06:53.073263 satori_python_core-0.9.2/src/satori/__init__.py
+-rw-r--r--   0        0        0     1627 2023-12-06 07:06:53.073263 satori_python_core-0.9.2/src/satori/config.py
+-rw-r--r--   0        0        0     2259 2023-12-06 07:06:53.073263 satori_python_core-0.9.2/src/satori/const.py
+-rw-r--r--   0        0        0    13593 2023-12-06 07:06:53.073263 satori_python_core-0.9.2/src/satori/element.py
+-rw-r--r--   0        0        0      451 2023-12-06 07:06:53.073263 satori_python_core-0.9.2/src/satori/exception.py
+-rw-r--r--   0        0        0     8751 2023-12-06 07:06:53.073263 satori_python_core-0.9.2/src/satori/model.py
+-rw-r--r--   0        0        0     3805 2023-12-06 07:06:53.073263 satori_python_core-0.9.2/src/satori/parser.py
+-rw-r--r--   0        0        0     3626 1970-01-01 00:00:00.000000 satori_python_core-0.9.2/PKG-INFO
```

### Comparing `satori_python_core-0.9.1/.mina/core.toml` & `satori_python_core-0.9.2/.mina/core.toml`

 * *Files identical despite different names*

### Comparing `satori_python_core-0.9.1/LICENSE` & `satori_python_core-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `satori_python_core-0.9.1/README.md` & `satori_python_core-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `satori_python_core-0.9.1/pyproject.toml` & `satori_python_core-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Operating System :: OS Independent",
 ]
-version = "0.9.1"
+version = "0.9.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/RF-Tar-Railt/satori-python"
 repository = "https://github.com/RF-Tar-Railt/satori-python"
```

### Comparing `satori_python_core-0.9.1/src/satori/__init__.py` & `satori_python_core-0.9.2/src/satori/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,11 +30,12 @@
 from .model import Channel as Channel
 from .model import ChannelType as ChannelType
 from .model import Event as Event
 from .model import Guild as Guild
 from .model import Login as Login
 from .model import LoginStatus as LoginStatus
 from .model import Member as Member
+from .model import MessageObject as MessageObject
 from .model import Role as Role
 from .model import User as User
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
```

### Comparing `satori_python_core-0.9.1/src/satori/config.py` & `satori_python_core-0.9.2/src/satori/config.py`

 * *Files identical despite different names*

### Comparing `satori_python_core-0.9.1/src/satori/const.py` & `satori_python_core-0.9.2/src/satori/const.py`

 * *Files identical despite different names*

### Comparing `satori_python_core-0.9.1/src/satori/element.py` & `satori_python_core-0.9.2/src/satori/element.py`

 * *Files 23% similar despite different names*

```diff
@@ -38,23 +38,27 @@
         attrs = " ".join(_attr(k, v) for k, v in vars(self).items() if not k.startswith("_"))
         attrs = f" {attrs}" if attrs else ""
         return f"<{self.get_type()}{attrs}/>"
 
 
 @dataclass
 class Text(Element):
+    """一段纯文本。"""
+
     text: str
 
     @override
     def __str__(self) -> str:
         return escape(self.text)
 
 
 @dataclass
 class At(Element):
+    """<at> 元素用于提及某个或某些用户。"""
+
     id: Optional[str] = None
     name: Optional[str] = None
     role: Optional[str] = None
     type: Optional[str] = None
 
     @staticmethod
     def at_role(
@@ -66,20 +70,24 @@
     @staticmethod
     def all(here: bool = False) -> "At":
         return At(type="here" if here else "all")
 
 
 @dataclass
 class Sharp(Element):
+    """<sharp> 元素用于提及某个频道。"""
+
     id: str
     name: Optional[str] = None
 
 
 @dataclass
 class Link(Element):
+    """<a> 元素用于显示一个链接。"""
+
     url: str
     display: Optional[str] = None
 
     @classmethod
     @override
     def from_raw(cls, raw: RawElement) -> "Link":
         res = cls(raw.attrs["href"], raw.children[0].attrs["text"] if raw.children else None)
@@ -133,119 +141,152 @@
         if extra:
             for k, v in extra.items():
                 setattr(self, k, True if v is ... else v)
 
 
 @dataclass
 class Image(Resource):
+    """<img> 元素用于表示图片。"""
+
     width: Optional[int] = None
     height: Optional[int] = None
 
     def get_type(self) -> str:
         return "img"
 
 
 @dataclass
 class Audio(Resource):
+    """<audio> 元素用于表示语音。"""
+
     pass
 
 
 @dataclass
 class Video(Resource):
+    """<video> 元素用于表示视频。"""
+
     pass
 
 
 @dataclass
 class File(Resource):
+    """<file> 元素用于表示文件。"""
+
     pass
 
 
 @dataclass
 class Style(Text):
-    @override
     @classmethod
+    @override
     def from_raw(cls, raw: RawElement):
         res = cls(raw.children[0].attrs["text"])
         for k, v in raw.attrs.items():
             setattr(res, k, v)
         return res
 
 
 @dataclass
 class Bold(Style):
+    """<b> 或 <strong> 元素用于将其中的内容以粗体显示。"""
+
     @override
     def __str__(self):
         return f"<b>{escape(self.text)}</b>"
 
 
 @dataclass
 class Italic(Style):
+    """<i> 或 <em> 元素用于将其中的内容以斜体显示。"""
+
     @override
     def __str__(self):
         return f"<i>{escape(self.text)}</i>"
 
 
 @dataclass
 class Underline(Style):
+    """<u> 或 <ins> 元素用于为其中的内容附加下划线。"""
+
     @override
     def __str__(self):
         return f"<u>{escape(self.text)}</u>"
 
 
 @dataclass
 class Strikethrough(Style):
+    """<s> 或 <del> 元素用于为其中的内容附加删除线。"""
+
     @override
     def __str__(self):
         return f"<s>{escape(self.text)}</s>"
 
 
 @dataclass
 class Spoiler(Style):
+    """<spl> 元素用于将其中的内容标记为剧透 (默认会被隐藏，点击后才显示)。"""
+
     @override
     def __str__(self):
         return f"<spl>{escape(self.text)}</spl>"
 
 
 @dataclass
 class Code(Style):
+    """<code> 元素用于将其中的内容以等宽字体显示 (通常还会有特定的背景色)。"""
+
     @override
     def __str__(self):
         return f"<code>{escape(self.text)}</code>"
 
 
 @dataclass
 class Superscript(Style):
+    """<sup> 元素用于将其中的内容以上标显示。"""
+
     @override
     def __str__(self):
         return f"<sup>{escape(self.text)}</sup>"
 
 
 @dataclass
 class Subscript(Style):
+    """<sub> 元素用于将其中的内容以下标显示。"""
+
     @override
     def __str__(self):
         return f"<sub>{escape(self.text)}</sub>"
 
 
 @dataclass
 class Br(Style):
+    """<br> 元素表示一个独立的换行。"""
+
     @override
     def __str__(self):
         return "<br/>"
 
 
 @dataclass
 class Paragraph(Style):
+    """<p> 元素表示一个段落。在渲染时，它与相邻的元素之间会确保有一个换行。"""
+
     @override
     def __str__(self):
         return f"<p>{escape(self.text)}</p>"
 
 
 @dataclass
 class Message(Element):
+    """<message> 元素的基本用法是表示一条消息。
+
+    子元素对应于消息的内容。如果其没有子元素，则消息不会被发送。
+    """
+
     id: Optional[str]
     forward: Optional[bool]
     content: List[Element]
 
     def __init__(
         self,
         id: Optional[str] = None,
@@ -273,26 +314,35 @@
             return f"<{_type}{attrs}/>"
         else:
             return f'<{_type}{attrs}>{"".join(str(e) for e in self.content)}</{_type}>'
 
 
 @dataclass
 class Quote(Message):
+    """<quote> 元素用于表示对消息引用。
+
+    它的子元素会被渲染为引用的内容。
+    """
+
     pass
 
 
 @dataclass
 class Author(Element):
+    """<author> 元素用于表示消息的作者。它的子元素会被渲染为作者的名字。"""
+
     id: str
     nickname: Optional[str] = None
     avatar: Optional[str] = None
 
 
 @dataclass
 class Button(Element):
+    """<button> 元素用于表示一个按钮。它的子元素会被渲染为按钮的文本。"""
+
     type: str
     display: Optional[str] = None
     id: Optional[str] = None
     href: Optional[str] = None
     text: Optional[str] = None
     theme: Optional[str] = None
 
@@ -329,14 +379,16 @@
         if self.display:
             return f'<button {" ".join(attr)}>{escape(self.display)}</button>'
         return f'<button {" ".join(attr)} />'
 
 
 @dataclass
 class Custom(Element):
+    """自定义元素用于构造标准元素以外的元素"""
+
     type: str
     attrs: Dict[str, Any]
     children: List[Element]
 
     def __init__(
         self,
         type: str,
@@ -371,14 +423,16 @@
         if self.children:
             return f"<{self.get_type()}{attrs}>{''.join(str(e) for e in self.children)}</{self.get_type()}>"
         return f"<{self.get_type()}{attrs}/>"
 
 
 @dataclass
 class Raw(Element):
+    """Raw 元素表示原始文本"""
+
     content: str
 
     @override
     def __str__(self):
         return self.content
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `satori_python_core-0.9.1/src/satori/model.py` & `satori_python_core-0.9.2/src/satori/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,54 +55,58 @@
         return res
 
 
 @dataclass
 class User:
     id: str
     name: Optional[str] = None
+    nick: Optional[str] = None
     avatar: Optional[str] = None
     is_bot: Optional[bool] = None
 
     @classmethod
     def parse(cls, raw: dict):
         return cls(**raw)
 
     def dump(self):
         res: Dict[str, Any] = {"id": self.id}
         if self.name:
             res["name"] = self.name
+        if self.nick:
+            res["nick"] = self.nick
         if self.avatar:
             res["avatar"] = self.avatar
         if self.is_bot:
             res["is_bot"] = self.is_bot
         return res
 
 
 @dataclass
 class Member:
     user: Optional[User] = None
+    nick: Optional[str] = None
     name: Optional[str] = None
     avatar: Optional[str] = None
     joined_at: Optional[datetime] = None
 
     @classmethod
     def parse(cls, raw: dict):
         data = raw.copy()
         if "user" in raw:
-            data["user"] = User(**raw["user"])
+            data["user"] = User.parse(raw["user"])
         if "joined_at" in raw:
             data["joined_at"] = datetime.fromtimestamp(int(raw["joined_at"]) / 1000)
         return cls(**data)
 
     def dump(self):
         res = {}
         if self.user:
             res["user"] = self.user.dump()
-        if self.name:
-            res["name"] = self.name
+        if self.nick or self.name:
+            res["nick"] = self.nick or self.name
         if self.avatar:
             res["avatar"] = self.avatar
         if self.joined_at:
             res["joined_at"] = int(self.joined_at.timestamp() * 1000)
         return res
 
 
@@ -190,15 +194,15 @@
 
 @dataclass
 class Ready:
     logins: List[Login]
 
 
 @dataclass
-class Message:
+class MessageObject:
     id: str
     content: List[Element]
     channel: Optional[Channel] = None
     guild: Optional[Guild] = None
     member: Optional[Member] = None
     user: Optional[User] = None
     created_at: Optional[datetime] = None
@@ -250,15 +254,15 @@
     timestamp: datetime
     argv: Optional[ArgvInteraction] = None
     button: Optional[ButtonInteraction] = None
     channel: Optional[Channel] = None
     guild: Optional[Guild] = None
     login: Optional[Login] = None
     member: Optional[Member] = None
-    message: Optional[Message] = None
+    message: Optional[MessageObject] = None
     operator: Optional[User] = None
     role: Optional[Role] = None
     user: Optional[User] = None
 
     @classmethod
     def parse(cls, raw: dict):
         data = {
@@ -277,15 +281,15 @@
         if "guild" in raw:
             data["guild"] = Guild.parse(raw["guild"])
         if "login" in raw:
             data["login"] = Login.parse(raw["login"])
         if "member" in raw:
             data["member"] = Member.parse(raw["member"])
         if "message" in raw:
-            data["message"] = Message.parse(raw["message"])
+            data["message"] = MessageObject.parse(raw["message"])
         if "operator" in raw:
             data["operator"] = User.parse(raw["operator"])
         if "role" in raw:
             data["role"] = Role.parse(raw["role"])
         if "user" in raw:
             data["user"] = User.parse(raw["user"])
         return cls(**data)
```

### Comparing `satori_python_core-0.9.1/src/satori/parser.py` & `satori_python_core-0.9.2/src/satori/parser.py`

 * *Files identical despite different names*

### Comparing `satori_python_core-0.9.1/PKG-INFO` & `satori_python_core-0.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satori-python-core
-Version: 0.9.1
+Version: 0.9.2
 Summary: Satori Protocol SDK for python, specify common part
 Home-page: https://github.com/RF-Tar-Railt/satori-python
 Author-Email: RF-Tar-Railt <rf_tar_railt@qq.com>
 License: MIT
 Classifier: Typing :: Typed
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

