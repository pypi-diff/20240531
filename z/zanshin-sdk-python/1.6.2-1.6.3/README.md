# Comparing `tmp/zanshin_sdk_python-1.6.2.tar.gz` & `tmp/zanshin_sdk_python-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zanshin_sdk_python-1.6.2.tar", max compression
+gzip compressed data, was "zanshin_sdk_python-1.6.3.tar", max compression
```

## Comparing `zanshin_sdk_python-1.6.2.tar` & `zanshin_sdk_python-1.6.3.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0    11357 2024-04-23 17:54:32.457851 zanshin_sdk_python-1.6.2/LICENSE
--rw-r--r--   0        0        0     5372 2024-04-23 17:54:32.457851 zanshin_sdk_python-1.6.2/README.md
--rw-r--r--   0        0        0     1523 2024-04-23 17:54:32.709851 zanshin_sdk_python-1.6.2/pyproject.toml
--rw-r--r--   0        0        0      745 2024-04-23 17:54:32.473851 zanshin_sdk_python-1.6.2/zanshinsdk/__init__.py
--rw-r--r--   0        0        0     1887 2024-04-23 17:54:32.473851 zanshin_sdk_python-1.6.2/zanshinsdk/alerts_history.py
--rw-r--r--   0        0        0   103609 2024-04-23 17:54:32.473851 zanshin_sdk_python-1.6.2/zanshinsdk/client.py
--rw-r--r--   0        0        0     4397 2024-04-23 17:54:32.473851 zanshin_sdk_python-1.6.2/zanshinsdk/docs/README.md
--rw-r--r--   0        0        0       60 2024-04-23 17:54:32.473851 zanshin_sdk_python-1.6.2/zanshinsdk/dummy_aws_credentials
--rw-r--r--   0        0        0     2038 2024-04-23 17:54:32.473851 zanshin_sdk_python-1.6.2/zanshinsdk/dummy_cloudformation_zanshin_service_role_template.json
--rw-r--r--   0        0        0     1782 2024-04-23 17:54:32.473851 zanshin_sdk_python-1.6.2/zanshinsdk/following_alerts_history.py
--rw-r--r--   0        0        0     5751 2024-04-23 17:54:32.473851 zanshin_sdk_python-1.6.2/zanshinsdk/iterator.py
--rw-r--r--   0        0        0     2471 2024-04-23 17:54:32.473851 zanshin_sdk_python-1.6.2/zanshinsdk/test_alerts_history.py
--rw-r--r--   0        0        0   113840 2024-04-23 17:54:32.477851 zanshin_sdk_python-1.6.2/zanshinsdk/test_client.py
--rw-r--r--   0        0        0     2542 2024-04-23 17:54:32.477851 zanshin_sdk_python-1.6.2/zanshinsdk/test_following_alerts_history.py
--rw-r--r--   0        0        0    10022 2024-04-23 17:54:32.477851 zanshin_sdk_python-1.6.2/zanshinsdk/test_iterator.py
--rw-r--r--   0        0        0       22 2024-04-23 17:54:32.705851 zanshin_sdk_python-1.6.2/zanshinsdk/version.py
--rw-r--r--   0        0        0     6681 1970-01-01 00:00:00.000000 zanshin_sdk_python-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-31 18:42:59.378902 zanshin_sdk_python-1.6.3/LICENSE
+-rw-r--r--   0        0        0     5372 2024-05-31 18:42:59.378902 zanshin_sdk_python-1.6.3/README.md
+-rw-r--r--   0        0        0     1523 2024-05-31 18:42:59.610903 zanshin_sdk_python-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0      745 2024-05-31 18:42:59.390902 zanshin_sdk_python-1.6.3/zanshinsdk/__init__.py
+-rw-r--r--   0        0        0     1887 2024-05-31 18:42:59.390902 zanshin_sdk_python-1.6.3/zanshinsdk/alerts_history.py
+-rw-r--r--   0        0        0   102874 2024-05-31 18:42:59.390902 zanshin_sdk_python-1.6.3/zanshinsdk/client.py
+-rw-r--r--   0        0        0        0 2024-05-31 18:42:59.390902 zanshin_sdk_python-1.6.3/zanshinsdk/common/__init__.py
+-rw-r--r--   0        0        0     1903 2024-05-31 18:42:59.390902 zanshin_sdk_python-1.6.3/zanshinsdk/common/enums.py
+-rw-r--r--   0        0        0     2530 2024-05-31 18:42:59.390902 zanshin_sdk_python-1.6.3/zanshinsdk/common/targets.py
+-rw-r--r--   0        0        0     1165 2024-05-31 18:42:59.390902 zanshin_sdk_python-1.6.3/zanshinsdk/common/validators.py
+-rw-r--r--   0        0        0     4397 2024-05-31 18:42:59.390902 zanshin_sdk_python-1.6.3/zanshinsdk/docs/README.md
+-rw-r--r--   0        0        0     1782 2024-05-31 18:42:59.390902 zanshin_sdk_python-1.6.3/zanshinsdk/following_alerts_history.py
+-rw-r--r--   0        0        0     5751 2024-05-31 18:42:59.390902 zanshin_sdk_python-1.6.3/zanshinsdk/iterator.py
+-rw-r--r--   0        0        0        0 2024-05-31 18:42:59.390902 zanshin_sdk_python-1.6.3/zanshinsdk/tests/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-31 18:42:59.394902 zanshin_sdk_python-1.6.3/zanshinsdk/tests/data/dummy_aws_credentials
+-rw-r--r--   0        0        0     2038 2024-05-31 18:42:59.394902 zanshin_sdk_python-1.6.3/zanshinsdk/tests/data/dummy_cloudformation_zanshin_service_role_template.json
+-rw-r--r--   0        0        0     2471 2024-05-31 18:42:59.394902 zanshin_sdk_python-1.6.3/zanshinsdk/tests/test_alerts_history.py
+-rw-r--r--   0        0        0   115562 2024-05-31 18:42:59.394902 zanshin_sdk_python-1.6.3/zanshinsdk/tests/test_client.py
+-rw-r--r--   0        0        0     2542 2024-05-31 18:42:59.394902 zanshin_sdk_python-1.6.3/zanshinsdk/tests/test_following_alerts_history.py
+-rw-r--r--   0        0        0    10022 2024-05-31 18:42:59.394902 zanshin_sdk_python-1.6.3/zanshinsdk/tests/test_iterator.py
+-rw-r--r--   0        0        0       22 2024-05-31 18:42:59.606903 zanshin_sdk_python-1.6.3/zanshinsdk/version.py
+-rw-r--r--   0        0        0     6681 1970-01-01 00:00:00.000000 zanshin_sdk_python-1.6.3/PKG-INFO
```

### Comparing `zanshin_sdk_python-1.6.2/LICENSE` & `zanshin_sdk_python-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6.2/README.md` & `zanshin_sdk_python-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6.2/pyproject.toml` & `zanshin_sdk_python-1.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zanshin-sdk-python"
-version = "1.6.2"
+version = "1.6.3"
 description = "Python SDK to access the Tenchi Security Zanshin API v1"
 license = "Apache Software License"
 authors = ["Tenchi Security <contact@tenchisecurity.com>"]
 readme = "README.md"
 packages = [{include = "zanshinsdk"}]
 homepage = "https://github.com/tenchi-security/zanshin-sdk-python"
 classifiers=[
```

### Comparing `zanshin_sdk_python-1.6.2/zanshinsdk/__init__.py` & `zanshin_sdk_python-1.6.3/zanshinsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6.2/zanshinsdk/alerts_history.py` & `zanshin_sdk_python-1.6.3/zanshinsdk/alerts_history.py`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6.2/zanshinsdk/client.py` & `zanshin_sdk_python-1.6.3/zanshinsdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,86 +14,53 @@
 from typing import Dict, Iterable, Iterator, Optional, Union
 from urllib.parse import urlparse
 from uuid import UUID
 
 import httpx
 from pydantic import BaseModel, Field
 
+from zanshinsdk.common.enums import (
+    AlertSeverity,
+    AlertsOrderOpts,
+    AlertState,
+    Day,
+    Frequency,
+    Languages,
+    OAuthTargetKind,
+    Roles,
+    ScanTargetGroupKind,
+    ScanTargetKind,
+    SortOpts,
+    TimeOfDay,
+)
+from zanshinsdk.common.targets import (
+    ScanTargetAWS,
+    ScanTargetAZURE,
+    ScanTargetBITBUCKET,
+    ScanTargetDOMAIN,
+    ScanTargetGCP,
+    ScanTargetGITHUB,
+    ScanTargetGITLAB,
+    ScanTargetGroupCredentialListORACLE,
+    ScanTargetGWORKSPACE,
+    ScanTargetHUAWEI,
+    ScanTargetJIRA,
+    ScanTargetMS365,
+    ScanTargetORACLE,
+    ScanTargetSALESFORCE,
+    ScanTargetSLACK,
+    ScanTargetZENDESK,
+)
+from zanshinsdk.common.validators import validate_class, validate_int, validate_uuid
 from zanshinsdk.version import __version__ as sdk_version
 
 CONFIG_DIR = Path.home() / ".tenchi"
 CONFIG_FILE = CONFIG_DIR / "config"
 
 
-class AlertState(str, Enum):
-    OPEN = "OPEN"
-    ACTIVE = "ACTIVE"
-    IN_PROGRESS = "IN_PROGRESS"
-    RISK_ACCEPTED = "RISK_ACCEPTED"
-    MITIGATING_CONTROL = "MITIGATING_CONTROL"
-    FALSE_POSITIVE = "FALSE_POSITIVE"
-    CLOSED = "CLOSED"
-
-
-class AlertSeverity(str, Enum):
-    CRITICAL = "CRITICAL"
-    HIGH = "HIGH"
-    MEDIUM = "MEDIUM"
-    LOW = "LOW"
-    INFO = "INFO"
-
-
-class ScanTargetKind(str, Enum):
-    AWS = "AWS"
-    GCP = "GCP"
-    AZURE = "AZURE"
-    HUAWEI = "HUAWEI"
-    DOMAIN = "DOMAIN"
-    ORACLE = "ORACLE"
-
-
-class AlertsOrderOpts(str, Enum):
-    SCAN_TARGET_ID = "scanTargetId"
-    RESOURCE = "resource"
-    RULE = "rule"
-    SEVERITY = "severity"
-    STATE = "state"
-    CREATED_AT = "createdAt"
-    UPDATED_AT = "updatedAt"
-
-
-class SortOpts(str, Enum):
-    ASC = "asc"
-    DESC = "desc"
-
-
-class Frequency(Enum):
-    SIX_HOURS = "6h"
-    TWELVE_HOURS = "12h"
-    DAILY = "1d"
-    WEEKLY = "7d"
-
-
-class TimeOfDay(Enum):
-    MORNING = "MORNING"
-    AFTERNOON = "AFTERNOON"
-    EVENING = "EVENING"
-    NIGHT = "NIGHT"
-
-
-class Day(Enum):
-    SUNDAY = "SUNDAY"
-    MONDAY = "MONDAY"
-    TUESDAY = "TUESDAY"
-    WEDNESDAY = "WEDNESDAY"
-    THURSDAY = "THURSDAY"
-    FRIDAY = "FRIDAY"
-    SATURDAY = "SATURDAY"
-
-
 class ScanTargetSchedule(BaseModel):
     frequency: Frequency
     time_of_day: Optional[TimeOfDay] = Field(TimeOfDay.NIGHT, alias="timeOfDay")
     day: Optional[Day] = Day.SUNDAY
 
     def value(self):
         if self.frequency in (Frequency.SIX_HOURS, Frequency.TWELVE_HOURS):
@@ -115,77 +82,14 @@
 
 DAILY = ScanTargetSchedule(frequency=Frequency.DAILY, time_of_day=TimeOfDay.NIGHT)
 WEEKLY = ScanTargetSchedule(
     frequency=Frequency.WEEKLY, time_of_day=TimeOfDay.NIGHT, day=Day.SUNDAY
 )
 
 
-class ScanTargetAWS(dict):
-    def __init__(self, account):
-        dict.__init__(self, account=account)
-
-
-class ScanTargetAZURE(dict):
-    def __init__(self, application_id, subscription_id, directory_id, secret):
-        dict.__init__(
-            self,
-            applicationId=application_id,
-            subscriptionId=subscription_id,
-            directoryId=directory_id,
-            secret=secret,
-        )
-
-
-class ScanTargetGCP(dict):
-    def __init__(self, project_id):
-        dict.__init__(self, projectId=project_id)
-
-
-class ScanTargetHUAWEI(dict):
-    def __init__(self, account_id):
-        dict.__init__(self, accountId=account_id)
-
-
-class ScanTargetDOMAIN(dict):
-    def __init__(self, domain):
-        dict.__init__(self, domain=domain)
-
-
-class ScanTargetORACLE(dict):
-    def __init__(self, compartment_id, region, tenancy_id, user_id, key_fingerprint):
-        dict.__init__(
-            self,
-            compartment_id=compartment_id,
-            region=region,
-            tenancy_id=tenancy_id,
-            user_id=user_id,
-            key_fingerprint=key_fingerprint,
-        )
-
-
-class ScanTargetGroupCredentialListORACLE(dict):
-    def __init__(self, region, tenancy_id, user_id, key_fingerprint):
-        dict.__init__(
-            self,
-            region=region,
-            tenancy_id=tenancy_id,
-            user_id=user_id,
-            key_fingerprint=key_fingerprint,
-        )
-
-
-class Roles(str, Enum):
-    ADMIN = "ADMIN"
-
-
-class Languages(str, Enum):
-    PT_BR = "pt-BR"
-    EN_US = "en-US"
-
-
 class Client:
     def __init__(
         self,
         profile: str = "default",
         api_key: Optional[str] = None,
         api_url: Optional[str] = None,
         user_agent: Optional[str] = None,
@@ -1012,53 +916,77 @@
         credential: Union[
             ScanTargetAWS,
             ScanTargetAZURE,
             ScanTargetGCP,
             ScanTargetHUAWEI,
             ScanTargetDOMAIN,
             ScanTargetORACLE,
+            ScanTargetZENDESK,
+            ScanTargetGWORKSPACE,
+            ScanTargetSLACK,
+            ScanTargetBITBUCKET,
+            ScanTargetJIRA,
+            ScanTargetGITLAB,
+            ScanTargetSALESFORCE,
+            ScanTargetMS365,
         ],
         schedule: ScanTargetSchedule = DAILY,
     ) -> Dict:
         """
         Create a new scan target in organization.
         <https://api.zanshin.tenchisecurity.com/#operation/createOrganizationScanTargets>
         :param organization_id: the ID of the organization
         :param kind: the Kind of scan target (AWS, GCP, AZURE)
         :param name: the name of the scan target
         :param credential: credentials to access the cloud account to be scanned:
             * For AWS scan targets, provide the account ID in the *account* field
             * For Azure scan targets, provide *applicationId*, *subscriptionId*, *directoryId* and *secret* fields.
             * For GCP scan targets, provide a *projectId* field
             * For DOMAIN scan targets, provide a URL in the *domain* field
+            * For ZENDESK scan target, provide *instance_url* field
+            * For Jira scan target, provide *jira_url* field
+            * For MS365 scan target, provide *tenant_id*, *application_id*, *secret* fields
+            * For GITHUB scan target, provide *installation_id*, *organizationName* fields
+            * For GWORKSPACE, SLACK, BITBUCKET, GITLAB, SALESFORCE no one credential are needed
         :param schedule: schedule as a string or enum version of the scan frequency
         :return: a dict representing the newly created scan target
         """
         validate_class(kind, ScanTargetKind)
         validate_class(name, str)
 
-        if kind == ScanTargetKind.AWS:
-            validate_class(credential, ScanTargetAWS)
-        elif kind == ScanTargetKind.AZURE:
-            validate_class(credential, ScanTargetAZURE)
-        elif kind == ScanTargetKind.GCP:
-            validate_class(credential, ScanTargetGCP)
-        elif kind == ScanTargetKind.HUAWEI:
-            validate_class(credential, ScanTargetHUAWEI)
-        elif kind == ScanTargetKind.DOMAIN:
-            validate_class(credential, ScanTargetDOMAIN)
-        elif kind == ScanTargetKind.ORACLE:
-            validate_class(credential, ScanTargetORACLE)
+        validator_credential_map = {
+            ScanTargetKind.AWS: ScanTargetAWS,
+            ScanTargetKind.AZURE: ScanTargetAZURE,
+            ScanTargetKind.GCP: ScanTargetGCP,
+            ScanTargetKind.HUAWEI: ScanTargetHUAWEI,
+            ScanTargetKind.DOMAIN: ScanTargetDOMAIN,
+            ScanTargetKind.ORACLE: ScanTargetORACLE,
+            ScanTargetKind.ZENDESK: ScanTargetZENDESK,
+            ScanTargetKind.GWORKSPACE: ScanTargetGWORKSPACE,
+            ScanTargetKind.SLACK: ScanTargetSLACK,
+            ScanTargetKind.BITBUCKET: ScanTargetBITBUCKET,
+            ScanTargetKind.JIRA: ScanTargetJIRA,
+            ScanTargetKind.GITLAB: ScanTargetGITLAB,
+            ScanTargetKind.SALESFORCE: ScanTargetSALESFORCE,
+            ScanTargetKind.MS365: ScanTargetMS365,
+            ScanTargetKind.GITHUB: ScanTargetGITHUB,
+        }
+
+        if not validator_credential_map.get(kind):
+            raise ValueError(f"Invalid kind: {kind}")
+
+        validate_class(credential, validator_credential_map.get(kind))
 
         body = {
             "name": name,
             "kind": kind,
             "credential": credential,
             "schedule": schedule.value(),
         }
+
         return self._request(
             "POST",
             f"/organizations/{validate_uuid(organization_id)}/scantargets",
             body=body,
         ).json()
 
     def get_organization_scan_target(
@@ -1174,14 +1102,54 @@
         """
         return self._request(
             "POST",
             f"/organizations/{validate_uuid(organization_id)}/scantargets/"
             f"{validate_uuid(scan_target_id)}/check",
         ).json()
 
+    ###################################################
+    # Scan Target OAuth
+    ###################################################
+
+    def get_kind_oauth_link(
+        self,
+        organization_id: Union[UUID, str],
+        scan_target_id: Union[UUID, str],
+        kind: Union[ScanTargetKind, OAuthTargetKind],
+    ) -> Dict:
+        """
+        Retrieve a link to authorize zanshin to read info from their target.
+
+        Mandatory for scan targets of kind:
+            * ZENDESK
+            * GWORKSPACE
+            * SLACK
+            * BITBUCKET
+            * JIRA
+            * GITLAB
+            * SALESFORCE
+        :return: a dict with the link
+        """
+        if kind.value not in [member.value for member in OAuthTargetKind]:
+            raise ValueError(f"{repr(kind.value)} is not eligible for OAuth link")
+
+        scan_type = (
+            "scanTargetGroupId"
+            if kind in [ScanTargetKind.BITBUCKET, ScanTargetKind.GITLAB]
+            else "scanTargetId"
+        )
+
+        path = (
+            f"/oauth/link"
+            f"?organizationId={validate_uuid(organization_id)}"
+            f"&{scan_type}={validate_uuid(scan_target_id)}"
+        )
+
+        return self._request("GET", path).json()
+
     def get_gworkspace_oauth_link(
         self, organization_id: Union[UUID, str], scan_target_id: Union[UUID, str]
     ) -> Dict:
         """
         Retrieve a link to allow the user to authorize zanshin to read info from their gworkspace environment.
         <https://api.zanshin.tenchisecurity.com/#operation/getGworkspaceOauthLink>
         :return: a dict with the link
@@ -1274,23 +1242,26 @@
         :param organization_id: the ID of the organization
         :param kind: The type of cloud of this scan target group
         :param name: the name of the scan target group
         :return: a dict representing the newly created scan target group
         """
         validate_class(kind, ScanTargetKind)
         validate_class(name, str)
-        if kind != ScanTargetKind.ORACLE:
+        group_kinds = [member.value for member in ScanTargetGroupKind]
+
+        if kind not in group_kinds:
             raise ValueError(
-                f"{repr(kind.value)} is not accepted. 'ORACLE' is expected"
+                f"{repr(kind.value)} is not accepted. '{group_kinds}' is expected"
             )
 
         body = {
             "name": name,
             "kind": kind,
         }
+
         return self._request(
             "POST",
             f"/organizations/{validate_uuid(organization_id)}/scantargetgroups",
             body=body,
         ).json()
 
     def update_scan_target_group(
@@ -2598,44 +2569,7 @@
                 f"{package_name} not present. {package_name} is required to perform AWS onboard."
             )
 
         module = module_from_spec(spec)
         sys.modules[package_name] = module
         spec.loader.exec_module(module)
         return module
-
-
-def validate_int(
-    value, min_value=None, max_value=None, required=False
-) -> Optional[int]:
-    if value is None:
-        if required:
-            raise ValueError("required integer parameter missing")
-        else:
-            return value
-    if not isinstance(value, int):
-        raise TypeError(f"{repr(value)} is not an integer")
-    if min_value and value < min_value:
-        raise ValueError(f"{value} shouldn't be lower than {min_value}")
-    if max_value and value > max_value:
-        raise ValueError(f"{value} shouldn't be higher than {max_value}")
-    return value
-
-
-def validate_class(value, class_type):
-    if not isinstance(value, class_type):
-        raise TypeError(f"{repr(value)} is not an instance of {class_type.__name__}")
-    return value
-
-
-def validate_uuid(uuid: Union[UUID, str]) -> str:
-    try:
-        if isinstance(uuid, str):
-            return str(UUID(uuid))
-
-        if isinstance(uuid, UUID):
-            return str(uuid)
-
-        raise TypeError
-    except (ValueError, TypeError) as ex:
-        ex.args = (f"{repr(uuid)} is not a valid UUID",)
-        raise ex
```

### Comparing `zanshin_sdk_python-1.6.2/zanshinsdk/docs/README.md` & `zanshin_sdk_python-1.6.3/zanshinsdk/docs/README.md`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6.2/zanshinsdk/dummy_cloudformation_zanshin_service_role_template.json` & `zanshin_sdk_python-1.6.3/zanshinsdk/tests/data/dummy_cloudformation_zanshin_service_role_template.json`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6.2/zanshinsdk/following_alerts_history.py` & `zanshin_sdk_python-1.6.3/zanshinsdk/following_alerts_history.py`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6.2/zanshinsdk/iterator.py` & `zanshin_sdk_python-1.6.3/zanshinsdk/iterator.py`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6.2/zanshinsdk/test_alerts_history.py` & `zanshin_sdk_python-1.6.3/zanshinsdk/tests/test_alerts_history.py`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6.2/zanshinsdk/test_client.py` & `zanshin_sdk_python-1.6.3/zanshinsdk/tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     ###################################################
     # __mock_aws_credentials__
     ###################################################
 
     def mock_aws_credentials(self):
         """Mocked AWS Credentials for moto."""
         moto_credentials_file_path = (
-            Path(__file__).parent.absolute() / "dummy_aws_credentials"
+            Path(__file__).parent.absolute() / "data/dummy_aws_credentials"
         )
         os.environ["AWS_SHARED_CREDENTIALS_FILE"] = str(moto_credentials_file_path)
 
     ###################################################
     # _update_client except
     ###################################################
 
@@ -1027,14 +1027,50 @@
         self.sdk.check_organization_scan_target(organization_id, scan_target_id)
 
         self.sdk._request.assert_called_once_with(
             "POST",
             f"/organizations/{organization_id}/scantargets/{scan_target_id}/check",
         )
 
+    def test_get_kind_oauth_link_should_call_api_with_scan_target_id(self):
+        organization_id = "822f4225-43e9-4922-b6b8-8b0620bdb1e3"
+        scan_target_id = "e22f4225-43e9-4922-b6b8-8b0620bdb110"
+        kind = zanshinsdk.ScanTargetKind.GITLAB
+
+        self.sdk.get_kind_oauth_link(organization_id, scan_target_id, kind)
+
+        self.sdk._request.assert_called_once_with(
+            "GET",
+            f"/oauth/link?"
+            f"organizationId={organization_id}"
+            f"&scanTargetGroupId={scan_target_id}",
+        )
+
+    def test_get_kind_oauth_link_should_call_api_with_scan_target_group_id(self):
+        organization_id = "822f4225-43e9-4922-b6b8-8b0620bdb1e3"
+        scan_target_id = "e22f4225-43e9-4922-b6b8-8b0620bdb110"
+        kind = zanshinsdk.ScanTargetKind.JIRA
+
+        self.sdk.get_kind_oauth_link(organization_id, scan_target_id, kind)
+
+        self.sdk._request.assert_called_once_with(
+            "GET",
+            f"/oauth/link?"
+            f"organizationId={organization_id}"
+            f"&scanTargetId={scan_target_id}",
+        )
+
+    def test_get_kind_oauth_link_should_raise_exception_with_invalid_kind(self):
+        organization_id = "822f4225-43e9-4922-b6b8-8b0620bdb1e3"
+        scan_target_id = "e22f4225-43e9-4922-b6b8-8b0620bdb110"
+        kind = zanshinsdk.ScanTargetKind.AWS
+
+        with self.assertRaises(ValueError):
+            self.sdk.get_kind_oauth_link(organization_id, scan_target_id, kind)
+
     def test_get_gworkspace_oauth_link(self):
         organization_id = "822f4225-43e9-4922-b6b8-8b0620bdb1e3"
         scan_target_id = "e22f4225-43e9-4922-b6b8-8b0620bdb110"
         self.sdk.get_gworkspace_oauth_link(organization_id, scan_target_id)
 
         self.sdk._request.assert_called_once_with(
             "GET",
@@ -1209,32 +1245,35 @@
 
         self.sdk._request.assert_called_once_with(
             "PUT",
             f"/organizations/{organization_id}/scantargetgroups/{scan_target_group_id}",
             body={"name": name},
         )
 
-    def test_create_scan_target_group(self):
+    def test_create_scan_target_group_should_call_api_with_valid_kind(self):
         organization_id = "822f4225-43e9-4922-b6b8-8b0620bdb1e3"
-        kind = zanshinsdk.ScanTargetKind.ORACLE
+        kind = zanshinsdk.ScanTargetKind.BITBUCKET
         name = "ScanTargetTest"
 
         self.sdk.create_scan_target_group(organization_id, kind, name)
 
-        with self.assertRaises(ValueError):
-            self.sdk.create_scan_target_group(
-                organization_id, zanshinsdk.ScanTargetKind.AWS, name
-            )
-
         self.sdk._request.assert_called_once_with(
             "POST",
             f"/organizations/{organization_id}/scantargetgroups",
             body={"name": name, "kind": kind},
         )
 
+    def test_create_scan_target_group_should_throw_exception_with_invalid_kind(self):
+        organization_id = "822f4225-43e9-4922-b6b8-8b0620bdb1e3"
+        kind = zanshinsdk.ScanTargetKind.AWS
+        name = "ScanTargetTest"
+
+        with self.assertRaises(ValueError):
+            self.sdk.create_scan_target_group(organization_id, kind, name)
+
     def test_iter_scan_target_group_compartments(self):
         organization_id = "822f4225-43e9-4922-b6b8-8b0620bdb1e3"
         scan_target_group_id = "322f4225-43e9-4922-b6b8-8b0620bdb110"
         try:
             next(
                 self.sdk.iter_scan_target_group_compartments(
                     organization_id, scan_target_group_id
@@ -3050,15 +3089,16 @@
                 status_code=200, json=lambda: {"id": created_scan_target_id}
             )
             client = zanshinsdk.Client()
             client._client.request = request
 
         # Create Mocked S3 tenchi-assets bucket
         with open(
-            "zanshinsdk/dummy_cloudformation_zanshin_service_role_template.json", "r"
+            "zanshinsdk/tests/data/dummy_cloudformation_zanshin_service_role_template.json",
+            "r",
         ) as dummy_template_file:
             DUMMY_TEMPLATE = json.load(dummy_template_file)
             s3 = boto3.client("s3", region_name="us-east-2")
             s3.create_bucket(
                 Bucket="tenchi-assets",
                 CreateBucketConfiguration={"LocationConstraint": "us-east-2"},
             )
@@ -3172,15 +3212,16 @@
                 status_code=200, json=lambda: {"id": created_scan_target_id}
             )
             client = zanshinsdk.Client()
             client._client.request = request
 
         # Create Mocked S3 tenchi-assets bucket
         with open(
-            "zanshinsdk/dummy_cloudformation_zanshin_service_role_template.json", "r"
+            "zanshinsdk/tests/data/dummy_cloudformation_zanshin_service_role_template.json",
+            "r",
         ) as dummy_template_file:
             DUMMY_TEMPLATE = json.load(dummy_template_file)
             s3 = boto3.client("s3", region_name="us-east-2")
             s3.create_bucket(
                 Bucket="tenchi-assets",
                 CreateBucketConfiguration={"LocationConstraint": "us-east-2"},
             )
```

### Comparing `zanshin_sdk_python-1.6.2/zanshinsdk/test_following_alerts_history.py` & `zanshin_sdk_python-1.6.3/zanshinsdk/tests/test_following_alerts_history.py`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6.2/zanshinsdk/test_iterator.py` & `zanshin_sdk_python-1.6.3/zanshinsdk/tests/test_iterator.py`

 * *Files identical despite different names*

### Comparing `zanshin_sdk_python-1.6.2/PKG-INFO` & `zanshin_sdk_python-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zanshin-sdk-python
-Version: 1.6.2
+Version: 1.6.3
 Summary: Python SDK to access the Tenchi Security Zanshin API v1
 Home-page: https://github.com/tenchi-security/zanshin-sdk-python
 License: Apache Software License
 Author: Tenchi Security
 Author-email: contact@tenchisecurity.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

