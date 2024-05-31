# Comparing `tmp/alibabacloud_emr-serverless-spark20230808-1.3.0.tar.gz` & `tmp/alibabacloud_emr-serverless-spark20230808-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_emr-serverless-spark20230808-1.3.0.tar", last modified: Wed May 22 17:10:55 2024, max compression
+gzip compressed data, was "dist/alibabacloud_emr-serverless-spark20230808-1.4.0.tar", last modified: Fri May 31 17:08:31 2024, max compression
```

## Comparing `alibabacloud_emr-serverless-spark20230808-1.3.0.tar` & `alibabacloud_emr-serverless-spark20230808-1.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/
--rw-r--r--   0 root         (0) root         (0)      669 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2520 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1163 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1248 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/alibabacloud_emr_serverless_spark20230808/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/alibabacloud_emr_serverless_spark20230808/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50860 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/alibabacloud_emr_serverless_spark20230808/client.py
--rw-r--r--   0 root         (0) root         (0)   136144 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/alibabacloud_emr_serverless_spark20230808/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/alibabacloud_emr_serverless_spark20230808.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2520 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/alibabacloud_emr_serverless_spark20230808.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      556 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/alibabacloud_emr_serverless_spark20230808.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/alibabacloud_emr_serverless_spark20230808.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/alibabacloud_emr_serverless_spark20230808.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/alibabacloud_emr_serverless_spark20230808.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2700 2024-05-22 17:10:55.000000 alibabacloud_emr-serverless-spark20230808-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)      755 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1163 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1248 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/alibabacloud_emr_serverless_spark20230808/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/alibabacloud_emr_serverless_spark20230808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65250 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/alibabacloud_emr_serverless_spark20230808/client.py
+-rw-r--r--   0 root         (0) root         (0)   150930 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/alibabacloud_emr_serverless_spark20230808/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/alibabacloud_emr_serverless_spark20230808.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2520 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/alibabacloud_emr_serverless_spark20230808.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      556 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/alibabacloud_emr_serverless_spark20230808.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/alibabacloud_emr_serverless_spark20230808.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/alibabacloud_emr_serverless_spark20230808.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/alibabacloud_emr_serverless_spark20230808.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2700 2024-05-31 17:08:31.000000 alibabacloud_emr-serverless-spark20230808-1.4.0/setup.py
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.3.0/ChangeLog.md` & `alibabacloud_emr-serverless-spark20230808-1.4.0/ChangeLog.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+2024-05-22 Version: 1.3.0
+- Support API AddMembers.
+- Support API GrantRoleToUsers.
+
+
 2024-05-21 Version: 1.2.0
 - Support API ListSessionClusters.
 
 
 2024-05-21 Version: 1.2.0
 - Support API ListSessionClusters.
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.3.0/LICENSE` & `alibabacloud_emr-serverless-spark20230808-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr-serverless-spark20230808-1.3.0/PKG-INFO` & `alibabacloud_emr-serverless-spark20230808-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_emr-serverless-spark20230808
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud emr-serverless-spark (20230808) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.3.0/README-CN.md` & `alibabacloud_emr-serverless-spark20230808-1.4.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr-serverless-spark20230808-1.3.0/README.md` & `alibabacloud_emr-serverless-spark20230808-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr-serverless-spark20230808-1.3.0/alibabacloud_emr_serverless_spark20230808/client.py` & `alibabacloud_emr-serverless-spark20230808-1.4.0/alibabacloud_emr_serverless_spark20230808/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -265,14 +265,146 @@
         @param request: CancelJobRunRequest
         @return: CancelJobRunResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.cancel_job_run_with_options_async(workspace_id, job_run_id, request, headers, runtime)
 
