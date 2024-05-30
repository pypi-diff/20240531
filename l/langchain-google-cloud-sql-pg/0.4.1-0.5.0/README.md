# Comparing `tmp/langchain_google_cloud_sql_pg-0.4.1-py3-none-any.whl.zip` & `tmp/langchain_google_cloud_sql_pg-0.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 29746 bytes, number of entries: 13
--rw-r--r--  2.0 unx     1034 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/__init__.py
--rw-r--r--  2.0 unx     4964 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/chat_message_history.py
--rw-r--r--  2.0 unx    14707 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/engine.py
--rw-r--r--  2.0 unx     2580 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/indexes.py
--rw-r--r--  2.0 unx    17740 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/loader.py
--rw-rw-r--  2.0 unx        0 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/py.typed
--rw-r--r--  2.0 unx    29576 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/vectorstore.py
--rw-r--r--  2.0 unx      622 b- defN 24-May-02 22:28 langchain_google_cloud_sql_pg/version.py
--rw-rw-r--  2.0 unx    11358 b- defN 24-May-02 22:30 langchain_google_cloud_sql_pg-0.4.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    20359 b- defN 24-May-02 22:30 langchain_google_cloud_sql_pg-0.4.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-02 22:30 langchain_google_cloud_sql_pg-0.4.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       30 b- defN 24-May-02 22:30 langchain_google_cloud_sql_pg-0.4.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1287 b- defN 24-May-02 22:30 langchain_google_cloud_sql_pg-0.4.1.dist-info/RECORD
-13 files, 104349 bytes uncompressed, 27530 bytes compressed:  73.6%
+Zip file size: 29767 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1034 b- defN 24-May-30 22:27 langchain_google_cloud_sql_pg/__init__.py
+-rw-r--r--  2.0 unx     4964 b- defN 24-May-30 22:27 langchain_google_cloud_sql_pg/chat_message_history.py
+-rw-r--r--  2.0 unx    14707 b- defN 24-May-30 22:27 langchain_google_cloud_sql_pg/engine.py
+-rw-r--r--  2.0 unx     2580 b- defN 24-May-30 22:27 langchain_google_cloud_sql_pg/indexes.py
+-rw-r--r--  2.0 unx    17740 b- defN 24-May-30 22:27 langchain_google_cloud_sql_pg/loader.py
+-rw-rw-r--  2.0 unx        0 b- defN 24-May-30 22:27 langchain_google_cloud_sql_pg/py.typed
+-rw-r--r--  2.0 unx    29576 b- defN 24-May-30 22:27 langchain_google_cloud_sql_pg/vectorstore.py
+-rw-r--r--  2.0 unx      622 b- defN 24-May-30 22:27 langchain_google_cloud_sql_pg/version.py
+-rw-rw-r--  2.0 unx    11358 b- defN 24-May-30 22:29 langchain_google_cloud_sql_pg-0.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    20487 b- defN 24-May-30 22:29 langchain_google_cloud_sql_pg-0.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 22:29 langchain_google_cloud_sql_pg-0.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       30 b- defN 24-May-30 22:29 langchain_google_cloud_sql_pg-0.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1287 b- defN 24-May-30 22:29 langchain_google_cloud_sql_pg-0.5.0.dist-info/RECORD
+13 files, 104477 bytes uncompressed, 27551 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: langchain_google_cloud_sql_pg/vectorstore.py
 Comment: 
 
 Filename: langchain_google_cloud_sql_pg/version.py
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.4.1.dist-info/LICENSE
+Filename: langchain_google_cloud_sql_pg-0.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.4.1.dist-info/METADATA
+Filename: langchain_google_cloud_sql_pg-0.5.0.dist-info/METADATA
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.4.1.dist-info/WHEEL
+Filename: langchain_google_cloud_sql_pg-0.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.4.1.dist-info/top_level.txt
+Filename: langchain_google_cloud_sql_pg-0.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: langchain_google_cloud_sql_pg-0.4.1.dist-info/RECORD
+Filename: langchain_google_cloud_sql_pg-0.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langchain_google_cloud_sql_pg/version.py

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.4.1"
+__version__ = "0.5.0"
```

## Comparing `langchain_google_cloud_sql_pg-0.4.1.dist-info/LICENSE` & `langchain_google_cloud_sql_pg-0.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langchain_google_cloud_sql_pg-0.4.1.dist-info/METADATA` & `langchain_google_cloud_sql_pg-0.5.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-google-cloud-sql-pg
-Version: 0.4.1
+Version: 0.5.0
 Summary: LangChain integrations for Google Cloud SQL for PostgreSQL
 Author-email: Google LLC <googleapis-packages@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -219,25 +219,27 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: cloud-sql-python-connector[asyncpg] <2.0.0,>=1.7.0
