# Comparing `tmp/neuropacs-1.6.6.tar.gz` & `tmp/neuropacs-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuropacs-1.6.6.tar", last modified: Fri Apr 12 21:19:38 2024, max compression
+gzip compressed data, was "neuropacs-1.6.7.tar", last modified: Fri May 31 05:53:31 2024, max compression
```

## Comparing `neuropacs-1.6.6.tar` & `neuropacs-1.6.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-12 21:19:38.262622 neuropacs-1.6.6/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1061 2024-02-21 03:24:17.000000 neuropacs-1.6.6/LICENSE
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-04-12 21:19:38.262343 neuropacs-1.6.6/PKG-INFO
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1708 2024-01-04 01:45:39.000000 neuropacs-1.6.6/README.md
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-12 21:19:38.257437 neuropacs-1.6.6/examples/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-24 02:20:58.000000 neuropacs-1.6.6/examples/__init__.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      970 2024-04-04 07:24:41.000000 neuropacs-1.6.6/examples/example1.py
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-12 21:19:38.258315 neuropacs-1.6.6/neuropacs/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      163 2024-04-12 21:19:04.000000 neuropacs-1.6.6/neuropacs/__init__.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1556 2024-04-12 21:16:50.000000 neuropacs-1.6.6/neuropacs/ex.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    22249 2024-04-12 21:18:50.000000 neuropacs-1.6.6/neuropacs/sdk.py
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-12 21:19:38.262035 neuropacs-1.6.6/neuropacs.egg-info/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-04-12 21:19:38.000000 neuropacs-1.6.6/neuropacs.egg-info/PKG-INFO
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      330 2024-04-12 21:19:38.000000 neuropacs-1.6.6/neuropacs.egg-info/SOURCES.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        1 2024-04-12 21:19:38.000000 neuropacs-1.6.6/neuropacs.egg-info/dependency_links.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      285 2024-04-12 21:19:38.000000 neuropacs-1.6.6/neuropacs.egg-info/requires.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       25 2024-04-12 21:19:38.000000 neuropacs-1.6.6/neuropacs.egg-info/top_level.txt
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       38 2024-04-12 21:19:38.262667 neuropacs-1.6.6/setup.cfg
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1346 2024-04-12 21:19:01.000000 neuropacs-1.6.6/setup.py
-drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-04-12 21:19:38.260778 neuropacs-1.6.6/tests/
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-09 22:18:09.000000 neuropacs-1.6.6/tests/__init__.py
--rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    26402 2024-01-06 03:43:44.000000 neuropacs-1.6.6/tests/tests_neuropacs.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-05-31 05:53:31.481015 neuropacs-1.6.7/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1061 2024-02-21 03:24:17.000000 neuropacs-1.6.7/LICENSE
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-05-31 05:53:31.480767 neuropacs-1.6.7/PKG-INFO
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1708 2024-01-04 01:45:39.000000 neuropacs-1.6.7/README.md
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-05-31 05:53:31.476942 neuropacs-1.6.7/examples/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-24 02:20:58.000000 neuropacs-1.6.7/examples/__init__.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      970 2024-05-18 19:30:13.000000 neuropacs-1.6.7/examples/example1.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-05-31 05:53:31.478287 neuropacs-1.6.7/neuropacs/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      163 2024-05-31 05:52:52.000000 neuropacs-1.6.7/neuropacs/__init__.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1553 2024-05-31 05:48:35.000000 neuropacs-1.6.7/neuropacs/ex.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    28526 2024-05-31 05:10:48.000000 neuropacs-1.6.7/neuropacs/sdk.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-05-31 05:53:31.480399 neuropacs-1.6.7/neuropacs.egg-info/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     2708 2024-05-31 05:53:31.000000 neuropacs-1.6.7/neuropacs.egg-info/PKG-INFO
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      330 2024-05-31 05:53:31.000000 neuropacs-1.6.7/neuropacs.egg-info/SOURCES.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        1 2024-05-31 05:53:31.000000 neuropacs-1.6.7/neuropacs.egg-info/dependency_links.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)      285 2024-05-31 05:53:31.000000 neuropacs-1.6.7/neuropacs.egg-info/requires.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       25 2024-05-31 05:53:31.000000 neuropacs-1.6.7/neuropacs.egg-info/top_level.txt
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)       38 2024-05-31 05:53:31.481059 neuropacs-1.6.7/setup.cfg
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)     1346 2024-05-31 05:52:48.000000 neuropacs-1.6.7/setup.py
+drwxr-xr-x   0 kerrickcavanaugh   (501) staff       (20)        0 2024-05-31 05:53:31.479801 neuropacs-1.6.7/tests/
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)        0 2023-12-09 22:18:09.000000 neuropacs-1.6.7/tests/__init__.py
+-rw-r--r--   0 kerrickcavanaugh   (501) staff       (20)    26402 2024-01-06 03:43:44.000000 neuropacs-1.6.7/tests/tests_neuropacs.py
```

### Comparing `neuropacs-1.6.6/LICENSE` & `neuropacs-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neuropacs-1.6.6/PKG-INFO` & `neuropacs-1.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuropacs
-Version: 1.6.6
+Version: 1.6.7
 Summary: NeuroPACS Python SDK
 Home-page: https://github.com/neuropacs/neuropacs-py-sdk
 Author: Kerrick Cavanaugh
 Author-email: kerrick@neuropacs.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neuropacs-1.6.6/README.md` & `neuropacs-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `neuropacs-1.6.6/examples/example1.py` & `neuropacs-1.6.7/examples/example1.py`

 * *Files identical despite different names*

