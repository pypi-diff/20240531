# Comparing `tmp/rov_db_access-1.0.8.tar.gz` & `tmp/rov_db_access-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rov_db_access-1.0.8.tar", max compression
+gzip compressed data, was "rov_db_access-1.0.9.tar", max compression
```

## Comparing `rov_db_access-1.0.8.tar` & `rov_db_access-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0        0 2024-01-29 18:44:26.776172 rov_db_access-1.0.8/README.md
--rw-r--r--   0        0        0      561 2024-05-30 16:31:48.626463 rov_db_access-1.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-20 20:01:43.946199 rov_db_access-1.0.8/rov_db_access/__init__.py
--rw-r--r--   0        0        0        0 2024-05-08 18:50:41.475751 rov_db_access-1.0.8/rov_db_access/authentication/__init__.py
--rw-r--r--   0        0        0     2332 2024-05-20 20:01:43.946696 rov_db_access-1.0.8/rov_db_access/authentication/models.py
--rw-r--r--   0        0        0     2483 2024-05-30 16:31:48.626817 rov_db_access-1.0.8/rov_db_access/authentication/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.917823 rov_db_access-1.0.8/rov_db_access/config/__init__.py
--rw-r--r--   0        0        0     2069 2024-05-15 15:24:19.907085 rov_db_access-1.0.8/rov_db_access/config/db_utils.py
--rw-r--r--   0        0        0      983 2024-05-20 20:01:43.947272 rov_db_access-1.0.8/rov_db_access/config/settings.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.918355 rov_db_access-1.0.8/rov_db_access/geodata/__init__.py
--rw-r--r--   0        0        0     1966 2024-05-20 13:50:20.918452 rov_db_access-1.0.8/rov_db_access/geodata/models.py
--rw-r--r--   0        0        0        0 2024-05-08 18:50:41.476424 rov_db_access-1.0.8/rov_db_access/gis/__init__.py
--rw-r--r--   0        0        0     8313 2024-05-28 22:12:46.563385 rov_db_access-1.0.8/rov_db_access/gis/models.py
--rw-r--r--   0        0        0       78 2024-05-20 13:50:20.918762 rov_db_access-1.0.8/rov_db_access/gis/test.py
--rw-r--r--   0        0        0    36288 2024-05-30 16:31:48.627256 rov_db_access-1.0.8/rov_db_access/gis/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.919463 rov_db_access-1.0.8/rov_db_access/ine/__init__.py
--rw-r--r--   0        0        0      850 2024-05-20 13:50:20.919583 rov_db_access-1.0.8/rov_db_access/ine/models.py
--rw-r--r--   0        0        0     2298 2024-05-20 13:50:20.919670 rov_db_access-1.0.8/rov_db_access/ine/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.919752 rov_db_access-1.0.8/rov_db_access/label_studio/__init__.py
--rw-r--r--   0        0        0     9115 2024-05-20 13:50:20.919967 rov_db_access-1.0.8/rov_db_access/label_studio/models.py
--rw-r--r--   0        0        0     7153 2024-05-20 13:50:20.920121 rov_db_access-1.0.8/rov_db_access/label_studio/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.920191 rov_db_access-1.0.8/rov_db_access/landing/__init__.py
--rw-r--r--   0        0        0     2124 2024-05-20 13:50:20.920282 rov_db_access-1.0.8/rov_db_access/landing/models.py
--rw-r--r--   0        0        0     5890 2024-05-20 13:50:20.920415 rov_db_access-1.0.8/rov_db_access/landing/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.920480 rov_db_access-1.0.8/rov_db_access/risks/__init__.py
--rw-r--r--   0        0        0     1176 2024-05-20 13:50:20.920564 rov_db_access-1.0.8/rov_db_access/risks/models.py
--rw-r--r--   0        0        0     6554 2024-05-27 19:05:01.933210 rov_db_access-1.0.8/rov_db_access/risks/worker.py
--rw-r--r--   0        0        0        0 2024-05-08 18:50:41.476890 rov_db_access-1.0.8/rov_db_access/sentinel/__init__.py
--rw-r--r--   0        0        0      412 2024-05-08 18:50:41.477041 rov_db_access-1.0.8/rov_db_access/sentinel/models.py
--rw-r--r--   0        0        0     5878 2024-05-20 13:50:20.921035 rov_db_access-1.0.8/rov_db_access/sentinel/worker.py
--rw-r--r--   0        0        0        0 2024-05-20 13:50:20.921067 rov_db_access-1.0.8/rov_db_access/utils/__init__.py
--rw-r--r--   0        0        0     5317 2024-05-20 20:01:43.948847 rov_db_access-1.0.8/rov_db_access/utils/geoserver_utils.py
--rw-r--r--   0        0        0     2078 2024-05-20 20:01:43.949178 rov_db_access-1.0.8/rov_db_access/utils/s3_utils.py
--rw-r--r--   0        0        0     1120 2024-05-20 13:50:20.921348 rov_db_access-1.0.8/rov_db_access/utils/utils.py
--rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 rov_db_access-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      587 2024-05-30 19:01:48.420519 rov_db_access-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-11-28 21:38:40.450138 rov_db_access-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 16:54:43.733541 rov_db_access-1.0.9/rov_db_access/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.778226 rov_db_access-1.0.9/rov_db_access/authentication/__init__.py
+-rw-r--r--   0        0        0     2394 2024-05-22 20:36:01.745636 rov_db_access-1.0.9/rov_db_access/authentication/models.py
+-rw-r--r--   0        0        0     2557 2024-05-30 19:01:48.421568 rov_db_access-1.0.9/rov_db_access/authentication/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:52:58.172569 rov_db_access-1.0.9/rov_db_access/config/__init__.py
+-rw-r--r--   0        0        0     2133 2024-05-14 15:53:52.686829 rov_db_access-1.0.9/rov_db_access/config/db_utils.py
+-rw-r--r--   0        0        0     1029 2024-05-27 16:53:58.265335 rov_db_access-1.0.9/rov_db_access/config/settings.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:52:58.174567 rov_db_access-1.0.9/rov_db_access/geodata/__init__.py
+-rw-r--r--   0        0        0     2032 2024-05-17 19:52:58.176075 rov_db_access-1.0.9/rov_db_access/geodata/models.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.782941 rov_db_access-1.0.9/rov_db_access/gis/__init__.py
+-rw-r--r--   0        0        0     8508 2024-05-30 19:01:48.422632 rov_db_access-1.0.9/rov_db_access/gis/models.py
+-rw-r--r--   0        0        0       81 2024-05-17 19:52:58.176594 rov_db_access-1.0.9/rov_db_access/gis/test.py
+-rw-r--r--   0        0        0    37360 2024-05-30 19:01:48.423689 rov_db_access-1.0.9/rov_db_access/gis/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:52:58.178602 rov_db_access-1.0.9/rov_db_access/ine/__init__.py
+-rw-r--r--   0        0        0      875 2024-05-17 19:52:58.178602 rov_db_access-1.0.9/rov_db_access/ine/models.py
+-rw-r--r--   0        0        0     2368 2024-05-27 16:54:12.750177 rov_db_access-1.0.9/rov_db_access/ine/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:52:58.179605 rov_db_access-1.0.9/rov_db_access/label_studio/__init__.py
+-rw-r--r--   0        0        0     9336 2024-05-17 19:52:58.180604 rov_db_access-1.0.9/rov_db_access/label_studio/models.py
+-rw-r--r--   0        0        0     7363 2024-05-17 19:52:58.181603 rov_db_access-1.0.9/rov_db_access/label_studio/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:52:58.181603 rov_db_access-1.0.9/rov_db_access/landing/__init__.py
+-rw-r--r--   0        0        0     2188 2024-05-17 19:52:58.182603 rov_db_access-1.0.9/rov_db_access/landing/models.py
+-rw-r--r--   0        0        0     6062 2024-05-17 19:52:58.183605 rov_db_access-1.0.9/rov_db_access/landing/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:52:58.184605 rov_db_access-1.0.9/rov_db_access/risks/__init__.py
+-rw-r--r--   0        0        0     1201 2024-05-17 19:52:58.184605 rov_db_access-1.0.9/rov_db_access/risks/models.py
+-rw-r--r--   0        0        0     6701 2024-05-30 19:01:48.424738 rov_db_access-1.0.9/rov_db_access/risks/worker.py
+-rw-r--r--   0        0        0        0 2024-04-19 20:09:14.791048 rov_db_access-1.0.9/rov_db_access/sentinel/__init__.py
+-rw-r--r--   0        0        0      427 2024-04-19 20:09:14.792050 rov_db_access-1.0.9/rov_db_access/sentinel/models.py
+-rw-r--r--   0        0        0     6053 2024-05-27 16:54:19.691495 rov_db_access-1.0.9/rov_db_access/sentinel/worker.py
+-rw-r--r--   0        0        0        0 2024-05-17 19:52:58.186636 rov_db_access-1.0.9/rov_db_access/utils/__init__.py
+-rw-r--r--   0        0        0     5461 2024-05-27 16:54:25.573783 rov_db_access-1.0.9/rov_db_access/utils/geoserver_utils.py
+-rw-r--r--   0        0        0     2141 2024-05-27 16:54:35.144230 rov_db_access-1.0.9/rov_db_access/utils/s3_utils.py
+-rw-r--r--   0        0        0     1157 2024-05-17 19:52:58.187649 rov_db_access-1.0.9/rov_db_access/utils/utils.py
+-rw-r--r--   0        0        0      965 1970-01-01 00:00:00.000000 rov_db_access-1.0.9/PKG-INFO
```

### Comparing `rov_db_access-1.0.8/rov_db_access/authentication/models.py` & `rov_db_access-1.0.9/rov_db_access/authentication/models.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from sqlalchemy import DateTime, ForeignKey, func
-from sqlalchemy.orm import DeclarativeBase, relationship
-from typing import Optional, List
-from datetime import datetime
-from sqlalchemy.orm import Mapped
-from sqlalchemy.orm import mapped_column
-
-
-class Base(DeclarativeBase):
-    """Base Class of the model"""
-
-
-class Organization(Base):
-    __tablename__ = "organization"
-    __table_args__ = {"schema": "admin"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[str]
-    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
-    bucket: Mapped[str] = mapped_column(server_default='upload-tif-images-test')
-    workspace: Mapped[str] = mapped_column(server_default='rovisen')
-    users: Mapped[List["User"]] = relationship(
-        back_populates='organization',
-        order_by="User.id"
-    )
-
-    def __repr__(self) -> str:
-        return f"Organization(id={self.id!r}, name={self.name!r}, #users={len(self.users)!r})"
-
-
-class User(Base):
-    __tablename__ = "user"
-    __table_args__ = {"schema": "admin"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    username: Mapped[str]
-    password: Mapped[str]
-    logged_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True))
-    organization_id: Mapped[int] = mapped_column(ForeignKey("admin.organization.id"))
-    organization: Mapped["Organization"] = relationship(back_populates="users")
-    roles: Mapped[List["Role"]] = relationship(secondary="admin.association_user_role")
-
-    def __repr__(self) -> str:
-        return f"User(id={self.id!r}, username={self.username!r}, logged_at={self.logged_at!r})"
-
-
-class Role(Base):
-    __tablename__ = "role"
-    __table_args__ = {"schema": "admin"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[str]
-
-    def __repr__(self) -> str:
-        return f"Role(id={self.id!r}, name={self.name!r})"
-
-
-class AssociationUserRole(Base):
-    __tablename__ = "association_user_role"
-    __table_args__ = {"schema": "admin"}
-    user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"), primary_key=True)
-    role_id: Mapped[int] = mapped_column(ForeignKey("admin.role.id"), primary_key=True)
-
-    def __repr__(self) -> str:
-        return f"AssociationUserRole(user_id={self.user_id!r}, role_id={self.role_id!r})"
+from sqlalchemy import DateTime, ForeignKey, func
+from sqlalchemy.orm import DeclarativeBase, relationship
+from typing import Optional, List
+from datetime import datetime
+from sqlalchemy.orm import Mapped
+from sqlalchemy.orm import mapped_column
+
+
+class Base(DeclarativeBase):
+    """Base Class of the model"""
+
+
+class Organization(Base):
+    __tablename__ = "organization"
+    __table_args__ = {"schema": "admin"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str]
+    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
+    bucket: Mapped[str] = mapped_column(server_default='upload-tif-images-test')
+    workspace: Mapped[str] = mapped_column(server_default='rovisen')
+    users: Mapped[List["User"]] = relationship(
+        back_populates='organization',
+        order_by="User.id"
+    )
+
+    def __repr__(self) -> str:
+        return f"Organization(id={self.id!r}, name={self.name!r}, #users={len(self.users)!r})"
+
+
+class User(Base):
+    __tablename__ = "user"
+    __table_args__ = {"schema": "admin"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    username: Mapped[str]
+    password: Mapped[str]
+    logged_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True))
+    organization_id: Mapped[int] = mapped_column(ForeignKey("admin.organization.id"))
+    organization: Mapped["Organization"] = relationship(back_populates="users")
+    roles: Mapped[List["Role"]] = relationship(secondary="admin.association_user_role")
+
+    def __repr__(self) -> str:
+        return f"User(id={self.id!r}, username={self.username!r}, logged_at={self.logged_at!r})"
+
+
+class Role(Base):
+    __tablename__ = "role"
+    __table_args__ = {"schema": "admin"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str]
+
+    def __repr__(self) -> str:
+        return f"Role(id={self.id!r}, name={self.name!r})"
+
+
+class AssociationUserRole(Base):
+    __tablename__ = "association_user_role"
+    __table_args__ = {"schema": "admin"}
+    user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"), primary_key=True)
+    role_id: Mapped[int] = mapped_column(ForeignKey("admin.role.id"), primary_key=True)
+
+    def __repr__(self) -> str:
+        return f"AssociationUserRole(user_id={self.user_id!r}, role_id={self.role_id!r})"
```

### Comparing `rov_db_access-1.0.8/rov_db_access/config/db_utils.py` & `rov_db_access-1.0.9/rov_db_access/config/db_utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-from sqlalchemy import Engine, create_engine, select
-from sqlalchemy.orm import Session
-from psycopg2 import OperationalError
-
-
-def init_db_engine(
-    db_user: str, db_password: str, db_host: str, db_port: str, db_name: str
-) -> Engine:
-    """Initializes sqlalchemy engine that connects to postgis database
-
-    Args:
-        db_user (str): the user name
-        db_password (str): the password
-        db_host (str): the url of the database host
-        db_port (str): the port of the connection
-        db_name (str): the name of the database
-
-    Returns:
-        Engine: connection to postgis database
-    """
-    return create_engine(
-        f"postgresql+psycopg2://{db_user}:{db_password}@{db_host}:{db_port}/{db_name}"
-    )
-
-
-class BaseWorker:
-    def __init__(self, db_user, db_password, db_host, db_port, db_name):
-        self.db_user = db_user
-        self.db_password = db_password
-        self.db_host = db_host
-        self.db_port = db_port
-        self.db_name = db_name
-
-        self.engine = self.init_db_engine()
-        self.session = Session(self.engine)
-
-    def init_db_engine(self) -> Engine:
-        """Initializes sqlalchemy engine that connects to postgis database
-
-        Args:
-            db_user (str): the user name
-            db_password (str): the password
-            db_host (str): the url of the database host
-            db_port (str): the port of the connection
-            db_name (str): the name of the database
-
-        Returns:
-            Engine: connection to postgis database
-        """
-        return create_engine(
-            f"postgresql+psycopg2://{self.db_user}:{self.db_password}@{self.db_host}:{self.db_port}/{self.db_name}"
-        )
-
-    def check_db_connection(self):
-        try:
-            self.session.execute(select(1))
-        except OperationalError as e:
-            print(f"Database connection error: {e}")
-            self.reconnect_db()
-
-    def reconnect_db(self):
-        self.engine = self.init_db_engine()
-        self.session = Session(self.engine)
-        print("Reconnected to database")
+from sqlalchemy import Engine, create_engine, select
+from sqlalchemy.orm import Session
+from psycopg2 import OperationalError
+
+
+def init_db_engine(
+    db_user: str, db_password: str, db_host: str, db_port: str, db_name: str
+) -> Engine:
+    """Initializes sqlalchemy engine that connects to postgis database
+
+    Args:
+        db_user (str): the user name
+        db_password (str): the password
+        db_host (str): the url of the database host
+        db_port (str): the port of the connection
+        db_name (str): the name of the database
+
+    Returns:
+        Engine: connection to postgis database
+    """
+    return create_engine(
+        f"postgresql+psycopg2://{db_user}:{db_password}@{db_host}:{db_port}/{db_name}"
+    )
+
+
+class BaseWorker:
+    def __init__(self, db_user, db_password, db_host, db_port, db_name):
+        self.db_user = db_user
+        self.db_password = db_password
+        self.db_host = db_host
+        self.db_port = db_port
+        self.db_name = db_name
+
+        self.engine = self.init_db_engine()
+        self.session = Session(self.engine)
+
+    def init_db_engine(self) -> Engine:
+        """Initializes sqlalchemy engine that connects to postgis database
+
+        Args:
+            db_user (str): the user name
+            db_password (str): the password
+            db_host (str): the url of the database host
+            db_port (str): the port of the connection
+            db_name (str): the name of the database
+
+        Returns:
+            Engine: connection to postgis database
+        """
+        return create_engine(
+            f"postgresql+psycopg2://{self.db_user}:{self.db_password}@{self.db_host}:{self.db_port}/{self.db_name}"
+        )
+
+    def check_db_connection(self):
+        try:
+            self.session.execute(select(1))
+        except OperationalError as e:
+            print(f"Database connection error: {e}")
+            self.reconnect_db()
+
+    def reconnect_db(self):
+        self.engine = self.init_db_engine()
+        self.session = Session(self.engine)
+        print("Reconnected to database")
```

### Comparing `rov_db_access-1.0.8/rov_db_access/gis/models.py` & `rov_db_access-1.0.9/rov_db_access/gis/models.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,195 +1,195 @@
-from geoalchemy2 import Geometry
-from typing import List
-from typing import Optional
-from datetime import datetime
-from sqlalchemy.orm import Mapped
-from sqlalchemy.orm import mapped_column
-from sqlalchemy.orm import relationship
-from sqlalchemy import ForeignKey, DateTime, func
-from sqlalchemy import JSON
-
-from rov_db_access.authentication.models import Organization, User, Base
-
-
-class Image(Base):
-    __tablename__ = "image"
-    __table_args__ = {"schema": "gis"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[Optional[str]]
-    url: Mapped[str]
-    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
-
-    data: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
-
-    user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"))
-    user: Mapped["User"] = relationship()
-
-    organization_id: Mapped[int] = mapped_column(ForeignKey("admin.organization.id"))
-    organization: Mapped["Organization"] = relationship()
-
-    bbox: Mapped[Geometry] = mapped_column(Geometry("POLYGON", srid=4326))
-    footprint: Mapped[Optional[Geometry]] = mapped_column(Geometry("POLYGON", srid=4326))
-
-    def __repr__(self) -> str:
-        return f"Image (id={self.id!r}, name={self.name!r}, url={self.url!r}, user_id={self.user_id!r}, organization_id={self.organization_id!r})"
-
-
-class InferenceModel(Base):
-    __tablename__ = "inference_model"
-    __table_args__ = {"schema": "gis"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[str]
-    title: Mapped[str]
-    description: Mapped[str]
-    img_url: Mapped[str]
-    price: Mapped[int] = mapped_column(server_default='0')
-    min_resolution: Mapped[float]
-    config: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
-
-    def __repr__(self) -> str:
-        return f"InferenceModel (id={self.id!r}, name={self.name!r}, price={self.price!r}, config={self.config!r})"
-
-
-class Mosaic(Base):
-    __tablename__ = "mosaic"
-    __table_args__ = {"schema": "gis"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[str]
-    description: Mapped[Optional[str]]
-    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
-    coverage_store: Mapped[str] = mapped_column(unique=True)
-
-    organization_id: Mapped[int] = mapped_column(ForeignKey("admin.organization.id"))
-    organization: Mapped["Organization"] = relationship()
-
-    def __repr__(self) -> str:
-        return f"Mosaic (id={self.id!r}, name={self.name!r}, organization_id={self.organization_id!r})"
-
-
-class Process(Base):
-    __tablename__ = "process"
-    __table_args__ = {"schema": "gis"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[str]
-    status: Mapped[str] = mapped_column(server_default="queued")
-    type: Mapped[str] = mapped_column(server_default="on demand")
-    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
-    finished_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True))
-    runtime: Mapped[int] = mapped_column(server_default="0")
-    area: Mapped[float] = mapped_column(server_default="0")
-    cost_estimated: Mapped[float] = mapped_column(server_default="0")
-
-    geom: Mapped[Optional[Geometry]] = mapped_column(Geometry("POLYGON", srid=4326))
-    mask: Mapped[Optional[Geometry]] = mapped_column(Geometry("POLYGON", srid=4326))
-
-    inference_model_id: Mapped[int] = mapped_column(ForeignKey("gis.inference_model.id"))
-    inference_model: Mapped["InferenceModel"] = relationship()
-
-    organization_id: Mapped[int] = mapped_column(ForeignKey("admin.organization.id"))
-    organization: Mapped["Organization"] = relationship()
-
-    user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"))
-    user: Mapped["User"] = relationship()
-
-    runs: Mapped[List["Run"]] = relationship(
-       back_populates="process",
-       order_by="Run.id",
-       cascade="all, delete"
-    )
-
-    def __repr__(self) -> str:
-        return f"Process(id={self.id!r}, name={self.name!r}, status={self.status!r}, inference_model_id={self.inference_model_id!r}), user_id={self.user_id!r})"
-
-
-class ResultsRaster(Base):
-    __tablename__ = "results_raster"
-    __table_args__ = {"schema": "gis"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    url: Mapped[str]
-    data: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
-    bbox: Mapped[Optional[Geometry]] = mapped_column(Geometry("POLYGON", srid=4326))
-
-    run_data_id: Mapped[int] = mapped_column(ForeignKey("gis.run_data.id", ondelete="CASCADE"))
-    run_data: Mapped["RunData"] = relationship(back_populates="results_raster")
-
-    def __repr__(self) -> str:
-        return f"ResultsRaster(id={self.id!r}, url={self.url!r}, run_data_id={self.run_data_id!r})"
-
-
-class ResultsVector(Base):
-    __tablename__ = "results_vector"
-    __table_args__ = {"schema": "gis"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    data: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
-    geom: Mapped[Geometry] = mapped_column(Geometry("MULTIPOLYGON", srid=4326))
-
-    run_data_id: Mapped[int] = mapped_column(ForeignKey("gis.run_data.id", ondelete="CASCADE"))
-    run_data: Mapped["RunData"] = relationship(back_populates="results_vector")
-
-    def __repr__(self) -> str:
-        return f"ResultsVector(id={self.id!r}, data={self.data!r}, geom={self.geom!r}, run_data_id={self.run_data_id!r})"
-
-
-class Run(Base):
-    __tablename__ = "run"
-    __table_args__ = {"schema": "gis"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    status: Mapped[str] = mapped_column(server_default="queued")
-    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
-    finished_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True))
-    engine: Mapped[str] = mapped_column(server_default="local")
-    runtime: Mapped[int] = mapped_column(server_default="0")
-    cost: Mapped[float] = mapped_column(server_default="0")
-
-    input_id: Mapped[int] = mapped_column(ForeignKey("gis.run_data.id", ondelete="CASCADE"), nullable=False)
-    input: Mapped["RunData"] = relationship("RunData", foreign_keys=[input_id])
-
-    output_id: Mapped[int] = mapped_column(ForeignKey("gis.run_data.id", ondelete="CASCADE"), nullable=False)
-    output: Mapped[Optional["RunData"]] = relationship("RunData", foreign_keys=[output_id])
-
-    inference_model_id: Mapped[int] = mapped_column(ForeignKey("gis.inference_model.id"))
-    inference_model: Mapped["InferenceModel"] = relationship()
-
-    process_id: Mapped[int] = mapped_column(ForeignKey("gis.process.id", ondelete="CASCADE"))
-    process: Mapped["Process"] = relationship()
-
-    def __repr__(self) -> str:
-        return f"Run(id={self.id!r}, status={self.status!r}, process_id={self.process_id!r}) inference_model_id={self.inference_model_id!r}, input_id={self.input_id}, output_id={self.output_id})"
-
-
-class RunData(Base):
-    __tablename__ = "run_data"
-    __table_args__ = {"schema": "gis"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    type: Mapped[str] = mapped_column(server_default='upload')
-    status: Mapped[str] = mapped_column(server_default='ready')
-    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
-
-    data: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
-
-    user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"))
-    user: Mapped["User"] = relationship()
-
-    organization_id: Mapped[int] = mapped_column(ForeignKey("admin.organization.id"))
-    organization: Mapped["Organization"] = relationship()
-
-    #used_by: Mapped[List["Run"]] = relationship(foreign_keys='id')
-    #
-    # origin_run: Mapped[Optional["Run"]] = relationship(
-    #     back_populates="output"
-    # )
-
-    results_vector: Mapped[List["ResultsVector"]] = relationship(
-       back_populates="run_data",
-       order_by="ResultsVector.id",
-       cascade="all, delete"
-    )
-
-    results_raster: Mapped[List["ResultsRaster"]] = relationship(
-        back_populates="run_data",
-        order_by="ResultsRaster.id",
-        cascade="all, delete"
-    )
-
-    def __repr__(self) -> str:
-        return f"RunData (id={self.id!r}, user_id={self.user_id!r}, status={self.status}, data={self.data}"
+from geoalchemy2 import Geometry
+from typing import List
+from typing import Optional
+from datetime import datetime
+from sqlalchemy.orm import Mapped
+from sqlalchemy.orm import mapped_column
+from sqlalchemy.orm import relationship
+from sqlalchemy import ForeignKey, DateTime, func
+from sqlalchemy import JSON
+
+from rov_db_access.authentication.models import Organization, User, Base
+
+
+class Image(Base):
+    __tablename__ = "image"
+    __table_args__ = {"schema": "gis"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[Optional[str]]
+    url: Mapped[str]
+    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
+
+    data: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
+
+    user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"))
+    user: Mapped["User"] = relationship()
+
+    organization_id: Mapped[int] = mapped_column(ForeignKey("admin.organization.id"))
+    organization: Mapped["Organization"] = relationship()
+
+    bbox: Mapped[Geometry] = mapped_column(Geometry("POLYGON", srid=4326))
+    footprint: Mapped[Optional[Geometry]] = mapped_column(Geometry("POLYGON", srid=4326))
+
+    def __repr__(self) -> str:
+        return f"Image (id={self.id!r}, name={self.name!r}, url={self.url!r}, user_id={self.user_id!r}, organization_id={self.organization_id!r})"
+
+
+class InferenceModel(Base):
+    __tablename__ = "inference_model"
+    __table_args__ = {"schema": "gis"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str]
+    title: Mapped[str]
+    description: Mapped[str]
+    img_url: Mapped[str]
+    price: Mapped[int] = mapped_column(server_default='0')
+    min_resolution: Mapped[float]
+    config: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
+
+    def __repr__(self) -> str:
+        return f"InferenceModel (id={self.id!r}, name={self.name!r}, price={self.price!r}, config={self.config!r})"
+
+
+class Mosaic(Base):
+    __tablename__ = "mosaic"
+    __table_args__ = {"schema": "gis"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str]
+    description: Mapped[Optional[str]]
+    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
+    coverage_store: Mapped[str] = mapped_column(unique=True)
+
+    organization_id: Mapped[int] = mapped_column(ForeignKey("admin.organization.id"))
+    organization: Mapped["Organization"] = relationship()
+
+    def __repr__(self) -> str:
+        return f"Mosaic (id={self.id!r}, name={self.name!r}, organization_id={self.organization_id!r})"
+
+
+class Process(Base):
+    __tablename__ = "process"
+    __table_args__ = {"schema": "gis"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str]
+    status: Mapped[str] = mapped_column(server_default="queued")
+    type: Mapped[str] = mapped_column(server_default="on demand")
+    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
+    finished_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True))
+    runtime: Mapped[int] = mapped_column(server_default="0")
+    area: Mapped[float] = mapped_column(server_default="0")
+    cost_estimated: Mapped[float] = mapped_column(server_default="0")
+
+    geom: Mapped[Optional[Geometry]] = mapped_column(Geometry("POLYGON", srid=4326))
+    mask: Mapped[Optional[Geometry]] = mapped_column(Geometry("POLYGON", srid=4326))
+
+    inference_model_id: Mapped[int] = mapped_column(ForeignKey("gis.inference_model.id"))
+    inference_model: Mapped["InferenceModel"] = relationship()
+
+    organization_id: Mapped[int] = mapped_column(ForeignKey("admin.organization.id"))
+    organization: Mapped["Organization"] = relationship()
+
+    user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"))
+    user: Mapped["User"] = relationship()
+
+    runs: Mapped[List["Run"]] = relationship(
+       back_populates="process",
+       order_by="Run.id",
+       cascade="all, delete"
+    )
+
+    def __repr__(self) -> str:
+        return f"Process(id={self.id!r}, name={self.name!r}, status={self.status!r}, inference_model_id={self.inference_model_id!r}), user_id={self.user_id!r})"
+
+
+class ResultsRaster(Base):
+    __tablename__ = "results_raster"
+    __table_args__ = {"schema": "gis"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    url: Mapped[str]
+    data: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
+    bbox: Mapped[Optional[Geometry]] = mapped_column(Geometry("POLYGON", srid=4326))
+
+    run_data_id: Mapped[int] = mapped_column(ForeignKey("gis.run_data.id", ondelete="CASCADE"))
+    run_data: Mapped["RunData"] = relationship(back_populates="results_raster")
+
+    def __repr__(self) -> str:
+        return f"ResultsRaster(id={self.id!r}, url={self.url!r}, run_data_id={self.run_data_id!r})"
+
+
+class ResultsVector(Base):
+    __tablename__ = "results_vector"
+    __table_args__ = {"schema": "gis"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    data: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
+    geom: Mapped[Geometry] = mapped_column(Geometry("MULTIPOLYGON", srid=4326))
+
+    run_data_id: Mapped[int] = mapped_column(ForeignKey("gis.run_data.id", ondelete="CASCADE"))
+    run_data: Mapped["RunData"] = relationship(back_populates="results_vector")
+
+    def __repr__(self) -> str:
+        return f"ResultsVector(id={self.id!r}, data={self.data!r}, geom={self.geom!r}, run_data_id={self.run_data_id!r})"
+
+
+class Run(Base):
+    __tablename__ = "run"
+    __table_args__ = {"schema": "gis"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    status: Mapped[str] = mapped_column(server_default="queued")
+    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
+    finished_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True))
+    engine: Mapped[str] = mapped_column(server_default="local")
+    runtime: Mapped[int] = mapped_column(server_default="0")
+    cost: Mapped[float] = mapped_column(server_default="0")
+
+    input_id: Mapped[int] = mapped_column(ForeignKey("gis.run_data.id", ondelete="CASCADE"), nullable=False)
+    input: Mapped["RunData"] = relationship("RunData", foreign_keys=[input_id])
+
+    output_id: Mapped[int] = mapped_column(ForeignKey("gis.run_data.id", ondelete="CASCADE"), nullable=False)
+    output: Mapped[Optional["RunData"]] = relationship("RunData", foreign_keys=[output_id])
+
+    inference_model_id: Mapped[int] = mapped_column(ForeignKey("gis.inference_model.id"))
+    inference_model: Mapped["InferenceModel"] = relationship()
+
+    process_id: Mapped[int] = mapped_column(ForeignKey("gis.process.id", ondelete="CASCADE"))
+    process: Mapped["Process"] = relationship()
+
+    def __repr__(self) -> str:
+        return f"Run(id={self.id!r}, status={self.status!r}, process_id={self.process_id!r}) inference_model_id={self.inference_model_id!r}, input_id={self.input_id}, output_id={self.output_id})"
+
+
+class RunData(Base):
+    __tablename__ = "run_data"
+    __table_args__ = {"schema": "gis"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    type: Mapped[str] = mapped_column(server_default='upload')
+    status: Mapped[str] = mapped_column(server_default='ready')
+    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
+
+    data: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
+
+    user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"))
+    user: Mapped["User"] = relationship()
+
+    organization_id: Mapped[int] = mapped_column(ForeignKey("admin.organization.id"))
+    organization: Mapped["Organization"] = relationship()
+
+    #used_by: Mapped[List["Run"]] = relationship(foreign_keys='id')
+    #
+    # origin_run: Mapped[Optional["Run"]] = relationship(
+    #     back_populates="output"
+    # )
+
+    results_vector: Mapped[List["ResultsVector"]] = relationship(
+       back_populates="run_data",
+       order_by="ResultsVector.id",
+       cascade="all, delete"
+    )
+
+    results_raster: Mapped[List["ResultsRaster"]] = relationship(
+        back_populates="run_data",
+        order_by="ResultsRaster.id",
+        cascade="all, delete"
+    )
+
+    def __repr__(self) -> str:
+        return f"RunData (id={self.id!r}, user_id={self.user_id!r}, status={self.status}, data={self.data}"
```

### Comparing `rov_db_access-1.0.8/rov_db_access/gis/worker.py` & `rov_db_access-1.0.9/rov_db_access/gis/worker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,940 +1,943 @@
-import os
-from typing import Literal, TypedDict, List, Optional
-
-import boto3
-import hashlib
-from botocore.client import Config
-from botocore.exceptions import ClientError
-
-from rov_db_access.authentication.models import User, Organization
-from rov_db_access.utils.geoserver_utils import GeoServerClient
-from rov_db_access.utils.s3_utils import S3Client
-from rov_db_access.utils.utils import wkbelement_to_wkt
-from rov_db_access.config.db_utils import init_db_engine
-from rov_db_access.config.settings import Settings
-from rov_db_access.sentinel.worker import is_valid_uuid
-from rov_db_access.gis.models import Process, Image, InferenceModel, RunData, ResultsRaster, Run, ResultsVector, Mosaic
-from sqlalchemy import select, and_, func
-from sqlalchemy.orm import Session
-
-settings = Settings()
-
-CreateProcessDict = TypedDict("CreateProcessDict", {
-    "name": str,
-    "inference_model_id": int,
-    "area": float,
-    "cost_estimated": float,
-    "images": List[dict],
-    "geom": str,
-    "mask": Optional[str]
-})
-
-CreateTaskingDict = TypedDict("CreateTaskingDict", {
-    "name": str,
-    "inference_model_id": int,
-    "area": float,
-    "cost_estimated": float,
-    "tasking_config": dict,
-    "geom": str,
-    "mask": Optional[str]
-})
-
-UploadImageDict = TypedDict("UploadImageDict", {
-    "name": str,
-    "url": str,
-    "bbox": str
-})
-
-
-def get_upload_s3_url():
-    region = settings.gis_inference_region
-    bucket_name = settings.gis_inference_bucket
-    access_key_id = settings.aws_key
-    secret_access_key = settings.aws_secret
-
-    s3 = boto3.client(
-        "s3",
-        aws_access_key_id=access_key_id,
-        aws_secret_access_key=secret_access_key,
-        config=Config(signature_version='s3v4', region_name=region)
-    )
-
-    # Generate a unique image name
-    raw_bytes = os.urandom(16)
-    image_name = hashlib.sha256(raw_bytes).hexdigest()
-    object_key = image_name + ".tif"
-
-    params = {
-        "Bucket": bucket_name,
-        "Key": object_key,
-    }
-
-    try:
-        upload_url = s3.generate_presigned_url(
-            "put_object",
-            Params=params,
-            ExpiresIn=60
-        )
-        return {"upload_url": upload_url, "object_key": object_key}
-
-    except ClientError as e:
-        return None
-
-
-def get_date(obj):
-    return tuple(map(int, obj["date"].split("/")[::-1]))
-
-
-class GisWorker:
-
-    def __init__(self) -> None:
-        self.engine = init_db_engine(
-            settings.db_rov_gis_user,
-            settings.db_rov_gis_password,
-            settings.db_rov_gis_host,
-            settings.db_rov_gis_port,
-            settings.db_rov_gis_database
-        )
-
-    def add_mosaic_result(self, raster_result_id: str, mosaic_id: str, user: User):
-        with Session(self.engine) as session:
-            mosaic = session.get(Mosaic, mosaic_id)
-            if mosaic is None:
-                print(f'No Raster with id ${raster_result_id} found!')
-                return None
-            if mosaic.organization_id != user.organization_id:
-                print(f'This mosaic is not from this org_id: {user.organization_id}')
-                return None
-
-            raster_result = session.get(ResultsRaster, raster_result_id)
-            if raster_result is None:
-                print(f'No Raster with id ${raster_result_id} found!')
-                return None
-
-            org_query = (
-                select(Organization.workspace)
-                .where(Organization.id == user.organization_id)
-                .limit(1)
-            )
-            workspace = session.scalar(org_query)
-
-            s3 = S3Client(settings.run_results_bucket, settings.s3_region)
-            granule_path = s3.get_file_url(key=raster_result.url)
-
-
-            geoserver_client = GeoServerClient()
-            print("BORRAR: url", geoserver_client.url)
-            print("BORRAR: server url", geoserver_client.server_url)
-            print("BORRAR: workspace", workspace
-                  )
-            geoserver_client.set_workspace(workspace)
-
-            print("BORRAR: coverage_store", mosaic.coverage_store)
-            print("BORRAR: granule_path", granule_path)
-
-            result = geoserver_client.add_mosaic_granule(mosaic.coverage_store, granule_path)
-            if result is None:
-                return False
-            return True
-
-    def remove_mosaic_result(self, raster_result_id: str, mosaic_id: str, user: User):
-        # TODO: get Fid of the geoserver table and remove granule
-        return False
-
-    def copy_process(self, process_id, user: User):
-        with Session(self.engine) as session:
-            process_to_copy = session.get(Process, process_id)
-            if process_to_copy is None:
-                print(f'No process with id ${id} found!')
-                return {}
-            elif process_to_copy.organization_id != user.organization_id:
-                print(f'This process is not from this org_id: {user.organization_id}')
-                return None
-            else:
-                process_type = process_to_copy.type
-                new_name = "Copy of " + process_to_copy.name
-                model_id: int = process_to_copy.inference_model_id
-                area: float = process_to_copy.area
-                cost_estimated: float = process_to_copy.cost_estimated
-                geom: str = wkbelement_to_wkt(process_to_copy.geom)
-                mask = wkbelement_to_wkt(process_to_copy.mask)
-                print(f'Process with id: {process_to_copy.id} found! type: {process_type}')
-
-                if process_type == 'on demand':
-                    process = Process(
-                        name=new_name,
-                        cost_estimated=cost_estimated,
-                        area=area,
-                        type=process_type,
-                        inference_model_id=model_id,
-                        organization_id=process_to_copy.organization_id,
-                        geom=geom,
-                        mask=mask,
-                        user_id=user.id
-                    )
-                    session.add(process)
-
-                    for run in process_to_copy.runs:
-                        print("BORRAR: run to copy: ", run)
-                        new_output = RunData(
-                            status="waiting",
-                            type=run.output.type,
-                            user_id=user.id,
-                            organization_id=process_to_copy.organization_id,
-                        )
-                        new_run = Run(
-                            status='queued',
-                            runtime=run.runtime,
-                            engine=run.engine,
-                            cost=run.cost,
-                            input=run.input,
-                            output=new_output,
-                            inference_model_id=run.inference_model_id,
-                            process=process
-                        )
-
-                        session.add(new_output)
-                        session.add(new_run)
-                    try:
-                        session.commit()
-                        return True
-                    except Exception as error:
-                        print("ERROR Create process. An exception occurred during DB insertion:", error)
-                        return False
-                elif process_type == 'tasking':
-                    data: CreateTaskingDict = {
-                        "name": new_name,
-                        "inference_model_id": model_id,
-                        "area": area,
-                        "cost_estimated": cost_estimated,
-                        "tasking_config": {},  # TODO: esto hay que hacerlo bien
-                        "geom": geom,
-                        "mask": mask
-                    }
-                    return self.create_tasking(data, user)
-                else:
-                    return False
-
-    def create_process(self, data: CreateProcessDict, user: User):
-        name = data["name"]
-        inference_model_id = data["inference_model_id"]
-        area = data["area"]
-        cost_estimated = data["cost_estimated"]
-        images = data["images"]
-        geom = data["geom"]
-        mask = data["mask"]
-        user_id = user.id
-        organization_id = user.organization_id
-
-        print(f'Creating process for user_id: {user_id}')
-
-        with Session(self.engine) as session:
-            # Check if inference_model_id exists
-            model = session.get(InferenceModel, inference_model_id)
-            if model is None:
-                return False
-
-            input_images = {
-                "sentinel": [],
-                "upload": []
-            }
-            unsorted_sentinel = []
-            for img in images:
-                img_type = img.get("type")
-                if img_type == "sentinel":
-                    data = {
-                        "id": img.get("id"),
-                        "date": img.get("date"),
-                        "title": img.get("title")
-                    }
-                    unsorted_sentinel.append(data)
-                elif img_type == "upload":
-                    input_images["upload"].append(img.get("id"))
-
-            input_images["sentinel"] = sorted(unsorted_sentinel, key=get_date)
-
-            print(f'Create process validation on images: {input_images}')
-            if len(input_images["upload"]) > 0:
-                # Check upload image exists
-                img_query_count = session.scalar(
-                    select(func.count(Image.id))
-                    .where(
-                        (Image.id.in_(input_images["upload"])) &
-                        (Image.organization_id == organization_id)
-                    )
-                )
-                if img_query_count != len(input_images["upload"]):
-                    print(f'Create process validation failed! An Upload image is not valid')
-                    return False
-
-            if len(input_images["sentinel"]) > 0:
-                # Check format of sentinel uuid
-                for data in input_images["sentinel"]:
-                    if not is_valid_uuid(data["id"]):
-                        print(f'Create process validation failed! A Sentinel image is not valid')
-                        return False
-
-            print(f'Create process validation ready!. Adding to DB...')
-            process = Process(
-                name=name,
-                cost_estimated=cost_estimated,
-                area=area,
-                type='on demand',
-                inference_model_id=inference_model_id,
-                organization_id=organization_id,
-                geom=geom,
-                mask=mask,
-                user_id=user_id
-            )
-
-            # if model is change detector with sentinel, then different process creation with multiple runs
-            if inference_model_id == 1:
-                if len(input_images["sentinel"]) < 2:
-                    print("ERROR Create change detector process. Not enough sentinel images:")
-                    return False
-                for i in range(len(input_images["sentinel"]) - 1):
-                    new_input = RunData(
-                        type='change',
-                        data={
-                            "t1": input_images["sentinel"][i],
-                            "t2": input_images["sentinel"][i+1],
-                            "mask": mask,
-                        },
-                        user_id=user_id,
-                        organization_id=organization_id
-                    )
-                    session.add(new_input)
-                    new_output = RunData(
-                        type='raster_result',
-                        status='waiting',
-                        user_id=user_id,
-                        organization_id=organization_id
-                    )
-                    session.add(new_output)
-                    new_run = Run(
-                        input=new_input,
-                        inference_model_id=inference_model_id,
-                        process=process,
-                        output=new_output,
-                    )
-                    session.add(new_run)
-                session.add(process)
-                try:
-                    session.commit()
-                    return True
-                except Exception as error:
-                    print("ERROR Create change detector process. An exception occurred during DB insertion:", error)
-                    return False
-            else:
-                for img in input_images["upload"]:
-                    new_input = RunData(
-                        type="raster_upload",
-                        status="ready",
-                        data={
-                            "id": img,
-                            "mask": mask,
-                        },
-                        user_id=user_id,
-                        organization_id=organization_id,    
-                    )
-                    session.add(new_input)
-
-                    new_output = RunData(
-                        type='raster_result',
-                        status='waiting',
-                        user_id=user_id,
-                        organization_id=organization_id
-                    )
-                    session.add(new_output)
-                    
-                    new_run = Run(
-                        input=new_input,
-                        inference_model_id=inference_model_id,
-                        process=process,
-                        output=new_output,
-                    )
-                    session.add(new_run)
-                session.add(process)
-                try:
-                    session.commit()
-                    return True
-                except Exception as error:
-                    print("ERROR Create process. An exception occurred during DB insertion:", error)
-                    return False
-
-    def create_tasking(self, data: CreateTaskingDict, user: User):
-        name = data["name"]
-        inference_model_id = data["inference_model_id"]
-        area = data["area"]
-        cost_estimated = data["cost_estimated"]
-        tasking_config = data["tasking_config"]
-        user_id = user.id
-        geom = data["geom"]
-        mask = data["mask"]
-        organization_id = user.organization_id
-
-        print(f'Creating tasking for user_id: {user_id}')
-
-        # Check if inference_model_id exists
-        with Session(self.engine) as session:
-            model = session.get(InferenceModel, inference_model_id)
-            if model is None:
-                return False
-
-            process = Process(
-                name=name,
-                cost_estimated=cost_estimated,
-                area=area,
-                inference_model_id=inference_model_id,
-                data=tasking_config,
-                organization_id=organization_id,
-                type='tasking',
-                geom=geom,
-                mask=mask,
-                user_id=user_id
-            )
-
-            session.add(process)
-            try:
-                session.commit()
-                return True
-            except Exception as error:
-                # handle the exception
-                print("Create tasking. An exception occurred during DB insertion:", error)
-                return False
-
-    def get_inference_models(self):
-        with Session(self.engine) as session:
-            query = (
-                select(InferenceModel)
-                .order_by(InferenceModel.id)
-            )
-            models = session.scalars(query).all()
-            if models is None or len(models) == 0:
-                return []
-            result = []
-            for model in models:
-                result.append({
-                    "id": model.id,
-                    "name": model.name,
-                    "title": model.title,
-                    "description": model.description,
-                    "img_url": model.img_url,
-                    "price": model.price,
-                    "min_resolution": model.min_resolution,
-                    "config": model.config
-                })
-            return result
-
-    def get_inference_model_by_id(self, id: str):
-        with Session(self.engine) as session:
-            model = session.get(InferenceModel, id)
-            if model is None:
-                return {}
-            print(f'Model with id: {id} found! ')
-            return {
-                "id": model.id,
-                "name": model.name,
-                "title": model.title,
-                "description": model.description,
-                "img_url": model.img_url,
-                "price": model.price,
-                "min_resolution": model.min_resolution,
-                "config": model.config
-            }
-
-    def load_images_by_org(self, organization_id: str):
-        with Session(self.engine) as session:
-            query = (
-                select(Image)
-                .where(
-                    (Image.organization_id == organization_id)
-                )
-            )
-            images = session.scalars(query)
-            if images is None:
-                return {}
-            result = []
-            for img in images:
-                bbox = None
-                footprint = None
-                if img.bbox is not None:
-                    bbox = wkbelement_to_wkt(img.bbox)
-                if img.footprint is not None:
-                    footprint = wkbelement_to_wkt(img.footprint)
-                result.append({
-                    "id": img.id,
-                    "name": img.name,
-                    "created_at": img.created_at,
-                    "url": img.url,
-                    "data": img.data,
-                    "bbox": bbox,
-                    "footprint": footprint,
-                    "user": img.user.username
-                })
-            return result
-
-    def load_mosaics_by_org(self, organization_id: str):
-        with Session(self.engine) as session:
-            query = (
-                select(Mosaic)
-                .where(
-                    (Mosaic.organization_id == organization_id)
-                )
-            )
-            mosaics = session.scalars(query)
-            if mosaics is None:
-                return {}
-            result = []
-            for mosaic in mosaics:
-                result.append({
-                    "id": mosaic.id,
-                    "name": mosaic.name,
-                    "description": mosaic.description,
-                    "created_at": mosaic.created_at,
-                    "coverage_store": mosaic.coverage_store,
-                    "workspace": mosaic.organization.workspace
-                })
-            return result
-
-    def load_process_by_id(self, id: str, user: User):
-        with Session(self.engine) as session:
-            process = session.get(Process, id)
-            if process is None:
-                print(f'No process with id ${id} found!')
-                return {}
-            elif process.organization_id != user.organization_id:
-                print(f'This process is not from this org_id: {user.organization_id}')
-                return None
-            else:
-                print(f'Process with id: {id} found! ')
-                geom = None
-                if process.geom is not None:
-                    geom = wkbelement_to_wkt(process.geom)
-                mask = None
-                if process.mask is not None:
-                    mask = wkbelement_to_wkt(process.mask)
-                return {
-                    "id": process.id,
-                    "name": process.name,
-                    "status": process.status,
-                    "type": process.type,
-                    "created_at": process.created_at,
-                    "finished_at": process.finished_at,
-                    "runtime": process.runtime,
-                    "area": process.area,
-                    "cost_estimated": process.cost_estimated,
-                    "inference_model_id": process.inference_model_id,
-                    "user_id": process.user_id,
-                    "organization_id": process.organization_id,
-                    "geom": geom,
-                    "mask": mask,
-                }
-
-    def load_processes_by_org(self, org_id: int):
-        with Session(self.engine) as session:
-            query = (
-                select(Process)
-                .where(Process.organization_id == org_id)
-                .order_by(Process.id)
-            )
-            processes = session.scalars(query).all()
-            if processes is None:
-                print(f'No processes for org_id ${org_id}')
-                return []
-            result = []
-            print(f'Processes for org_id={org_id} found!: {len(processes)} processes')
-            for process in processes:
-                geom = None
-                if process.geom is not None:
-                    geom = wkbelement_to_wkt(process.geom)
-                mask = None
-                if process.mask is not None:
-                    mask = wkbelement_to_wkt(process.mask)
-                result.append({
-                    "id": process.id,
-                    "name": process.name,
-                    "status": process.status,
-                    "type": process.type,
-                    "created_at": process.created_at,
-                    "finished_at": process.finished_at,
-                    "runtime": process.runtime,
-                    "area": process.area,
-                    "cost_estimated": process.cost_estimated,
-                    "inference_model_id": process.inference_model_id,
-                    "user_id": process.user_id,
-                    "organization_id": process.organization_id,
-                    "geom": geom,
-                    "mask": mask,
-                })
-            return result
-
-    def load_results_by_run_id(self, id: str):
-        results = {
-            "vector": [],
-            "raster": []
-        }
-        with Session(self.engine) as session:
-            output_id = session.scalar(select(Run.output_id).where(Run.id == id))
-            query_vector = (
-                select(ResultsVector)
-                .where(ResultsVector.run_data_id == output_id)
-                .order_by(ResultsVector.id)
-            )
-            vector_results = session.scalars(query_vector).all()
-            if len(vector_results) == 0:
-                print(f'No vector results for run_id ${id}')
-            else:
-                print(f'Vector results for run_id={id} found!: {len(vector_results)} results')
-                for vector_result in vector_results:
-                    wkt = wkbelement_to_wkt(vector_result.geom)
-                    results["vector"].append({
-                        "id": vector_result.id,
-                        "data": vector_result.data,
-                        "geom": wkt
-                    })
-
-            query_raster = (
-                select(ResultsRaster)
-                .where(ResultsRaster.run_data_id == output_id)
-                .order_by(ResultsRaster.id)
-            )
-            raster_results = session.scalars(query_raster).all()
-            if len(raster_results) == 0:
-                print(f'No raster results for run_id ${id}')
-            else:
-                print(f'Raster results for run_id={id} found!: {len(raster_results)} results')
-                for raster_result in raster_results:
-                    wkt = wkbelement_to_wkt(raster_result.bbox)
-                    results["raster"].append({
-                        "id": raster_result.id,
-                        "url": raster_result.url,
-                        "data": raster_result.data,
-                        "bbox": wkt
-                    })
-
-            return results
-
-    def load_runs_by_process(self, id: str, user: User):
-        with Session(self.engine) as session:
-            organization_id = session.scalar(select(Process.organization_id).where(Process.id == id))
-
-            if organization_id is None or organization_id != user.organization_id:
-                return None
-
-            query_run = (
-                select(Run)
-                .where(Run.process_id == id)
-            )
-            runs = session.scalars(query_run).all()
-            if len(runs) == 0:
-                print(f'No runs for process_id ${id}')
-                return []
-            print(f'Runs for process_id={id} found!: {len(runs)} processes')
-            results = []
-
-            for run in runs:
-                results.append({
-                    "id": run.id,
-                    "status": run.status,
-                    "created_at": run.created_at,
-                    "finished_at": run.finished_at,
-                    "engine": run.engine,
-                    "runtime": run.runtime,
-                    "cost": run.cost,
-                    "input_id": run.input_id,
-                    "output_id": run.output_id,
-                    "inference_model_id": run.inference_model_id,
-                })
-
-            return results
-
-    def load_run_by_id(self, id: str, user: User):
-        with Session(self.engine) as session:
-            run = session.get(Run, id)
-            if run is None:
-                print(f'No run with id ${id} found!')
-                return {}
-            elif run.process.organization_id != user.organization_id:
-                print(f'This process is not from this org_id: {user.organization_id}')
-                return None
-            else:
-                print(f'Run with id: {id} found! ')
-                return {
-                    "id": run.id,
-                    "status": run.status,
-                    "created_at": run.created_at,
-                    "finished_at": run.finished_at,
-                    "engine": run.engine,
-                    "runtime": run.runtime,
-                    "cost": run.cost,
-                    "process_id": run.process_id,
-                    "inference_model_id": run.inference_model_id,
-                    "input_id": run.input_id,
-                    "output_id": run.output_id
-                }
-
-    def upload_image(self, img: UploadImageDict, user: User):
-        name = img["name"]
-        url = img["url"]
-        bbox = img["bbox"]
-        print(f'Adding new uploaded image: {name} from user_id: {user.id}')
-        with Session(self.engine) as session:
-            new_image = Image(
-                name=name,
-                url=url,
-                bbox=bbox,
-                user_id=user.id,
-                organization_id=user.organization_id
-            )
-            session.add(new_image)
-            session.commit()
-            return new_image
-
-    def add_run_data_output(self, run_id, data=None):
-        with Session(self.engine) as session:
-            output = session.scalar(select(Run.output).where(Run.id == run_id))
-            if output is None:
-                print(f'Corrupted run with id {run_id}')
-            else:
-                output.data = data
-                output.status = "ready"
-                session.commit()
-
-    def add_raster_results(self, run_data_id, object_key, data=None, bbox=None):
-        with Session(self.engine) as session:
-            new_result = ResultsRaster(
-                url=object_key,
-                data=data,
-                bbox=bbox,
-                run_data_id=run_data_id,
-            )
-            session.add(new_result)
-            session.commit()
-            return new_result
-        
-    def add_vector_result(self, run_data_id, geom, data=None):
-        with Session(self.engine) as session:
-            new_result = ResultsVector(
-                data=data,
-                geom=geom,
-                run_data_id=run_data_id,
-            )
-            session.add(new_result)
-            session.commit()
-            return new_result
-        
-    def add_vector_results(self, run_data_id, vector_results):
-        with Session(self.engine) as session:
-            for result in vector_results:
-                new_result = ResultsVector(
-                    data=result.data,
-                    geom=result.geom,
-                    run_data_id=run_data_id,
-                )
-                session.add(new_result)
-            session.commit()
-            return new_result
-
-    def delete_process(self, id: str, user: User):
-        with Session(self.engine) as session:
-            query = (
-                select(Process)
-                .where(
-                    and_(
-                        (Process.id == id),
-                        (Process.organization_id == user.organization_id)
-                    )
-                )
-                .limit(1)
-            )
-            process = session.scalar(query)
-            if process is None:
-                print(f'No process with id ${id} found!')
-                return False
-            else:
-                print(f'Deleting process with id: {id}')
-                session.delete(process)
-                session.commit()
-                return True
-
-    def get_raster_img_url(self, id: str, user: User):
-        with Session(self.engine) as session:
-            raster = session.get(ResultsRaster, id)
-            if raster is None:
-                print(f'No raster result with id: {id} found!')
-                return None
-            else:
-                print(f'Raster result with id: {id} found!')
-                return raster.url
-
-    def get_run_data_data(self, id: str, user: User):
-        with Session(self.engine) as session:
-            run_data = session.get(RunData, id)
-            if run_data is None:
-                print(f'No run_data with id ${id} found!')
-                return None
-            else:
-                print(f'Run_data with id: {id} found!')
-                data = run_data.data
-                if run_data.organization_id != user.organization_id:
-                    print(f'No permission allowed for this user!')
-                    return None
-                if data is None:
-                    print(f'No data for run_data id ${id} found!')
-                    return None
-                return data
-
-    def edit_process_name(self, id: str, name: str, user: User):
-        with Session(self.engine) as session:
-            query = (
-                select(Process)
-                .where(
-                    and_(
-                        (Process.id == id),
-                        (Process.organization_id == user.organization_id)
-                    )
-                )
-                .limit(1)
-            )
-            process = session.scalar(query)
-            if process is None:
-                print(f'No process with id ${id} found!')
-                return False
-            else:
-                print(f'Editing process name with id: {id}')
-                process.name = name
-                session.commit()
-                return True
-
-#######################################
-######### library methods #############
-#######################################
-
-    def update_run_status(self, run_id: int, status: Literal['queued', 'running', 'finished', 'failed', 'canceled']):
-        """
-        Updates the status of the run
-
-        Args:
-            run_id: The id of the run
-            status: The new status of the run
-        """
-        assert isinstance(run_id, int), 'Invalid run_id!'
-        assert status in ['queued', 'running', 'finished', 'failed', 'canceled'], 'Invalid status!'
-
-        with Session(self.engine) as session:
-            run = session.get(Run, run_id)
-            if run is None:
-                print(f'No run with id ${run_id} found!')
-                return False
-            run.status = status
-            if status == 'running':
-                run.process.status = 'running'
-            session.commit()
-            return True
-
-    def upload_run_results(self, run_id: int, runtime: int, bbox: str, files_path: str, raster_name: str, preview_name: str, file_names: list[str]=[], data: dict=None):
-        """
-        Uploads the files to the S3 bucket and updates the run status to finished
-
-        Args:
-            run_id: The id of the run
-            bbox: The bbox of the raster
-            files_path: The path where the files are located
-            runtime: The runtime of the run
-            raster_name: The name of the raster file
-            preview_name: The name of the preview file (i.e: thumbnail.png)
-            file_names: Array with the names of additional files to upload
-            data: additional data to store in the results raster table
-        """
-        assert isinstance(run_id, int), 'Invalid run_id!'
-        assert bbox is None or isinstance(bbox, str), 'Invalid bbox!'
-        assert isinstance(runtime, (int, float)), 'Invalid runtime!'
-        runtime = int(runtime)
-        assert isinstance(files_path, str), 'Invalid files_path!'
-        assert raster_name is None or isinstance(raster_name, str), 'Invalid raster_name!'
-        assert preview_name is None or isinstance(preview_name, str), 'Invalid preview_name!'
-        assert isinstance(file_names, list), 'Invalid file_names!'
-        assert data is None or isinstance(data, dict), 'Invalid data!'
-
-        assert raster_name is not None or len(file_names) != 0, 'No files to upload!'
-
-        with Session(self.engine) as session:
-            # actual function
-            run = session.get(Run, run_id)
-            if run is None:
-                print(f'No run with id {run_id} found!')
-                return False
-
-            process_id = run.process_id
-            org_id = run.process.organization_id
-            run_id = run.id
-
-            # upload files to bucket
-            s3_client = S3Client(settings.run_results_bucket, settings.s3_region)
-            bucket_base_directory = f"{org_id}/{process_id}/{run_id}/"
-
-            for file_name in file_names:
-                if not isinstance(file_name, str):
-                    print('Invalid file_name!')
-                    return False
-                print(f'Uploading file: {file_name}')
-                object_key = bucket_base_directory + file_name
-                file_path = os.path.join(files_path, file_name)
-                s3_client.upload_file(file_path, object_key)
-                print(f'File uploaded to S3 with key: {object_key}')
-
-            if raster_name is not None:
-                print(f'Uploading raster file: {raster_name}')
-                object_key = bucket_base_directory + raster_name
-                file_path = os.path.join(files_path, raster_name)
-                s3_client.upload_file(file_path, object_key)
-                print(f'File uploaded to S3 with key: {object_key}')
-                self.add_raster_results(run_id, object_key, data, bbox)
-
-            # update RunData status and data
-            run_data_data = {
-                'bbox': bbox,
-                'preview': bucket_base_directory + preview_name
-            }
-            self.add_run_data_output(run_id=run_id, data=run_data_data)
-
-            # update Run status
-            # when all runs of a process are finished, an SQL trigger will update the process status
-            run.status = 'finished'
-            run.finished_at = func.now()
-
-            # SQL trigger will update the process runtime
-            run.runtime = runtime
-            # run.filepath = bucket_base_directory
-            session.commit()
-
-            return True
-
-    def load_queued_runs_ids_by_model(self, model_id: str):
-        with Session(self.engine) as session:
-            query_runs = (
-                select(Run.id)
-                .where(Run.inference_model_id == model_id)
-                .where(Run.status == 'queued')
-                .order_by(Run.id)
-            )
-            runs = session.scalars(query_runs).all()
-            if runs is None or len(runs) == 0:
-                return []
-            else:
-                print(f'Queued runs found!: {len(runs)} results')
-                return runs
-
-    def load_run_input(self, run_id: str):
-        with Session(self.engine) as session:
-            query = select(Run.input).where(Run.id == run_id)
-            input = session.scalar(query)
-            if input is None:
-                print('Run with corrupted Input data')
-                return None
-            elif input.status == 'waiting':
-                print('Run data is not ready yet')
-                return None
-            else:
-                return input.data
+import os
+from typing import Literal, TypedDict, List, Optional
+
+import boto3
+import hashlib
+from botocore.client import Config
+from botocore.exceptions import ClientError
+
+from rov_db_access.authentication.models import User, Organization
+from rov_db_access.utils.geoserver_utils import GeoServerClient
+from rov_db_access.utils.s3_utils import S3Client
+from rov_db_access.utils.utils import wkbelement_to_wkt
+from rov_db_access.config.db_utils import init_db_engine
+from rov_db_access.config.settings import Settings
+from rov_db_access.sentinel.worker import is_valid_uuid
+from rov_db_access.gis.models import Process, Image, InferenceModel, RunData, ResultsRaster, Run, ResultsVector, Mosaic
+from sqlalchemy import select, and_, func
+from sqlalchemy.orm import Session
+
+settings = Settings()
+
+CreateProcessDict = TypedDict("CreateProcessDict", {
+    "name": str,
+    "inference_model_id": int,
+    "area": float,
+    "cost_estimated": float,
+    "images": List[dict],
+    "geom": str,
+    "mask": Optional[str]
+})
+
+CreateTaskingDict = TypedDict("CreateTaskingDict", {
+    "name": str,
+    "inference_model_id": int,
+    "area": float,
+    "cost_estimated": float,
+    "tasking_config": dict,
+    "geom": str,
+    "mask": Optional[str]
+})
+
+UploadImageDict = TypedDict("UploadImageDict", {
+    "name": str,
+    "url": str,
+    "bbox": str
+})
+
+
+def get_upload_s3_url():
+    region = settings.gis_inference_region
+    bucket_name = settings.gis_inference_bucket
+    access_key_id = settings.aws_key
+    secret_access_key = settings.aws_secret
+
+    s3 = boto3.client(
+        "s3",
+        aws_access_key_id=access_key_id,
+        aws_secret_access_key=secret_access_key,
+        config=Config(signature_version='s3v4', region_name=region)
+    )
+
+    # Generate a unique image name
+    raw_bytes = os.urandom(16)
+    image_name = hashlib.sha256(raw_bytes).hexdigest()
+    object_key = image_name + ".tif"
+
+    params = {
+        "Bucket": bucket_name,
+        "Key": object_key,
+    }
+
+    try:
+        upload_url = s3.generate_presigned_url(
+            "put_object",
+            Params=params,
+            ExpiresIn=60
+        )
+        return {"upload_url": upload_url, "object_key": object_key}
+
+    except ClientError as e:
+        return None
+
+
+def get_date(obj):
+    return tuple(map(int, obj["date"].split("/")[::-1]))
+
+
+class GisWorker:
+
+    def __init__(self) -> None:
+        self.engine = init_db_engine(
+            settings.db_rov_gis_user,
+            settings.db_rov_gis_password,
+            settings.db_rov_gis_host,
+            settings.db_rov_gis_port,
+            settings.db_rov_gis_database
+        )
+
+    def add_mosaic_result(self, raster_result_id: str, mosaic_id: str, user: User):
+        with Session(self.engine) as session:
+            mosaic = session.get(Mosaic, mosaic_id)
+            if mosaic is None:
+                print(f'No Raster with id ${raster_result_id} found!')
+                return None
+            if mosaic.organization_id != user.organization_id:
+                print(f'This mosaic is not from this org_id: {user.organization_id}')
+                return None
+
+            raster_result = session.get(ResultsRaster, raster_result_id)
+            if raster_result is None:
+                print(f'No Raster with id ${raster_result_id} found!')
+                return None
+
+            org_query = (
+                select(Organization.workspace)
+                .where(Organization.id == user.organization_id)
+                .limit(1)
+            )
+            workspace = session.scalar(org_query)
+
+            s3 = S3Client(settings.run_results_bucket, settings.s3_region)
+            granule_path = s3.get_file_url(key=raster_result.url)
+
+
+            geoserver_client = GeoServerClient()
+            print("BORRAR: url", geoserver_client.url)
+            print("BORRAR: server url", geoserver_client.server_url)
+            print("BORRAR: workspace", workspace
+                  )
+            geoserver_client.set_workspace(workspace)
+
+            print("BORRAR: coverage_store", mosaic.coverage_store)
+            print("BORRAR: granule_path", granule_path)
+
+            result = geoserver_client.add_mosaic_granule(mosaic.coverage_store, granule_path)
+            if result is None:
+                return False
+            return True
+
+    def remove_mosaic_result(self, raster_result_id: str, mosaic_id: str, user: User):
+        # TODO: get Fid of the geoserver table and remove granule
+        return False
+
+    def copy_process(self, process_id, user: User):
+        with Session(self.engine) as session:
+            process_to_copy = session.get(Process, process_id)
+            if process_to_copy is None:
+                print(f'No process with id ${id} found!')
+                return {}
+            elif process_to_copy.organization_id != user.organization_id:
+                print(f'This process is not from this org_id: {user.organization_id}')
+                return None
+            else:
+                process_type = process_to_copy.type
+                new_name = "Copy of " + process_to_copy.name
+                model_id: int = process_to_copy.inference_model_id
+                area: float = process_to_copy.area
+                cost_estimated: float = process_to_copy.cost_estimated
+                geom: str = wkbelement_to_wkt(process_to_copy.geom)
+                mask = wkbelement_to_wkt(process_to_copy.mask)
+                print(f'Process with id: {process_to_copy.id} found! type: {process_type}')
+
+                if process_type == 'on demand':
+                    process = Process(
+                        name=new_name,
+                        cost_estimated=cost_estimated,
+                        area=area,
+                        type=process_type,
+                        inference_model_id=model_id,
+                        organization_id=process_to_copy.organization_id,
+                        geom=geom,
+                        mask=mask,
+                        user_id=user.id
+                    )
+                    session.add(process)
+
+                    for run in process_to_copy.runs:
+                        print("BORRAR: run to copy: ", run)
+                        new_output = RunData(
+                            status="waiting",
+                            type=run.output.type,
+                            user_id=user.id,
+                            organization_id=process_to_copy.organization_id,
+                        )
+                        new_run = Run(
+                            status='queued',
+                            runtime=run.runtime,
+                            engine=run.engine,
+                            cost=run.cost,
+                            input=run.input,
+                            output=new_output,
+                            inference_model_id=run.inference_model_id,
+                            process=process
+                        )
+
+                        session.add(new_output)
+                        session.add(new_run)
+                    try:
+                        session.commit()
+                        return True
+                    except Exception as error:
+                        print("ERROR Create process. An exception occurred during DB insertion:", error)
+                        return False
+                elif process_type == 'tasking':
+                    data: CreateTaskingDict = {
+                        "name": new_name,
+                        "inference_model_id": model_id,
+                        "area": area,
+                        "cost_estimated": cost_estimated,
+                        "tasking_config": {},  # TODO: esto hay que hacerlo bien
+                        "geom": geom,
+                        "mask": mask
+                    }
+                    return self.create_tasking(data, user)
+                else:
+                    return False
+
+    def create_process(self, data: CreateProcessDict, user: User):
+        name = data["name"]
+        inference_model_id = data["inference_model_id"]
+        area = data["area"]
+        cost_estimated = data["cost_estimated"]
+        images = data["images"]
+        geom = data["geom"]
+        mask = data["mask"]
+        user_id = user.id
+        organization_id = user.organization_id
+
+        print(f'Creating process for user_id: {user_id}')
+
+        with Session(self.engine) as session:
+            # Check if inference_model_id exists
+            model = session.get(InferenceModel, inference_model_id)
+            if model is None:
+                return False
+
+            input_images = {
+                "sentinel": [],
+                "upload": []
+            }
+            unsorted_sentinel = []
+            for img in images:
+                img_type = img.get("type")
+                if img_type == "sentinel":
+                    data = {
+                        "id": img.get("id"),
+                        "date": img.get("date"),
+                        "title": img.get("title")
+                    }
+                    unsorted_sentinel.append(data)
+                elif img_type == "upload":
+                    input_images["upload"].append(img.get("id"))
+
+            input_images["sentinel"] = sorted(unsorted_sentinel, key=get_date)
+
+            print(f'Create process validation on images: {input_images}')
+            if len(input_images["upload"]) > 0:
+                # Check upload image exists
+                img_query_count = session.scalar(
+                    select(func.count(Image.id))
+                    .where(
+                        (Image.id.in_(input_images["upload"])) &
+                        (Image.organization_id == organization_id)
+                    )
+                )
+                if img_query_count != len(input_images["upload"]):
+                    print(f'Create process validation failed! An Upload image is not valid')
+                    return False
+
+            if len(input_images["sentinel"]) > 0:
+                # Check format of sentinel uuid
+                for data in input_images["sentinel"]:
+                    if not is_valid_uuid(data["id"]):
+                        print(f'Create process validation failed! A Sentinel image is not valid')
+                        return False
+
+            print(f'Create process validation ready!. Adding to DB...')
+            process = Process(
+                name=name,
+                cost_estimated=cost_estimated,
+                area=area,
+                type='on demand',
+                inference_model_id=inference_model_id,
+                organization_id=organization_id,
+                geom=geom,
+                mask=mask,
+                user_id=user_id
+            )
+
+            # if model is change detector with sentinel, then different process creation with multiple runs
+            if inference_model_id == 1:
+                if len(input_images["sentinel"]) < 2:
+                    print("ERROR Create change detector process. Not enough sentinel images:")
+                    return False
+                for i in range(len(input_images["sentinel"]) - 1):
+                    new_input = RunData(
+                        type='change',
+                        data={
+                            "t1": input_images["sentinel"][i],
+                            "t2": input_images["sentinel"][i+1],
+                            "mask": mask,
+                        },
+                        user_id=user_id,
+                        organization_id=organization_id
+                    )
+                    session.add(new_input)
+                    new_output = RunData(
+                        type='raster_result',
+                        status='waiting',
+                        user_id=user_id,
+                        organization_id=organization_id
+                    )
+                    session.add(new_output)
+                    new_run = Run(
+                        input=new_input,
+                        inference_model_id=inference_model_id,
+                        process=process,
+                        output=new_output,
+                    )
+                    session.add(new_run)
+                session.add(process)
+                try:
+                    session.commit()
+                    return True
+                except Exception as error:
+                    print("ERROR Create change detector process. An exception occurred during DB insertion:", error)
+                    return False
+            else:
+                for img in input_images["upload"]:
+                    new_input = RunData(
+                        type="raster_upload",
+                        status="ready",
+                        data={
+                            "id": img,
+                            "mask": mask,
+                        },
+                        user_id=user_id,
+                        organization_id=organization_id,    
+                    )
+                    session.add(new_input)
+
+                    new_output = RunData(
+                        type='raster_result',
+                        status='waiting',
+                        user_id=user_id,
+                        organization_id=organization_id
+                    )
+                    session.add(new_output)
+                    
+                    new_run = Run(
+                        input=new_input,
+                        inference_model_id=inference_model_id,
+                        process=process,
+                        output=new_output,
+                    )
+                    session.add(new_run)
+                session.add(process)
+                try:
+                    session.commit()
+                    return True
+                except Exception as error:
+                    print("ERROR Create process. An exception occurred during DB insertion:", error)
+                    return False
+
+    def create_tasking(self, data: CreateTaskingDict, user: User):
+        name = data["name"]
+        inference_model_id = data["inference_model_id"]
+        area = data["area"]
+        cost_estimated = data["cost_estimated"]
+        tasking_config = data["tasking_config"]
+        user_id = user.id
+        geom = data["geom"]
+        mask = data["mask"]
+        organization_id = user.organization_id
+
+        print(f'Creating tasking for user_id: {user_id}')
+
+        # Check if inference_model_id exists
+        with Session(self.engine) as session:
+            model = session.get(InferenceModel, inference_model_id)
+            if model is None:
+                return False
+
+            process = Process(
+                name=name,
+                cost_estimated=cost_estimated,
+                area=area,
+                inference_model_id=inference_model_id,
+                data=tasking_config,
+                organization_id=organization_id,
+                type='tasking',
+                geom=geom,
+                mask=mask,
+                user_id=user_id
+            )
+
+            session.add(process)
+            try:
+                session.commit()
+                return True
+            except Exception as error:
+                # handle the exception
+                print("Create tasking. An exception occurred during DB insertion:", error)
+                return False
+
+    def get_inference_models(self):
+        with Session(self.engine) as session:
+            query = (
+                select(InferenceModel)
+                .order_by(InferenceModel.id)
+            )
+            models = session.scalars(query).all()
+            if models is None or len(models) == 0:
+                return []
+            result = []
+            for model in models:
+                result.append({
+                    "id": model.id,
+                    "name": model.name,
+                    "title": model.title,
+                    "description": model.description,
+                    "img_url": model.img_url,
+                    "price": model.price,
+                    "min_resolution": model.min_resolution,
+                    "config": model.config
+                })
+            return result
+
+    def get_inference_model_by_id(self, id: str):
+        with Session(self.engine) as session:
+            model = session.get(InferenceModel, id)
+            if model is None:
+                return {}
+            print(f'Model with id: {id} found! ')
+            return {
+                "id": model.id,
+                "name": model.name,
+                "title": model.title,
+                "description": model.description,
+                "img_url": model.img_url,
+                "price": model.price,
+                "min_resolution": model.min_resolution,
+                "config": model.config
+            }
+
+    def load_images_by_org(self, organization_id: str):
+        with Session(self.engine) as session:
+            query = (
+                select(Image)
+                .where(
+                    (Image.organization_id == organization_id)
+                )
+            )
+            images = session.scalars(query)
+            if images is None:
+                return {}
+            result = []
+            for img in images:
+                bbox = None
+                footprint = None
+                if img.bbox is not None:
+                    bbox = wkbelement_to_wkt(img.bbox)
+                if img.footprint is not None:
+                    footprint = wkbelement_to_wkt(img.footprint)
+                result.append({
+                    "id": img.id,
+                    "name": img.name,
+                    "created_at": img.created_at,
+                    "url": img.url,
+                    "data": img.data,
+                    "bbox": bbox,
+                    "footprint": footprint,
+                    "user": img.user.username
+                })
+            return result
+
+    def load_mosaics_by_org(self, organization_id: str):
+        with Session(self.engine) as session:
+            query = (
+                select(Mosaic)
+                .where(
+                    (Mosaic.organization_id == organization_id)
+                )
+            )
+            mosaics = session.scalars(query)
+            if mosaics is None:
+                return {}
+            result = []
+            for mosaic in mosaics:
+                result.append({
+                    "id": mosaic.id,
+                    "name": mosaic.name,
+                    "description": mosaic.description,
+                    "created_at": mosaic.created_at,
+                    "coverage_store": mosaic.coverage_store,
+                    "workspace": mosaic.organization.workspace
+                })
+            return result
+
+    def load_process_by_id(self, id: str, user: User):
+        with Session(self.engine) as session:
+            process = session.get(Process, id)
+            if process is None:
+                print(f'No process with id ${id} found!')
+                return {}
+            elif process.organization_id != user.organization_id:
+                print(f'This process is not from this org_id: {user.organization_id}')
+                return None
+            else:
+                print(f'Process with id: {id} found! ')
+                geom = None
+                if process.geom is not None:
+                    geom = wkbelement_to_wkt(process.geom)
+                mask = None
+                if process.mask is not None:
+                    mask = wkbelement_to_wkt(process.mask)
+                return {
+                    "id": process.id,
+                    "name": process.name,
+                    "status": process.status,
+                    "type": process.type,
+                    "created_at": process.created_at,
+                    "finished_at": process.finished_at,
+                    "runtime": process.runtime,
+                    "area": process.area,
+                    "cost_estimated": process.cost_estimated,
+                    "inference_model_id": process.inference_model_id,
+                    "user_id": process.user_id,
+                    "organization_id": process.organization_id,
+                    "geom": geom,
+                    "mask": mask,
+                }
+
+    def load_processes_by_org(self, org_id: int):
+        with Session(self.engine) as session:
+            query = (
+                select(Process)
+                .where(Process.organization_id == org_id)
+                .order_by(Process.id)
+            )
+            processes = session.scalars(query).all()
+            if processes is None:
+                print(f'No processes for org_id ${org_id}')
+                return []
+            result = []
+            print(f'Processes for org_id={org_id} found!: {len(processes)} processes')
+            for process in processes:
+                geom = None
+                if process.geom is not None:
+                    geom = wkbelement_to_wkt(process.geom)
+                mask = None
+                if process.mask is not None:
+                    mask = wkbelement_to_wkt(process.mask)
+                result.append({
+                    "id": process.id,
+                    "name": process.name,
+                    "status": process.status,
+                    "type": process.type,
+                    "created_at": process.created_at,
+                    "finished_at": process.finished_at,
+                    "runtime": process.runtime,
+                    "area": process.area,
+                    "cost_estimated": process.cost_estimated,
+                    "inference_model_id": process.inference_model_id,
+                    "user_id": process.user_id,
+                    "organization_id": process.organization_id,
+                    "geom": geom,
+                    "mask": mask,
+                })
+            return result
+
+    def load_results_by_run_id(self, id: str):
+        results = {
+            "vector": [],
+            "raster": []
+        }
+        with Session(self.engine) as session:
+            output_id = session.scalar(select(Run.output_id).where(Run.id == id))
+            query_vector = (
+                select(ResultsVector)
+                .where(ResultsVector.run_data_id == output_id)
+                .order_by(ResultsVector.id)
+            )
+            vector_results = session.scalars(query_vector).all()
+            if len(vector_results) == 0:
+                print(f'No vector results for run_id ${id}')
+            else:
+                print(f'Vector results for run_id={id} found!: {len(vector_results)} results')
+                for vector_result in vector_results:
+                    wkt = wkbelement_to_wkt(vector_result.geom)
+                    results["vector"].append({
+                        "id": vector_result.id,
+                        "data": vector_result.data,
+                        "geom": wkt
+                    })
+
+            query_raster = (
+                select(ResultsRaster)
+                .where(ResultsRaster.run_data_id == output_id)
+                .order_by(ResultsRaster.id)
+            )
+            raster_results = session.scalars(query_raster).all()
+            if len(raster_results) == 0:
+                print(f'No raster results for run_id ${id}')
+            else:
+                print(f'Raster results for run_id={id} found!: {len(raster_results)} results')
+                for raster_result in raster_results:
+                    wkt = wkbelement_to_wkt(raster_result.bbox)
+                    results["raster"].append({
+                        "id": raster_result.id,
+                        "url": raster_result.url,
+                        "data": raster_result.data,
+                        "bbox": wkt
+                    })
+
+            return results
+
+    def load_runs_by_process(self, id: str, user: User):
+        with Session(self.engine) as session:
+            organization_id = session.scalar(select(Process.organization_id).where(Process.id == id))
+
+            if organization_id is None or organization_id != user.organization_id:
+                return None
+
+            query_run = (
+                select(Run)
+                .where(Run.process_id == id)
+            )
+            runs = session.scalars(query_run).all()
+            if len(runs) == 0:
+                print(f'No runs for process_id ${id}')
+                return []
+            print(f'Runs for process_id={id} found!: {len(runs)} processes')
+            results = []
+
+            for run in runs:
+                results.append({
+                    "id": run.id,
+                    "status": run.status,
+                    "created_at": run.created_at,
+                    "finished_at": run.finished_at,
+                    "engine": run.engine,
+                    "runtime": run.runtime,
+                    "cost": run.cost,
+                    "input_id": run.input_id,
+                    "output_id": run.output_id,
+                    "inference_model_id": run.inference_model_id,
+                })
+
+            return results
+
+    def load_run_by_id(self, id: str, user: User):
+        with Session(self.engine) as session:
+            run = session.get(Run, id)
+            if run is None:
+                print(f'No run with id ${id} found!')
+                return {}
+            elif run.process.organization_id != user.organization_id:
+                print(f'This process is not from this org_id: {user.organization_id}')
+                return None
+            else:
+                print(f'Run with id: {id} found! ')
+                return {
+                    "id": run.id,
+                    "status": run.status,
+                    "created_at": run.created_at,
+                    "finished_at": run.finished_at,
+                    "engine": run.engine,
+                    "runtime": run.runtime,
+                    "cost": run.cost,
+                    "process_id": run.process_id,
+                    "inference_model_id": run.inference_model_id,
+                    "input_id": run.input_id,
+                    "output_id": run.output_id
+                }
+
+    def upload_image(self, img: UploadImageDict, user: User):
+        name = img["name"]
+        url = img["url"]
+        bbox = img["bbox"]
+        print(f'Adding new uploaded image: {name} from user_id: {user.id}')
+        with Session(self.engine) as session:
+            new_image = Image(
+                name=name,
+                url=url,
+                bbox=bbox,
+                user_id=user.id,
+                organization_id=user.organization_id
+            )
+            session.add(new_image)
+            session.commit()
+            return new_image
+
+    def add_run_data_output(self, run_id, data=None):
+        with Session(self.engine) as session:
+            output_id = session.scalar(select(Run.output_id).where(Run.id == run_id))
+            output = session.get(RunData, output_id)
+            if output is None:
+                print(f'Corrupted run with id {run_id}')
+            else:
+                output.data = data
+                output.status = "ready"
+                session.commit()
+
+    def add_raster_results(self, run_data_id, object_key, data=None, bbox=None):
+        with Session(self.engine) as session:
+            new_result = ResultsRaster(
+                url=object_key,
+                data=data,
+                bbox=bbox,
+                run_data_id=run_data_id,
+            )
+            session.add(new_result)
+            session.commit()
+            return new_result
+        
+    def add_vector_result(self, run_data_id, geom, data=None):
+        with Session(self.engine) as session:
+            new_result = ResultsVector(
+                data=data,
+                geom=geom,
+                run_data_id=run_data_id,
+            )
+            session.add(new_result)
+            session.commit()
+            return new_result
+        
+    def add_vector_results(self, run_data_id, vector_results):
+        with Session(self.engine) as session:
+            for result in vector_results:
+                new_result = ResultsVector(
+                    data=result.data,
+                    geom=result.geom,
+                    run_data_id=run_data_id,
+                )
+                session.add(new_result)
+            session.commit()
+            return new_result
+
+    def delete_process(self, id: str, user: User):
+        with Session(self.engine) as session:
+            query = (
+                select(Process)
+                .where(
+                    and_(
+                        (Process.id == id),
+                        (Process.organization_id == user.organization_id)
+                    )
+                )
+                .limit(1)
+            )
+            process = session.scalar(query)
+            if process is None:
+                print(f'No process with id ${id} found!')
+                return False
+            else:
+                print(f'Deleting process with id: {id}')
+                session.delete(process)
+                session.commit()
+                return True
+
+    def get_raster_img_url(self, id: str, user: User):
+        with Session(self.engine) as session:
+            raster = session.get(ResultsRaster, id)
+            if raster is None:
+                print(f'No raster result with id: {id} found!')
+                return None
+            else:
+                print(f'Raster result with id: {id} found!')
+                return raster.url
+
+    def get_run_data_data(self, id: str, user: User):
+        with Session(self.engine) as session:
+            run_data = session.get(RunData, id)
+            if run_data is None:
+                print(f'No run_data with id ${id} found!')
+                return None
+            else:
+                print(f'Run_data with id: {id} found!')
+                data = run_data.data
+                if run_data.organization_id != user.organization_id:
+                    print(f'No permission allowed for this user!')
+                    return None
+                if data is None:
+                    print(f'No data for run_data id ${id} found!')
+                    return None
+                return data
+
+    def edit_process_name(self, id: str, name: str, user: User):
+        with Session(self.engine) as session:
+            query = (
+                select(Process)
+                .where(
+                    and_(
+                        (Process.id == id),
+                        (Process.organization_id == user.organization_id)
+                    )
+                )
+                .limit(1)
+            )
+            process = session.scalar(query)
+            if process is None:
+                print(f'No process with id ${id} found!')
+                return False
+            else:
+                print(f'Editing process name with id: {id}')
+                process.name = name
+                session.commit()
+                return True
+
+#######################################
+######### library methods #############
+#######################################
+
+    def update_run_status(self, run_id: int, status: Literal['queued', 'running', 'finished', 'failed', 'canceled']):
+        """
+        Updates the status of the run
+
+        Args:
+            run_id: The id of the run
+            status: The new status of the run
+        """
+        assert isinstance(run_id, int), 'Invalid run_id!'
+        assert status in ['queued', 'running', 'finished', 'failed', 'canceled'], 'Invalid status!'
+
+        with Session(self.engine) as session:
+            run = session.get(Run, run_id)
+            if run is None:
+                print(f'No run with id ${run_id} found!')
+                return False
+            run.status = status
+            if status == 'running':
+                run.process.status = 'running'
+            session.commit()
+            return True
+
+    def upload_run_results(self, run_id: int, runtime: int, bbox: str, files_path: str, raster_name: str, preview_name: str, file_names: list[str]=[], data: dict=None):
+        """
+        Uploads the files to the S3 bucket and updates the run status to finished
+
+        Args:
+            run_id: The id of the run
+            bbox: The bbox of the raster
+            files_path: The path where the files are located
+            runtime: The runtime of the run
+            raster_name: The name of the raster file
+            preview_name: The name of the preview file (i.e: thumbnail.png)
+            file_names: Array with the names of additional files to upload
+            data: additional data to store in the results raster table
+        """
+        assert isinstance(run_id, int), 'Invalid run_id!'
+        assert bbox is None or isinstance(bbox, str), 'Invalid bbox!'
+        assert isinstance(runtime, (int, float)), 'Invalid runtime!'
+        runtime = int(runtime)
+        assert isinstance(files_path, str), 'Invalid files_path!'
+        assert raster_name is None or isinstance(raster_name, str), 'Invalid raster_name!'
+        assert preview_name is None or isinstance(preview_name, str), 'Invalid preview_name!'
+        assert isinstance(file_names, list), 'Invalid file_names!'
+        assert data is None or isinstance(data, dict), 'Invalid data!'
+
+        assert raster_name is not None or len(file_names) != 0, 'No files to upload!'
+
+        with Session(self.engine) as session:
+            # actual function
+            run = session.get(Run, run_id)
+            if run is None:
+                print(f'No run with id {run_id} found!')
+                return False
+
+            process_id = run.process_id
+            org_id = run.process.organization_id
+            run_id = run.id
+
+            # upload files to bucket
+            s3_client = S3Client(settings.run_results_bucket, settings.s3_region)
+            bucket_base_directory = f"{org_id}/{process_id}/{run_id}/"
+
+            for file_name in file_names:
+                if not isinstance(file_name, str):
+                    print('Invalid file_name!')
+                    return False
+                print(f'Uploading file: {file_name}')
+                object_key = bucket_base_directory + file_name
+                file_path = os.path.join(files_path, file_name)
+                s3_client.upload_file(file_path, object_key)
+                print(f'File uploaded to S3 with key: {object_key}')
+
+            if raster_name is not None:
+                print(f'Uploading raster file: {raster_name}')
+                object_key = bucket_base_directory + raster_name
+                file_path = os.path.join(files_path, raster_name)
+                s3_client.upload_file(file_path, object_key)
+                print(f'File uploaded to S3 with key: {object_key}')
+                self.add_raster_results(run_id, object_key, data, bbox)
+
+            # update RunData status and data
+            run_data_data = {
+                'bbox': bbox,
+                'preview': bucket_base_directory + preview_name
+            }
+            self.add_run_data_output(run_id=run_id, data=run_data_data)
+
+            # update Run status
+            # when all runs of a process are finished, an SQL trigger will update the process status
+            run.status = 'finished'
+            run.finished_at = func.now()
+
+            # SQL trigger will update the process runtime
+            run.runtime = runtime
+            # run.filepath = bucket_base_directory
+            session.commit()
+
+            return True
+
+    def load_queued_runs_ids_by_model(self, model_id: str):
+        with Session(self.engine) as session:
+            query_runs = (
+                select(Run.id)
+                .where(Run.inference_model_id == model_id)
+                .where(Run.status == 'queued')
+                .order_by(Run.id)
+            )
+            runs = session.scalars(query_runs).all()
+            if runs is None or len(runs) == 0:
+                return []
+            else:
+                print(f'Queued runs found!: {len(runs)} results')
+                return runs
+
+    def load_run_input(self, run_id: str):
+        with Session(self.engine) as session:
+            query = select(Run.input_id).where(Run.id == run_id)
+            input_id = session.scalar(query)
+            input = session.get(RunData, input_id)
+            
+            if input is None:
+                print('Run with corrupted Input data')
+                return None
+            elif input.status == 'waiting':
+                print('Run data is not ready yet')
+                return None
+            else:
+                return input.data
```

### Comparing `rov_db_access-1.0.8/rov_db_access/ine/models.py` & `rov_db_access-1.0.9/rov_db_access/ine/models.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from geoalchemy2 import Geometry
-from sqlalchemy.orm import DeclarativeBase
-from sqlalchemy.orm import Mapped
-from sqlalchemy.orm import mapped_column
-
-
-class Base(DeclarativeBase):
-    """Base Class of the model"""
-
-
-class BuildingsNico(Base):
-    __tablename__ = "pompeya_buildings_nico_merged"
-    id: Mapped[int] = mapped_column(primary_key=True)
-    geom: Mapped[Geometry] = mapped_column(Geometry("MULTIPOLYGON", srid=32719))
-
-    def __repr__(self) -> str:
-        return f"Buildings_Nico (id={self.id!r},  geom={self.geom!r})"
-
-
-class BuildingsPost(Base):
-    __tablename__ = "buildings_instances_post_pompeya"
-    id: Mapped[int] = mapped_column(primary_key=True)
-    geom: Mapped[Geometry] = mapped_column(Geometry("POLYGON", srid=4326))
-
-    def __repr__(self) -> str:
+from geoalchemy2 import Geometry
+from sqlalchemy.orm import DeclarativeBase
+from sqlalchemy.orm import Mapped
+from sqlalchemy.orm import mapped_column
+
+
+class Base(DeclarativeBase):
+    """Base Class of the model"""
+
+
+class BuildingsNico(Base):
+    __tablename__ = "pompeya_buildings_nico_merged"
+    id: Mapped[int] = mapped_column(primary_key=True)
+    geom: Mapped[Geometry] = mapped_column(Geometry("MULTIPOLYGON", srid=32719))
+
+    def __repr__(self) -> str:
+        return f"Buildings_Nico (id={self.id!r},  geom={self.geom!r})"
+
+
+class BuildingsPost(Base):
+    __tablename__ = "buildings_instances_post_pompeya"
+    id: Mapped[int] = mapped_column(primary_key=True)
+    geom: Mapped[Geometry] = mapped_column(Geometry("POLYGON", srid=4326))
+
+    def __repr__(self) -> str:
         return f"Buildings_Post (id={self.id!r},  geom={self.geom!r})"
```

### Comparing `rov_db_access-1.0.8/rov_db_access/ine/worker.py` & `rov_db_access-1.0.9/rov_db_access/ine/worker.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-from typing import TypedDict, List
-from sqlalchemy.orm import Session
-from sqlalchemy import select, func, create_engine
-from rov_db_access.config.settings import Settings
-
-from rov_db_access.ine.models import BuildingsNico, BuildingsPost
-
-settings = Settings()
-
-CountDifferenceDict = TypedDict("CountDifferenceDict", {"bbox": List[float], "layer_t1": str, "layer_t2": str})
-
-
-class IneWorker:
-
-    def __init__(self) -> None:
-
-        self.engine = create_engine(
-            f"postgresql+psycopg2://{settings.db_ine_url}"
-        )
-
-
-    def count_difference(self, data: CountDifferenceDict):
-        bbox = data.get("bbox")
-        layer_t1 = data.get("layer_t1")
-        layer_t2 = data.get("layer_t2")
-        result = {
-            layer_t1: 0,
-            layer_t2: 0
-        }
-        if len(bbox) != 4:
-            return result
-
-        # transformer = Transformer.from_crs("EPSG:4326", "EPSG:32719")
-        # e1, n1 = transformer.transform(bbox[0], bbox[1])
-        # e2, n2 = transformer.transform(bbox[2], bbox[3])
-
-        with Session(self.engine) as session:
-            pre_query = (
-                select(
-                    func.count()
-                )
-                .where(
-                    func.ST_Intersects(
-                        # func.ST_MakeEnvelope(e1, n1, e2, n2, 32719),
-                        func.ST_Transform(func.ST_MakeEnvelope(bbox[0], bbox[1], bbox[2], bbox[3], 4326), 32719),
-                        BuildingsNico.geom
-                    )
-                )
-            )
-            pre_count = session.scalar(pre_query)
-            print("Pre count: ", pre_count)
-            result[layer_t1] = pre_count
-
-            post_query = (
-                select(
-                    func.count()
-                )
-                .where(
-                    func.ST_Intersects(
-                        # func.ST_MakeEnvelope(e1, n1, e2, n2, 32719),
-                        func.ST_Transform(func.ST_MakeEnvelope(bbox[0], bbox[1],bbox[2], bbox[3],4326), 32719),
-                        func.ST_Transform(BuildingsPost.geom, 32719)
-                    )
-                )
-            )
-            post_count = session.scalar(post_query)
-            print("Post count: ", post_count)
-            result[layer_t2] = post_count
-
-            return result
+from typing import TypedDict, List
+from sqlalchemy.orm import Session
+from sqlalchemy import select, func, create_engine
+from rov_db_access.config.settings import Settings
+
+from rov_db_access.ine.models import BuildingsNico, BuildingsPost
+
+settings = Settings()
+
+CountDifferenceDict = TypedDict("CountDifferenceDict", {"bbox": List[float], "layer_t1": str, "layer_t2": str})
+
+
+class IneWorker:
+
+    def __init__(self) -> None:
+
+        self.engine = create_engine(
+            f"postgresql+psycopg2://{settings.db_ine_url}"
+        )
+
+
+    def count_difference(self, data: CountDifferenceDict):
+        bbox = data.get("bbox")
+        layer_t1 = data.get("layer_t1")
+        layer_t2 = data.get("layer_t2")
+        result = {
+            layer_t1: 0,
+            layer_t2: 0
+        }
+        if len(bbox) != 4:
+            return result
+
+        # transformer = Transformer.from_crs("EPSG:4326", "EPSG:32719")
+        # e1, n1 = transformer.transform(bbox[0], bbox[1])
+        # e2, n2 = transformer.transform(bbox[2], bbox[3])
+
+        with Session(self.engine) as session:
+            pre_query = (
+                select(
+                    func.count()
+                )
+                .where(
+                    func.ST_Intersects(
+                        # func.ST_MakeEnvelope(e1, n1, e2, n2, 32719),
+                        func.ST_Transform(func.ST_MakeEnvelope(bbox[0], bbox[1], bbox[2], bbox[3], 4326), 32719),
+                        BuildingsNico.geom
+                    )
+                )
+            )
+            pre_count = session.scalar(pre_query)
+            print("Pre count: ", pre_count)
+            result[layer_t1] = pre_count
+
+            post_query = (
+                select(
+                    func.count()
+                )
+                .where(
+                    func.ST_Intersects(
+                        # func.ST_MakeEnvelope(e1, n1, e2, n2, 32719),
+                        func.ST_Transform(func.ST_MakeEnvelope(bbox[0], bbox[1],bbox[2], bbox[3],4326), 32719),
+                        func.ST_Transform(BuildingsPost.geom, 32719)
+                    )
+                )
+            )
+            post_count = session.scalar(post_query)
+            print("Post count: ", post_count)
+            result[layer_t2] = post_count
+
+            return result
```

### Comparing `rov_db_access-1.0.8/rov_db_access/label_studio/models.py` & `rov_db_access-1.0.9/rov_db_access/label_studio/models.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,221 +1,221 @@
-from geoalchemy2 import Geometry
-from sqlalchemy import String, ForeignKey, DateTime, func
-from typing import List
-from typing import Optional
-from datetime import datetime
-from sqlalchemy.orm import Mapped
-from sqlalchemy.orm import mapped_column
-from sqlalchemy.orm import relationship
-
-from rov_db_access.authentication.models import User, Base
-
-
-class AssociationBatchLayer(Base):
-    __tablename__ = "association_batch_layer"
-    __table_args__ = {"schema": "label_studio"}
-    batch_id: Mapped[int] = mapped_column(ForeignKey("label_studio.batch.id"), primary_key=True)
-    layer_id: Mapped[int] = mapped_column(ForeignKey("label_studio.layer.id"), primary_key=True)
-
-    # association between Popject -> Association -> Type
-    # project_associations: Mapped[List["AssociationProjectType"]] = relationship(back_populates='type')
-
-    # many-to-many relationship to Type, bypassing the `Association` class
-    # projects: Mapped[List["Project"]] = relationship(
-    #     secondary="association_project_type",
-    #     back_populates="types"
-    # )
-
-    def __repr__(self) -> str:
-        return f"AssociationBatchLayer(batch_id={self.batch_id!r}, layer_id={self.layer_id!r})"
-
-
-class AssociationProjectType(Base):
-    __tablename__ = "association_project_type"
-    __table_args__ = {"schema": "label_studio"}
-    project_id: Mapped[int] = mapped_column(ForeignKey("label_studio.project.id"), primary_key=True)
-    type_id: Mapped[int] = mapped_column(ForeignKey("label_studio.type.id"), primary_key=True)
-
-    # project: Mapped["Project"] = relationship(back_populates="types_associations")
-    ##type: Mapped["Type"] = relationship(back_populates="project_associations")
-
-    def __repr__(self) -> str:
-        return f"AssociationProjectType(project_id={self.project_id!r}, type_id={self.type_id!r})"
-
-
-class AssociationProjectUserRole(Base):
-    __tablename__ = "association_project_user_role"
-    __table_args__ = {"schema": "label_studio"}
-    user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"), primary_key=True)
-    project_id: Mapped[int] = mapped_column(ForeignKey("label_studio.project.id"), primary_key=True)
-    role_rl_id: Mapped[int] = mapped_column(ForeignKey("label_studio.role_rl.id"), primary_key=True)
-    user: Mapped["User"] = relationship()
-    project: Mapped["Project"] = relationship(back_populates="user_role_associations")
-    role_rl: Mapped["RoleRL"] = relationship()
-
-    def __repr__(self) -> str:
-        return f"AssociationProjectUserRole(user_id={self.user_id!r}, project_id={self.project_id!r}, role_rl_id={self.role_rl_id!r}, user={self.user!r}, project={self.project!r}, role_rl={self.role_rl!r})"
-
-
-class AssociationTaskImage(Base):
-    __tablename__ = "association_task_image"
-    __table_args__ = {"schema": "label_studio"}
-    task_id: Mapped[int] = mapped_column(ForeignKey("label_studio.task.id"), primary_key=True)
-    image_rl_id: Mapped[int] = mapped_column(ForeignKey("label_studio.image_rl.id"), primary_key=True)
-
-    def __repr__(self) -> str:
-        return f"AssociationTaskImage(task_id={self.task_id!r}, image_rl_id={self.image_rl_id!r})"
-
-
-class Batch(Base):
-    __tablename__ = "batch"
-    __table_args__ = {"schema": "label_studio"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[str]
-    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
-    project_id: Mapped[int] = mapped_column(ForeignKey("label_studio.project.id"))
-    project: Mapped["Project"] = relationship(back_populates="batches")
-
-    layers: Mapped[List["Layer"]] = relationship(
-        secondary="label_studio.association_batch_layer"
-    )
-    tasks: Mapped[List["Task"]] = relationship(
-        back_populates='batch',
-        order_by="Task.id"
-    )
-
-    def __repr__(self) -> str:
-        return f"Batch(id={self.id!r}, name={self.name!r}, layers={self.layers!r}, created_at={self.created_at!r}, project={self.project!r}, tasks={self.tasks!r})"
-
-
-class ImageRL(Base):
-    __tablename__ = "image_rl"
-    __table_args__ = {"schema": "label_studio"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    url: Mapped[str]
-    in_storage: Mapped[bool] = mapped_column(default=False)
-
-    def __repr__(self) -> str:
-        return f"ImageRL(id={self.id!r}, url={self.url!r}, in_storage={self.in_storage!r})"
-
-
-class Label(Base):
-    __tablename__ = "label"
-    __table_args__ = {"schema": "label_studio"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[Optional[str]]
-    time: Mapped[Optional[int]]
-    status: Mapped[str]
-    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
-    modified_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), onupdate=func.now())
-    geom = mapped_column(Geometry("POLYGON", srid=4326))
-
-    task_id: Mapped[int] = mapped_column(ForeignKey("label_studio.task.id"))
-    task: Mapped["Task"] = relationship(back_populates="labels")
-
-    user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"))
-    user: Mapped["User"] = relationship()
-
-    type_id: Mapped[int] = mapped_column(ForeignKey("label_studio.type.id"))
-    type: Mapped["Type"] = relationship()
-
-    def __repr__(self) -> str:
-        return f"Label(id={self.id!r}, name={self.name!r}, time={self.time!r}, status={self.status!r}, created_at={self.created_at!r}, modified_at={self.modified_at!r}, geom={self.geom!r}, task={self.task!r}, user={self.user!r}, type={self.type!r})"
-
-
-class Layer(Base):
-    __tablename__ = "layer"
-    __table_args__ = {"schema": "label_studio"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[str]
-    url: Mapped[str]
-
-    def __repr__(self) -> str:
-        return f"Layer(id={self.id!r}, name={self.name!r}, url={self.url!r})"
-
-
-class Project(Base):
-    __tablename__ = "project"
-    __table_args__ = {"schema": "label_studio"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[str]
-
-    # association between Popject -> Association -> Type
-    # types_associations: Mapped[List["AssociationProjectType"]] = relationship(back_populates='project')
-
-    # many-to-many relationship to Type, bypassing the `Association` class
-    types: Mapped[List["Type"]] = relationship(
-        secondary="label_studio.association_project_type",
-        order_by="Type.name"
-    )
-    user_role_associations: Mapped[List["AssociationProjectUserRole"]] = relationship(
-        back_populates='project'
-    )
-    batches: Mapped[List["Batch"]] = relationship(
-        back_populates='project',
-        order_by='Batch.id'
-    )
-
-    def __repr__(self) -> str:
-        return f"Project(id={self.id!r}, name={self.name!r}, types={self.types!r}, batches={self.batches!r})"
-
-
-class RoleRL(Base):
-    __tablename__ = "role_rl"
-    __table_args__ = {"schema": "label_studio"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[str]
-
-    def __repr__(self) -> str:
-        return f"RoleRL(id={self.id!r}, name={self.name!r})"
-
-
-class Task(Base):
-    __tablename__ = "task"
-    __table_args__ = {"schema": "label_studio"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[str]
-    time: Mapped[Optional[int]]
-    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
-    modified_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), onupdate=func.now())
-    status: Mapped[str]
-    bbox: Mapped[Optional[Geometry]] = mapped_column(Geometry("POLYGON", srid=4326))
-    comments: Mapped[Optional[str]]
-    is_valid: Mapped[bool] = mapped_column(server_default='True')
-
-    batch_id: Mapped[int] = mapped_column(ForeignKey("label_studio.batch.id"))
-    batch: Mapped["Batch"] = relationship(back_populates="tasks")
-
-    images_rl: Mapped[List[ImageRL]] = relationship(
-        secondary="label_studio.association_task_image",
-        order_by="ImageRL.id"
-    )
-
-    labels: Mapped[List["Label"]] = relationship(
-        back_populates="task",
-        order_by="Label.id"
-    )
-
-    def __repr__(self) -> str:
-        return f"Task(id={self.id!r}, name={self.name!r}, time={self.time!r}, created_at={self.created_at!r}, modified_at={self.modified_at!r}, status={self.status!r}, comments={self.comments!r}, images_rl={self.images_rl!r}, bbox={self.bbox!r}, labels={self.labels!r})"
-
-
-class Type(Base):
-    __tablename__ = "type"
-    __table_args__ = {"schema": "label_studio"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[str]
-    colour: Mapped[str] = mapped_column(String(7), default='#000000')
-
-    # association between Popject -> Association -> Type
-    # project_associations: Mapped[List["AssociationProjectType"]] = relationship(back_populates='type')
-
-    # many-to-many relationship to Type, bypassing the `Association` class
-    # projects: Mapped[List["Project"]] = relationship(
-    #     secondary="association_project_type",
-    #     back_populates="types"
-    # )
-
-    def __repr__(self) -> str:
-        return f"Type(id={self.id!r}, name={self.name!r}, colour={self.colour!r})"
-
-
+from geoalchemy2 import Geometry
+from sqlalchemy import String, ForeignKey, DateTime, func
+from typing import List
+from typing import Optional
+from datetime import datetime
+from sqlalchemy.orm import Mapped
+from sqlalchemy.orm import mapped_column
+from sqlalchemy.orm import relationship
+
+from rov_db_access.authentication.models import User, Base
+
+
+class AssociationBatchLayer(Base):
+    __tablename__ = "association_batch_layer"
+    __table_args__ = {"schema": "label_studio"}
+    batch_id: Mapped[int] = mapped_column(ForeignKey("label_studio.batch.id"), primary_key=True)
+    layer_id: Mapped[int] = mapped_column(ForeignKey("label_studio.layer.id"), primary_key=True)
+
+    # association between Popject -> Association -> Type
+    # project_associations: Mapped[List["AssociationProjectType"]] = relationship(back_populates='type')
+
+    # many-to-many relationship to Type, bypassing the `Association` class
+    # projects: Mapped[List["Project"]] = relationship(
+    #     secondary="association_project_type",
+    #     back_populates="types"
+    # )
+
+    def __repr__(self) -> str:
+        return f"AssociationBatchLayer(batch_id={self.batch_id!r}, layer_id={self.layer_id!r})"
+
+
+class AssociationProjectType(Base):
+    __tablename__ = "association_project_type"
+    __table_args__ = {"schema": "label_studio"}
+    project_id: Mapped[int] = mapped_column(ForeignKey("label_studio.project.id"), primary_key=True)
+    type_id: Mapped[int] = mapped_column(ForeignKey("label_studio.type.id"), primary_key=True)
+
+    # project: Mapped["Project"] = relationship(back_populates="types_associations")
+    ##type: Mapped["Type"] = relationship(back_populates="project_associations")
+
+    def __repr__(self) -> str:
+        return f"AssociationProjectType(project_id={self.project_id!r}, type_id={self.type_id!r})"
+
+
+class AssociationProjectUserRole(Base):
+    __tablename__ = "association_project_user_role"
+    __table_args__ = {"schema": "label_studio"}
+    user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"), primary_key=True)
+    project_id: Mapped[int] = mapped_column(ForeignKey("label_studio.project.id"), primary_key=True)
+    role_rl_id: Mapped[int] = mapped_column(ForeignKey("label_studio.role_rl.id"), primary_key=True)
+    user: Mapped["User"] = relationship()
+    project: Mapped["Project"] = relationship(back_populates="user_role_associations")
+    role_rl: Mapped["RoleRL"] = relationship()
+
+    def __repr__(self) -> str:
+        return f"AssociationProjectUserRole(user_id={self.user_id!r}, project_id={self.project_id!r}, role_rl_id={self.role_rl_id!r}, user={self.user!r}, project={self.project!r}, role_rl={self.role_rl!r})"
+
+
+class AssociationTaskImage(Base):
+    __tablename__ = "association_task_image"
+    __table_args__ = {"schema": "label_studio"}
+    task_id: Mapped[int] = mapped_column(ForeignKey("label_studio.task.id"), primary_key=True)
+    image_rl_id: Mapped[int] = mapped_column(ForeignKey("label_studio.image_rl.id"), primary_key=True)
+
+    def __repr__(self) -> str:
+        return f"AssociationTaskImage(task_id={self.task_id!r}, image_rl_id={self.image_rl_id!r})"
+
+
+class Batch(Base):
+    __tablename__ = "batch"
+    __table_args__ = {"schema": "label_studio"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str]
+    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
+    project_id: Mapped[int] = mapped_column(ForeignKey("label_studio.project.id"))
+    project: Mapped["Project"] = relationship(back_populates="batches")
+
+    layers: Mapped[List["Layer"]] = relationship(
+        secondary="label_studio.association_batch_layer"
+    )
+    tasks: Mapped[List["Task"]] = relationship(
+        back_populates='batch',
+        order_by="Task.id"
+    )
+
+    def __repr__(self) -> str:
+        return f"Batch(id={self.id!r}, name={self.name!r}, layers={self.layers!r}, created_at={self.created_at!r}, project={self.project!r}, tasks={self.tasks!r})"
+
+
+class ImageRL(Base):
+    __tablename__ = "image_rl"
+    __table_args__ = {"schema": "label_studio"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    url: Mapped[str]
+    in_storage: Mapped[bool] = mapped_column(default=False)
+
+    def __repr__(self) -> str:
+        return f"ImageRL(id={self.id!r}, url={self.url!r}, in_storage={self.in_storage!r})"
+
+
+class Label(Base):
+    __tablename__ = "label"
+    __table_args__ = {"schema": "label_studio"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[Optional[str]]
+    time: Mapped[Optional[int]]
+    status: Mapped[str]
+    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
+    modified_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), onupdate=func.now())
+    geom = mapped_column(Geometry("POLYGON", srid=4326))
+
+    task_id: Mapped[int] = mapped_column(ForeignKey("label_studio.task.id"))
+    task: Mapped["Task"] = relationship(back_populates="labels")
+
+    user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"))
+    user: Mapped["User"] = relationship()
+
+    type_id: Mapped[int] = mapped_column(ForeignKey("label_studio.type.id"))
+    type: Mapped["Type"] = relationship()
+
+    def __repr__(self) -> str:
+        return f"Label(id={self.id!r}, name={self.name!r}, time={self.time!r}, status={self.status!r}, created_at={self.created_at!r}, modified_at={self.modified_at!r}, geom={self.geom!r}, task={self.task!r}, user={self.user!r}, type={self.type!r})"
+
+
+class Layer(Base):
+    __tablename__ = "layer"
+    __table_args__ = {"schema": "label_studio"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str]
+    url: Mapped[str]
+
+    def __repr__(self) -> str:
+        return f"Layer(id={self.id!r}, name={self.name!r}, url={self.url!r})"
+
+
+class Project(Base):
+    __tablename__ = "project"
+    __table_args__ = {"schema": "label_studio"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str]
+
+    # association between Popject -> Association -> Type
+    # types_associations: Mapped[List["AssociationProjectType"]] = relationship(back_populates='project')
+
+    # many-to-many relationship to Type, bypassing the `Association` class
+    types: Mapped[List["Type"]] = relationship(
+        secondary="label_studio.association_project_type",
+        order_by="Type.name"
+    )
+    user_role_associations: Mapped[List["AssociationProjectUserRole"]] = relationship(
+        back_populates='project'
+    )
+    batches: Mapped[List["Batch"]] = relationship(
+        back_populates='project',
+        order_by='Batch.id'
+    )
+
+    def __repr__(self) -> str:
+        return f"Project(id={self.id!r}, name={self.name!r}, types={self.types!r}, batches={self.batches!r})"
+
+
+class RoleRL(Base):
+    __tablename__ = "role_rl"
+    __table_args__ = {"schema": "label_studio"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str]
+
+    def __repr__(self) -> str:
+        return f"RoleRL(id={self.id!r}, name={self.name!r})"
+
+
+class Task(Base):
+    __tablename__ = "task"
+    __table_args__ = {"schema": "label_studio"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str]
+    time: Mapped[Optional[int]]
+    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
+    modified_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), onupdate=func.now())
+    status: Mapped[str]
+    bbox: Mapped[Optional[Geometry]] = mapped_column(Geometry("POLYGON", srid=4326))
+    comments: Mapped[Optional[str]]
+    is_valid: Mapped[bool] = mapped_column(server_default='True')
+
+    batch_id: Mapped[int] = mapped_column(ForeignKey("label_studio.batch.id"))
+    batch: Mapped["Batch"] = relationship(back_populates="tasks")
+
+    images_rl: Mapped[List[ImageRL]] = relationship(
+        secondary="label_studio.association_task_image",
+        order_by="ImageRL.id"
+    )
+
+    labels: Mapped[List["Label"]] = relationship(
+        back_populates="task",
+        order_by="Label.id"
+    )
+
+    def __repr__(self) -> str:
+        return f"Task(id={self.id!r}, name={self.name!r}, time={self.time!r}, created_at={self.created_at!r}, modified_at={self.modified_at!r}, status={self.status!r}, comments={self.comments!r}, images_rl={self.images_rl!r}, bbox={self.bbox!r}, labels={self.labels!r})"
+
+
+class Type(Base):
+    __tablename__ = "type"
+    __table_args__ = {"schema": "label_studio"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str]
+    colour: Mapped[str] = mapped_column(String(7), default='#000000')
+
+    # association between Popject -> Association -> Type
+    # project_associations: Mapped[List["AssociationProjectType"]] = relationship(back_populates='type')
+
+    # many-to-many relationship to Type, bypassing the `Association` class
+    # projects: Mapped[List["Project"]] = relationship(
+    #     secondary="association_project_type",
+    #     back_populates="types"
+    # )
+
+    def __repr__(self) -> str:
+        return f"Type(id={self.id!r}, name={self.name!r}, colour={self.colour!r})"
+
+
```

### Comparing `rov_db_access-1.0.8/rov_db_access/label_studio/worker.py` & `rov_db_access-1.0.9/rov_db_access/label_studio/worker.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,210 +1,210 @@
-from typing import TypedDict, List
-from PIL import Image as im
-import io
-
-from rov_sent_api.sentinel_api import SentinelApi
-from shapely import wkt
-from sqlalchemy.orm import Session
-from sqlalchemy import select, insert
-
-from rov_db_access.config.db_utils import init_db_engine
-from rov_db_access.label_studio.models import Task, Label, Project
-from rov_db_access.config.settings import Settings
-from rov_db_access.utils.utils import wkbelement_to_wkt
-
-import rasterio
-from rasterio.session import AWSSession
-
-settings = Settings()
-
-SaveLabelDict = TypedDict("SaveLabelDict", {
-    "task_id": str,
-    "task_is_valid": bool,
-    "user_id": int,
-    "updated_labels": List[dict],
-    "new_labels": List[dict]
-})
-
-
-class RovLabelStudioWorker:
-
-    def __init__(self) -> None:
-
-        self.engine = init_db_engine(
-            settings.db_rov_gis_user,
-            settings.db_rov_gis_password,
-            settings.db_rov_gis_host,
-            settings.db_rov_gis_port,
-            settings.db_rov_gis_database
-        )
-
-    def load_projects(self):
-        with Session(self.engine) as session:
-            project_query = (
-                select(Project)
-            )
-            projects = session.execute(project_query).all()
-            projects_list = []
-            for project in projects:
-                project = project[0]
-                types = []
-                for type in project.types:
-                    types.append({
-                        "id": type.id,
-                        "name": type.name,
-                        "colour": type.colour
-                    })
-                batches = len(project.batches)
-                projects_list.append({
-                    "id": project.id,
-                    "name": project.name,
-                    "types": types,
-                    "batches": batches
-                })
-            return projects_list
-
-    def load_project(self, id: str):
-        with Session(self.engine) as session:
-            project_query = (
-                select(Project)
-                .where(Project.id == id)
-                .limit(1)
-            )
-            project = session.scalar(project_query)
-            if project is None:
-                return {}
-            print(f'Load project with id: {id} found! Batches:  #{len(project.batches)}')
-            types = []
-            for type in project.types:
-                types.append({
-                    "id": type.id,
-                    "name": type.name,
-                    "colour": type.colour
-                })
-            batches = []
-            for batch in project.batches:
-                tasks = []
-                for task in batch.tasks:
-                    tasks.append({
-                        "id": task.id,
-                        "name": task.name,
-                        "status": task.status
-                    })
-                batches.append({
-                    "id": batch.id,
-                    "name": batch.name,
-                    "tasks": tasks
-                })
-            return {
-                "id": project.id,
-                "name": project.name,
-                "types": types,
-                "batches": batches
-            }
-
-    def get_task(self, id: str):
-        with Session(self.engine) as session:
-            task_query = (
-                select(Task)
-                .where(Task.id == id)
-                .limit(1)
-            )
-            task = session.scalar(task_query)
-            if task is None:
-                return {}
-            print(f'Get task with id: {id} found is {task}')
-            bbox_wkt = wkbelement_to_wkt(task.bbox)
-            labels = []
-            images = []
-            for label in task.labels:
-                labels.append({
-                    "id": label.id,
-                    "name": label.name,
-                    "time": label.time,
-                    "status": label.status,
-                    "created_at": label.created_at,
-                    "modified_at": label.modified_at,
-                    "geom": wkbelement_to_wkt(label.geom),
-                    "type_id": label.type_id
-                })
-            for image in task.images_rl:
-                images.append({
-                    "id": image.id,
-                    "in_storage": image.in_storage,
-                    "url": image.url
-                })
-            return {
-                "id": task.id,
-                "name": task.name,
-                "time": task.time,
-                "bbox": bbox_wkt,
-                "created_at": task.created_at,
-                "modified_at": task.modified_at,
-                "status": task.status,
-                "comments": task.comments,
-                "is_valid": task.is_valid,
-                "labels": labels,
-                "images": images
-            }
-
-    def get_cog_image_window(self, path: str, geom: str):
-        geometry = wkt.loads(geom)
-        bbox = geometry.bounds
-        bbox_adapted = (bbox[0], bbox[3], bbox[2], bbox[1])
-        print(f'get_cog_image_window to find image path: {path} and bbox={bbox_adapted}')
-        rasterio_session = AWSSession(aws_unsigned=True, region_name='us-west-2', endpoint_url='s3.us-west-2.amazonaws.com')
-        with rasterio.Env(session=rasterio_session) as env:
-            sen_api = SentinelApi(settings.sentinel_user, settings.sentinel_password)
-            image_array = sen_api.extract_window_from_cog(
-                path,
-                'TCI',
-                window_coords=bbox_adapted
-            )
-            print("Rasterio image_array found! ")
-            data = im.fromarray(image_array, mode='RGB')
-            img_bytes = io.BytesIO()
-            data.save(img_bytes, format='png')
-            return img_bytes
-
-    def save_label(self, data: SaveLabelDict):
-        task_id = data["task_id"]
-        task_is_valid = data["task_is_valid"]
-        user_id = data["user_id"]
-        new_labels = data["new_labels"]
-
-        with Session(self.engine) as session:
-            task_query = (
-                select(Task)
-                .where(Task.id == task_id)
-                .limit(1)
-            )
-            task = session.scalar(task_query)
-            if task is None:
-                return False
-            print(f'Save label to task with id: {id} found is {task}')
-
-            new_labels_insertion = []
-            for new_label in new_labels:
-                new_labels_insertion.append({
-                    "name": new_label.get("name"),
-                    "time": new_label.get("time"),
-                    "status": "edited",
-                    "geom": new_label.get("geom"),
-                    "task_id": task_id,
-                    "user_id": user_id,
-                    "type_id": new_label.get("type_id")
-                })
-
-            task.is_valid = task_is_valid
-            task.status = "edited"
-
-            if len(new_labels_insertion) > 0:
-                session.execute(
-                    insert(Label),
-                    new_labels_insertion
-                )
-            try:
-                session.commit()
-                return True
-            except:
-                return False
+from typing import TypedDict, List
+from PIL import Image as im
+import io
+
+from rov_sent_api.sentinel_api import SentinelApi
+from shapely import wkt
+from sqlalchemy.orm import Session
+from sqlalchemy import select, insert
+
+from rov_db_access.config.db_utils import init_db_engine
+from rov_db_access.label_studio.models import Task, Label, Project
+from rov_db_access.config.settings import Settings
+from rov_db_access.utils.utils import wkbelement_to_wkt
+
+import rasterio
+from rasterio.session import AWSSession
+
+settings = Settings()
+
+SaveLabelDict = TypedDict("SaveLabelDict", {
+    "task_id": str,
+    "task_is_valid": bool,
+    "user_id": int,
+    "updated_labels": List[dict],
+    "new_labels": List[dict]
+})
+
+
+class RovLabelStudioWorker:
+
+    def __init__(self) -> None:
+
+        self.engine = init_db_engine(
+            settings.db_rov_gis_user,
+            settings.db_rov_gis_password,
+            settings.db_rov_gis_host,
+            settings.db_rov_gis_port,
+            settings.db_rov_gis_database
+        )
+
+    def load_projects(self):
+        with Session(self.engine) as session:
+            project_query = (
+                select(Project)
+            )
+            projects = session.execute(project_query).all()
+            projects_list = []
+            for project in projects:
+                project = project[0]
+                types = []
+                for type in project.types:
+                    types.append({
+                        "id": type.id,
+                        "name": type.name,
+                        "colour": type.colour
+                    })
+                batches = len(project.batches)
+                projects_list.append({
+                    "id": project.id,
+                    "name": project.name,
+                    "types": types,
+                    "batches": batches
+                })
+            return projects_list
+
+    def load_project(self, id: str):
+        with Session(self.engine) as session:
+            project_query = (
+                select(Project)
+                .where(Project.id == id)
+                .limit(1)
+            )
+            project = session.scalar(project_query)
+            if project is None:
+                return {}
+            print(f'Load project with id: {id} found! Batches:  #{len(project.batches)}')
+            types = []
+            for type in project.types:
+                types.append({
+                    "id": type.id,
+                    "name": type.name,
+                    "colour": type.colour
+                })
+            batches = []
+            for batch in project.batches:
+                tasks = []
+                for task in batch.tasks:
+                    tasks.append({
+                        "id": task.id,
+                        "name": task.name,
+                        "status": task.status
+                    })
+                batches.append({
+                    "id": batch.id,
+                    "name": batch.name,
+                    "tasks": tasks
+                })
+            return {
+                "id": project.id,
+                "name": project.name,
+                "types": types,
+                "batches": batches
+            }
+
+    def get_task(self, id: str):
+        with Session(self.engine) as session:
+            task_query = (
+                select(Task)
+                .where(Task.id == id)
+                .limit(1)
+            )
+            task = session.scalar(task_query)
+            if task is None:
+                return {}
+            print(f'Get task with id: {id} found is {task}')
+            bbox_wkt = wkbelement_to_wkt(task.bbox)
+            labels = []
+            images = []
+            for label in task.labels:
+                labels.append({
+                    "id": label.id,
+                    "name": label.name,
+                    "time": label.time,
+                    "status": label.status,
+                    "created_at": label.created_at,
+                    "modified_at": label.modified_at,
+                    "geom": wkbelement_to_wkt(label.geom),
+                    "type_id": label.type_id
+                })
+            for image in task.images_rl:
+                images.append({
+                    "id": image.id,
+                    "in_storage": image.in_storage,
+                    "url": image.url
+                })
+            return {
+                "id": task.id,
+                "name": task.name,
+                "time": task.time,
+                "bbox": bbox_wkt,
+                "created_at": task.created_at,
+                "modified_at": task.modified_at,
+                "status": task.status,
+                "comments": task.comments,
+                "is_valid": task.is_valid,
+                "labels": labels,
+                "images": images
+            }
+
+    def get_cog_image_window(self, path: str, geom: str):
+        geometry = wkt.loads(geom)
+        bbox = geometry.bounds
+        bbox_adapted = (bbox[0], bbox[3], bbox[2], bbox[1])
+        print(f'get_cog_image_window to find image path: {path} and bbox={bbox_adapted}')
+        rasterio_session = AWSSession(aws_unsigned=True, region_name='us-west-2', endpoint_url='s3.us-west-2.amazonaws.com')
+        with rasterio.Env(session=rasterio_session) as env:
+            sen_api = SentinelApi(settings.sentinel_user, settings.sentinel_password)
+            image_array = sen_api.extract_window_from_cog(
+                path,
+                'TCI',
+                window_coords=bbox_adapted
+            )
+            print("Rasterio image_array found! ")
+            data = im.fromarray(image_array, mode='RGB')
+            img_bytes = io.BytesIO()
+            data.save(img_bytes, format='png')
+            return img_bytes
+
+    def save_label(self, data: SaveLabelDict):
+        task_id = data["task_id"]
+        task_is_valid = data["task_is_valid"]
+        user_id = data["user_id"]
+        new_labels = data["new_labels"]
+
+        with Session(self.engine) as session:
+            task_query = (
+                select(Task)
+                .where(Task.id == task_id)
+                .limit(1)
+            )
+            task = session.scalar(task_query)
+            if task is None:
+                return False
+            print(f'Save label to task with id: {id} found is {task}')
+
+            new_labels_insertion = []
+            for new_label in new_labels:
+                new_labels_insertion.append({
+                    "name": new_label.get("name"),
+                    "time": new_label.get("time"),
+                    "status": "edited",
+                    "geom": new_label.get("geom"),
+                    "task_id": task_id,
+                    "user_id": user_id,
+                    "type_id": new_label.get("type_id")
+                })
+
+            task.is_valid = task_is_valid
+            task.status = "edited"
+
+            if len(new_labels_insertion) > 0:
+                session.execute(
+                    insert(Label),
+                    new_labels_insertion
+                )
+            try:
+                session.commit()
+                return True
+            except:
+                return False
```

### Comparing `rov_db_access-1.0.8/rov_db_access/landing/models.py` & `rov_db_access-1.0.9/rov_db_access/landing/models.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from datetime import datetime
-from typing import Optional
-
-from geoalchemy2 import Geometry
-from sqlalchemy import DateTime, func
-from sqlalchemy.orm import DeclarativeBase
-from sqlalchemy.orm import Mapped
-from sqlalchemy.orm import mapped_column
-
-
-class Base(DeclarativeBase):
-    """Base Class of the model"""
-
-
-class Articles(Base):
-    __tablename__ = "articles"
-    id: Mapped[int] = mapped_column(primary_key=True)
-    title: Mapped[str]
-    content: Mapped[str]
-    location: Mapped[Optional[Geometry]] = mapped_column(Geometry("POINT", srid=4326))
-    zoom: Mapped[float] = mapped_column(server_default="1")
-    date: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
-
-    def __repr__(self) -> str:
-        return f"Articles (id={self.id!r},  title={self.title!r})"
-
-
-class Members(Base):
-    __tablename__ = "members"
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[str]
-    profession: Mapped[str]
-    description: Mapped[Optional[str]]
-    photo_url: Mapped[str]
-    linkedin: Mapped[Optional[str]]
-    github: Mapped[Optional[str]]
-    order: Mapped[int] = mapped_column(server_default="999")
-    job: Mapped[str]
-
-    def __repr__(self) -> str:
-        return f"Members (id={self.id!r},  name={self.name!r})"
-
-
-class Newsletter(Base):
-    __tablename__ = "newsletter"
-    id: Mapped[int] = mapped_column(primary_key=True)
-    title: Mapped[str]
-    content: Mapped[str]
-    author: Mapped[str]
-    is_published: Mapped[bool] = mapped_column(server_default='False')
-    date: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
-
-    def __repr__(self) -> str:
-        return f"Newsletter (id={self.id!r},  title={self.title!r})"
-
-
-class Subscribers(Base):
-    __tablename__ = "subscribers"
-    id: Mapped[int] = mapped_column(primary_key=True)
-    name: Mapped[str]
-    email: Mapped[str]
-    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
-
-    def __repr__(self) -> str:
+from datetime import datetime
+from typing import Optional
+
+from geoalchemy2 import Geometry
+from sqlalchemy import DateTime, func
+from sqlalchemy.orm import DeclarativeBase
+from sqlalchemy.orm import Mapped
+from sqlalchemy.orm import mapped_column
+
+
+class Base(DeclarativeBase):
+    """Base Class of the model"""
+
+
+class Articles(Base):
+    __tablename__ = "articles"
+    id: Mapped[int] = mapped_column(primary_key=True)
+    title: Mapped[str]
+    content: Mapped[str]
+    location: Mapped[Optional[Geometry]] = mapped_column(Geometry("POINT", srid=4326))
+    zoom: Mapped[float] = mapped_column(server_default="1")
+    date: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
+
+    def __repr__(self) -> str:
+        return f"Articles (id={self.id!r},  title={self.title!r})"
+
+
+class Members(Base):
+    __tablename__ = "members"
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str]
+    profession: Mapped[str]
+    description: Mapped[Optional[str]]
+    photo_url: Mapped[str]
+    linkedin: Mapped[Optional[str]]
+    github: Mapped[Optional[str]]
+    order: Mapped[int] = mapped_column(server_default="999")
+    job: Mapped[str]
+
+    def __repr__(self) -> str:
+        return f"Members (id={self.id!r},  name={self.name!r})"
+
+
+class Newsletter(Base):
+    __tablename__ = "newsletter"
+    id: Mapped[int] = mapped_column(primary_key=True)
+    title: Mapped[str]
+    content: Mapped[str]
+    author: Mapped[str]
+    is_published: Mapped[bool] = mapped_column(server_default='False')
+    date: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
+
+    def __repr__(self) -> str:
+        return f"Newsletter (id={self.id!r},  title={self.title!r})"
+
+
+class Subscribers(Base):
+    __tablename__ = "subscribers"
+    id: Mapped[int] = mapped_column(primary_key=True)
+    name: Mapped[str]
+    email: Mapped[str]
+    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
+
+    def __repr__(self) -> str:
         return f"Subscribers (id={self.id!r},  name={self.name!r})"
```

### Comparing `rov_db_access-1.0.8/rov_db_access/risks/models.py` & `rov_db_access-1.0.9/rov_db_access/risks/models.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from datetime import datetime
-from typing import Optional
-
-from geoalchemy2 import Geometry
-from sqlalchemy import DateTime, ForeignKey, JSON, func
-from sqlalchemy.orm import Mapped, mapped_column, relationship
-
-from rov_db_access.authentication.models import User, Base as GisBase
-
-
-class UserResultsHistory(GisBase):
-    __tablename__ = "user_results_history"
-    __table_args__ = {"schema": "risks"}
-    id: Mapped[int] = mapped_column(primary_key=True)
-    user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"))
-    user: Mapped["User"] = relationship()
-    name: Mapped[str]
-    address: Mapped[str]
-    location: Mapped[Geometry] = mapped_column(Geometry("POINT", srid=4326))
-    data: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
-    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
-    saved: Mapped[Optional[bool]] = mapped_column(server_default="false")
-
-    def __repr__(self) -> str:
-        return f"UserResultsHistory (id={self.id!r}, name={self.name!r}, address={self.address!r} user_id={self.user_id!r}, location={self.location!r}, data={self.data!r}, created_at={self.created_at!r})"
+from datetime import datetime
+from typing import Optional
+
+from geoalchemy2 import Geometry
+from sqlalchemy import DateTime, ForeignKey, JSON, func
+from sqlalchemy.orm import Mapped, mapped_column, relationship
+
+from rov_db_access.authentication.models import User, Base as GisBase
+
+
+class UserResultsHistory(GisBase):
+    __tablename__ = "user_results_history"
+    __table_args__ = {"schema": "risks"}
+    id: Mapped[int] = mapped_column(primary_key=True)
+    user_id: Mapped[int] = mapped_column(ForeignKey("admin.user.id"))
+    user: Mapped["User"] = relationship()
+    name: Mapped[str]
+    address: Mapped[str]
+    location: Mapped[Geometry] = mapped_column(Geometry("POINT", srid=4326))
+    data: Mapped[Optional[JSON]] = mapped_column(type_=JSON)
+    created_at: Mapped[Optional[datetime]] = mapped_column(DateTime(timezone=True), server_default=func.now())
+    saved: Mapped[Optional[bool]] = mapped_column(server_default="false")
+
+    def __repr__(self) -> str:
+        return f"UserResultsHistory (id={self.id!r}, name={self.name!r}, address={self.address!r} user_id={self.user_id!r}, location={self.location!r}, data={self.data!r}, created_at={self.created_at!r})"
```

### Comparing `rov_db_access-1.0.8/rov_db_access/risks/worker.py` & `rov_db_access-1.0.9/rov_db_access/risks/worker.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-from typing import TypedDict, List
-
-from geoalchemy2 import WKTElement
-from geoalchemy2.shape import to_shape
-from sqlalchemy.orm import Session, Bundle
-from sqlalchemy import select, func
-from rov_db_access.config.db_utils import init_db_engine
-from rov_db_access.config.settings import Settings
-from shapely import wkb
-from pyproj import Transformer
-
-from rov_db_access.utils.utils import wkbelement_to_wkt
-from rov_db_access.geodata.models import FloodHazard, TsunamiHazard, RMHazard, VolcanicHazard, VolcanicHazardPyroclast, WildfireHazard
-from rov_db_access.risks.models import UserResultsHistory
-
-settings = Settings()
-
-CalculateRiskDict = TypedDict("CalculateRiskDict", {"lat": float, "lng": float, "radius": int, "layers": List[str]})
-Risks = [FloodHazard, TsunamiHazard, RMHazard, VolcanicHazard, VolcanicHazardPyroclast, WildfireHazard]
-
-
-class RisksWorker:
-
-    def __init__(self) -> None:
-
-        self.engine = init_db_engine(
-            settings.db_rov_geodata_user,
-            settings.db_rov_geodata_password,
-            settings.db_rov_geodata_host,
-            settings.db_rov_geodata_port,
-            settings.db_rov_geodata_database
-        )
-
-    def calculate_risk(self, data: CalculateRiskDict):
-        lat = data.get("lat")
-        lng = data.get("lng")
-        radius = data.get("radius")
-        layers = data.get("layers")
-        transformer = Transformer.from_crs("EPSG:4326", "EPSG:32719")
-        e, n = transformer.transform(lat, lng)
-
-        point_wkt_32719 = WKTElement('POINT({0} {1})'.format(e, n), srid=32719)
-        point_32719_geom = to_shape(point_wkt_32719)
-        circle_32719_geom = point_32719_geom.buffer(radius)
-        circle_32719_wkb = wkb.dumps(circle_32719_geom, hex=True, srid=32719)
-        circle_32719_area = circle_32719_geom.area
-
-        with Session(self.engine) as session:
-            result = {}
-            for layer in layers:
-                result[layer] = []
-                risk_classes = list(filter(lambda x: x.__tablename__ == layer, Risks))
-                if len(risk_classes) < 1:
-                    break
-                risk_class = risk_classes[0]
-
-                risk_query = (
-                    select(
-                        Bundle(
-                            "risk",
-                            risk_class.id,
-                            risk_class.risk_weight,
-                            func.ST_Transform(risk_class.geom, 4326)
-                        ),
-                        Bundle(
-                            "data",
-                            func.ST_Transform(
-                                func.ST_Intersection(circle_32719_wkb, func.ST_Transform(risk_class.geom, 32719)),
-                                4326
-                            ),
-                            func.ST_Area(
-                                func.ST_Intersection(circle_32719_wkb, func.ST_Transform(risk_class.geom, 32719))
-                            ),
-                            func.ST_Distance(
-                                point_wkt_32719,
-                                func.ST_Transform(risk_class.geom, 32719)
-                            )
-                        )
-                    )
-                    .where(func.ST_Intersects(circle_32719_wkb, func.ST_Transform(risk_class.geom, 32719)))
-                )
-
-                risk_result = session.execute(risk_query)
-                for row in risk_result:
-                    print(f"layer: {layer}, risk id {row.risk.id}")
-                    percentage = round(100 * row.data.ST_Area / circle_32719_area, 2)
-                    weight = row.risk.risk_weight
-                    score = weight * (row.data.ST_Area / circle_32719_area) + (1-weight)/(row.data.ST_Distance + 1)
-                    print(f"layer: {layer}, distance: {row.data.ST_Distance}, area: {row.data.ST_Area}, score: {score}")
-                    result[layer].append({
-                        "id": row.risk.id,
-                        "risk_weight": row.risk.risk_weight,
-                        "geom": wkbelement_to_wkt(row.risk.ST_Transform),
-                        "intersection": wkbelement_to_wkt(row.data.ST_Transform),
-                        "area_intersected": row.data.ST_Area,
-                        "distance": row.data.ST_Distance,
-                        "percentage_covered": percentage,
-                        "score": score
-                    })
-            return result
-
-
-class GisRisksWorker:
-
-    def __init__(self) -> None:
-        self.engine = init_db_engine(
-            settings.db_rov_gis_user,
-            settings.db_rov_gis_password,
-            settings.db_rov_gis_host,
-            settings.db_rov_gis_port,
-            settings.db_rov_gis_database
-        )
-
-    def register_user_result(self, user_id: int, lat: float, lng: float, data: str, name: str, address: str):
-        location = WKTElement(f'POINT({lng} {lat})', srid=4326)
-        with Session(self.engine) as session:
-            user_results_history = UserResultsHistory(user_id=user_id, location=location, data=data, name=name, address=address)
-            session.add(user_results_history)
-            session.commit()
-            return {"id": user_results_history.id, "location": f'POINT({lng} {lat})', "name": user_results_history.name, "address": user_results_history.address}
-
-    def get_user_results(self, user_id: int):
-        with Session(self.engine) as session:
-            user_results_history = session.query(UserResultsHistory).filter(UserResultsHistory.user_id == user_id).all()
-            results = []
-            for result in user_results_history:
-                results.append({
-                    "id": result.id,
-                    "name": result.name,
-                    "address": result.address,
-                    "location": wkbelement_to_wkt(result.location),
-                    "data": result.data,
-                    "created_at": result.created_at,
-                    "saved": result.saved
-                })
-            return results
-
-    def save_analysis(self, user_id: int, analysis_id: int, saved: bool):
-        with Session(self.engine) as session:
-            user_results_history = session.query(UserResultsHistory).filter(UserResultsHistory.user_id == user_id).filter(UserResultsHistory.id == analysis_id).first()
-            user_results_history.saved = saved
-            session.commit()
-            return {
-                "id": user_results_history.id,
-                "name": user_results_history.name,
-                "saved": user_results_history.saved
-            }
+from typing import TypedDict, List
+
+from geoalchemy2 import WKTElement
+from geoalchemy2.shape import to_shape
+from sqlalchemy.orm import Session, Bundle
+from sqlalchemy import select, func
+from rov_db_access.config.db_utils import init_db_engine
+from rov_db_access.config.settings import Settings
+from shapely import wkb
+from pyproj import Transformer
+
+from rov_db_access.utils.utils import wkbelement_to_wkt
+from rov_db_access.geodata.models import FloodHazard, TsunamiHazard, RMHazard, VolcanicHazard, VolcanicHazardPyroclast, WildfireHazard
+from rov_db_access.risks.models import UserResultsHistory
+
+settings = Settings()
+
+CalculateRiskDict = TypedDict("CalculateRiskDict", {"lat": float, "lng": float, "radius": int, "layers": List[str]})
+Risks = [FloodHazard, TsunamiHazard, RMHazard, VolcanicHazard, VolcanicHazardPyroclast, WildfireHazard]
+
+
+class RisksWorker:
+
+    def __init__(self) -> None:
+
+        self.engine = init_db_engine(
+            settings.db_rov_geodata_user,
+            settings.db_rov_geodata_password,
+            settings.db_rov_geodata_host,
+            settings.db_rov_geodata_port,
+            settings.db_rov_geodata_database
+        )
+
+    def calculate_risk(self, data: CalculateRiskDict):
+        lat = data.get("lat")
+        lng = data.get("lng")
+        radius = data.get("radius")
+        layers = data.get("layers")
+        transformer = Transformer.from_crs("EPSG:4326", "EPSG:32719")
+        e, n = transformer.transform(lat, lng)
+
+        point_wkt_32719 = WKTElement('POINT({0} {1})'.format(e, n), srid=32719)
+        point_32719_geom = to_shape(point_wkt_32719)
+        circle_32719_geom = point_32719_geom.buffer(radius)
+        circle_32719_wkb = wkb.dumps(circle_32719_geom, hex=True, srid=32719)
+        circle_32719_area = circle_32719_geom.area
+
+        with Session(self.engine) as session:
+            result = {}
+            for layer in layers:
+                result[layer] = []
+                risk_classes = list(filter(lambda x: x.__tablename__ == layer, Risks))
+                if len(risk_classes) < 1:
+                    break
+                risk_class = risk_classes[0]
+
+                risk_query = (
+                    select(
+                        Bundle(
+                            "risk",
+                            risk_class.id,
+                            risk_class.risk_weight,
+                            func.ST_Transform(risk_class.geom, 4326)
+                        ),
+                        Bundle(
+                            "data",
+                            func.ST_Transform(
+                                func.ST_Intersection(circle_32719_wkb, func.ST_Transform(risk_class.geom, 32719)),
+                                4326
+                            ),
+                            func.ST_Area(
+                                func.ST_Intersection(circle_32719_wkb, func.ST_Transform(risk_class.geom, 32719))
+                            ),
+                            func.ST_Distance(
+                                point_wkt_32719,
+                                func.ST_Transform(risk_class.geom, 32719)
+                            )
+                        )
+                    )
+                    .where(func.ST_Intersects(circle_32719_wkb, func.ST_Transform(risk_class.geom, 32719)))
+                )
+
+                risk_result = session.execute(risk_query)
+                for row in risk_result:
+                    print(f"layer: {layer}, risk id {row.risk.id}")
+                    percentage = round(100 * row.data.ST_Area / circle_32719_area, 2)
+                    weight = row.risk.risk_weight
+                    score = weight * (row.data.ST_Area / circle_32719_area) + (1-weight)/(row.data.ST_Distance + 1)
+                    print(f"layer: {layer}, distance: {row.data.ST_Distance}, area: {row.data.ST_Area}, score: {score}")
+                    result[layer].append({
+                        "id": row.risk.id,
+                        "risk_weight": row.risk.risk_weight,
+                        "geom": wkbelement_to_wkt(row.risk.ST_Transform),
+                        "intersection": wkbelement_to_wkt(row.data.ST_Transform),
+                        "area_intersected": row.data.ST_Area,
+                        "distance": row.data.ST_Distance,
+                        "percentage_covered": percentage,
+                        "score": score
+                    })
+            return result
+
+
+class GisRisksWorker:
+
+    def __init__(self) -> None:
+        self.engine = init_db_engine(
+            settings.db_rov_gis_user,
+            settings.db_rov_gis_password,
+            settings.db_rov_gis_host,
+            settings.db_rov_gis_port,
+            settings.db_rov_gis_database
+        )
+
+    def register_user_result(self, user_id: int, lat: float, lng: float, data: str, name: str, address: str):
+        location = WKTElement(f'POINT({lng} {lat})', srid=4326)
+        with Session(self.engine) as session:
+            user_results_history = UserResultsHistory(user_id=user_id, location=location, data=data, name=name, address=address)
+            session.add(user_results_history)
+            session.commit()
+            return {"id": user_results_history.id, "location": f'POINT({lng} {lat})', "name": user_results_history.name, "address": user_results_history.address}
+
+    def get_user_results(self, user_id: int):
+        with Session(self.engine) as session:
+            user_results_history = session.query(UserResultsHistory).filter(UserResultsHistory.user_id == user_id).all()
+            results = []
+            for result in user_results_history:
+                results.append({
+                    "id": result.id,
+                    "name": result.name,
+                    "address": result.address,
+                    "location": wkbelement_to_wkt(result.location),
+                    "data": result.data,
+                    "created_at": result.created_at,
+                    "saved": result.saved
+                })
+            return results
+
+    def save_analysis(self, user_id: int, analysis_id: int, saved: bool):
+        with Session(self.engine) as session:
+            user_results_history = session.query(UserResultsHistory).filter(UserResultsHistory.user_id == user_id).filter(UserResultsHistory.id == analysis_id).first()
+            user_results_history.saved = saved
+            session.commit()
+            return {
+                "id": user_results_history.id,
+                "name": user_results_history.name,
+                "saved": user_results_history.saved
+            }
```

### Comparing `rov_db_access-1.0.8/rov_db_access/sentinel/worker.py` & `rov_db_access-1.0.9/rov_db_access/sentinel/worker.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-import re
-from datetime import datetime
-from typing import TypedDict
-
-from rov_sent_api.sentinel_api import SentinelApi
-from sqlalchemy.orm import Session
-from sqlalchemy import select
-
-from rov_db_access.config.db_utils import init_db_engine
-from rov_db_access.sentinel.models import Tiles
-from rov_db_access.config.settings import Settings
-from rov_db_access.utils.utils import wkbelement_to_wkt
-
-settings = Settings()
-
-SentinelSearchDict = TypedDict("SentinelSearchDict", {
-    "tile": str,
-    "init_date": str,
-    "end_date": str,
-    "cloud": int
-})
-SentinelSearchByGeomDict = TypedDict("SentinelSearchByGeomDict", {
-    "polygon": str,
-    "init_date": str,
-    "end_date": str,
-    "cloud": int
-})
-SentinelImageDict = TypedDict("SentinelImageDict", {
-    "uuid": str,
-    "tile": str,
-    "date": str,
-    "cloud": float,
-    "footprint": str
-})
-
-
-def is_valid_uuid(input_string):
-    pattern = r"^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$"
-    return bool(re.match(pattern, input_string))
-
-# def get_presigned_url_s3_by_key(s3_key):
-#         if s3_key is None:
-#             return None
-#
-#         s3 = boto3.client("s3", aws_access_key_id=settings.aws_key,
-#                           aws_secret_access_key=settings.aws_secret,
-#                           config=Config(signature_version='s3v4', region_name='us-east-2'))
-#         try:
-#             url = s3.generate_presigned_url(
-#                 'get_object',
-#                 Params={'Bucket': settings.sentinel_s3_bucket,
-#                         'Key': f"{s3_key}"},
-#                 ExpiresIn=60
-#             )
-#             return url
-#         except ClientError as e:
-#             return None
-
-
-class SentinelSearchWorker:
-
-    def __init__(self) -> None:
-
-        self.products = None
-
-        self.engine = init_db_engine(
-            settings.db_rov_sentinel_user,
-            settings.db_rov_sentinel_password,
-            settings.db_rov_sentinel_host,
-            settings.db_rov_sentinel_port,
-            settings.db_rov_sentinel_database
-        )
-
-    def get_products_by_tile(self, query: SentinelSearchDict):
-        query["init_date"] = datetime.strptime(query["init_date"], "%d/%m/%Y")
-        query["end_date"] = datetime.strptime(query["end_date"], "%d/%m/%Y")
-        tile = query.pop("tile")
-        init_date = query.pop("init_date")
-        end_date = query.pop("end_date")
-        cloud = query.pop("cloud")
-
-        sen_api = SentinelApi(settings.sentinel_user, settings.sentinel_password)
-        self.products = sen_api.find(
-            sen_api.ProductType.S2MSI2A,
-            tile=tile,
-            init_date=init_date,
-            end_date=end_date,
-            cloud_cover=cloud
-        )
-        print("Sentinel query results count : ", len(self.products))
-
-        l2_products = {}
-
-        for product in self.products:
-            l2_products[product["id"]] = product
-
-        results = []
-        for uuid, product in l2_products.items():
-            try:
-                online = sen_api.sentinel.is_online(uuid)
-            except:
-                online = False
-
-            results.append({
-                "title": product["title"],
-                "date": product["date"].strftime("%d/%m/%Y"),
-                "tile": product["tileId"],
-                "cloud": product["cloudCover"],
-                "uuid": product["id"],
-                "footprint": product["footprint"],
-                "online": online,
-                "quicklook": product["Quicklook"]
-            })
-        return results
-
-    def get_geom_tiles(self):
-        result_tiles = []
-        with Session(self.engine) as session:
-            query = select(Tiles).where(Tiles.required).order_by(Tiles.name)
-            for tile in session.scalars(query):
-                geom_wkt = wkbelement_to_wkt(tile.geom)
-                result_tiles.append({
-                    "id": tile.id,
-                    "name": tile.name,
-                    "geom": geom_wkt
-                })
-            return result_tiles
-
-    def get_products_by_geom(self, query: SentinelSearchByGeomDict):
-        polygon = query.pop("polygon")
-        query["init_date"] = datetime.strptime(query["init_date"], "%d/%m/%Y")
-        query["end_date"] = datetime.strptime(query["end_date"], "%d/%m/%Y")
-        init_date = query.pop("init_date")
-        end_date = query.pop("end_date")
-        cloud = query.pop("cloud")
-        sen_api = SentinelApi(settings.sentinel_user, settings.sentinel_password)
-        print("Sentinel query by geom input polygont: ", polygon)
-        self.products = sen_api.findGeom(
-            productType=SentinelApi.ProductType.S2MSI2A,
-            polygon=polygon,
-            init_date=init_date,
-            end_date=end_date,
-            cloud_cover=cloud
-        )
-        print("Sentinel query by geom results count: ", len(self.products))
-
-        l2_products = {}
-
-        for product in self.products:
-            l2_products[product["id"]] = product
-
-        results = []
-        for uuid, product in l2_products.items():
-            results.append({
-                "title": product["title"],
-                "date": product["date"].strftime("%d/%m/%Y"),
-                "tile": product["tileId"],
-                "cloud": product["cloudCover"],
-                "uuid": product["id"],
-                "footprint": product["footprint"],
-                "quicklook": product["Quicklook"]
-            })
-        return results
-
-    def get_tile(self, name: str):
-        with Session(self.engine) as session:
-            query = select(Tiles).where(Tiles.name == name)
-            tile = session.scalar(query)
-            geom_wkt = wkbelement_to_wkt(tile.geom)
-            return {
-                "id": tile.id,
-                "name": tile.name,
-                "geom": geom_wkt,
-                "required": tile.required
-            }
+import re
+from datetime import datetime
+from typing import TypedDict
+
+from rov_sent_api.sentinel_api import SentinelApi
+from sqlalchemy.orm import Session
+from sqlalchemy import select
+
+from rov_db_access.config.db_utils import init_db_engine
+from rov_db_access.sentinel.models import Tiles
+from rov_db_access.config.settings import Settings
+from rov_db_access.utils.utils import wkbelement_to_wkt
+
+settings = Settings()
+
+SentinelSearchDict = TypedDict("SentinelSearchDict", {
+    "tile": str,
+    "init_date": str,
+    "end_date": str,
+    "cloud": int
+})
+SentinelSearchByGeomDict = TypedDict("SentinelSearchByGeomDict", {
+    "polygon": str,
+    "init_date": str,
+    "end_date": str,
+    "cloud": int
+})
+SentinelImageDict = TypedDict("SentinelImageDict", {
+    "uuid": str,
+    "tile": str,
+    "date": str,
+    "cloud": float,
+    "footprint": str
+})
+
+
+def is_valid_uuid(input_string):
+    pattern = r"^[0-9a-fA-F]{8}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{4}-[0-9a-fA-F]{12}$"
+    return bool(re.match(pattern, input_string))
+
+# def get_presigned_url_s3_by_key(s3_key):
+#         if s3_key is None:
+#             return None
+#
+#         s3 = boto3.client("s3", aws_access_key_id=settings.aws_key,
+#                           aws_secret_access_key=settings.aws_secret,
+#                           config=Config(signature_version='s3v4', region_name='us-east-2'))
+#         try:
+#             url = s3.generate_presigned_url(
+#                 'get_object',
+#                 Params={'Bucket': settings.sentinel_s3_bucket,
+#                         'Key': f"{s3_key}"},
+#                 ExpiresIn=60
+#             )
+#             return url
+#         except ClientError as e:
+#             return None
+
+
+class SentinelSearchWorker:
+
+    def __init__(self) -> None:
+
+        self.products = None
+
+        self.engine = init_db_engine(
+            settings.db_rov_sentinel_user,
+            settings.db_rov_sentinel_password,
+            settings.db_rov_sentinel_host,
+            settings.db_rov_sentinel_port,
+            settings.db_rov_sentinel_database
+        )
+
+    def get_products_by_tile(self, query: SentinelSearchDict):
+        query["init_date"] = datetime.strptime(query["init_date"], "%d/%m/%Y")
+        query["end_date"] = datetime.strptime(query["end_date"], "%d/%m/%Y")
+        tile = query.pop("tile")
+        init_date = query.pop("init_date")
+        end_date = query.pop("end_date")
+        cloud = query.pop("cloud")
+
+        sen_api = SentinelApi(settings.sentinel_user, settings.sentinel_password)
+        self.products = sen_api.find(
+            sen_api.ProductType.S2MSI2A,
+            tile=tile,
+            init_date=init_date,
+            end_date=end_date,
+            cloud_cover=cloud
+        )
+        print("Sentinel query results count : ", len(self.products))
+
+        l2_products = {}
+
+        for product in self.products:
+            l2_products[product["id"]] = product
+
+        results = []
+        for uuid, product in l2_products.items():
+            try:
+                online = sen_api.sentinel.is_online(uuid)
+            except:
+                online = False
+
+            results.append({
+                "title": product["title"],
+                "date": product["date"].strftime("%d/%m/%Y"),
+                "tile": product["tileId"],
+                "cloud": product["cloudCover"],
+                "uuid": product["id"],
+                "footprint": product["footprint"],
+                "online": online,
+                "quicklook": product["Quicklook"]
+            })
+        return results
+
+    def get_geom_tiles(self):
+        result_tiles = []
+        with Session(self.engine) as session:
+            query = select(Tiles).where(Tiles.required).order_by(Tiles.name)
+            for tile in session.scalars(query):
+                geom_wkt = wkbelement_to_wkt(tile.geom)
+                result_tiles.append({
+                    "id": tile.id,
+                    "name": tile.name,
+                    "geom": geom_wkt
+                })
+            return result_tiles
+
+    def get_products_by_geom(self, query: SentinelSearchByGeomDict):
+        polygon = query.pop("polygon")
+        query["init_date"] = datetime.strptime(query["init_date"], "%d/%m/%Y")
+        query["end_date"] = datetime.strptime(query["end_date"], "%d/%m/%Y")
+        init_date = query.pop("init_date")
+        end_date = query.pop("end_date")
+        cloud = query.pop("cloud")
+        sen_api = SentinelApi(settings.sentinel_user, settings.sentinel_password)
+        print("Sentinel query by geom input polygont: ", polygon)
+        self.products = sen_api.findGeom(
+            productType=SentinelApi.ProductType.S2MSI2A,
+            polygon=polygon,
+            init_date=init_date,
+            end_date=end_date,
+            cloud_cover=cloud
+        )
+        print("Sentinel query by geom results count: ", len(self.products))
+
+        l2_products = {}
+
+        for product in self.products:
+            l2_products[product["id"]] = product
+
+        results = []
+        for uuid, product in l2_products.items():
+            results.append({
+                "title": product["title"],
+                "date": product["date"].strftime("%d/%m/%Y"),
+                "tile": product["tileId"],
+                "cloud": product["cloudCover"],
+                "uuid": product["id"],
+                "footprint": product["footprint"],
+                "quicklook": product["Quicklook"]
+            })
+        return results
+
+    def get_tile(self, name: str):
+        with Session(self.engine) as session:
+            query = select(Tiles).where(Tiles.name == name)
+            tile = session.scalar(query)
+            geom_wkt = wkbelement_to_wkt(tile.geom)
+            return {
+                "id": tile.id,
+                "name": tile.name,
+                "geom": geom_wkt,
+                "required": tile.required
+            }
```

### Comparing `rov_db_access-1.0.8/rov_db_access/utils/geoserver_utils.py` & `rov_db_access-1.0.9/rov_db_access/utils/geoserver_utils.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,144 +1,144 @@
-import os
-import urllib
-from pprint import pprint
-from rov_db_access.config.settings import Settings
-
-import requests
-settings = Settings()
-
-
-class GeoServerClient:
-    workspace = None
-
-    def __init__(self):
-        self.server_url = settings.geoserver_api_url
-        self.session = requests.Session()
-        self.session.auth = (settings.geoserver_api_user, settings.geoserver_api_password)
-        self.url = settings.geoserver_api_url + "/geoserver/rest"
-
-    def __coverage_store_url(self) -> str:
-        return os.path.join(self.url, f"workspaces/{self.workspace}/coveragestores")
-
-    def reload_config(self):
-        """
-        Reloads the GeoServer catalog and configuration from disk.
-        This operation is used in cases where an external tool has modified the on-disk configuration.
-        This operation will also force GeoServer to drop any internal caches and reconnect to all data stores.
-        """
-        try:
-            self.session.post(url=f"{self.url}/reload")
-            print("Geoserver config reloaded")
-        except Exception as e:
-            print(f"Error reloading config: {e}")
-
-    def set_workspace(self, workspace: str):
-        self.workspace = workspace
-
-    def add_mosaic_granule(self, coverage_store: str, granule_path: str):
-        """Adds a new granule to an existing imagemosaic
-
-        Args:
-            coverage_store (str): name of the coverage store
-            granule_path (str): url to granule
-        """
-        try:
-            response = self.session.post(
-                url=os.path.join(
-                    self.__coverage_store_url(), f"{coverage_store}/remote.imagemosaic"
-                ),
-                data=granule_path,
-                headers={"Content-Type": "text/plain"},
-            )
-            response.raise_for_status()
-            print(f'Geoserver new granule added for coverage: {coverage_store}')
-            return response
-        except Exception as e:
-            print(f"Error adding granule into coverage: {coverage_store}. ERROR: {e}")
-            return None
-
-    def create_empty_mosaic(self, coverage_store: str, zip_path: str):
-        """Creates an empty mosaic in geoserver
-
-        Args:
-            coverage_store (str): name of the coverage store
-            zip_path (str): path to a .zip file containing .properties configuration files
-            for mosaic
-        """
-        with open(zip_path, "rb") as zip:
-            data = zip.read()
-        response = self.session.put(
-            url=os.path.join(
-                self.__coverage_store_url(),
-                f"{coverage_store}/file.imagemosaic?configure=none",
-            ),
-            data=data,
-            headers={"Content-Type": "application/zip"},
-        )
-        pprint(response.status_code)
-
-    def delete_mosaic_granule(self, coverage_store: str, coverage_name: str, granule_id: str):
-        """deletes granule based on it's id
-
-        Args:
-            coverage_store (str): name of coverage store that contains granule
-            coverage_name (str): name of the coverage layer
-            granule_id (str): granule identifier. Accessible through the index of granules.
-        """
-        try:
-            response = self.session.delete(
-                url=os.path.join(
-                    self.__coverage_store_url(),
-                    f"{coverage_store}/coverages/{coverage_name}/index/granules/{granule_id}",
-                )
-            )
-            pprint(response.status_code)
-        except Exception as e:
-            print(f"Error deleting granule: {e}")
-        pass
-
-    def list_coverages(self, coverage_store: str):
-        """Lists all coverages currently hosted in specified coverage store"""
-        response = self.session.get(
-            url=os.path.join(
-                self.__coverage_store_url(), f"{coverage_store}/coverages.xml?list=all"
-            )
-        )
-        pprint(response.text)
-
-    def list_mosaic_granules(
-        self, coverage_store: str, coverage: str, filter: str = ""
-    ):
-        """Lists all granules belonging to a specified coverage"""
-        query_url = f"{coverage_store}/coverages/{coverage}/index/granules.json"
-        if filter != "":
-            filter = urllib.parse.quote(filter)
-            query_url += f"?filter={filter}"
-        response = self.session.get(
-            url=os.path.join(
-                self.__coverage_store_url(),
-                query_url,
-            )
-        )
-        if response.status_code == 200:
-            return response.json()
-        else:
-            raise Exception(f"Failed listing mosaic granules: {response}")
-
-    def setup_mosaic_config(self, coverage_store: str, xml_path: str):
-        """Sends an xml with the mosaic configuration to the geoserver
-
-        Args:
-            coverage_store (str): name of the coveragestore to configure
-            xml_path (str): path to xml
-        """
-        # open xml file and send it to geoserver
-        with open(xml_path) as xml:
-            response = self.session.post(
-                url=os.path.join(
-                    self.__coverage_store_url(),
-                    f"{coverage_store}/coverages",
-                ),
-                data=xml,
-                headers={"Content-Type": "text/xml"},
-            )
-            pprint(response.status_code)
+import os
+import urllib
+from pprint import pprint
+from rov_db_access.config.settings import Settings
+
+import requests
+settings = Settings()
+
+
+class GeoServerClient:
+    workspace = None
+
+    def __init__(self):
+        self.server_url = settings.geoserver_api_url
+        self.session = requests.Session()
+        self.session.auth = (settings.geoserver_api_user, settings.geoserver_api_password)
+        self.url = settings.geoserver_api_url + "/geoserver/rest"
+
+    def __coverage_store_url(self) -> str:
+        return os.path.join(self.url, f"workspaces/{self.workspace}/coveragestores")
+
+    def reload_config(self):
+        """
+        Reloads the GeoServer catalog and configuration from disk.
+        This operation is used in cases where an external tool has modified the on-disk configuration.
+        This operation will also force GeoServer to drop any internal caches and reconnect to all data stores.
+        """
+        try:
+            self.session.post(url=f"{self.url}/reload")
+            print("Geoserver config reloaded")
+        except Exception as e:
+            print(f"Error reloading config: {e}")
+
+    def set_workspace(self, workspace: str):
+        self.workspace = workspace
+
+    def add_mosaic_granule(self, coverage_store: str, granule_path: str):
+        """Adds a new granule to an existing imagemosaic
+
+        Args:
+            coverage_store (str): name of the coverage store
+            granule_path (str): url to granule
+        """
+        try:
+            response = self.session.post(
+                url=os.path.join(
+                    self.__coverage_store_url(), f"{coverage_store}/remote.imagemosaic"
+                ),
+                data=granule_path,
+                headers={"Content-Type": "text/plain"},
+            )
+            response.raise_for_status()
+            print(f'Geoserver new granule added for coverage: {coverage_store}')
+            return response
+        except Exception as e:
+            print(f"Error adding granule into coverage: {coverage_store}. ERROR: {e}")
+            return None
+
+    def create_empty_mosaic(self, coverage_store: str, zip_path: str):
+        """Creates an empty mosaic in geoserver
+
+        Args:
+            coverage_store (str): name of the coverage store
+            zip_path (str): path to a .zip file containing .properties configuration files
+            for mosaic
+        """
+        with open(zip_path, "rb") as zip:
+            data = zip.read()
+        response = self.session.put(
+            url=os.path.join(
+                self.__coverage_store_url(),
+                f"{coverage_store}/file.imagemosaic?configure=none",
+            ),
+            data=data,
+            headers={"Content-Type": "application/zip"},
+        )
+        pprint(response.status_code)
+
+    def delete_mosaic_granule(self, coverage_store: str, coverage_name: str, granule_id: str):
+        """deletes granule based on it's id
+
+        Args:
+            coverage_store (str): name of coverage store that contains granule
+            coverage_name (str): name of the coverage layer
+            granule_id (str): granule identifier. Accessible through the index of granules.
+        """
+        try:
+            response = self.session.delete(
+                url=os.path.join(
+                    self.__coverage_store_url(),
+                    f"{coverage_store}/coverages/{coverage_name}/index/granules/{granule_id}",
+                )
+            )
+            pprint(response.status_code)
+        except Exception as e:
+            print(f"Error deleting granule: {e}")
+        pass
+
+    def list_coverages(self, coverage_store: str):
+        """Lists all coverages currently hosted in specified coverage store"""
+        response = self.session.get(
+            url=os.path.join(
+                self.__coverage_store_url(), f"{coverage_store}/coverages.xml?list=all"
+            )
+        )
+        pprint(response.text)
+
+    def list_mosaic_granules(
+        self, coverage_store: str, coverage: str, filter: str = ""
+    ):
+        """Lists all granules belonging to a specified coverage"""
+        query_url = f"{coverage_store}/coverages/{coverage}/index/granules.json"
+        if filter != "":
+            filter = urllib.parse.quote(filter)
+            query_url += f"?filter={filter}"
+        response = self.session.get(
+            url=os.path.join(
+                self.__coverage_store_url(),
+                query_url,
+            )
+        )
+        if response.status_code == 200:
+            return response.json()
+        else:
+            raise Exception(f"Failed listing mosaic granules: {response}")
+
+    def setup_mosaic_config(self, coverage_store: str, xml_path: str):
+        """Sends an xml with the mosaic configuration to the geoserver
+
+        Args:
+            coverage_store (str): name of the coveragestore to configure
+            xml_path (str): path to xml
+        """
+        # open xml file and send it to geoserver
+        with open(xml_path) as xml:
+            response = self.session.post(
+                url=os.path.join(
+                    self.__coverage_store_url(),
+                    f"{coverage_store}/coverages",
+                ),
+                data=xml,
+                headers={"Content-Type": "text/xml"},
+            )
+            pprint(response.status_code)
```

### Comparing `rov_db_access-1.0.8/rov_db_access/utils/utils.py` & `rov_db_access-1.0.9/rov_db_access/utils/utils.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from typing import Optional
-
-from geoalchemy2 import WKBElement
-from geoalchemy2.shape import to_shape, from_shape
-from shapely import wkt, get_srid
-
-
-def wkt_to_wkbelement(wkt_str: str) -> WKBElement:
-    shapely_geometry = wkt.loads(wkt_str)
-    if shapely_geometry.geom_type == "MultiPolygon":
-        shapely_geometry = list(shapely_geometry.geoms)[0]
-    return from_shape(shapely_geometry, srid=4326)
-
-
-def ewkt_to_wkbelement(ewkt: str) -> WKBElement:
-    wkt_str = ewkt[ewkt.find(";") + 1: -1]
-    shapely_geometry = wkt.loads(wkt_str)
-    if shapely_geometry.geom_type == "MultiPolygon":
-        shapely_geometry = list(shapely_geometry.geoms)[0]
-    return from_shape(shapely_geometry, srid=4326)
-
-
-def wkbelement_to_ewkt(ewkt: WKBElement) -> str:
-    geometry = to_shape(ewkt)
-    srid = get_srid(geometry)
-    if srid == 0:
-        srid = 4326
-    srid_str = '='.join(['SRID', srid])
-    wkt_str = geometry.wkt
-    ewkt = ';'.join([srid_str, wkt_str])
-    return ewkt
-
-
-def wkbelement_to_wkt(ewkt: Optional[WKBElement]) -> Optional[str]:
-    if ewkt is None:
-        return None
-    return to_shape(ewkt).wkt
+from typing import Optional
+
+from geoalchemy2 import WKBElement
+from geoalchemy2.shape import to_shape, from_shape
+from shapely import wkt, get_srid
+
+
+def wkt_to_wkbelement(wkt_str: str) -> WKBElement:
+    shapely_geometry = wkt.loads(wkt_str)
+    if shapely_geometry.geom_type == "MultiPolygon":
+        shapely_geometry = list(shapely_geometry.geoms)[0]
+    return from_shape(shapely_geometry, srid=4326)
+
+
+def ewkt_to_wkbelement(ewkt: str) -> WKBElement:
+    wkt_str = ewkt[ewkt.find(";") + 1: -1]
+    shapely_geometry = wkt.loads(wkt_str)
+    if shapely_geometry.geom_type == "MultiPolygon":
+        shapely_geometry = list(shapely_geometry.geoms)[0]
+    return from_shape(shapely_geometry, srid=4326)
+
+
+def wkbelement_to_ewkt(ewkt: WKBElement) -> str:
+    geometry = to_shape(ewkt)
+    srid = get_srid(geometry)
+    if srid == 0:
+        srid = 4326
+    srid_str = '='.join(['SRID', srid])
+    wkt_str = geometry.wkt
+    ewkt = ';'.join([srid_str, wkt_str])
+    return ewkt
+
+
+def wkbelement_to_wkt(ewkt: Optional[WKBElement]) -> Optional[str]:
+    if ewkt is None:
+        return None
+    return to_shape(ewkt).wkt
```

### Comparing `rov_db_access-1.0.8/PKG-INFO` & `rov_db_access-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rov-db-access
-Version: 1.0.8
+Version: 1.0.9
 Summary: 
 Author: Pablo Cano
 Author-email: pablo.cano@rovisen.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

