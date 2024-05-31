# Comparing `tmp/entegywrapper-7.3.0.tar.gz` & `tmp/entegywrapper-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entegywrapper-7.3.0.tar", max compression
+gzip compressed data, was "entegywrapper-8.0.0.tar", max compression
```

## Comparing `entegywrapper-7.3.0.tar` & `entegywrapper-8.0.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2739 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/README.md
--rw-r--r--   0        0        0     8479 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/__init__.py
--rw-r--r--   0        0        0        0 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/attendance_tracking/__init__.py
--rw-r--r--   0        0        0     5790 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/attendance_tracking/attendance_tracking.py
--rw-r--r--   0        0        0        0 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/content/__init__.py
--rw-r--r--   0        0        0    12282 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/content/categories.py
--rw-r--r--   0        0        0    11413 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/content/content.py
--rw-r--r--   0        0        0     3276 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/content/documents.py
--rw-r--r--   0        0        0     6983 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/content/multi_link.py
--rw-r--r--   0        0        0      716 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/errors.py
--rw-r--r--   0        0        0        0 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/notification/__init__.py
--rw-r--r--   0        0        0     5749 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/notification/notification.py
--rw-r--r--   0        0        0        0 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/plugins/__init__.py
--rw-r--r--   0        0        0     1323 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/plugins/ext_auth.py
--rw-r--r--   0        0        0        0 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/points/__init__.py
--rw-r--r--   0        0        0     4729 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/points/point_management.py
--rw-r--r--   0        0        0        0 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/profiles/__init__.py
--rw-r--r--   0        0        0     4312 2024-05-29 03:17:06.255041 entegywrapper-7.3.0/entegywrapper/profiles/profile_custom.py
--rw-r--r--   0        0        0    11869 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/entegywrapper/profiles/profile_links.py
--rw-r--r--   0        0        0     2354 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/entegywrapper/profiles/profile_payments.py
--rw-r--r--   0        0        0     6139 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/entegywrapper/profiles/profile_types.py
--rw-r--r--   0        0        0    16614 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/entegywrapper/profiles/profiles.py
--rw-r--r--   0        0        0        1 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/entegywrapper/py.typed
--rw-r--r--   0        0        0        0 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/entegywrapper/schemas/__init__.py
--rw-r--r--   0        0        0      236 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/entegywrapper/schemas/attendance_tracking.py
--rw-r--r--   0        0        0     6771 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/entegywrapper/schemas/content.py
--rw-r--r--   0        0        0      286 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/entegywrapper/schemas/lead_capture.py
--rw-r--r--   0        0        0      334 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/entegywrapper/schemas/page_settings.py
--rw-r--r--   0        0        0     1260 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/entegywrapper/schemas/points.py
--rw-r--r--   0        0        0     4975 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/entegywrapper/schemas/profile.py
--rw-r--r--   0        0        0     2068 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/entegywrapper/schemas/project.py
--rw-r--r--   0        0        0      329 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/entegywrapper/schemas/schedule.py
--rw-r--r--   0        0        0      935 2024-05-29 03:17:06.259040 entegywrapper-7.3.0/pyproject.toml
--rw-r--r--   0        0        0     3445 1970-01-01 00:00:00.000000 entegywrapper-7.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2739 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/README.md
+-rw-r--r--   0        0        0     8479 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/entegywrapper/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/entegywrapper/attendance_tracking/__init__.py
+-rw-r--r--   0        0        0     5790 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/entegywrapper/attendance_tracking/attendance_tracking.py
+-rw-r--r--   0        0        0        0 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/entegywrapper/content/__init__.py
+-rw-r--r--   0        0        0    12282 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/entegywrapper/content/categories.py
+-rw-r--r--   0        0        0    11413 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/entegywrapper/content/content.py
+-rw-r--r--   0        0        0     3276 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/entegywrapper/content/documents.py
+-rw-r--r--   0        0        0     6983 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/entegywrapper/content/multi_link.py
+-rw-r--r--   0        0        0      716 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/entegywrapper/errors.py
+-rw-r--r--   0        0        0        0 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/entegywrapper/notification/__init__.py
+-rw-r--r--   0        0        0     5749 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/entegywrapper/notification/notification.py
+-rw-r--r--   0        0        0        0 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/entegywrapper/plugins/__init__.py
+-rw-r--r--   0        0        0     1323 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/entegywrapper/plugins/ext_auth.py
+-rw-r--r--   0        0        0        0 2024-05-31 05:19:29.338832 entegywrapper-8.0.0/entegywrapper/points/__init__.py
+-rw-r--r--   0        0        0     4729 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/points/point_management.py
+-rw-r--r--   0        0        0        0 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/profiles/__init__.py
+-rw-r--r--   0        0        0     4312 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/profiles/profile_custom.py
+-rw-r--r--   0        0        0    11869 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/profiles/profile_links.py
+-rw-r--r--   0        0        0     2354 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/profiles/profile_payments.py
+-rw-r--r--   0        0        0     6139 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/profiles/profile_types.py
+-rw-r--r--   0        0        0    16598 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/profiles/profiles.py
+-rw-r--r--   0        0        0        1 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/py.typed
+-rw-r--r--   0        0        0        0 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/schemas/__init__.py
+-rw-r--r--   0        0        0      236 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/schemas/attendance_tracking.py
+-rw-r--r--   0        0        0     6776 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/schemas/content.py
+-rw-r--r--   0        0        0      286 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/schemas/lead_capture.py
+-rw-r--r--   0        0        0      339 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/schemas/page_settings.py
+-rw-r--r--   0        0        0     1265 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/schemas/points.py
+-rw-r--r--   0        0        0     4974 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/schemas/profile.py
+-rw-r--r--   0        0        0     2093 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/schemas/project.py
+-rw-r--r--   0        0        0      329 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/entegywrapper/schemas/schedule.py
+-rw-r--r--   0        0        0      935 2024-05-31 05:19:29.342832 entegywrapper-8.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3445 1970-01-01 00:00:00.000000 entegywrapper-8.0.0/PKG-INFO
```

### Comparing `entegywrapper-7.3.0/README.md` & `entegywrapper-8.0.0/README.md`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/__init__.py` & `entegywrapper-8.0.0/entegywrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/attendance_tracking/attendance_tracking.py` & `entegywrapper-8.0.0/entegywrapper/attendance_tracking/attendance_tracking.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/content/categories.py` & `entegywrapper-8.0.0/entegywrapper/content/categories.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/content/content.py` & `entegywrapper-8.0.0/entegywrapper/content/content.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/content/documents.py` & `entegywrapper-8.0.0/entegywrapper/content/documents.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/content/multi_link.py` & `entegywrapper-8.0.0/entegywrapper/content/multi_link.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/errors.py` & `entegywrapper-8.0.0/entegywrapper/errors.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/notification/notification.py` & `entegywrapper-8.0.0/entegywrapper/notification/notification.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/plugins/ext_auth.py` & `entegywrapper-8.0.0/entegywrapper/plugins/ext_auth.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/points/point_management.py` & `entegywrapper-8.0.0/entegywrapper/points/point_management.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/profiles/profile_custom.py` & `entegywrapper-8.0.0/entegywrapper/profiles/profile_custom.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/profiles/profile_links.py` & `entegywrapper-8.0.0/entegywrapper/profiles/profile_links.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/profiles/profile_payments.py` & `entegywrapper-8.0.0/entegywrapper/profiles/profile_payments.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/profiles/profile_types.py` & `entegywrapper-8.0.0/entegywrapper/profiles/profile_types.py`

 * *Files identical despite different names*