### Comparing `neuropacs-1.6.6/neuropacs/ex.py` & `neuropacs-1.6.7/neuropacs/ex.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,52 @@
 from sdk import Neuropacs
 
 def main():
     # api_key = "your_api_key"
     api_key = "m0ig54amrl87awtwlizcuji2bxacjm"
     server_url = "https://sl3tkzp9ve.execute-api.us-east-2.amazonaws.com/dev/"
     product_id = "PD/MSA/PSP-v1.0"
-    result_format = "TXT"
+    result_format = "JSON"
 
 
     # PRINT CURRENT VERSION
     # version = Neuropacs.PACKAGE_VERSION
 
     # INITIALIZE NEUROPACS SDK
     # npcs = Neuropacs.init(server_url, server_url, api_key)
     npcs = Neuropacs(server_url, api_key)
 
     # CREATE A CONNECTION   
     conn = npcs.connect()
     print(conn)
 
-    # # CREATE A NEW JOB
+    # # # # CREATE A NEW JOB
     order = npcs.new_job()
     print(order)
 
-    # # UPLOAD A DATASET
+    # # # # UPLOAD A DATASET
     # upload = npcs.upload("../dicom_examples/DICOM_small/woo_I0", "test123", order)
     # print(upload)
-    datasetID = npcs.upload_dataset("../dicom_examples/DICOM_small", None, None, callback=lambda data: print(f"Dataset ID: {data['datasetId']}, Progress: {data['progress']}%, Files Uploaded: {data['filesUploaded']}"))
-    print(datasetID)
+    # datasetID = npcs.upload_dataset("../dicom_examples/06_001", order, order, callback=lambda data: print(data))
+    # datasetID = npcs.upload_dataset("../dicom_examples/06_001", order, order)
 
-    # verUpl = npcs.validate_upload(["woo_I0", "woo_I2", "woo_I3", "woo_I4", "TEST234","woo_I7", "woo_I8", "woo_I9","woo_I10", "woo_I11"], "AHw8Wqpb2Ts8ffeTvlAR", "I2C1mIU8IsiFwkTZfpsd")
+    # 
+    # print(datasetID)
+
+    # verUpl = npcs.validate_upload("../dicom_examples/06_001", "e7d6902d-b49f-4dae-9a41-4fe8cf510aab", "e7d6902d-b49f-4dae-9a41-4fe8cf510aab")
     # print(verUpl)
 
     # # # START A JOB
-    # job = npcs.run_job(product_id, "Ri8vzdAXlWmiLgEV1JUC","dfjujor327nf415vubj7x")
-    # print(job)
+    job = npcs.run_job(product_id, "e7d6902d-b49f-4dae-9a41-4fe8cf510aab","e7d6902d-b49f-4dae-9a41-4fe8cf510aab")
+    print(job)
 
-    # # CHECK STATUS
-    # status = npcs.check_status("TEST", "dfjujor327nf415vubj7x")
+    # # # CHECK STATUS
+    # status = npcs.check_status("TEST", "WgcvoJQk3xFNiOPMoPZ6")
     # print(status)
 
-    # # # GET RESULTS
-    # results = npcs.get_results(result_format, "TEST", "rnxor3q9euor9r088x0mnl")
+    # # # # GET RESULTS
+    # results = npcs.get_results(result_format, "WgcvoJQk3xFNiOPMoPZ6", "WgcvoJQk3xFNiOPMoPZ6")
     # print(results)
 
     
 
 main()
```

### Comparing `neuropacs-1.6.6/neuropacs/sdk.py` & `neuropacs-1.6.7/neuropacs/sdk.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import os
 import requests
 import json
 from Crypto.Random import get_random_bytes
 from Crypto.Util.Padding import pad
 import base64
-import string
-import secrets
+import zipfile
+import io
+import uuid
 from datetime import datetime
-from tqdm import tqdm
-import hashlib
 from Crypto.Cipher import AES
 from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import padding
 from cryptography.hazmat.primitives.asymmetric import padding
 from cryptography.hazmat.primitives import serialization
 import requests
 
@@ -26,14 +25,15 @@
         self.client = client
         self.aes_key = self.__generate_aes_key()
         self.connection_id = ""
         self.aes_key = ""
         self.dataset_upload = False
         self.files_uploaded = 0
 
+    # Private methods
     def __generate_aes_key(self):
         """Generate an 16-byte AES key for AES-CTR encryption.
 
         :return: AES key encoded as a base64 string.
         """
         aes_key = get_random_bytes(16)
         aes_key_base64 = base64.b64encode(aes_key).decode('utf-8')