+    def create_sql_statement_with_options(
+        self,
+        workspace_id: str,
+        request: emr_serverless_spark_20230808_models.CreateSqlStatementRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_serverless_spark_20230808_models.CreateSqlStatementResponse:
+        """
+        @summary 使用session运行SQL
+        
+        @param request: CreateSqlStatementRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateSqlStatementResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        body = {}
+        if not UtilClient.is_unset(request.code_content):
+            body['codeContent'] = request.code_content
+        if not UtilClient.is_unset(request.default_catalog):
+            body['defaultCatalog'] = request.default_catalog
+        if not UtilClient.is_unset(request.default_database):
+            body['defaultDatabase'] = request.default_database
+        if not UtilClient.is_unset(request.limit):
+            body['limit'] = request.limit
+        if not UtilClient.is_unset(request.sql_compute_id):
+            body['sqlComputeId'] = request.sql_compute_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateSqlStatement',
+            version='2023-08-08',
+            protocol='HTTPS',
+            pathname=f'/api/interactive/v1/workspace/{OpenApiUtilClient.get_encode_param(workspace_id)}/statement',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_serverless_spark_20230808_models.CreateSqlStatementResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def create_sql_statement_with_options_async(
+        self,
+        workspace_id: str,
+        request: emr_serverless_spark_20230808_models.CreateSqlStatementRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_serverless_spark_20230808_models.CreateSqlStatementResponse:
+        """
+        @summary 使用session运行SQL
+        
+        @param request: CreateSqlStatementRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: CreateSqlStatementResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        body = {}
+        if not UtilClient.is_unset(request.code_content):
+            body['codeContent'] = request.code_content
+        if not UtilClient.is_unset(request.default_catalog):
+            body['defaultCatalog'] = request.default_catalog
+        if not UtilClient.is_unset(request.default_database):
+            body['defaultDatabase'] = request.default_database
+        if not UtilClient.is_unset(request.limit):
+            body['limit'] = request.limit
+        if not UtilClient.is_unset(request.sql_compute_id):
+            body['sqlComputeId'] = request.sql_compute_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query),
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='CreateSqlStatement',
+            version='2023-08-08',
+            protocol='HTTPS',
+            pathname=f'/api/interactive/v1/workspace/{OpenApiUtilClient.get_encode_param(workspace_id)}/statement',
+            method='PUT',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_serverless_spark_20230808_models.CreateSqlStatementResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def create_sql_statement(
+        self,
+        workspace_id: str,
+        request: emr_serverless_spark_20230808_models.CreateSqlStatementRequest,
+    ) -> emr_serverless_spark_20230808_models.CreateSqlStatementResponse:
+        """
+        @summary 使用session运行SQL
+        
+        @param request: CreateSqlStatementRequest
+        @return: CreateSqlStatementResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.create_sql_statement_with_options(workspace_id, request, headers, runtime)
+
+    async def create_sql_statement_async(
+        self,
+        workspace_id: str,
+        request: emr_serverless_spark_20230808_models.CreateSqlStatementRequest,
+    ) -> emr_serverless_spark_20230808_models.CreateSqlStatementResponse:
+        """
+        @summary 使用session运行SQL
+        
+        @param request: CreateSqlStatementRequest
+        @return: CreateSqlStatementResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.create_sql_statement_with_options_async(workspace_id, request, headers, runtime)
+
     def get_job_run_with_options(
         self,
         workspace_id: str,
         job_run_id: str,
         request: emr_serverless_spark_20230808_models.GetJobRunRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
@@ -377,14 +509,126 @@
         @param request: GetJobRunRequest
         @return: GetJobRunResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_job_run_with_options_async(workspace_id, job_run_id, request, headers, runtime)
 
+    def get_sql_statement_with_options(
+        self,
+        workspace_id: str,
+        statement_id: str,
+        request: emr_serverless_spark_20230808_models.GetSqlStatementRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_serverless_spark_20230808_models.GetSqlStatementResponse:
+        """
+        @summary 获取Sql Statement状态
+        
+        @param request: GetSqlStatementRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSqlStatementResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetSqlStatement',
+            version='2023-08-08',
+            protocol='HTTPS',
+            pathname=f'/api/interactive/v1/workspace/{OpenApiUtilClient.get_encode_param(workspace_id)}/statement/{OpenApiUtilClient.get_encode_param(statement_id)}',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_serverless_spark_20230808_models.GetSqlStatementResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def get_sql_statement_with_options_async(
+        self,
+        workspace_id: str,
+        statement_id: str,
+        request: emr_serverless_spark_20230808_models.GetSqlStatementRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_serverless_spark_20230808_models.GetSqlStatementResponse:
+        """
+        @summary 获取Sql Statement状态
+        
+        @param request: GetSqlStatementRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSqlStatementResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='GetSqlStatement',
+            version='2023-08-08',
+            protocol='HTTPS',
+            pathname=f'/api/interactive/v1/workspace/{OpenApiUtilClient.get_encode_param(workspace_id)}/statement/{OpenApiUtilClient.get_encode_param(statement_id)}',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_serverless_spark_20230808_models.GetSqlStatementResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def get_sql_statement(
+        self,
+        workspace_id: str,
+        statement_id: str,
+        request: emr_serverless_spark_20230808_models.GetSqlStatementRequest,
+    ) -> emr_serverless_spark_20230808_models.GetSqlStatementResponse:
+        """
+        @summary 获取Sql Statement状态
+        
+        @param request: GetSqlStatementRequest
+        @return: GetSqlStatementResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.get_sql_statement_with_options(workspace_id, statement_id, request, headers, runtime)
+
+    async def get_sql_statement_async(
+        self,
+        workspace_id: str,
+        statement_id: str,
+        request: emr_serverless_spark_20230808_models.GetSqlStatementRequest,
+    ) -> emr_serverless_spark_20230808_models.GetSqlStatementResponse:
+        """
+        @summary 获取Sql Statement状态
+        
+        @param request: GetSqlStatementRequest
+        @return: GetSqlStatementResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.get_sql_statement_with_options_async(workspace_id, statement_id, request, headers, runtime)
+
     def grant_role_to_users_with_options(
         self,
         request: emr_serverless_spark_20230808_models.GrantRoleToUsersRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> emr_serverless_spark_20230808_models.GrantRoleToUsersResponse:
         """
@@ -524,14 +768,16 @@
         if not UtilClient.is_unset(tmp_req.tags):
             request.tags_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tags, 'tags', 'json')
         query = {}
         if not UtilClient.is_unset(request.creator):
             query['creator'] = request.creator
         if not UtilClient.is_unset(request.end_time_shrink):
             query['endTime'] = request.end_time_shrink
+        if not UtilClient.is_unset(request.job_run_deployment_id):
+            query['jobRunDeploymentId'] = request.job_run_deployment_id
         if not UtilClient.is_unset(request.job_run_id):
             query['jobRunId'] = request.job_run_id
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.name):
             query['name'] = request.name
         if not UtilClient.is_unset(request.next_token):
@@ -593,14 +839,16 @@
         if not UtilClient.is_unset(tmp_req.tags):
             request.tags_shrink = OpenApiUtilClient.array_to_string_with_specified_style(tmp_req.tags, 'tags', 'json')
         query = {}
         if not UtilClient.is_unset(request.creator):
             query['creator'] = request.creator
         if not UtilClient.is_unset(request.end_time_shrink):
             query['endTime'] = request.end_time_shrink
+        if not UtilClient.is_unset(request.job_run_deployment_id):
+            query['jobRunDeploymentId'] = request.job_run_deployment_id
         if not UtilClient.is_unset(request.job_run_id):
             query['jobRunId'] = request.job_run_id
         if not UtilClient.is_unset(request.max_results):
             query['maxResults'] = request.max_results
         if not UtilClient.is_unset(request.name):
             query['name'] = request.name
         if not UtilClient.is_unset(request.next_token):
@@ -1284,7 +1532,119 @@
         
         @param request: StartJobRunRequest
         @return: StartJobRunResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.start_job_run_with_options_async(workspace_id, request, headers, runtime)
+
+    def terminate_sql_statement_with_options(
+        self,
+        workspace_id: str,
+        statement_id: str,
+        request: emr_serverless_spark_20230808_models.TerminateSqlStatementRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_serverless_spark_20230808_models.TerminateSqlStatementResponse:
+        """
+        @summary 终止 session statement
+        
+        @param request: TerminateSqlStatementRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TerminateSqlStatementResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='TerminateSqlStatement',
+            version='2023-08-08',
+            protocol='HTTPS',
+            pathname=f'/api/interactive/v1/workspace/{OpenApiUtilClient.get_encode_param(workspace_id)}/statement/{OpenApiUtilClient.get_encode_param(statement_id)}/terminate',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_serverless_spark_20230808_models.TerminateSqlStatementResponse(),
+            self.call_api(params, req, runtime)
+        )
+
+    async def terminate_sql_statement_with_options_async(
+        self,
+        workspace_id: str,
+        statement_id: str,
+        request: emr_serverless_spark_20230808_models.TerminateSqlStatementRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> emr_serverless_spark_20230808_models.TerminateSqlStatementResponse:
+        """
+        @summary 终止 session statement
+        
+        @param request: TerminateSqlStatementRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TerminateSqlStatementResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.region_id):
+            query['regionId'] = request.region_id
+        req = open_api_models.OpenApiRequest(
+            headers=headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='TerminateSqlStatement',
+            version='2023-08-08',
+            protocol='HTTPS',
+            pathname=f'/api/interactive/v1/workspace/{OpenApiUtilClient.get_encode_param(workspace_id)}/statement/{OpenApiUtilClient.get_encode_param(statement_id)}/terminate',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='json',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            emr_serverless_spark_20230808_models.TerminateSqlStatementResponse(),
+            await self.call_api_async(params, req, runtime)
+        )
+
+    def terminate_sql_statement(
+        self,
+        workspace_id: str,
+        statement_id: str,
+        request: emr_serverless_spark_20230808_models.TerminateSqlStatementRequest,
+    ) -> emr_serverless_spark_20230808_models.TerminateSqlStatementResponse:
+        """
+        @summary 终止 session statement
+        
+        @param request: TerminateSqlStatementRequest
+        @return: TerminateSqlStatementResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.terminate_sql_statement_with_options(workspace_id, statement_id, request, headers, runtime)
+
+    async def terminate_sql_statement_async(
+        self,
+        workspace_id: str,
+        statement_id: str,
+        request: emr_serverless_spark_20230808_models.TerminateSqlStatementRequest,
+    ) -> emr_serverless_spark_20230808_models.TerminateSqlStatementResponse:
+        """
+        @summary 终止 session statement
+        
+        @param request: TerminateSqlStatementRequest
+        @return: TerminateSqlStatementResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.terminate_sql_statement_with_options_async(workspace_id, statement_id, request, headers, runtime)
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.3.0/alibabacloud_emr_serverless_spark20230808/models.py` & `alibabacloud_emr-serverless-spark20230808-1.4.0/alibabacloud_emr_serverless_spark20230808/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -750,35 +750,38 @@
         category_biz_id: str = None,
         content: str = None,
         creator: int = None,
         default_catalog_id: str = None,
         default_database: str = None,
         default_resource_queue_id: str = None,
         default_sql_compute_id: str = None,
+        deployment_id: str = None,
         extra_artifact_ids: List[str] = None,
         extra_spark_submit_params: str = None,
         files: List[str] = None,
         gmt_created: str = None,
         gmt_modified: str = None,
         has_changed: bool = None,
         has_commited: bool = None,
+        is_streaming: bool = None,
         jars: List[str] = None,
         last_run_resource_queue_id: str = None,
         modifier: int = None,
         name: str = None,
         py_files: List[str] = None,
         spark_args: str = None,
         spark_conf: List[SparkConf] = None,
         spark_driver_cores: int = None,
         spark_driver_memory: int = None,
         spark_entrypoint: str = None,
         spark_executor_cores: int = None,
         spark_executor_memory: int = None,
         spark_log_level: str = None,
         spark_log_path: str = None,
+        spark_submit_clause: str = None,
         spark_version: str = None,
         tags: Dict[str, str] = None,
         type: str = None,
     ):
         self.archives = archives
         self.artifact_url = artifact_url
         # This parameter is required.
@@ -787,24 +790,26 @@
         self.content = content
         # This parameter is required.
         self.creator = creator
         self.default_catalog_id = default_catalog_id
         self.default_database = default_database
         self.default_resource_queue_id = default_resource_queue_id
         self.default_sql_compute_id = default_sql_compute_id
+        self.deployment_id = deployment_id
         self.extra_artifact_ids = extra_artifact_ids
         self.extra_spark_submit_params = extra_spark_submit_params
         self.files = files
         # This parameter is required.
         self.gmt_created = gmt_created
         # This parameter is required.
         self.gmt_modified = gmt_modified
         self.has_changed = has_changed
         # This parameter is required.
         self.has_commited = has_commited
+        self.is_streaming = is_streaming
         self.jars = jars
         self.last_run_resource_queue_id = last_run_resource_queue_id
         # This parameter is required.
         self.modifier = modifier
         # This parameter is required.
         self.name = name
         self.py_files = py_files
@@ -819,14 +824,15 @@
         self.spark_executor_cores = spark_executor_cores
         # This parameter is required.
         self.spark_executor_memory = spark_executor_memory
         # This parameter is required.
         self.spark_log_level = spark_log_level
         # This parameter is required.
         self.spark_log_path = spark_log_path
+        self.spark_submit_clause = spark_submit_clause
         # This parameter is required.
         self.spark_version = spark_version
         self.tags = tags
         # This parameter is required.
         self.type = type
 
     def validate(self):
@@ -857,28 +863,32 @@
             result['defaultCatalogId'] = self.default_catalog_id
         if self.default_database is not None:
             result['defaultDatabase'] = self.default_database
         if self.default_resource_queue_id is not None:
             result['defaultResourceQueueId'] = self.default_resource_queue_id
         if self.default_sql_compute_id is not None:
             result['defaultSqlComputeId'] = self.default_sql_compute_id
+        if self.deployment_id is not None:
+            result['deploymentId'] = self.deployment_id
         if self.extra_artifact_ids is not None:
             result['extraArtifactIds'] = self.extra_artifact_ids
         if self.extra_spark_submit_params is not None:
             result['extraSparkSubmitParams'] = self.extra_spark_submit_params
         if self.files is not None:
             result['files'] = self.files
         if self.gmt_created is not None:
             result['gmtCreated'] = self.gmt_created
         if self.gmt_modified is not None:
             result['gmtModified'] = self.gmt_modified
         if self.has_changed is not None:
             result['hasChanged'] = self.has_changed
         if self.has_commited is not None:
             result['hasCommited'] = self.has_commited
+        if self.is_streaming is not None:
+            result['isStreaming'] = self.is_streaming
         if self.jars is not None:
             result['jars'] = self.jars
         if self.last_run_resource_queue_id is not None:
             result['lastRunResourceQueueId'] = self.last_run_resource_queue_id
         if self.modifier is not None:
             result['modifier'] = self.modifier
         if self.name is not None:
@@ -901,14 +911,16 @@
             result['sparkExecutorCores'] = self.spark_executor_cores
         if self.spark_executor_memory is not None:
             result['sparkExecutorMemory'] = self.spark_executor_memory
         if self.spark_log_level is not None:
             result['sparkLogLevel'] = self.spark_log_level
         if self.spark_log_path is not None:
             result['sparkLogPath'] = self.spark_log_path
+        if self.spark_submit_clause is not None:
+            result['sparkSubmitClause'] = self.spark_submit_clause
         if self.spark_version is not None:
             result['sparkVersion'] = self.spark_version
         if self.tags is not None:
             result['tags'] = self.tags
         if self.type is not None:
             result['type'] = self.type
         return result
@@ -931,28 +943,32 @@
             self.default_catalog_id = m.get('defaultCatalogId')
         if m.get('defaultDatabase') is not None:
             self.default_database = m.get('defaultDatabase')
         if m.get('defaultResourceQueueId') is not None:
             self.default_resource_queue_id = m.get('defaultResourceQueueId')
         if m.get('defaultSqlComputeId') is not None:
             self.default_sql_compute_id = m.get('defaultSqlComputeId')
+        if m.get('deploymentId') is not None:
+            self.deployment_id = m.get('deploymentId')
         if m.get('extraArtifactIds') is not None:
             self.extra_artifact_ids = m.get('extraArtifactIds')
         if m.get('extraSparkSubmitParams') is not None:
             self.extra_spark_submit_params = m.get('extraSparkSubmitParams')
         if m.get('files') is not None:
             self.files = m.get('files')
         if m.get('gmtCreated') is not None:
             self.gmt_created = m.get('gmtCreated')
         if m.get('gmtModified') is not None:
             self.gmt_modified = m.get('gmtModified')
         if m.get('hasChanged') is not None:
             self.has_changed = m.get('hasChanged')
         if m.get('hasCommited') is not None:
             self.has_commited = m.get('hasCommited')
+        if m.get('isStreaming') is not None:
+            self.is_streaming = m.get('isStreaming')
         if m.get('jars') is not None:
             self.jars = m.get('jars')
         if m.get('lastRunResourceQueueId') is not None:
             self.last_run_resource_queue_id = m.get('lastRunResourceQueueId')
         if m.get('modifier') is not None:
             self.modifier = m.get('modifier')
         if m.get('name') is not None:
@@ -976,14 +992,16 @@
             self.spark_executor_cores = m.get('sparkExecutorCores')
         if m.get('sparkExecutorMemory') is not None:
             self.spark_executor_memory = m.get('sparkExecutorMemory')
         if m.get('sparkLogLevel') is not None:
             self.spark_log_level = m.get('sparkLogLevel')
         if m.get('sparkLogPath') is not None:
             self.spark_log_path = m.get('sparkLogPath')
+        if m.get('sparkSubmitClause') is not None:
+            self.spark_submit_clause = m.get('sparkSubmitClause')
         if m.get('sparkVersion') is not None:
             self.spark_version = m.get('sparkVersion')
         if m.get('tags') is not None:
             self.tags = m.get('tags')
         if m.get('type') is not None:
             self.type = m.get('type')
         return self
@@ -1485,14 +1503,174 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = CancelJobRunResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class CreateSqlStatementRequest(TeaModel):
+    def __init__(
+        self,
+        code_content: str = None,
+        default_catalog: str = None,
+        default_database: str = None,
+        limit: int = None,
+        sql_compute_id: str = None,
+        region_id: str = None,
+    ):
+        self.code_content = code_content
+        self.default_catalog = default_catalog
+        self.default_database = default_database
+        self.limit = limit
+        self.sql_compute_id = sql_compute_id
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.code_content is not None:
+            result['codeContent'] = self.code_content
+        if self.default_catalog is not None:
+            result['defaultCatalog'] = self.default_catalog
+        if self.default_database is not None:
+            result['defaultDatabase'] = self.default_database
+        if self.limit is not None:
+            result['limit'] = self.limit
+        if self.sql_compute_id is not None:
+            result['sqlComputeId'] = self.sql_compute_id
+        if self.region_id is not None:
+            result['regionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('codeContent') is not None:
+            self.code_content = m.get('codeContent')
+        if m.get('defaultCatalog') is not None:
+            self.default_catalog = m.get('defaultCatalog')
+        if m.get('defaultDatabase') is not None:
+            self.default_database = m.get('defaultDatabase')
+        if m.get('limit') is not None:
+            self.limit = m.get('limit')
+        if m.get('sqlComputeId') is not None:
+            self.sql_compute_id = m.get('sqlComputeId')
+        if m.get('regionId') is not None:
+            self.region_id = m.get('regionId')
+        return self
+
+
+class CreateSqlStatementResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        statement_id: str = None,
+    ):
+        self.statement_id = statement_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.statement_id is not None:
+            result['statementId'] = self.statement_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('statementId') is not None:
+            self.statement_id = m.get('statementId')
+        return self
+
+
+class CreateSqlStatementResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: CreateSqlStatementResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('data') is not None:
+            temp_model = CreateSqlStatementResponseBodyData()
+            self.data = temp_model.from_map(m['data'])
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class CreateSqlStatementResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: CreateSqlStatementResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = CreateSqlStatementResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetJobRunRequest(TeaModel):
     def __init__(
         self,
         region_id: str = None,
     ):
         self.region_id = region_id
 
@@ -1811,14 +1989,215 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetJobRunResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetSqlStatementRequest(TeaModel):
+    def __init__(
+        self,
+        region_id: str = None,
+    ):
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.region_id is not None:
+            result['regionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('regionId') is not None:
+            self.region_id = m.get('regionId')
+        return self
+
+
+class GetSqlStatementResponseBodyDataSqlOutputs(TeaModel):
+    def __init__(
+        self,
+        rows: str = None,
+        schema: str = None,
+    ):
+        self.rows = rows
+        self.schema = schema
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.rows is not None:
+            result['rows'] = self.rows
+        if self.schema is not None:
+            result['schema'] = self.schema
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('rows') is not None:
+            self.rows = m.get('rows')
+        if m.get('schema') is not None:
+            self.schema = m.get('schema')
+        return self
+
+
+class GetSqlStatementResponseBodyData(TeaModel):
+    def __init__(
+        self,
+        execution_time: List[int] = None,
+        sql_error_code: str = None,
+        sql_error_message: str = None,
+        sql_outputs: List[GetSqlStatementResponseBodyDataSqlOutputs] = None,
+        state: str = None,
+        statement_id: str = None,
+    ):
+        self.execution_time = execution_time
+        self.sql_error_code = sql_error_code
+        self.sql_error_message = sql_error_message
+        self.sql_outputs = sql_outputs
+        self.state = state
+        self.statement_id = statement_id
+
+    def validate(self):
+        if self.sql_outputs:
+            for k in self.sql_outputs:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.execution_time is not None:
+            result['executionTime'] = self.execution_time
+        if self.sql_error_code is not None:
+            result['sqlErrorCode'] = self.sql_error_code
+        if self.sql_error_message is not None:
+            result['sqlErrorMessage'] = self.sql_error_message
+        result['sqlOutputs'] = []
+        if self.sql_outputs is not None:
+            for k in self.sql_outputs:
+                result['sqlOutputs'].append(k.to_map() if k else None)
+        if self.state is not None:
+            result['state'] = self.state
+        if self.statement_id is not None:
+            result['statementId'] = self.statement_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('executionTime') is not None:
+            self.execution_time = m.get('executionTime')
+        if m.get('sqlErrorCode') is not None:
+            self.sql_error_code = m.get('sqlErrorCode')
+        if m.get('sqlErrorMessage') is not None:
+            self.sql_error_message = m.get('sqlErrorMessage')
+        self.sql_outputs = []
+        if m.get('sqlOutputs') is not None:
+            for k in m.get('sqlOutputs'):
+                temp_model = GetSqlStatementResponseBodyDataSqlOutputs()
+                self.sql_outputs.append(temp_model.from_map(k))
+        if m.get('state') is not None:
+            self.state = m.get('state')
+        if m.get('statementId') is not None:
+            self.statement_id = m.get('statementId')
+        return self
+
+
+class GetSqlStatementResponseBody(TeaModel):
+    def __init__(
+        self,
+        data: GetSqlStatementResponseBodyData = None,
+        request_id: str = None,
+    ):
+        self.data = data
+        self.request_id = request_id
+
+    def validate(self):
+        if self.data:
+            self.data.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.data is not None:
+            result['data'] = self.data.to_map()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('data') is not None:
+            temp_model = GetSqlStatementResponseBodyData()
+            self.data = temp_model.from_map(m['data'])
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class GetSqlStatementResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetSqlStatementResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetSqlStatementResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GrantRoleToUsersRequest(TeaModel):
     def __init__(
         self,
         role_arn: str = None,
         user_arns: List[str] = None,
         region_id: str = None,
     ):
@@ -2022,27 +2401,29 @@
 
 
 class ListJobRunsRequest(TeaModel):
     def __init__(
         self,
         creator: str = None,
         end_time: ListJobRunsRequestEndTime = None,
+        job_run_deployment_id: str = None,
         job_run_id: str = None,
         max_results: int = None,
         name: str = None,
         next_token: str = None,
         region_id: str = None,
         resource_queue_id: str = None,
         start_time: ListJobRunsRequestStartTime = None,
         states: List[str] = None,
         tags: List[ListJobRunsRequestTags] = None,
     ):
         # 创建用户Uid。
         self.creator = creator
         self.end_time = end_time
+        self.job_run_deployment_id = job_run_deployment_id
         # 作业id。
         self.job_run_id = job_run_id
         # 一次获取的最大记录数。
         self.max_results = max_results
         # 作业名称。
         self.name = name
         # 标记当前开始读取的位置，置空表示从头开始。
@@ -2071,14 +2452,16 @@
             return _map
 
         result = dict()
         if self.creator is not None:
             result['creator'] = self.creator
         if self.end_time is not None:
             result['endTime'] = self.end_time.to_map()
+        if self.job_run_deployment_id is not None:
+            result['jobRunDeploymentId'] = self.job_run_deployment_id
         if self.job_run_id is not None:
             result['jobRunId'] = self.job_run_id
         if self.max_results is not None:
             result['maxResults'] = self.max_results
         if self.name is not None:
             result['name'] = self.name
         if self.next_token is not None:
@@ -2100,14 +2483,16 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('creator') is not None:
             self.creator = m.get('creator')
         if m.get('endTime') is not None:
             temp_model = ListJobRunsRequestEndTime()
             self.end_time = temp_model.from_map(m['endTime'])
+        if m.get('jobRunDeploymentId') is not None:
+            self.job_run_deployment_id = m.get('jobRunDeploymentId')
         if m.get('jobRunId') is not None:
             self.job_run_id = m.get('jobRunId')
         if m.get('maxResults') is not None:
             self.max_results = m.get('maxResults')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('nextToken') is not None:
@@ -2130,27 +2515,29 @@
 
 
 class ListJobRunsShrinkRequest(TeaModel):
     def __init__(
         self,
         creator: str = None,
         end_time_shrink: str = None,
+        job_run_deployment_id: str = None,
         job_run_id: str = None,
         max_results: int = None,
         name: str = None,
         next_token: str = None,
         region_id: str = None,
         resource_queue_id: str = None,
         start_time_shrink: str = None,
         states_shrink: str = None,
         tags_shrink: str = None,
     ):
         # 创建用户Uid。
         self.creator = creator
         self.end_time_shrink = end_time_shrink
+        self.job_run_deployment_id = job_run_deployment_id
         # 作业id。
         self.job_run_id = job_run_id
         # 一次获取的最大记录数。
         self.max_results = max_results
         # 作业名称。
         self.name = name
         # 标记当前开始读取的位置，置空表示从头开始。
@@ -2172,14 +2559,16 @@
             return _map
 
         result = dict()
         if self.creator is not None:
             result['creator'] = self.creator
         if self.end_time_shrink is not None:
             result['endTime'] = self.end_time_shrink
+        if self.job_run_deployment_id is not None:
+            result['jobRunDeploymentId'] = self.job_run_deployment_id
         if self.job_run_id is not None:
             result['jobRunId'] = self.job_run_id
         if self.max_results is not None:
             result['maxResults'] = self.max_results
         if self.name is not None:
             result['name'] = self.name
         if self.next_token is not None:
@@ -2198,14 +2587,16 @@
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('creator') is not None:
             self.creator = m.get('creator')
         if m.get('endTime') is not None:
             self.end_time_shrink = m.get('endTime')
+        if m.get('jobRunDeploymentId') is not None:
+            self.job_run_deployment_id = m.get('jobRunDeploymentId')
         if m.get('jobRunId') is not None:
             self.job_run_id = m.get('jobRunId')
         if m.get('maxResults') is not None:
             self.max_results = m.get('maxResults')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('nextToken') is not None:
@@ -4057,7 +4448,102 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = StartJobRunResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class TerminateSqlStatementRequest(TeaModel):
+    def __init__(
+        self,
+        region_id: str = None,
+    ):
+        self.region_id = region_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.region_id is not None:
+            result['regionId'] = self.region_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('regionId') is not None:
+            self.region_id = m.get('regionId')
+        return self
+
+
+class TerminateSqlStatementResponseBody(TeaModel):
+    def __init__(
+        self,
+        request_id: str = None,
+    ):
+        self.request_id = request_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.request_id is not None:
+            result['requestId'] = self.request_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('requestId') is not None:
+            self.request_id = m.get('requestId')
+        return self
+
+
+class TerminateSqlStatementResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: TerminateSqlStatementResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = TerminateSqlStatementResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.3.0/alibabacloud_emr_serverless_spark20230808.egg-info/PKG-INFO` & `alibabacloud_emr-serverless-spark20230808-1.4.0/alibabacloud_emr_serverless_spark20230808.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-emr-serverless-spark20230808
-Version: 1.3.0
+Version: 1.4.0
 Summary: Alibaba Cloud emr-serverless-spark (20230808) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_emr-serverless-spark20230808-1.3.0/alibabacloud_emr_serverless_spark20230808.egg-info/SOURCES.txt` & `alibabacloud_emr-serverless-spark20230808-1.4.0/alibabacloud_emr_serverless_spark20230808.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alibabacloud_emr-serverless-spark20230808-1.3.0/setup.py` & `alibabacloud_emr-serverless-spark20230808-1.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_emr-serverless-spark20230808.
 
-Created on 22/05/2024
+Created on 31/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_emr_serverless_spark20230808"
 NAME = "alibabacloud_emr-serverless-spark20230808" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud emr-serverless-spark (20230808) SDK Library for Python"
```

