# Comparing `tmp/wf_airtable_api_schema-0.5.0.tar.gz` & `tmp/wf_airtable_api_schema-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_airtable_api_schema-0.5.0.tar", max compression
+gzip compressed data, was "wf_airtable_api_schema-0.6.0.tar", max compression
```

## Comparing `wf_airtable_api_schema-0.5.0.tar` & `wf_airtable_api_schema-0.6.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
--rw-r--r--   0        0        0     1088 2022-01-03 22:41:31.067000 wf_airtable_api_schema-0.5.0/LICENSE
--rw-r--r--   0        0        0      787 2023-10-02 17:33:58.955814 wf_airtable_api_schema-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-03-28 16:57:29.611904 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/__init__.py
--rw-r--r--   0        0        0      446 2022-04-27 20:23:43.029666 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/__init__.py
--rw-r--r--   0        0        0      358 2022-05-31 17:10:12.202678 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/base_model.py
--rw-r--r--   0        0        0      340 2022-05-31 16:56:36.738571 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/contact_info.py
--rw-r--r--   0        0        0     3307 2023-10-02 16:45:30.984586 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/educators.py
--rw-r--r--   0        0        0     1514 2022-07-18 20:13:02.028874 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/educators_schools.py
--rw-r--r--   0        0        0     1196 2022-05-31 16:56:36.715133 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/geo_area_contacts.py
--rw-r--r--   0        0        0     1200 2022-05-31 16:56:36.729437 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/geo_area_target_communities.py
--rw-r--r--   0        0        0      371 2022-05-31 16:56:36.731670 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/guides_schools.py
--rw-r--r--   0        0        0      750 2022-05-31 16:56:36.743721 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/hubs.py
--rw-r--r--   0        0        0      390 2022-05-31 16:56:36.734057 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/languages.py
--rw-r--r--   0        0        0      552 2022-05-31 16:56:36.723037 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/montessori_certifications.py
--rw-r--r--   0        0        0     1028 2022-05-31 16:56:36.745899 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/partners.py
--rw-r--r--   0        0        0      734 2022-05-31 16:56:36.740926 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/pods.py
--rw-r--r--   0        0        0      743 2022-06-21 18:59:46.831320 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/response.py
--rw-r--r--   0        0        0     2721 2022-05-31 17:35:19.317457 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/schools.py
--rw-r--r--   0        0        0     2183 2023-10-02 16:43:10.444509 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/ssj_typeform_start_a_school.py
--rw-r--r--   0        0        0      172 2022-05-31 16:56:12.051519 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/target_communities.py
--rw-r--r--   0        0        0      258 2022-05-31 16:56:16.091750 wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/utils.py
--rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 wf_airtable_api_schema-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1088 2022-01-03 22:41:31.067000 wf_airtable_api_schema-0.6.0/LICENSE
+-rw-r--r--   0        0        0      787 2024-05-31 19:01:11.536862 wf_airtable_api_schema-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-03-28 16:57:29.611904 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/__init__.py
+-rw-r--r--   0        0        0      555 2024-05-31 19:01:02.022629 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/__init__.py
+-rw-r--r--   0        0        0     1547 2024-05-31 19:01:02.022792 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/auto_response_email_template.py
+-rw-r--r--   0        0        0      358 2022-05-31 17:10:12.202678 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/base_model.py
+-rw-r--r--   0        0        0      340 2022-05-31 16:56:36.738571 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/contact_info.py
+-rw-r--r--   0        0        0     3470 2024-05-31 19:01:02.023003 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/educators.py
+-rw-r--r--   0        0        0     1521 2024-05-31 19:01:02.023193 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/educators_schools.py
+-rw-r--r--   0        0        0     1360 2024-05-31 19:01:02.023379 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/geo_area_contacts.py
+-rw-r--r--   0        0        0     1207 2024-05-31 19:01:02.023564 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/geo_area_target_communities.py
+-rw-r--r--   0        0        0     1196 2024-05-31 19:01:02.023710 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/geo_areas.py
+-rw-r--r--   0        0        0      371 2022-05-31 16:56:36.731670 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/guides_schools.py
+-rw-r--r--   0        0        0      757 2024-05-31 19:01:02.023892 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/hubs.py
+-rw-r--r--   0        0        0      390 2024-05-13 15:14:25.839292 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/languages.py
+-rw-r--r--   0        0        0      552 2022-05-31 16:56:36.723037 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/montessori_certifications.py
+-rw-r--r--   0        0        0     1035 2024-05-31 19:01:02.024082 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/partners.py
+-rw-r--r--   0        0        0      741 2024-05-31 19:01:02.024258 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/pods.py
+-rw-r--r--   0        0        0      804 2024-05-31 19:01:02.024441 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/response.py
+-rw-r--r--   0        0        0     2728 2024-05-31 19:01:02.024628 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/schools.py
+-rw-r--r--   0        0        0     2654 2024-05-31 19:01:02.029497 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/ssj_fillout_get_involved.py
+-rw-r--r--   0        0        0     2183 2023-10-02 16:43:10.444509 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/ssj_typeform_start_a_school.py
+-rw-r--r--   0        0        0      172 2022-05-31 16:56:12.051519 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/target_communities.py
+-rw-r--r--   0        0        0      258 2022-05-31 16:56:16.091750 wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/utils.py
+-rw-r--r--   0        0        0      905 1970-01-01 00:00:00.000000 wf_airtable_api_schema-0.6.0/PKG-INFO
```

### Comparing `wf_airtable_api_schema-0.5.0/LICENSE` & `wf_airtable_api_schema-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_airtable_api_schema-0.5.0/pyproject.toml` & `wf_airtable_api_schema-0.6.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "wf-airtable-api-schema"
-version = "0.5.0"
+version = "0.6.0"
 description = "Simple package defining a schema translation layer between the client and Airtable bases"
 authors = ["Benjamin Jaffe-Talberg <ben.talberg@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/WildflowerSchools/wf-airtable-api-schema"
 classifiers = [
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     'Programming Language :: Python',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pydantic = "^1.9.0"
+pydantic = "^2.7.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/educators.py` & `wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/educators.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Union
 
-from .base_model import BaseModel
+from .base_model import BaseModel, RootModel
 
 from . import response as response_models
 from .languages import CreateAPILanguagesFields
 from .montessori_certifications import CreateAPIMontessoriCertificationsFields
 from .utils import copy_field
 
 MODEL_TYPE = "educator"
@@ -21,23 +21,26 @@
     affiliation_agreement_url: Optional[str] = None
     current_roles: Optional[list[str]] = None
     race_and_ethnicity: Optional[list[str]] = None
     educational_attainment: Optional[str] = None
     income_background_as_child: Optional[str] = None
     household_income: Optional[str] = None
     gender: Optional[str] = None
-    lgbtqia_identifying: Optional[bool] = False
+    lgbtqia_identifying: Optional[bool] = None
     pronouns: Optional[str] = None
     discovery_newsletter: Optional[bool] = False
     etl_newsletter: Optional[bool] = False
     initial_interest_in_governance_model: Optional[str] = None
+    initial_interest_in_age_classrooms: Optional[list[str]] = None
+    status: Optional[str] = None
 
 
-class CreateAPIEducatorFields(CommonAPIEducatorFields):
+class CreateUpdateAPIEducatorFields(CommonAPIEducatorFields):
     email: Optional[str] = None
+    get_involved_response_id: Optional[str] = None
     start_a_school_response_id: Optional[str] = None
     assigned_partner_id: Optional[str] = None
     target_community_id: Optional[str] = None
     montessori_certifications: Optional[list[CreateAPIMontessoriCertificationsFields]] = []
     languages: Optional[list[CreateAPILanguagesFields]] = []
 
 
@@ -73,16 +76,16 @@
     hub: Optional[response_models.APILinksAndData] = None
 
 
 class APIEducatorData(response_models.APIData):
     fields: APIEducatorFields
 
 
-class ListAPIEducatorData(BaseModel):
-    __root__: list[APIEducatorData]
+class ListAPIEducatorData(RootModel):
+    root: list[APIEducatorData]
 
 
 class APIEducatorResponse(response_models.APIResponse):
     data: APIEducatorData
 
 
 class ListAPIEducatorResponse(response_models.ListAPIResponse):
```

### Comparing `wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/educators_schools.py` & `wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/educators_schools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import date
 from enum import Enum
 from typing import Optional, Union
 
-from .base_model import BaseModel
+from .base_model import BaseModel, RootModel
 from . import response as response_models
 
 MODEL_TYPE = "educator_school"
 
 
 class APIEducatorSchoolRoles(str, Enum):
     FOUNDER = "Founder"
@@ -40,16 +40,16 @@
     school: Optional[response_models.APILinksAndData] = None
 
 
 class APIEducatorSchoolData(response_models.APIData):
     fields: APIEducatorSchoolFields
 
 
-class ListAPIEducatorSchoolData(BaseModel):
-    __root__: list[APIEducatorSchoolData]
+class ListAPIEducatorSchoolData(RootModel):
+    root: list[APIEducatorSchoolData]
 
 
 class APIEducatorSchoolResponse(response_models.APIResponse):
     data: APIEducatorSchoolData
 
 
 class ListAPIEducatorSchoolResponse(response_models.ListAPIResponse):
```

### Comparing `wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/geo_area_contacts.py` & `wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/geo_area_contacts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Union
 
-from .base_model import BaseModel
+from .base_model import BaseModel, RootModel
 from . import response as response_models
 
 MODEL_TYPE = "area_contact"
 
 
 class APIGeoAreaContactFields(BaseModel):
     area_name: Optional[str] = None
@@ -14,27 +14,29 @@
     first_contact_email: Optional[str] = None
     assigned_rse_name: Optional[str] = None
     hub_name: Optional[str] = None
     sendgrid_template_id: Optional[str] = None
     latitude: Optional[float] = None
     longitude: Optional[float] = None
     geocode: Optional[dict] = None
+    # auto_response_email_template_ids: Optional[list[str]] = None
 
 
 class APIGeoAreaContactRelationships(BaseModel):
     hub: Optional[response_models.APILinksAndData] = None
     assigned_rse: Optional[response_models.APILinksAndData] = None
+    auto_response_email_templates: Optional[list[response_models.APILinksAndData]] = None
 
 
 class APIGeoAreaContactData(response_models.APIData):
     fields: APIGeoAreaContactFields
 
 
-class ListAPIGeoAreaContactData(BaseModel):
-    __root__: list[APIGeoAreaContactData]
+class ListAPIGeoAreaContactData(RootModel):
+    root: list[APIGeoAreaContactData]
 
 
 class APIGeoAreaContactResponse(response_models.APIResponse):
     data: APIGeoAreaContactData
 
 
 class ListAPIGeoAreaContactResponse(response_models.ListAPIResponse):
```

### Comparing `wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/geo_area_target_communities.py` & `wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/geo_area_target_communities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Union
 
-from .base_model import BaseModel
+from .base_model import BaseModel, RootModel
 from . import response as response_models
 
 MODEL_TYPE = "area_target_community"
 
 
 class APIGeoAreaTargetCommunityFields(BaseModel):
     area_name: Optional[str] = None
@@ -23,16 +23,16 @@
     target_community: Optional[response_models.APILinksAndData] = None
 
 
 class APIGeoAreaTargetCommunityData(response_models.APIData):
     fields: APIGeoAreaTargetCommunityFields
 
 
-class ListAPIGeoAreaTargetCommunityData(BaseModel):
-    __root__: list[APIGeoAreaTargetCommunityData]
+class ListAPIGeoAreaTargetCommunityData(RootModel):
+    root: list[APIGeoAreaTargetCommunityData]
 
 
 class APIGeoAreaTargetCommunityResponse(response_models.APIResponse):
     data: APIGeoAreaTargetCommunityData
 
 
 class ListAPIGeoAreaTargetCommunityResponse(response_models.ListAPIResponse):
```

### Comparing `wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/hubs.py` & `wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/hubs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Union
 
-from .base_model import BaseModel
+from .base_model import BaseModel, RootModel
 from . import response as response_models
 
 MODEL_TYPE = "hub"
 
 
 class APIHubFields(BaseModel):
     name: Optional[str] = None
@@ -16,16 +16,16 @@
     schools: Optional[response_models.APILinksAndData] = None
 
 
 class APIHubData(response_models.APIData):
     fields: APIHubFields
 
 
-class ListAPIHubData(BaseModel):
-    __root__: list[APIHubData]
+class ListAPIHubData(RootModel):
+    root: list[APIHubData]
 
 
 class APIHubResponse(response_models.APIResponse):
     data: APIHubData
 
 
 class ListAPIHubResponse(response_models.ListAPIResponse):
```

### Comparing `wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/montessori_certifications.py` & `wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/montessori_certifications.py`

 * *Files identical despite different names*

### Comparing `wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/partners.py` & `wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/partners.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Union
 
-from .base_model import BaseModel
+from .base_model import BaseModel, RootModel
 from . import response as response_models
 
 MODEL_TYPE = "partner"
 
 
 class APIPartnerFields(BaseModel):
     name: Optional[str] = None
@@ -21,16 +21,16 @@
     educators_partner_guiding: Optional[response_models.APILinksAndData] = None
 
 
 class APIPartnerData(response_models.APIData):
     fields: APIPartnerFields
 
 
-class ListAPIPartnerData(BaseModel):
-    __root__: list[APIPartnerData]
+class ListAPIPartnerData(RootModel):
+    root: list[APIPartnerData]
 
 
 class APIPartnerResponse(response_models.APIResponse):
     data: APIPartnerData
 
 
 class ListAPIPartnerResponse(response_models.ListAPIResponse):
```

### Comparing `wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/pods.py` & `wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/pods.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Union
 
-from .base_model import BaseModel
+from .base_model import BaseModel, RootModel
 from . import response as response_models
 
 MODEL_TYPE = "pod"
 
 
 class APIPodFields(BaseModel):
     name: Optional[str] = None
@@ -16,16 +16,16 @@
     schools: Optional[response_models.APILinksAndData] = None
 
 
 class APIPodData(response_models.APIData):
     fields: APIPodFields
 
 
-class ListAPIPodData(BaseModel):
-    __root__: list[APIPodData]
+class ListAPIPodData(RootModel):
+    root: list[APIPodData]
 
 
 class APIPodResponse(response_models.APIResponse):
     data: APIPodData
 
 
 class ListAPIPodResponse(response_models.ListAPIResponse):
```

### Comparing `wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/response.py` & `wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 from typing import Optional, Union
 
 from .base_model import BaseModel
 
 
 class APILinks(BaseModel):
-    links: Optional[dict[str, Optional[str]]]
+    links: Optional[dict[str, Optional[str]]] = None
 
 
 class APIDataBase(BaseModel):
     id: str
     type: str
 
 
 class APIDataWithFields(BaseModel):
     id: str
     type: str
     fields: dict
 
 
 class APILinksAndData(APILinks):
-    data: Optional[Union[str, APIDataWithFields, APIDataBase, list[Union[str, APIDataWithFields, APIDataBase]]]]
+    data: Optional[Union[str, APIDataWithFields, APIDataBase, list[Union[str, APIDataWithFields, APIDataBase]]]] = None
 
 
 class APIData(APIDataWithFields):
     fields: dict
-    relationships: dict[str, Optional[Union[APILinksAndData, APILinks]]]
+    relationships: dict[str, Optional[Union[APILinksAndData, APILinks, list[Union[APILinksAndData, APILinks]]]]]
     links: dict[str, Optional[str]]
 
 
 class APIResponse(APILinks):
     data: APIData
-    meta: Optional[dict]
+    meta: Optional[dict] = None
 
 
 class ListAPIResponse(APIResponse):
     data: list[Union[APIData, dict]]
```

### Comparing `wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/schools.py` & `wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/schools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from datetime import date
 from typing import Optional, Union
 
 from pydantic import HttpUrl
 
-from .base_model import BaseModel
+from .base_model import BaseModel, RootModel
 from . import response as response_models
 from .utils import copy_field
 
 MODEL_TYPE = "school"
 
 
 class APISchoolFields(BaseModel):
@@ -64,16 +64,16 @@
     primary_contacts: Optional[response_models.APILinksAndData] = None
 
 
 class APISchoolData(response_models.APIData):
     fields: APISchoolFields
 
 
-class ListAPISchoolData(BaseModel):
-    __root__: list[APISchoolData]
+class ListAPISchoolData(RootModel):
+    root: list[APISchoolData]
 
 
 class APISchoolResponse(response_models.APIResponse):
     data: APISchoolData
 
 
 class ListAPISchoolResponse(response_models.ListAPIResponse):
```

### Comparing `wf_airtable_api_schema-0.5.0/wf_airtable_api_schema/models/ssj_typeform_start_a_school.py` & `wf_airtable_api_schema-0.6.0/wf_airtable_api_schema/models/ssj_typeform_start_a_school.py`

 * *Files identical despite different names*

### Comparing `wf_airtable_api_schema-0.5.0/PKG-INFO` & `wf_airtable_api_schema-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: wf-airtable-api-schema
-Version: 0.5.0
+Version: 0.6.0
 Summary: Simple package defining a schema translation layer between the client and Airtable bases
 Home-page: https://github.com/WildflowerSchools/wf-airtable-api-schema
 License: MIT
 Author: Benjamin Jaffe-Talberg
 Author-email: ben.talberg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Project-URL: Repository, https://github.com/WildflowerSchools/wf-airtable-api-schema
```