@@ -173,22 +173,345 @@
 
             return decrypted_data
         except Exception as e:
             if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
                 raise Exception(e.args[0]['neuropacsError']) 
             else:
                 raise Exception("AES decryption failed!")
-    
-    def __generate_filename(self):
-        """Generate a filename for byte data
-        :return: 20 character random alphanumeric string
-        """
-        characters = string.ascii_letters + string.digits
-        random_string = ''.join(secrets.choice(characters) for _ in range(20))
-        return random_string
+
+    def __generate_unique_uuid(self):
+        """Generate a random v4 uuid
+        :return: V4 UUID string
+        """
+        return str(uuid.uuid4())
+
+    def __read_file_contents(self, file_path):
+        """
+        Read file conents of file at file_path
+
+        :param str file_path Path to the file to be read
+
+        :return: File contents in bytes
+        """
+        with open(file_path, 'rb') as file:
+            contents = file.read()
+        return contents
+
+    def __new_multipart_upload(self, dataset_id, zip_index, order_id):
+        """
+        Start a new multipart upload
+
+        :param str dataset_id Base64 dataset_id
+        :param int zip_index Index of zip file
+        :param str order_id Base65 order_id
+
+        :returns AWS upload_id
+        """
+        try:
+            encrypted_order_id = self.__encrypt_aes_ctr(order_id, "string", "string")
+        
+            headers = {'Content-type': 'text/plain', 'Connection-Id': self.connection_id,'Order-Id': encrypted_order_id, 'Client': self.client}
+
+            body = {
+                'datasetId': dataset_id,
+                'zipIndex': str(zip_index)
+            }
+
+            encrypted_body = self.__encrypt_aes_ctr(body, "json", "string")
+
+            res = requests.post(f"{self.server_url}/api/multipartUploadRequest/", data=encrypted_body, headers=headers)
+
+            if not res.ok:
+                raise Exception(json.loads(res.text)["error"])
+
+            text = res.text
+            res_json = self.__decrypt_aes_ctr(text, "json")
+            upload_id = res_json["uploadId"]
+
+            return upload_id
+
+        except Exception as e:
+            raise Exception(f"Multipart upload initialization failed: {str(e)}")
+            
+
+    def __complete_multipart_upload(self, order_id, dataset_id, zip_index, upload_id, upload_parts):
+        """
+        Complete a new multipart upload
+
+        :param str order_id Base64 order_id
+        :param str dataset_id Base64 dataset_id
+        :param int zip_index Index of zip file
+        :param str upload_id Base64 upload_id
+        :param dict upload_parts Uploaded parts dict
+
+        :returns Status code
+        """
+        try:
+            encrypted_order_id = self.__encrypt_aes_ctr(order_id, "string", "string")
+        
+            headers = {'Content-type': 'text/plain', 'Connection-Id': self.connection_id,'Order-Id': encrypted_order_id, 'Client': self.client}
+
+            body = {
+                'datasetId': dataset_id,
+                'zipIndex': zip_index,
+                'uploadId': upload_id,
+                'uploadParts': upload_parts
+            }
+
+            encrypted_body = self.__encrypt_aes_ctr(body, "json", "string")
+
+            res = requests.post(f"{self.server_url}/api/completeMultipartUpload/", data=encrypted_body, headers=headers)
+
+            if not res.ok:
+                raise Exception(json.loads(res.text)["error"])
+
+            return 200
+
+        except Exception as e:
+            raise Exception(f"ultipart upload completion failed: {str(e)}")
+
+    def __upload_part(self, upload_id, dataset_id, zip_index, order_id, part_number, part_data):
+        """
+        Upload a part of the multipart upload
+
+        :param str upload_id Base64 upload_id
+        :param str dataset_id Base64 dataset_id
+        :param int zip_index Index of zip file
+        :param str order_id Base64 orderId
+        :param int part_number Part number
+        :param bytes part_data Part data
+
+        :return Etag
+        """
+        try:
+            encrypted_order_id = self.__encrypt_aes_ctr(order_id, "string", "string")
+        
+            headers = {'Content-type': 'text/plain', 'connection-id': self.connection_id,'order-id': encrypted_order_id, 'client': self.client}
+
+            body = {
+                'datasetId': dataset_id,
+                'uploadId': upload_id,
+                'partNumber': str(part_number),
+                'zipIndex': str(zip_index)
+            }
+
+            encrypted_body = self.__encrypt_aes_ctr(body, "json", "string")
+
+            res = requests.post(f"{self.server_url}/api/multipartPresignedUrl/", data=encrypted_body, headers=headers)
+            
+            if not res.ok:
+                raise Exception(json.loads(res.text)["error"])
+
+            text = res.text
+            res_json = self.__decrypt_aes_ctr(text, "json")
+            presigned_url = res_json["presignedURL"] # URL to upload part
+
+
+            fail = False
+            for attempt in range(3):
+                upload_res = requests.put(presigned_url, data=part_data)
+
+                if not upload_res.ok:
+                    fail = True
+                else:
+                    e_tag = upload_res.headers.get('ETag')
+                    return e_tag
+
+            if fail:
+                raise Exception("Upload failed after 3 attempts")
+
+        except Exception as e:
+            raise Exception(f"Upload part failed: {str(e)}")
+
+
+    def __split_zip_contents(self, zip_contents, part_size):
+        """
+        Split zip contents into chunk of part_size for upload
+
+        :param bytes zip_contents Bytes content of zip file
+        :param int part_size Size of each chunk
+        """
+        try:
+            parts = []
+            start = 0
+            while start < len(zip_contents):
+                end = min(start + part_size, len(zip_contents))
+                parts.append(zip_contents[start:end])
+                start = end
+            return parts
+        except Exception as error:
+            raise Exception(f"Partitioning blob failed: {str(error)}")
+
+    def __attempt_upload_dataset(self, directory, order_id=None, dataset_id=None, callback=None):
+        """Upload a dataset to the server
+
+        :param str directory: Path to dataset folder to be uploaded.
+        :param str order_id: Base64 order_id
+        :param str dataset_id: Base64 dataset_id
+        :param str callback: Function to be called after every upload
+
+        :return: Upload status code.
+        """
+        try:
+            if isinstance(directory,str):
+                if not os.path.isdir(directory):
+                    raise Exception("Path not a directory") 
+            else:
+                raise Exception("Path must be a string") 
+
+            if order_id is None:
+                order_id = self.order_id
+
+            if dataset_id is None:
+                dataset_id = self.__generate_unique_uuid()
+
+            zip_builder_object = {} # Object of chunks, each value is an array of files
+
+            # Calculate number of files in the directory
+            total_files = 0 
+            for dirpath, _, filenames in os.walk(directory):
+                for filename in filenames:
+                    file_path = os.path.join(dirpath, filename) # Get full file path
+                    if os.path.isfile(file_path):
+                        total_files += 1
+
+            files_processed = 0
+
+            max_zip_size = 250000000 # Max size of zip file (25 MB)
+            total_parts = 0 # Counts total parts the dataset is divided into
+            cur_zip_size = 0 # Counts size of current zip file
+            zip_index = 0 # Counts index of zip file
+
+            for dirpath, _, filenames in os.walk(directory):
+                for filename in filenames:
+                    file_path = os.path.join(dirpath, filename) # Get full file path
+                    # Throw error if not a file
+                    if not os.path.isfile(file_path):
+                        raise Exception(f"Object {file_path} is not a file.")
+
+                    cur_zip_size += os.path.getsize(file_path) # Increment current file set size
+
+                    # Create list at zipIndex if it does not already exist
+                    if zip_index not in zip_builder_object:
+                        zip_builder_object[zip_index] = []
+                        total_parts += 1
+
+                
+                    # Push file to the list at zipIndex 
+                    zip_builder_object[zip_index].append({"filename": filename, "path": file_path})
+
+                    # If current chunk size is larger than max, start next chunk
+                    if cur_zip_size > max_zip_size:
+                        zip_index += 1
+                        cur_zip_size = 0
+
+                    files_processed += 1 # Increment number of processed files
+
+                    if callback is not None:
+                        # Calculate progress and round to two decimal places
+                        progress = (files_processed / total_files) * 100
+                        progress = round(progress, 2)
+
+                        # Ensure progress is exactly 100 if it's effectively 100
+                        progress = 100 if progress == 100.0 else progress
+                        callback({
+                            'dataset_id': dataset_id,
+                            'progress': progress,
+                            'status': "Preprocessing"
+                        })
+
+            # Start zipping and uploading each chunk
+            for chunk in zip_builder_object:
+                # Get upload_id for this chunk
+                upload_id = self.__new_multipart_upload(dataset_id, chunk, order_id)
+
+                # BytesIO object to hold the ZIP file in memory
+                zip_buffer = io.BytesIO()
+
+                # Create a write stream into the zip file
+                with zipfile.ZipFile(zip_buffer, 'w', zipfile.ZIP_DEFLATED) as zip_file:
+                    cur_chunk = zip_builder_object[chunk]
+                    # For each file in the chunk, add to zip buffer
+                    for file in range(len(cur_chunk)):
+                        filename = cur_chunk[file]['filename']
+                        path = cur_chunk[file]['path']
+                        file_contents = self.__read_file_contents(path)
+                        zip_file.writestr(filename, file_contents)
+                        # Call progress callback
+                        if callback is not None:
+                            # Calculate progress and round to two decimal places
+                            progress = ((file+1) / len(cur_chunk)) * 100
+                            progress = round(progress, 2)
+
+                            # Ensure progress is exactly 100 if it's effectively 100
+                            progress = 100 if progress == 100.0 else progress
+                            callback({
+                                'dataset_id': dataset_id,
+                                'progress': progress,
+                                'status': f"Compressing part {chunk+1}/{total_parts}"
+                            })
+
+                # Seek to the beginning of the BytesIO object before reading
+                zip_buffer.seek(0)
+
+                # Get zip file contents in memory
+                zip_file_contents = zip_buffer.getvalue()
+
+                part_size = 5 * 1024 * 1024 # 5MB minimum part size
+
+                # Break zip contents into chunks of part_size
+                zip_parts = self.__split_zip_contents(zip_file_contents, part_size)
+
+                final_parts = [] # Holds part details for complete multi upload
+
+                for up in range(len(zip_parts)):
+                    e_tag = self.__upload_part(upload_id, dataset_id, chunk, order_id, up+1, zip_parts[up])
+
+                    final_parts.append({'PartNumber': up+1, 'ETag': e_tag})
+
+                    # Call progress callback
+                    if callback is not None:
+                        # Calculate progress and round to two decimal places
+                        progress = ((up+1) / len(zip_parts)) * 100
+                        progress = round(progress, 2)
+
+                        # Ensure progress is exactly 100 if it's effectively 100
+                        progress = 100 if progress == 100.0 else progress
+                        callback({
+                            'dataset_id': dataset_id,
+                            'progress': progress,
+                            'status': f"Uploading part {chunk+1}/{total_parts}"
+                        })
+
+                self.__complete_multipart_upload(order_id, dataset_id, str(chunk), upload_id, final_parts)
+
+            return 201
+
+        except Exception as e:
+           raise Exception(f"Dataset upload failed: {str(e)}")
+
+    def __split_array(self, array, part_size):
+        """
+        Split array into part_size pieces for processing.
+        
+        :param str array List to be split
+        :param int part_size Size of each chunk
+
+        :return: List of chunks
+        """
+        if part_size <= 0:
+            raise ValueError("Chunk size must be greater than 0")
+
+        result = []
+        for i in range(0, len(array), part_size):
+            chunk = array[i:i + part_size]
+            result.append(chunk)
+        return result
+
+    # Public Methods
 
     def get_public_key(self, server_url=None):
         """Retrieve public key from server.
 
         :param str server_url: Server URL of Neuropacs instance
 
         :return: Base64 string public key.
@@ -197,24 +520,21 @@
         if server_url is None:
             server_url = self.server_url
 
         try:
             res = requests.get(f"{server_url}/api/getPubKey")
 
             if not res.ok:
-                raise Exception({"neuropacsError": f"{res.text}"})
+                raise Exception(json.loads(res.text)["error"])
 
             json = res.json()
             pub_key = json['pub_key']
             return pub_key
         except Exception as e:
-            if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
-                raise Exception(e.args[0]['neuropacsError']) 
-            else:
-                raise Exception("Public key retrieval failed.")
+            raise Exception(f"Public key retrieval failed: {str(e)}")
             
             
     def connect(self):
         """Create a connection with the server
 
         :param str client: Client source (default = 'api')
 