### Comparing `entegywrapper-7.3.0/entegywrapper/profiles/profiles.py` & `entegywrapper-8.0.0/entegywrapper/profiles/profiles.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,30 +24,30 @@
 
 def all_profiles(
     self: EntegyAPI,
     *,
     include_custom_fields: bool = False,
     include_permissions: bool = False,
     status: Optional[str] = None,
-    profile_type: Optional[ProfileType] = None,
+    profile_type: Optional[str] = None,
     updated_after: Optional[str] = None,
     created_after: Optional[str] = None,
 ) -> Generator[Profile, None, None]:
     """
     Yields all user profiles.
 
     Parameters
     ----------
         `include_custom_fields` (`bool`, optional): whether to include custom fields for each profile; defaults to `False`
 
         `include_permissions` (`bool`, optional): whether to include permissions for each profile; defaults to `False`
 
         `status` (`str`, optional): only select profiles with this status; defaults to `None`
 
-        `profile_type` (`ProfileType`, optional): only select profiles of this type; defaults to `None`
+        `profile_type` (`str`, optional): only select profiles of this type; defaults to `None`
 
         `updated_after` (`str`, optional): only select profiles updated after this time; defaults to `None`
 
         `created_after` (`str`, optional): only select profiles created after this time; defaults to `None`
 
     Yields
     ------
```

### Comparing `entegywrapper-7.3.0/entegywrapper/schemas/content.py` & `entegywrapper-8.0.0/entegywrapper/schemas/content.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Optional
 
 from pydantic import BaseModel
 
 from .page_settings import PageSetting
 
 
-class TemplateType(Enum):
+class TemplateType(str, Enum):
     @classmethod
     def _missing_(cls, value):
         """Enables case-insensitive lookup."""
         if value is None:
             raise ValueError("None is not a valid value for this Enum.")
 
         if not isinstance(value, str):
```

### Comparing `entegywrapper-7.3.0/entegywrapper/schemas/points.py` & `entegywrapper-8.0.0/entegywrapper/schemas/points.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from enum import Enum
 
 from pydantic import BaseModel
 
 from .profile import Profile
 
 
-class PointType(Enum):
+class PointType(str, Enum):
     COMMENT = "Comment"
     COMMENT_WITH_IMAGE = "CommentWithImage"
     STATUS = "Status"
     STATUS_WITH_IMAGE = "StatusWithImage"
     VIEW_COMMENT = "ViewComment"
     PROFILE_LOGIN = "ProfileLogin"
     PROFILE_UPDATED = "ProfileUpdated"
```

### Comparing `entegywrapper-7.3.0/entegywrapper/schemas/profile.py` & `entegywrapper-8.0.0/entegywrapper/schemas/profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 from typing import Any, Optional
 
 from pydantic import BaseModel, field_validator
 
 from .project import ProjectEventInfo, ProjectStatus, ProjectType, SoftwareElement
 
 
-class ProfileExtendedPrivacy(Enum):
-    PUBLIC = "Public"
-    CONNECTIONS = "Connections"
-    HIDDEN = "Hidden"
+class ProfileExtendedPrivacy(int, Enum):
+    PUBLIC = 0
+    CONNECTIONS = 1
+    HIDDEN = 2
 
 
 class Permissions(BaseModel):
     loggedInApp: Optional[bool] = None
     loggedInCapture: Optional[bool] = None
     showInList: Optional[bool] = None
     allowMessaging: Optional[bool] = None
@@ -63,15 +63,15 @@
     externalReference: str
     isOrganiser: Optional[bool] = None
     allowAppLogin: Optional[bool] = None
     price: Optional[int] = None
     moduleId: Optional[int] = None
 
 
-class CustomProfileFieldType(Enum):
+class CustomProfileFieldType(str, Enum):
     MULTI_CHOICE = "MultiChoice"
     SHORT_TEXT = "ShortText"
     MEDIUM_TEXT = "MediumText"
     LONG_TEXT = "LongText"
     FACEBOOK = "Facebook"
     TWITTER = "Twitter"
     INSTAGRAM = "Instagram"
@@ -128,29 +128,29 @@
     contactNumber: Optional[str] = None
     imageUrl: Optional[str] = None
     enabled: Optional[bool] = None
     permissions: Optional[Permissions] = None
     customFields: Optional[dict[str, Any]] = None
 
 
-class ProfileIdentifier(Enum):
+class ProfileIdentifier(str, Enum):
     PROFILE_ID = "profileId"
     EXTERNAL_REFERENCE = "externalReference"
     INTERNAL_REFERENCE = "internalReference"
     BADGE_REFERENCE = "badgeReference"
 
 
-class PaymentStatus(Enum):
+class PaymentStatus(str, Enum):
     PENDING = "Pending"
     CANCELLED = "Cancelled"
     PAID = "Paid"
     REFUNDED = "Refunded"
 
 
-class PaymentMethod(Enum):
+class PaymentMethod(str, Enum):
     NONE = "None"
     CREDIT_CARD = "CreditCard"
     DIRECT_DEPOSIT = "DirectDeposit"
     CASH = "Cash"
     CHEQUE = "Cheque"
     OTHER = "Other"
```

### Comparing `entegywrapper-7.3.0/entegywrapper/schemas/project.py` & `entegywrapper-8.0.0/entegywrapper/schemas/project.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 from enum import Enum
 from typing import Optional
 
 from pydantic import BaseModel
 
 
-class ApiKeyPermission(Enum):
+class ApiKeyPermission(str, Enum):
     VIEW_CONTENT = "ViewContent"
     EDIT_CONTENT = "EditContent"
     EDIT_PROFILES = "EditProfiles"
     VIEW_PROFILES = "ViewProfiles"
     ACHIEVEMENTS = "Achievements"
     SEND_NOTIFICATIONS = "SendNotifications"
 
 
-class Region(Enum):
+class Region(str, Enum):
     AU = "61a948f2-d505-4b0b-81de-31af6925647e"
     US = "2b9bd3fc-405e-4df5-888d-f5323e2b5093"
     EU = "86f89b50-1bbb-4019-9ca2-b2d9f4167064"
 
 
 class ProjectEventInfo(BaseModel):
     startDate: str
     endDate: str
 
 
-class ProjectType(Enum):
+class ProjectType(str, Enum):
     EVENT = "Event"
     ONGOING = "Ongoing"
     DEMO = "Demo"
     PORTAL = "Portal"
     DEMO_TEMPLATE = "DemoTemplate"
 
 
-class ProjectStatus(Enum):
+class ProjectStatus(str, Enum):
     DRAFT = "Draft"
     HAND_OVER = "HandOver"
     POPULATE_AND_TESTING = "PopulateAndTesting"
     PRODUCTION = "Production"
     FINISHED = "Finished"
     EXPIRED = "Expired"
     CANCELED = "Canceled"
 
 
-class SoftwareElement(Enum):
+class SoftwareElement(str, Enum):
     APP = "App"
     STORE_LISTING = "StoreListing"
     ENGAGE = "Engage"
     CAPTURE = "Capture"
     TRACK = "Track"
     INTERACT = "Interact"
     REGISTRATION = "Registration"
```

### Comparing `entegywrapper-7.3.0/pyproject.toml` & `entegywrapper-8.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["poetry-core>=1.0.0a5"]
 build-backend = "poetry.core.masonry.api"
 
 [project]
 name = "entegywrapper"
-version = "7.3.0"
+version = "8.0.0"
 requires-python = ">=3.10"
 
 [tool.black]
 line-length = 100
 
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.poetry]
 name = "entegywrapper"
-version = "7.3.0"
+version = "8.0.0"
 description = "Python SDK for the Entegy API"
 authors = [
     "Situ Development <developer@situ.com.au>",
     "William Sawyer <william@situ.com.au>",
     "Nathan Thomas <nathan@situ.com.au>",
 ]
 readme = "README.md"
```

### Comparing `entegywrapper-7.3.0/PKG-INFO` & `entegywrapper-8.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: entegywrapper
-Version: 7.3.0
+Version: 8.0.0
 Summary: Python SDK for the Entegy API
 Home-page: https://github.com/SituDevelopment/entegy-sdk-python
 Author: Situ Development
 Author-email: developer@situ.com.au
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

