# Comparing `tmp/hhdm_apiclient_wrapper-24.1.0.dev1.tar.gz` & `tmp/hhdm_apiclient_wrapper-24.1.25.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hhdm_apiclient_wrapper-24.1.0.dev1.tar", max compression
+gzip compressed data, was "hhdm_apiclient_wrapper-24.1.25.dev1.tar", max compression
```

## Comparing `hhdm_apiclient_wrapper-24.1.0.dev1.tar` & `hhdm_apiclient_wrapper-24.1.25.dev1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      261 2023-12-29 17:07:07.063934 hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/__init__.py
--rw-r--r--   0        0        0     1486 2023-12-29 17:07:07.079510 hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/authentication_manager.py
--rw-r--r--   0        0        0    11836 2023-12-29 22:48:14.230579 hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/base_api_client.py
--rw-r--r--   0        0        0   600322 2023-12-29 18:23:25.169237 hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/generated/api_client.py
--rw-r--r--   0        0        0      597 2023-12-29 17:07:07.079510 hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/models/__init__.py
--rw-r--r--   0        0        0     2909 2023-12-29 18:14:58.336320 hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/models/api_attachment_models.py
--rw-r--r--   0        0        0     4192 2023-12-29 18:14:58.336320 hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/models/api_models.py
--rw-r--r--   0        0        0      783 2023-12-29 17:07:07.079510 hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/models/authentication_models.py
--rw-r--r--   0        0        0     2329 2023-12-29 18:14:58.336320 hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/models/mileage_models.py
--rw-r--r--   0        0        0     1018 2023-01-10 16:11:28.787196 hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/oauth_authentication_manager.py
--rw-r--r--   0        0        0     1075 2023-01-10 16:11:28.785196 hhdm_apiclient_wrapper-24.1.0.dev1/LICENSE
--rw-r--r--   0        0        0     1032 2023-12-29 23:55:26.367097 hhdm_apiclient_wrapper-24.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0      273 2023-12-29 18:15:19.185970 hhdm_apiclient_wrapper-24.1.0.dev1/README.md
--rw-r--r--   0        0        0      852 1970-01-01 00:00:00.000000 hhdm_apiclient_wrapper-24.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0      261 2024-01-16 16:35:39.118715 hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/__init__.py
+-rw-r--r--   0        0        0     1486 2024-03-04 16:29:41.364181 hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/authentication_manager.py
+-rw-r--r--   0        0        0    11836 2024-03-04 16:30:24.533456 hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/base_api_client.py
+-rw-r--r--   0        0        0   600426 2024-03-04 16:30:24.535971 hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/generated/api_client.py
+-rw-r--r--   0        0        0      597 2024-01-16 16:35:39.121716 hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/models/__init__.py
+-rw-r--r--   0        0        0     2909 2024-03-04 16:30:24.535971 hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/models/api_attachment_models.py
+-rw-r--r--   0        0        0     4597 2024-05-31 03:35:41.855160 hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/models/api_models.py
+-rw-r--r--   0        0        0      783 2024-01-16 16:35:39.122714 hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/models/authentication_models.py
+-rw-r--r--   0        0        0     2329 2024-03-04 16:30:24.537972 hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/models/mileage_models.py
+-rw-r--r--   0        0        0     1018 2024-01-16 16:35:39.123715 hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/oauth_authentication_manager.py
+-rw-r--r--   0        0        0     1075 2024-01-16 16:35:39.113052 hhdm_apiclient_wrapper-24.1.25.dev1/LICENSE
+-rw-r--r--   0        0        0     1034 2024-05-31 03:41:12.976074 hhdm_apiclient_wrapper-24.1.25.dev1/pyproject.toml
+-rw-r--r--   0        0        0      273 2024-03-04 16:30:24.530456 hhdm_apiclient_wrapper-24.1.25.dev1/README.md
+-rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 hhdm_apiclient_wrapper-24.1.25.dev1/PKG-INFO
```

### Comparing `hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/authentication_manager.py` & `hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/authentication_manager.py`

 * *Files identical despite different names*

### Comparing `hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/base_api_client.py` & `hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/base_api_client.py`

 * *Files identical despite different names*

### Comparing `hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/generated/api_client.py` & `hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/generated/api_client.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     async def update_ambient_measurement_attachment(self, account_id: str, ambient_measurement_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}AmbientMeasurements/{ambient_measurement_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_ambient_measurement_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, ambient_measurement_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_ambient_measurement_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             ambient_measurement_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, ambient_measurement_id, None, None)
@@ -157,15 +157,15 @@
 
             return await self._set_ambient_measurement_attachment_server_state_to_completed(add_attached_file_response, ambient_measurement_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, ambient_measurement_id, source_path, file_name, message=e)
 
     async def add_attachment_to_ambient_measurement(self, account_id: str, ambient_measurement_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to ambient_measurement.
-        
+        
         :param account_id: str, 
         :param ambient_measurement_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -320,15 +320,15 @@
     async def update_car_attachment(self, account_id: str, car_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}Cars/{car_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_car_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, car_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_car_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             car_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, car_id, None, None)
@@ -352,15 +352,15 @@
 
             return await self._set_car_attachment_server_state_to_completed(add_attached_file_response, car_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, car_id, source_path, file_name, message=e)
 
     async def add_attachment_to_car(self, account_id: str, car_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to car.
-        
+        
         :param account_id: str, 
         :param car_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -515,15 +515,15 @@
     async def update_championship_attachment(self, account_id: str, championship_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}Championships/{championship_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_championship_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, championship_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_championship_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             championship_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, championship_id, None, None)
@@ -547,15 +547,15 @@
 
             return await self._set_championship_attachment_server_state_to_completed(add_attached_file_response, championship_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, championship_id, source_path, file_name, message=e)
 
     async def add_attachment_to_championship(self, account_id: str, championship_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to championship.
-        
+        
         :param account_id: str, 
         :param championship_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -686,15 +686,15 @@
     async def update_event_attachment(self, account_id: str, event_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}Events/{event_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_event_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, event_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_event_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             event_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, event_id, None, None)
@@ -718,15 +718,15 @@
 
             return await self._set_event_attachment_server_state_to_completed(add_attached_file_response, event_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, event_id, source_path, file_name, message=e)
 
     async def add_attachment_to_event(self, account_id: str, event_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to event.
-        
+        
         :param account_id: str, 
         :param event_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -867,15 +867,15 @@
     async def update_event_car_data_attachment(self, account_id: str, event_car_data_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}EventCarDatas/{event_car_data_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_event_car_data_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, event_car_data_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_event_car_data_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             event_car_data_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, event_car_data_id, None, None)
@@ -899,15 +899,15 @@
 
             return await self._set_event_car_data_attachment_server_state_to_completed(add_attached_file_response, event_car_data_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, event_car_data_id, source_path, file_name, message=e)
 
     async def add_attachment_to_event_car_data(self, account_id: str, event_car_data_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to event_car_data.
-        
+        
         :param account_id: str, 
         :param event_car_data_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -1038,15 +1038,15 @@
     async def update_lap_attachment(self, account_id: str, lap_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}Laps/{lap_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_lap_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, lap_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_lap_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             lap_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, lap_id, None, None)
@@ -1070,15 +1070,15 @@
 
             return await self._set_lap_attachment_server_state_to_completed(add_attached_file_response, lap_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, lap_id, source_path, file_name, message=e)
 
     async def add_attachment_to_lap(self, account_id: str, lap_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to lap.
-        
+        
         :param account_id: str, 
         :param lap_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -1209,15 +1209,15 @@
     async def update_part_attachment(self, account_id: str, part_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}Parts/{part_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_part_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, part_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_part_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             part_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, part_id, None, None)
@@ -1241,15 +1241,15 @@
 
             return await self._set_part_attachment_server_state_to_completed(add_attached_file_response, part_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, part_id, source_path, file_name, message=e)
 
     async def add_attachment_to_part(self, account_id: str, part_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to part.
-        
+        
         :param account_id: str, 
         :param part_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -1394,15 +1394,15 @@
     async def update_part_category_attachment(self, account_id: str, part_category_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}PartCategories/{part_category_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_part_category_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, part_category_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_part_category_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             part_category_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, part_category_id, None, None)
@@ -1426,15 +1426,15 @@
 
             return await self._set_part_category_attachment_server_state_to_completed(add_attached_file_response, part_category_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, part_category_id, source_path, file_name, message=e)
 
     async def add_attachment_to_part_category(self, account_id: str, part_category_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to part_category.
-        
+        
         :param account_id: str, 
         :param part_category_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -1565,15 +1565,15 @@
     async def update_planned_run_attachment(self, account_id: str, planned_run_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}PlannedRuns/{planned_run_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_planned_run_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, planned_run_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_planned_run_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             planned_run_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, planned_run_id, None, None)
@@ -1597,15 +1597,15 @@
 
             return await self._set_planned_run_attachment_server_state_to_completed(add_attached_file_response, planned_run_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, planned_run_id, source_path, file_name, message=e)
 
     async def add_attachment_to_planned_run(self, account_id: str, planned_run_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to planned_run.
-        
+        
         :param account_id: str, 
         :param planned_run_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -1760,15 +1760,15 @@
     async def update_reference_pressure_run_attachment(self, account_id: str, reference_pressure_run_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}ReferencePressureRuns/{reference_pressure_run_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_reference_pressure_run_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, reference_pressure_run_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_reference_pressure_run_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             reference_pressure_run_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, reference_pressure_run_id, None, None)
@@ -1792,15 +1792,15 @@
 
             return await self._set_reference_pressure_run_attachment_server_state_to_completed(add_attached_file_response, reference_pressure_run_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, reference_pressure_run_id, source_path, file_name, message=e)
 
     async def add_attachment_to_reference_pressure_run(self, account_id: str, reference_pressure_run_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to reference_pressure_run.
-        
+        
         :param account_id: str, 
         :param reference_pressure_run_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -1955,15 +1955,15 @@
     async def update_run_plan_attachment(self, account_id: str, run_plan_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}RunPlans/{run_plan_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_run_plan_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, run_plan_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_run_plan_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             run_plan_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, run_plan_id, None, None)
@@ -1987,15 +1987,15 @@
 
             return await self._set_run_plan_attachment_server_state_to_completed(add_attached_file_response, run_plan_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, run_plan_id, source_path, file_name, message=e)
 
     async def add_attachment_to_run_plan(self, account_id: str, run_plan_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to run_plan.
-        
+        
         :param account_id: str, 
         :param run_plan_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -2150,15 +2150,15 @@
     async def update_run_sheet_attachment(self, account_id: str, run_sheet_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}RunSheets/{run_sheet_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_run_sheet_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, run_sheet_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_run_sheet_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             run_sheet_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, run_sheet_id, None, None)
@@ -2182,15 +2182,15 @@
 
             return await self._set_run_sheet_attachment_server_state_to_completed(add_attached_file_response, run_sheet_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, run_sheet_id, source_path, file_name, message=e)
 
     async def add_attachment_to_run_sheet(self, account_id: str, run_sheet_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to run_sheet.
-        
+        
         :param account_id: str, 
         :param run_sheet_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -2331,15 +2331,15 @@
     async def update_session_car_data_attachment(self, account_id: str, session_car_data_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}SessionCarDatas/{session_car_data_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_session_car_data_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, session_car_data_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_session_car_data_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             session_car_data_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, session_car_data_id, None, None)
@@ -2363,15 +2363,15 @@
 
             return await self._set_session_car_data_attachment_server_state_to_completed(add_attached_file_response, session_car_data_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, session_car_data_id, source_path, file_name, message=e)
 
     async def add_attachment_to_session_car_data(self, account_id: str, session_car_data_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to session_car_data.
-        
+        
         :param account_id: str, 
         :param session_car_data_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -2526,15 +2526,15 @@
     async def update_setup_attachment(self, account_id: str, setup_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}Setups/{setup_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_setup_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, setup_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_setup_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             setup_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, setup_id, None, None)
@@ -2558,15 +2558,15 @@
 
             return await self._set_setup_attachment_server_state_to_completed(add_attached_file_response, setup_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, setup_id, source_path, file_name, message=e)
 
     async def add_attachment_to_setup(self, account_id: str, setup_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to setup.
-        
+        
         :param account_id: str, 
         :param setup_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -2721,15 +2721,15 @@
     async def update_track_attachment(self, account_id: str, track_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}Tracks/{track_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_track_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, track_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_track_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             track_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, track_id, None, None)
@@ -2753,15 +2753,15 @@
 
             return await self._set_track_attachment_server_state_to_completed(add_attached_file_response, track_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, track_id, source_path, file_name, message=e)
 
     async def add_attachment_to_track(self, account_id: str, track_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to track.
-        
+        
         :param account_id: str, 
         :param track_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -2914,15 +2914,15 @@
     async def update_tyre_attachment(self, account_id: str, tyre_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}Tyres/{tyre_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_tyre_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, tyre_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_tyre_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             tyre_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, tyre_id, None, None)
@@ -2946,15 +2946,15 @@
 
             return await self._set_tyre_attachment_server_state_to_completed(add_attached_file_response, tyre_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, tyre_id, source_path, file_name, message=e)
 
     async def add_attachment_to_tyre(self, account_id: str, tyre_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to tyre.
-        
+        
         :param account_id: str, 
         :param tyre_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -3109,15 +3109,15 @@
     async def update_tyre_set_attachment(self, account_id: str, tyre_set_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}TyreSets/{tyre_set_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_tyre_set_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, tyre_set_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_tyre_set_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             tyre_set_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, tyre_set_id, None, None)
@@ -3141,15 +3141,15 @@
 
             return await self._set_tyre_set_attachment_server_state_to_completed(add_attached_file_response, tyre_set_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, tyre_set_id, source_path, file_name, message=e)
 
     async def add_attachment_to_tyre_set(self, account_id: str, tyre_set_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to tyre_set.
-        
+        
         :param account_id: str, 
         :param tyre_set_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -3280,15 +3280,15 @@
     async def update_tyre_set_pressure_adjustment_attachment(self, account_id: str, tyre_set_pressure_adjustment_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}TyreSetPressureAdjustments/{tyre_set_pressure_adjustment_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_tyre_set_pressure_adjustment_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, tyre_set_pressure_adjustment_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_tyre_set_pressure_adjustment_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             tyre_set_pressure_adjustment_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, tyre_set_pressure_adjustment_id, None, None)
@@ -3312,15 +3312,15 @@
 
             return await self._set_tyre_set_pressure_adjustment_attachment_server_state_to_completed(add_attached_file_response, tyre_set_pressure_adjustment_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, tyre_set_pressure_adjustment_id, source_path, file_name, message=e)
 
     async def add_attachment_to_tyre_set_pressure_adjustment(self, account_id: str, tyre_set_pressure_adjustment_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to tyre_set_pressure_adjustment.
-        
+        
         :param account_id: str, 
         :param tyre_set_pressure_adjustment_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -3475,15 +3475,15 @@
     async def update_tyre_specification_attachment(self, account_id: str, tyre_specification_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}TyreSpecifications/{tyre_specification_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_tyre_specification_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, tyre_specification_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_tyre_specification_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             tyre_specification_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, tyre_specification_id, None, None)
@@ -3507,15 +3507,15 @@
 
             return await self._set_tyre_specification_attachment_server_state_to_completed(add_attached_file_response, tyre_specification_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, tyre_specification_id, source_path, file_name, message=e)
 
     async def add_attachment_to_tyre_specification(self, account_id: str, tyre_specification_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to tyre_specification.
-        
+        
         :param account_id: str, 
         :param tyre_specification_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -3670,15 +3670,15 @@
     async def update_tyre_wear_sheet_attachment(self, account_id: str, tyre_wear_sheet_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}TyreWearSheets/{tyre_wear_sheet_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_tyre_wear_sheet_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, tyre_wear_sheet_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_tyre_wear_sheet_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             tyre_wear_sheet_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, tyre_wear_sheet_id, None, None)
@@ -3702,15 +3702,15 @@
 
             return await self._set_tyre_wear_sheet_attachment_server_state_to_completed(add_attached_file_response, tyre_wear_sheet_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, tyre_wear_sheet_id, source_path, file_name, message=e)
 
     async def add_attachment_to_tyre_wear_sheet(self, account_id: str, tyre_wear_sheet_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to tyre_wear_sheet.
-        
+        
         :param account_id: str, 
         :param tyre_wear_sheet_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -4054,15 +4054,15 @@
     async def update_driver_attachment(self, account_id: str, driver_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}Drivers/{driver_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_driver_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, driver_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_driver_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             driver_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, driver_id, None, None)
@@ -4086,15 +4086,15 @@
 
             return await self._set_driver_attachment_server_state_to_completed(add_attached_file_response, driver_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, driver_id, source_path, file_name, message=e)
 
     async def add_attachment_to_driver(self, account_id: str, driver_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to driver.
-        
+        
         :param account_id: str, 
         :param driver_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -4211,15 +4211,15 @@
     async def update_lap_sector_attachment(self, account_id: str, lap_sector_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}LapSectors/{lap_sector_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_lap_sector_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, lap_sector_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_lap_sector_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             lap_sector_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, lap_sector_id, None, None)
@@ -4243,15 +4243,15 @@
 
             return await self._set_lap_sector_attachment_server_state_to_completed(add_attached_file_response, lap_sector_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, lap_sector_id, source_path, file_name, message=e)
 
     async def add_attachment_to_lap_sector(self, account_id: str, lap_sector_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to lap_sector.
-        
+        
         :param account_id: str, 
         :param lap_sector_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -4406,15 +4406,15 @@
     async def update_car_manufacturer_attachment(self, account_id: str, car_manufacturer_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}CarManufacturers/{car_manufacturer_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_car_manufacturer_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, car_manufacturer_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_car_manufacturer_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             car_manufacturer_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, car_manufacturer_id, None, None)
@@ -4438,15 +4438,15 @@
 
             return await self._set_car_manufacturer_attachment_server_state_to_completed(add_attached_file_response, car_manufacturer_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, car_manufacturer_id, source_path, file_name, message=e)
 
     async def add_attachment_to_car_manufacturer(self, account_id: str, car_manufacturer_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to car_manufacturer.
-        
+        
         :param account_id: str, 
         :param car_manufacturer_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -4577,15 +4577,15 @@
     async def update_car_model_attachment(self, account_id: str, car_model_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}CarModels/{car_model_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_car_model_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, car_model_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_car_model_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             car_model_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, car_model_id, None, None)
@@ -4609,15 +4609,15 @@
 
             return await self._set_car_model_attachment_server_state_to_completed(add_attached_file_response, car_model_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, car_model_id, source_path, file_name, message=e)
 
     async def add_attachment_to_car_model(self, account_id: str, car_model_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to car_model.
-        
+        
         :param account_id: str, 
         :param car_model_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -4772,15 +4772,15 @@
     async def update_category_attachment(self, account_id: str, category_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}Categories/{category_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_category_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, category_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_category_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             category_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, category_id, None, None)
@@ -4804,15 +4804,15 @@
 
             return await self._set_category_attachment_server_state_to_completed(add_attached_file_response, category_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, category_id, source_path, file_name, message=e)
 
     async def add_attachment_to_category(self, account_id: str, category_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to category.
-        
+        
         :param account_id: str, 
         :param category_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -4967,15 +4967,15 @@
     async def update_issue_list_category_attachment(self, account_id: str, issue_list_category_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}IssueListCategories/{issue_list_category_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_issue_list_category_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, issue_list_category_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_issue_list_category_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             issue_list_category_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, issue_list_category_id, None, None)
@@ -4999,15 +4999,15 @@
 
             return await self._set_issue_list_category_attachment_server_state_to_completed(add_attached_file_response, issue_list_category_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, issue_list_category_id, source_path, file_name, message=e)
 
     async def add_attachment_to_issue_list_category(self, account_id: str, issue_list_category_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to issue_list_category.
-        
+        
         :param account_id: str, 
         :param issue_list_category_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -5162,15 +5162,15 @@
     async def update_job_list_category_attachment(self, account_id: str, job_list_category_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}JobListCategories/{job_list_category_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_job_list_category_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, job_list_category_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_job_list_category_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             job_list_category_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, job_list_category_id, None, None)
@@ -5194,15 +5194,15 @@
 
             return await self._set_job_list_category_attachment_server_state_to_completed(add_attached_file_response, job_list_category_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, job_list_category_id, source_path, file_name, message=e)
 
     async def add_attachment_to_job_list_category(self, account_id: str, job_list_category_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to job_list_category.
-        
+        
         :param account_id: str, 
         :param job_list_category_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -5357,15 +5357,15 @@
     async def update_job_list_template_attachment(self, account_id: str, job_list_template_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}JobListTemplates/{job_list_template_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_job_list_template_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, job_list_template_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_job_list_template_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             job_list_template_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, job_list_template_id, None, None)
@@ -5389,15 +5389,15 @@
 
             return await self._set_job_list_template_attachment_server_state_to_completed(add_attached_file_response, job_list_template_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, job_list_template_id, source_path, file_name, message=e)
 
     async def add_attachment_to_job_list_template(self, account_id: str, job_list_template_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to job_list_template.
-        
+        
         :param account_id: str, 
         :param job_list_template_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -5528,15 +5528,15 @@
     async def update_job_list_template_item_attachment(self, account_id: str, job_list_template_item_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}JobListTemplateItems/{job_list_template_item_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_job_list_template_item_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, job_list_template_item_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_job_list_template_item_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             job_list_template_item_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, job_list_template_item_id, None, None)
@@ -5560,15 +5560,15 @@
 
             return await self._set_job_list_template_item_attachment_server_state_to_completed(add_attached_file_response, job_list_template_item_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, job_list_template_item_id, source_path, file_name, message=e)
 
     async def add_attachment_to_job_list_template_item(self, account_id: str, job_list_template_item_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to job_list_template_item.
-        
+        
         :param account_id: str, 
         :param job_list_template_item_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -5699,15 +5699,15 @@
     async def update_session_attachment(self, account_id: str, session_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}Sessions/{session_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_session_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, session_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_session_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             session_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, session_id, None, None)
@@ -5731,15 +5731,15 @@
 
             return await self._set_session_attachment_server_state_to_completed(add_attached_file_response, session_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, session_id, source_path, file_name, message=e)
 
     async def add_attachment_to_session(self, account_id: str, session_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to session.
-        
+        
         :param account_id: str, 
         :param session_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -5894,15 +5894,15 @@
     async def update_team_attachment(self, account_id: str, team_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}Teams/{team_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_team_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, team_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_team_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             team_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, team_id, None, None)
@@ -5926,15 +5926,15 @@
 
             return await self._set_team_attachment_server_state_to_completed(add_attached_file_response, team_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, team_id, source_path, file_name, message=e)
 
     async def add_attachment_to_team(self, account_id: str, team_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to team.
-        
+        
         :param account_id: str, 
         :param team_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -6065,15 +6065,15 @@
     async def update_track_sector_definition_attachment(self, account_id: str, track_sector_definition_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}TrackSectorDefinitions/{track_sector_definition_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_track_sector_definition_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, track_sector_definition_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_track_sector_definition_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             track_sector_definition_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, track_sector_definition_id, None, None)
@@ -6097,15 +6097,15 @@
 
             return await self._set_track_sector_definition_attachment_server_state_to_completed(add_attached_file_response, track_sector_definition_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, track_sector_definition_id, source_path, file_name, message=e)
 
     async def add_attachment_to_track_sector_definition(self, account_id: str, track_sector_definition_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to track_sector_definition.
-        
+        
         :param account_id: str, 
         :param track_sector_definition_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -6260,15 +6260,15 @@
     async def update_session_object_issue_attachment(self, account_id: str, session_object_issue_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}SessionObjectIssues/{session_object_issue_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_session_object_issue_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, session_object_issue_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_session_object_issue_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             session_object_issue_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, session_object_issue_id, None, None)
@@ -6292,15 +6292,15 @@
 
             return await self._set_session_object_issue_attachment_server_state_to_completed(add_attached_file_response, session_object_issue_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, session_object_issue_id, source_path, file_name, message=e)
 
     async def add_attachment_to_session_object_issue(self, account_id: str, session_object_issue_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to session_object_issue.
-        
+        
         :param account_id: str, 
         :param session_object_issue_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -6455,15 +6455,15 @@
     async def update_session_object_job_attachment(self, account_id: str, session_object_job_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}SessionObjectJobs/{session_object_job_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_session_object_job_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, session_object_job_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_session_object_job_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             session_object_job_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, session_object_job_id, None, None)
@@ -6487,15 +6487,15 @@
 
             return await self._set_session_object_job_attachment_server_state_to_completed(add_attached_file_response, session_object_job_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, session_object_job_id, source_path, file_name, message=e)
 
     async def add_attachment_to_session_object_job(self, account_id: str, session_object_job_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to session_object_job.
-        
+        
         :param account_id: str, 
         :param session_object_job_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -6710,15 +6710,15 @@
     async def update_brake_disc_specification_attachment(self, account_id: str, brake_disc_specification_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}BrakeDiscSpecifications/{brake_disc_specification_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_brake_disc_specification_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, brake_disc_specification_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_brake_disc_specification_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             brake_disc_specification_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, brake_disc_specification_id, None, None)
@@ -6742,15 +6742,15 @@
 
             return await self._set_brake_disc_specification_attachment_server_state_to_completed(add_attached_file_response, brake_disc_specification_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, brake_disc_specification_id, source_path, file_name, message=e)
 
     async def add_attachment_to_brake_disc_specification(self, account_id: str, brake_disc_specification_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to brake_disc_specification.
-        
+        
         :param account_id: str, 
         :param brake_disc_specification_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -6905,15 +6905,15 @@
     async def update_brake_pad_specification_attachment(self, account_id: str, brake_pad_specification_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}BrakePadSpecifications/{brake_pad_specification_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_brake_pad_specification_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, brake_pad_specification_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_brake_pad_specification_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             brake_pad_specification_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, brake_pad_specification_id, None, None)
@@ -6937,15 +6937,15 @@
 
             return await self._set_brake_pad_specification_attachment_server_state_to_completed(add_attached_file_response, brake_pad_specification_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, brake_pad_specification_id, source_path, file_name, message=e)
 
     async def add_attachment_to_brake_pad_specification(self, account_id: str, brake_pad_specification_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to brake_pad_specification.
-        
+        
         :param account_id: str, 
         :param brake_pad_specification_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -7098,15 +7098,15 @@
     async def update_brake_disc_attachment(self, account_id: str, brake_disc_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}BrakeDiscs/{brake_disc_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_brake_disc_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, brake_disc_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_brake_disc_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             brake_disc_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, brake_disc_id, None, None)
@@ -7130,15 +7130,15 @@
 
             return await self._set_brake_disc_attachment_server_state_to_completed(add_attached_file_response, brake_disc_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, brake_disc_id, source_path, file_name, message=e)
 
     async def add_attachment_to_brake_disc(self, account_id: str, brake_disc_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to brake_disc.
-        
+        
         :param account_id: str, 
         :param brake_disc_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -7291,15 +7291,15 @@
     async def update_brake_pad_attachment(self, account_id: str, brake_pad_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}BrakePads/{brake_pad_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_brake_pad_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, brake_pad_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_brake_pad_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             brake_pad_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, brake_pad_id, None, None)
@@ -7323,15 +7323,15 @@
 
             return await self._set_brake_pad_attachment_server_state_to_completed(add_attached_file_response, brake_pad_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, brake_pad_id, source_path, file_name, message=e)
 
     async def add_attachment_to_brake_pad(self, account_id: str, brake_pad_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to brake_pad.
-        
+        
         :param account_id: str, 
         :param brake_pad_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -7484,15 +7484,15 @@
     async def update_brake_set_attachment(self, account_id: str, brake_set_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}BrakeSets/{brake_set_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_brake_set_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, brake_set_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_brake_set_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             brake_set_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, brake_set_id, None, None)
@@ -7516,15 +7516,15 @@
 
             return await self._set_brake_set_attachment_server_state_to_completed(add_attached_file_response, brake_set_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, brake_set_id, source_path, file_name, message=e)
 
     async def add_attachment_to_brake_set(self, account_id: str, brake_set_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to brake_set.
-        
+        
         :param account_id: str, 
         :param brake_set_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -7665,15 +7665,15 @@
     async def update_user_attachment(self, account_id: str, user_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}Users/{user_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_user_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, user_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_user_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             user_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, user_id, None, None)
@@ -7697,15 +7697,15 @@
 
             return await self._set_user_attachment_server_state_to_completed(add_attached_file_response, user_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, user_id, source_path, file_name, message=e)
 
     async def add_attachment_to_user(self, account_id: str, user_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to user.
-        
+        
         :param account_id: str, 
         :param user_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -7836,15 +7836,15 @@
     async def update_part_item_attachment(self, account_id: str, part_item_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}PartItems/{part_item_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_part_item_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, part_item_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_part_item_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             part_item_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, part_item_id, None, None)
@@ -7868,15 +7868,15 @@
 
             return await self._set_part_item_attachment_server_state_to_completed(add_attached_file_response, part_item_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, part_item_id, source_path, file_name, message=e)
 
     async def add_attachment_to_part_item(self, account_id: str, part_item_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to part_item.
-        
+        
         :param account_id: str, 
         :param part_item_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -8007,15 +8007,15 @@
     async def update_track_configuration_attachment(self, account_id: str, track_configuration_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}TrackConfigurations/{track_configuration_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_track_configuration_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, track_configuration_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_track_configuration_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             track_configuration_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, track_configuration_id, None, None)
@@ -8039,15 +8039,15 @@
 
             return await self._set_track_configuration_attachment_server_state_to_completed(add_attached_file_response, track_configuration_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, track_configuration_id, source_path, file_name, message=e)
 
     async def add_attachment_to_track_configuration(self, account_id: str, track_configuration_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to track_configuration.
-        
+        
         :param account_id: str, 
         :param track_configuration_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -8178,15 +8178,15 @@
     async def update_track_speed_trap_definition_attachment(self, account_id: str, track_speed_trap_definition_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}TrackSpeedTrapDefinitions/{track_speed_trap_definition_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_track_speed_trap_definition_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, track_speed_trap_definition_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_track_speed_trap_definition_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             track_speed_trap_definition_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, track_speed_trap_definition_id, None, None)
@@ -8210,15 +8210,15 @@
 
             return await self._set_track_speed_trap_definition_attachment_server_state_to_completed(add_attached_file_response, track_speed_trap_definition_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, track_speed_trap_definition_id, source_path, file_name, message=e)
 
     async def add_attachment_to_track_speed_trap_definition(self, account_id: str, track_speed_trap_definition_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to track_speed_trap_definition.
-        
+        
         :param account_id: str, 
         :param track_speed_trap_definition_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -8335,15 +8335,15 @@
     async def update_lap_speed_trap_attachment(self, account_id: str, lap_speed_trap_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}LapSpeedTraps/{lap_speed_trap_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_lap_speed_trap_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, lap_speed_trap_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_lap_speed_trap_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             lap_speed_trap_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, lap_speed_trap_id, None, None)
@@ -8367,15 +8367,15 @@
 
             return await self._set_lap_speed_trap_attachment_server_state_to_completed(add_attached_file_response, lap_speed_trap_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, lap_speed_trap_id, source_path, file_name, message=e)
 
     async def add_attachment_to_lap_speed_trap(self, account_id: str, lap_speed_trap_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to lap_speed_trap.
-        
+        
         :param account_id: str, 
         :param lap_speed_trap_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -8530,15 +8530,15 @@
     async def update_lap_marker_attachment(self, account_id: str, lap_marker_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}LapMarkers/{lap_marker_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_lap_marker_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, lap_marker_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_lap_marker_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             lap_marker_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, lap_marker_id, None, None)
@@ -8562,15 +8562,15 @@
 
             return await self._set_lap_marker_attachment_server_state_to_completed(add_attached_file_response, lap_marker_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, lap_marker_id, source_path, file_name, message=e)
 
     async def add_attachment_to_lap_marker(self, account_id: str, lap_marker_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to lap_marker.
-        
+        
         :param account_id: str, 
         :param lap_marker_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -8725,15 +8725,15 @@
     async def update_lap_track_status_marker_attachment(self, account_id: str, lap_track_status_marker_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}LapTrackStatusMarkers/{lap_track_status_marker_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_lap_track_status_marker_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, lap_track_status_marker_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_lap_track_status_marker_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             lap_track_status_marker_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, lap_track_status_marker_id, None, None)
@@ -8757,15 +8757,15 @@
 
             return await self._set_lap_track_status_marker_attachment_server_state_to_completed(add_attached_file_response, lap_track_status_marker_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, lap_track_status_marker_id, source_path, file_name, message=e)
 
     async def add_attachment_to_lap_track_status_marker(self, account_id: str, lap_track_status_marker_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to lap_track_status_marker.
-        
+        
         :param account_id: str, 
         :param lap_track_status_marker_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -8896,15 +8896,15 @@
     async def update_planned_lap_attachment(self, account_id: str, planned_lap_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}PlannedLaps/{planned_lap_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_planned_lap_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, planned_lap_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_planned_lap_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             planned_lap_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, planned_lap_id, None, None)
@@ -8928,15 +8928,15 @@
 
             return await self._set_planned_lap_attachment_server_state_to_completed(add_attached_file_response, planned_lap_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, planned_lap_id, source_path, file_name, message=e)
 
     async def add_attachment_to_planned_lap(self, account_id: str, planned_lap_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to planned_lap.
-        
+        
         :param account_id: str, 
         :param planned_lap_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -9089,15 +9089,15 @@
     async def update_issue_list_issue_attachment(self, account_id: str, issue_list_issue_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}IssueListIssues/{issue_list_issue_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_issue_list_issue_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, issue_list_issue_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_issue_list_issue_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             issue_list_issue_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, issue_list_issue_id, None, None)
@@ -9121,15 +9121,15 @@
 
             return await self._set_issue_list_issue_attachment_server_state_to_completed(add_attached_file_response, issue_list_issue_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, issue_list_issue_id, source_path, file_name, message=e)
 
     async def add_attachment_to_issue_list_issue(self, account_id: str, issue_list_issue_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to issue_list_issue.
-        
+        
         :param account_id: str, 
         :param issue_list_issue_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -9282,15 +9282,15 @@
     async def update_assembly_iteration_attachment(self, account_id: str, assembly_iteration_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}AssemblyIterations/{assembly_iteration_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_assembly_iteration_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, assembly_iteration_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_assembly_iteration_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             assembly_iteration_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, assembly_iteration_id, None, None)
@@ -9314,15 +9314,15 @@
 
             return await self._set_assembly_iteration_attachment_server_state_to_completed(add_attached_file_response, assembly_iteration_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, assembly_iteration_id, source_path, file_name, message=e)
 
     async def add_attachment_to_assembly_iteration(self, account_id: str, assembly_iteration_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to assembly_iteration.
-        
+        
         :param account_id: str, 
         :param assembly_iteration_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -9477,15 +9477,15 @@
     async def update_session_type_attachment(self, account_id: str, session_type_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}SessionTypes/{session_type_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_session_type_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, session_type_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_session_type_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             session_type_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, session_type_id, None, None)
@@ -9509,15 +9509,15 @@
 
             return await self._set_session_type_attachment_server_state_to_completed(add_attached_file_response, session_type_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, session_type_id, source_path, file_name, message=e)
 
     async def add_attachment_to_session_type(self, account_id: str, session_type_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to session_type.
-        
+        
         :param account_id: str, 
         :param session_type_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -9670,15 +9670,15 @@
     async def update_named_assembly_attachment(self, account_id: str, named_assembly_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}NamedAssemblies/{named_assembly_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_named_assembly_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, named_assembly_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_named_assembly_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             named_assembly_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, named_assembly_id, None, None)
@@ -9702,15 +9702,15 @@
 
             return await self._set_named_assembly_attachment_server_state_to_completed(add_attached_file_response, named_assembly_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, named_assembly_id, source_path, file_name, message=e)
 
     async def add_attachment_to_named_assembly(self, account_id: str, named_assembly_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to named_assembly.
-        
+        
         :param account_id: str, 
         :param named_assembly_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
@@ -9864,15 +9864,15 @@
     async def update_session_status_attachment(self, account_id: str, session_status_id: str, attached_file_id: str, update_model: UpdateModel) -> bool:
         response = await self.put_request(account_id, f"{self.api_endpoint}SessionStatuses/{session_status_id}/Attachments/{attached_file_id}", update_model)
         return response.ok
 
     async def _set_session_status_attachment_server_state_to_completed(self, add_attached_file_response: ApiAddAttachedFileResponse, session_status_id: str) -> AddAttachmentResult:
         # update the server attached file state to AvailableOnServer = 2
         update_result = await self.update_session_status_attachment(
-            add_attached_file_response.account_id,
+            add_attached_file_response.account_id,
             session_status_id,
             add_attached_file_response.attached_file_id,
             UpdateModel(None, [ParameterUpdateModel("ServerAttachedFileState", "2")])
         )
 
         if update_result:
             return AddAttachmentResult(AddAttachmentStatus.SUCCESS, add_attached_file_response, session_status_id, None, None)
@@ -9896,15 +9896,15 @@
 
             return await self._set_session_status_attachment_server_state_to_completed(add_attached_file_response, session_status_id)
         except Exception as e:
             return AddAttachmentResult(AddAttachmentStatus.FAILED_TO_UPLOAD, add_attached_file_response, session_status_id, source_path, file_name, message=e)
 
     async def add_attachment_to_session_status(self, account_id: str, session_status_id: str, model: ApiPrepareUploadModel, file) -> AddAttachmentResult:
         r"""Add attachment to session_status.
-        
+        
         :param account_id: str, 
         :param session_status_id: str,
         :param model: :class:`ApiPrepareUploadModel <ApiPrepareUploadModel>` upload configuration,
         :param file: path of the file to upload on the local filesystem, or stream-like object to upload
         :return: :class:`AddAttachmentResult <AddAttachmentResult>` object
         :rtype: AddAttachmentResult
         """
```

### Comparing `hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/models/__init__.py` & `hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/models/api_attachment_models.py` & `hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/models/api_attachment_models.py`

 * *Files identical despite different names*

### Comparing `hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/models/api_models.py` & `hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/models/api_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -31,22 +31,30 @@
         return {
             'Name': self.name,
             'Value': self.value
         }
 
 
 class CreateModel(IApiModel):
-    def __init__(self, copy_from_last: bool, copy_all: bool, index: int, parameter_updates: List[ParameterUpdateModel]) -> None:
+    def __init__(
+            self,
+            copy_from_last: bool = False,
+            copy_all: bool = False,
+            index: int | None = None,
+            parameter_updates: List[ParameterUpdateModel] = [],
+            copy_from_id: str | None = None) -> None:
         self.copy_from_last = copy_from_last
         self.copy_all = copy_all
         self.index = index
         self.parameter_updates = parameter_updates
-    
+        self.copy_from_id = copy_from_id
+
     def serialize(self) -> Dict:
         return {
+            'CopyFromId': self.copy_from_id,
             'CopyFromLast': self.copy_from_last,
             'CopyAll': self.copy_all,
             'Index': self.index,
             'ParameterUpdates': list([param.serialize() for param in self.parameter_updates])
         }
 
 
@@ -87,16 +95,23 @@
             'ChampionshipId': self.championship_id,
             'EventId': self.event_id,
             'CarId': self.car_id
         }
 
 
 class AssociationCreateModel(CreateModel):
-    def __init__(self, copy_from_last: bool, copy_all: bool, index: int, parameter_updates: List[ParameterUpdateModel], **associations_to_add) -> None:
-        super().__init__(copy_from_last, copy_all, index, parameter_updates)
+    def __init__(
+            self,
+            copy_from_last: bool = False,
+            copy_all: bool = False,
+            index: int | None = None,
+            parameter_updates: List[ParameterUpdateModel] = [],
+            copy_from_id: str | None = None,
+            **associations_to_add) -> None:
+        super().__init__(copy_from_last, copy_all, index, parameter_updates, copy_from_id)
         self.associations_to_add = associations_to_add
 
     def serialize(self) -> Dict:
         return {
             **super().serialize(),
             **self.associations_to_add
         }
```

### Comparing `hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/models/authentication_models.py` & `hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/models/authentication_models.py`

 * *Files identical despite different names*

### Comparing `hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/models/mileage_models.py` & `hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/models/mileage_models.py`

 * *Files identical despite different names*

### Comparing `hhdm_apiclient_wrapper-24.1.0.dev1/hhdm_apiclient_wrapper/oauth_authentication_manager.py` & `hhdm_apiclient_wrapper-24.1.25.dev1/hhdm_apiclient_wrapper/oauth_authentication_manager.py`

 * *Files identical despite different names*

### Comparing `hhdm_apiclient_wrapper-24.1.0.dev1/LICENSE` & `hhdm_apiclient_wrapper-24.1.25.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `hhdm_apiclient_wrapper-24.1.0.dev1/pyproject.toml` & `hhdm_apiclient_wrapper-24.1.25.dev1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hhdm-apiclient-wrapper"
-version = "24.1.0.dev1"
+version = "24.1.25.dev1"
 authors = [
   { name="HH Development", email="support@hh-dev.com" },
 ]
 description = "Wrapper for use of the HH Data Management Api Client"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.10"
@@ -16,15 +16,15 @@
 ]
 
 [project.urls]
 "Homepage" = "https://hh-dev.com/HHDataManagement"
 "Issues and Feedback" = "https://hh-dev.com/Contact"
 [tool.poetry]
 name = "hhdm-apiclient-wrapper"
-version = "24.1.0.dev1"
+version = "24.1.25.dev1"
 description = "Wrapper for use of the HH Data Management Api Client"
 authors = ["HH Development <support@hh-dev.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 lz4 = "^4.3.2"
```

### Comparing `hhdm_apiclient_wrapper-24.1.0.dev1/PKG-INFO` & `hhdm_apiclient_wrapper-24.1.25.dev1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: hhdm-apiclient-wrapper
-Version: 24.1.0.dev1
+Version: 24.1.25.dev1
 Summary: Wrapper for use of the HH Data Management Api Client
 Author: HH Development
 Author-email: support@hh-dev.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: lz4 (>=4.3.2,<5.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: validators (>=0.22.0,<0.23.0)
 Description-Content-Type: text/markdown
 
 ## hhdm_apiclient_wrapper
```