@@ -237,283 +557,143 @@
             }
 
             encrypted_body = self.__oaep_encrypt(body)
 
             res = requests.post(f"{self.server_url}/api/connect/", data=encrypted_body, headers=headers)
 
             if not res.ok:
-                raise Exception({"neuropacsError": f"{res.text}"})
+                raise Exception(json.loads(res.text)["error"])
 
             json = res.json()
             connection_id = json["connectionID"]
             self.connection_id = connection_id
             current_datetime = datetime.now()
             formatted_datetime = current_datetime.strftime("%Y-%m-%d %H:%M:%S")
             return {
                 "timestamp": formatted_datetime + " UTC",
                 "connection_id": connection_id,
                 "aes_key": aes_key,
             }
         except Exception as e:
-            if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
-                raise Exception(e.args[0]['neuropacsError']) 
-            else:
-                raise Exception("Connection failed.")
+            raise Exception(f"Connection creation failed: {str(e)}")
             
 
 
-    def upload_dataset(self, directory, order_id=None, connection_id=None, callback=None):
+    def upload_dataset(self, directory, order_id=None, dataset_id=None, callback=None):
         """Upload a dataset to the server
 
         :param str directory: Path to dataset folder to be uploaded.
         :param str order_id: Base64 order_id
-        :param str connection_id: Base64 connection_id
+        :param str dataset_id: Base64 dataset_id
         :param str callback: Function to be called after every upload
 
         :return: Upload status code.
         """