-Requires-Dist: langchain-core <2.0.0,>=0.1.1
-Requires-Dist: langchain-community <0.1.0,>=0.0.18
-Requires-Dist: numpy <2.0.0,>=1.24.4
+Requires-Dist: langchain-core <1.0.0,>=0.1.1
+Requires-Dist: langchain-community <0.3.0,>=0.0.18
 Requires-Dist: pgvector <1.0.0,>=0.2.5
 Requires-Dist: SQLAlchemy[asyncio] <3.0.0,>=2.0.25
+Requires-Dist: numpy ==1.24.4 ; python_version <= "3.8"
+Requires-Dist: numpy <2.0.0,>=1.24.4 ; python_version > "3.8"
 Provides-Extra: test
 Requires-Dist: black[jupyter] ==23.12.1 ; extra == 'test'
 Requires-Dist: isort ==5.13.2 ; extra == 'test'
-Requires-Dist: mypy ==1.9.0 ; extra == 'test'
-Requires-Dist: pytest-asyncio ==0.23.5.post1 ; extra == 'test'
+Requires-Dist: mypy ==1.10.0 ; extra == 'test'
+Requires-Dist: pytest-asyncio ==0.23.7 ; extra == 'test'
 Requires-Dist: pytest ==7.4.4 ; extra == 'test'
+Requires-Dist: pytest-cov ==5.0.0 ; extra == 'test'
 
 Cloud SQL for PostgreSQL for LangChain
 ===================================================================
 
 |preview| |pypi| |versions|
 
 - `Client Library Documentation`_
```

## Comparing `langchain_google_cloud_sql_pg-0.4.1.dist-info/RECORD` & `langchain_google_cloud_sql_pg-0.5.0.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 langchain_google_cloud_sql_pg/__init__.py,sha256=7sz60HhKzCg_1f3mrLbyYgnAkjvhMo3xKt9S_bm1A0A,1034
 langchain_google_cloud_sql_pg/chat_message_history.py,sha256=P5tDXVUF7o_yLNAMQ7VTzmKmIBR74FDs6DTI-Jh7BEg,4964
 langchain_google_cloud_sql_pg/engine.py,sha256=BAQQbsIlUQ2IxMMsO1_YtBmgYpTJfjTCE4lmbV0wmvk,14707
 langchain_google_cloud_sql_pg/indexes.py,sha256=UYbXMcZXBvaU7FFa7IjhXvBvCuDdxr0Tq2pgyQrKVtU,2580
 langchain_google_cloud_sql_pg/loader.py,sha256=G2yI3QiS2mHxYSUgVIQPDhgCBw1-ARlCvLZJrEQt-HM,17740
 langchain_google_cloud_sql_pg/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 langchain_google_cloud_sql_pg/vectorstore.py,sha256=-zKkgpoAGTfF7y3tbS0AxihF6UW_uDjd5Rzoxp2KD3g,29576
-langchain_google_cloud_sql_pg/version.py,sha256=lyhj8ZqCp_c181C39EsQQ0JVsjJhyv5RVg17Lp_sKdg,622
-langchain_google_cloud_sql_pg-0.4.1.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
-langchain_google_cloud_sql_pg-0.4.1.dist-info/METADATA,sha256=vUCL_7shfxeje30eNUxid_OkcU3pnAOc4LkDvuePxek,20359
-langchain_google_cloud_sql_pg-0.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-langchain_google_cloud_sql_pg-0.4.1.dist-info/top_level.txt,sha256=B0E28f-0MRQQTiqWKALorDWbFG2scm-DwzRuYdQHOOA,30
-langchain_google_cloud_sql_pg-0.4.1.dist-info/RECORD,,
+langchain_google_cloud_sql_pg/version.py,sha256=FPR3qm-o4U8nIoNrHLeO8j63tJ3wLkpc_KQRC-B3foE,622
+langchain_google_cloud_sql_pg-0.5.0.dist-info/LICENSE,sha256=z8d0m5b2O9McPEK1xHG_dWgUBT6EfBDz6wA0F7xSPTA,11358
+langchain_google_cloud_sql_pg-0.5.0.dist-info/METADATA,sha256=eljT4ayBwEKbq65BapYrQdQ5Ndb9VOapTxBCaUuHAoI,20487
+langchain_google_cloud_sql_pg-0.5.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+langchain_google_cloud_sql_pg-0.5.0.dist-info/top_level.txt,sha256=B0E28f-0MRQQTiqWKALorDWbFG2scm-DwzRuYdQHOOA,30
+langchain_google_cloud_sql_pg-0.5.0.dist-info/RECORD,,
```