-        if order_id is None:
-            order_id = self.order_id
-
-        if connection_id is None:
-            connection_id = self.connection_id
-
         try:
-            self.dataset_upload = True
-            
-            if isinstance(directory,str):
-                if not os.path.isdir(directory):
-                    raise Exception({"neuropacsError": "Path not a directory!"}) 
-            else:
-                raise Exception({"neuropacsError": "Path must be a string!"}) 
-
-            dataset_id = self.__generate_filename()
-
-            total_files = sum(len(filenames) for _, _, filenames in os.walk(directory))
-
-            files_uploaded = 0
-
-            with tqdm(total=total_files, desc="Uploading", unit="file") as prog_bar:
-                for dirpath, _, filenames in os.walk(directory):
-                    for filename in filenames:
-                        file_path = os.path.join(dirpath, filename)
-                        status = self.upload(file_path, dataset_id, order_id, connection_id)
-                        if status != 201:
-                            if callback is not None:
-                               callback({
-                                'datasetId': dataset_id,
-                                'progress': -1,
-                                }) 
-                            raise Exception({"neuropacsError": "Upload failed!"})
-                        files_uploaded += 1
-                        if callback is not None:
-                            # Calculate progress and round to two decimal places
-                            progress = (files_uploaded / total_files) * 100
-                            progress = round(progress, 2)
-
-                            # Ensure progress is exactly 100 if it's effectively 100
-                            progress = 100 if progress == 100.0 else progress
-                            callback({
-                                'datasetId': dataset_id,
-                                'progress': progress,
-                                'filesUploaded': files_uploaded
-                            })
-                        
-                        prog_bar.update(1)  # Update the outer progress bar for each file
-            
-            return dataset_id
-
+            # Attempt upload
+            result = self.__attempt_upload_dataset(directory, order_id, dataset_id, callback)
+            # Return result
+            return result
         except Exception as e:
-            if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
-                raise Exception(e.args[0]['neuropacsError']) 
-            else:
-                raise Exception("Dataset upload failed.")
+            raise Exception(f"Dataset upload failed: {str(e)}")
 
 
-    def upload(self, data, dataset_id, order_id=None, connection_id=None):
-        """Upload a file to the server
+    def validate_upload(self, directory, dataset_id, order_id=None, callback=None):
+        """
+        Validate dataset upload
 
-        :param str/bytes data: Path of file to be uploaded or byte array
+        :param list directory Path to dataset
         :param str dataset_id Base64 dataset_id
-        :param str order_id: Base64 order_id 
-        :param str connection_id: Base64 connection_id
+        :param str order_id Base64 order_id
 
-        :return: Upload status code.
+        :returns List of missing files
         """
+        try:
+            if order_id is None:
+                order_id = self.order_id
 
-        # if not self.dataset_upload:
-
-        if order_id is None:
-            order_id = self.order_id
-
-        if connection_id is None:
-            connection_id = self.connection_id
-
-        # get file name
-        filename = ""
-        if isinstance(data,bytes):
-            filename = self.__generate_filename()
-        elif isinstance(data,str):
-            if os.path.isfile(data):
-                normalized_path = os.path.normpath(data)
-                directories = normalized_path.split(os.sep)
-                filename = directories[-1]
-            else:
-                raise Exception({"neuropacsError": "Path not a file!"})
-        else:
-            raise Exception({"neuropacsError": "Unsupported data type!"})
-
-        # encrypt order ID
-        encrypted_order_id = self.__encrypt_aes_ctr(order_id, "string", "string")
-
-        # create headers
-        headers = {"Content-Type": "application/octet-stream",'connection-id': connection_id, 'client': self.client, 'order-id': encrypted_order_id, 'filename': filename, 'dataset-id': dataset_id}
-
-        # get s3 upload params
-        res = requests.get(f"{self.server_url}/api/uploadRequest/", headers=headers)
-
-        if not res.ok:
-            raise Exception({"neuropacsError": f"{res.text}"})
-
-        decrypted_s3_info = self.__decrypt_aes_ctr(res.text, "json")
-
-        presigned_url = decrypted_s3_info["presignedURL"]
-
-        form = {
-            "Content-Disposition": "form-data",
-            "filename": filename,
-            "name":"test123"
-        }
-
-        BOUNDARY = "neuropacs----------"
-        DELIM = ";"
-        CRLF = "\r\n"
-        SEPARATOR="--"+BOUNDARY+CRLF
-        END="--"+BOUNDARY+"--"+CRLF
-        CONTENT_TYPE = "Content-Type: application/octet-stream"
-
-        header = SEPARATOR
-        for key, value in form.items():
-            header += f"{key}: {value}"
-            header += DELIM
-        header += CRLF
-        header += CONTENT_TYPE
-        header += CRLF + CRLF
-
-        header_bytes = header.encode("utf-8")
-
-        footer_bytes = END.encode("utf-8")
+            file_list = []
 
-        encrypted_order_id = self.__encrypt_aes_ctr(order_id, "string", "string")
+            for dirpath, _, filenames in os.walk(directory):
+                for filename in filenames:
+                    file_path = os.path.join(dirpath, filename) # Get full file path
+                    size = os.path.getsize(file_path)
+                    file_list.append({'name': filename, 'size': size})
 
-        payload_data = None
+            validation_parts = self.__split_array(file_list, 100)
 
-        if isinstance(data, bytes):
-            # encrypted_binary_data = self.__encrypt_aes_ctr(data, "bytes","bytes")
-            payload_data = header_bytes + data + footer_bytes
+            encrypted_order_id = self.__encrypt_aes_ctr(order_id, "string", "string")
         
-        elif isinstance(data,str):
-            with open(data, 'rb') as f:
-                binary_data = f.read()
-                # encrypted_binary_data = self.__encrypt_aes_ctr(binary_data, "bytes","bytes")
-                payload_data = header_bytes + binary_data + footer_bytes
-
+            headers = {'Content-type': 'text/plain', 'connection-id': self.connection_id, 'dataset-id': dataset_id,'order-id': encrypted_order_id, 'client': self.client}
 
-        res = requests.put(presigned_url, data=payload_data)
+            total_validated = 0 # Total files validated
 
-        if not res.ok:
-            raise Exception({"neuropacsError": f"{res.text}"})
-
-        return 201
-
-    def validate_upload(self, file_array, dataset_id, order_id=None, connection_id=None):
-        """
-        Validate dataset upload
-        """
-        if connection_id is None:
-            connection_id = self.connection_id
-        if order_id is None:
-            order_id = self.order_id
-        try:
-            encrypted_order_id = self.__encrypt_aes_ctr(order_id, "string", "string")
-        
-            headers = {'Content-type': 'text/plain', 'connection-id': connection_id, 'dataset-id': dataset_id,'order-id': encrypted_order_id, 'client': self.client}
+            total_missing_files = [] # Store list of missing files
 
-            body = {
-                'fileArray': file_array,
-            }
+            for val in range(len(validation_parts)):
+                body = {
+                    'fileMetadata': validation_parts[val],
+                }
 
-            encrypted_body = self.__encrypt_aes_ctr(body, "json", "string")
+                encrypted_body = self.__encrypt_aes_ctr(body, "json", "string")
 
-            res = requests.post(f"{self.server_url}/api/verifyUpload/", data=encrypted_body, headers=headers)
+                res = requests.post(f"{self.server_url}/api/verifyUpload/", data=encrypted_body, headers=headers)
             
-            if not res.ok:
-                raise Exception({"neuropacsError": f"{res.text}"})
+                if not res.ok:
+                    raise Exception(json.loads(res.text)["error"])
 
-            text = res.text
-            decrypted_dataset_validation = self.__decrypt_aes_ctr(text, "string")
-            return decrypted_dataset_validation
+                text = res.text
+                decrypted_dataset_validation = self.__decrypt_aes_ctr(text, "json")
+                total_missing_files = total_missing_files + decrypted_dataset_validation['missingFiles']
+                total_validated += len(validation_parts[val])
 
-        except Exception as e:
-            if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
-                raise Exception(e.args[0]['neuropacsError'])
-            else:
-                raise Exception(f"Result retrieval failed!")
-        
+            return {'missingFiles': total_missing_files}
 
+        except Exception as e:
+            raise Exception(f"Upload validation failed: {str(e)}")
 
 
-    def new_job (self, connection_id=None):
+    def new_job (self):
         """Create a new order
 
-        :param str connection_id: Base64 connection_id
-
         :return: Base64 string order_id.
         """
-
-        if connection_id is None:
-            connection_id = self.connection_id
-
         try:
-            headers = {'Content-type': 'text/plain', 'connection-id': connection_id, 'client': self.client}
+            headers = {'Content-type': 'text/plain', 'connection-id': self.connection_id, 'client': self.client}
 
             res = requests.post(f"{self.server_url}/api/newJob/", headers=headers)
 
             if not res.ok:
-                raise Exception({"neuropacsError": f"{res.text}"})
+                raise Exception(json.loads(res.text)["error"])
 
             text = res.text
             decrypted_text = self.__decrypt_aes_ctr(text, "string")
             self.order_id = decrypted_text
             return decrypted_text
         except Exception as e:
-            if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
-                raise Exception(e.args[0]['neuropacsError'])
-            else:
-                raise Exception("Job creation failed.")            
+            raise Exception(f"Job creation failed: {str(e)}")
+           
 
 
-    def run_job(self, product_id, order_id=None, dataset_id=None, connection_id=None):
+    def run_job(self, product_id, order_id=None, dataset_id=None):
         """Run a job
         
         :param str productID: Product to be executed.
         :prarm str order_id: Base64 order_id 
         :prarm str dataset_id: Base64 dataset_id 
-        :param str connection_id: Base64 connection_id
         
         :return: Job run status code.
         """
-        if order_id == None:
-            order_id = self.order_id
-
-        if connection_id is None:
-            connection_id = self.connection_id
 
         try:
-            headers = {'Content-type': 'text/plain', 'connection-id': connection_id, 'client': self.client}
+
+            if order_id == None:
+                order_id = self.order_id
+                
+            headers = {'Content-type': 'text/plain', 'connection-id': self.connection_id, 'client': self.client}
 
             body={}
             if dataset_id is None:
                 body = {
                     'orderID': order_id,
                     'productID': product_id,
                 }
@@ -525,43 +705,37 @@
                 }
 
             encryptedBody = self.__encrypt_aes_ctr(body, "json", "string")
 
             res = requests.post(f"{self.server_url}/api/runJob/", data=encryptedBody, headers=headers)
             
             if not res.ok:
-                raise Exception({"neuropacsError": f"{res.text}"})
+                raise Exception(json.loads(res.text)["error"])
 
             return res.status_code
                 
         except Exception as e:
-            if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
-                raise Exception(e.args[0]['neuropacsError'])
-            else:
-                raise Exception("Job run failed.")  
+            raise Exception(f"Job run failed: {str(e)}")
+  
 
 
-    def check_status(self, order_id=None, dataset_id=None, connection_id=None):
+    def check_status(self, order_id=None, dataset_id=None):
         """Check job status
 
         :param str order_id: Base64 order_id (optional)
         :param str dataset_id: Base64 dataset_id (optional)
-        :param str connection_id: Base64 connection_id
 
         :return: Job status message.
         """
         if order_id is None:
             order_id = self.order_id
 
-        if connection_id is None:
-            connection_id = self.connection_id
-
         try:
 
-            headers = {'Content-type': 'text/plain', 'connection-id': connection_id, 'client': self.client}
+            headers = {'Content-type': 'text/plain', 'connection-id': self.connection_id, 'client': self.client}
 
             if dataset_id is not None:
                 body = {
                     'orderID': order_id,
                     'datasetID': dataset_id
                 }
             else:
@@ -570,46 +744,38 @@
                 }
 
             encryptedBody = self.__encrypt_aes_ctr(body, "json", "string")
 
             res = requests.post(f"{self.server_url}/api/checkStatus/", data=encryptedBody, headers=headers)
             
             if not res.ok:
-                raise Exception({"neuropacsError": f"{res.text}"})
+                raise Exception(json.loads(res.text)["error"])
             
             text = res.text
             json = self.__decrypt_aes_ctr(text, "json")
             return json
             
         except Exception as e:
-            if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
-                raise Exception(e.args[0]['neuropacsError'])
-            else:
-                raise Exception("Status check failed.")  
+            raise Exception(f"Status check failed: {str(e)}")
+ 
 
 
-    def get_results(self, format, order_id=None, dataset_id=None, connection_id=None):
+    def get_results(self, format, order_id=None, dataset_id=None):
         """Get job results
 
         :param str format: Format of file data
         :prarm str order_id: Base64 order_id (optional)
-        :param str connection_id: Base64 connection_id
 
         :return: AES encrypted file data in specified format
         """
-
-        if order_id is None:
-            order_id = self.order_id
-
-        if connection_id is None:
-            connection_id = self.connection_id
-        
         try:
-        
-            headers = {'Content-type': 'text/plain', 'connection-id': connection_id, 'client': self.client}
+            if order_id is None:
+                order_id = self.order_id
+
+            headers = {'Content-type': 'text/plain', 'connection-id': self.connection_id, 'client': self.client}
 
             if dataset_id is not None:
                 body = {
                     'orderID': order_id,
                     'format': format,
                     'datasetID': dataset_id
                 }
@@ -618,28 +784,26 @@
                     'orderID': order_id,
                     'format': format               
                 }
 
             validFormats = ["TXT", "XML", "JSON", "PDF", "DCM"]
 
             if format not in validFormats:
-                raise Exception({"neuropacsError" : "Invalid format! Valid formats include: \"TXT\", \"JSON\", \"XML\", \"PDF\", \"DCM\" ."})
+                raise Exception("Invalid format! Valid formats include: \"TXT\", \"JSON\", \"XML\", \"PDF\", \"DCM\" .")
 
             encrypted_body = self.__encrypt_aes_ctr(body, "json", "string")
 
             res = requests.post(f"{self.server_url}/api/getResults/", data=encrypted_body, headers=headers)
             
             if not res.ok:
-                raise Exception({"neuropacsError": f"{res.text}"})
+                raise Exception(json.loads(res.text)["error"])
 
             text = res.text
             decrypted_file_data = self.__decrypt_aes_ctr(text, "string")
             return decrypted_file_data
 
         except Exception as e:
-            if(isinstance(e.args[0], dict) and 'neuropacsError' in e.args[0]):
-                raise Exception(e.args[0]['neuropacsError'])
-            else:
-                raise Exception(f"Result retrieval failed!")
+            raise Exception(f"Result retrieval failed: {str(e)}")
+
```

### Comparing `neuropacs-1.6.6/neuropacs.egg-info/PKG-INFO` & `neuropacs-1.6.7/neuropacs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuropacs
-Version: 1.6.6
+Version: 1.6.7
 Summary: NeuroPACS Python SDK
 Home-page: https://github.com/neuropacs/neuropacs-py-sdk
 Author: Kerrick Cavanaugh
 Author-email: kerrick@neuropacs.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `neuropacs-1.6.6/setup.py` & `neuropacs-1.6.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='neuropacs',
-    version='1.6.6',
+    version='1.6.7',
     description='NeuroPACS Python SDK',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Kerrick Cavanaugh',
     author_email='kerrick@neuropacs.com',
     url='https://github.com/neuropacs/neuropacs-py-sdk',
     packages=find_packages(),
```

### Comparing `neuropacs-1.6.6/tests/tests_neuropacs.py` & `neuropacs-1.6.7/tests/tests_neuropacs.py`

 * *Files identical despite different names*

