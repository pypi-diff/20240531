# Comparing `tmp/appmesh-1.1.8-py3-none-any.whl.zip` & `tmp/appmesh-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 16482 bytes, number of entries: 6
--rw-r--r--  2.0 unx       11 b- defN 24-May-29 12:22 appmesh/__init__.py
--rw-r--r--  2.0 unx    59591 b- defN 24-May-29 12:22 appmesh/appmesh_client.py
--rw-r--r--  2.0 unx    10945 b- defN 24-May-29 12:22 appmesh-1.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-29 12:22 appmesh-1.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-May-29 12:22 appmesh-1.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      455 b- defN 24-May-29 12:22 appmesh-1.1.8.dist-info/RECORD
-6 files, 71102 bytes uncompressed, 15660 bytes compressed:  78.0%
+Zip file size: 16456 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       11 b- defN 24-May-30 23:13 appmesh/__init__.py
+-rw-r--r--  2.0 unx    59591 b- defN 24-May-30 23:13 appmesh/appmesh_client.py
+-rw-r--r--  2.0 unx    10928 b- defN 24-May-30 23:13 appmesh-1.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-30 23:13 appmesh-1.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-30 23:13 appmesh-1.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      455 b- defN 24-May-30 23:13 appmesh-1.1.9.dist-info/RECORD
+6 files, 71085 bytes uncompressed, 15634 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: appmesh/__init__.py
 Comment: 
 
 Filename: appmesh/appmesh_client.py
 Comment: 
 
-Filename: appmesh-1.1.8.dist-info/METADATA
+Filename: appmesh-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: appmesh-1.1.8.dist-info/WHEEL
+Filename: appmesh-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: appmesh-1.1.8.dist-info/top_level.txt
+Filename: appmesh-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: appmesh-1.1.8.dist-info/RECORD
+Filename: appmesh-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `appmesh-1.1.8.dist-info/METADATA` & `appmesh-1.1.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: appmesh
-Version: 1.1.8
+Version: 1.1.9
 Summary: Client SDK for App Mesh
 Home-page: https://github.com/laoshanxi/app-mesh
 Author: laoshanxi
 Author-email: 178029200@qq.com
 License: MIT
 Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3
@@ -23,36 +23,35 @@
   <img alt="Coverity Scan Build Status"
        src="https://img.shields.io/coverity/scan/21528.svg"/>
 </a>
 [![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/laoshanxi/app-mesh/badge)](https://api.securityscorecards.dev/projects/github.com/laoshanxi/app-mesh)
 
 # App Mesh
 
-App Mesh is a `Multi-Tenant`, `Cloud Native`, `Micro Service` application management platform, used to manage, schedule and monitor applications. Each app can be a specific microservice for service discovery or a normal app with replication, the app-mesh will guarantee all defined applications run on time with defined behavior and resource requests. The platform can run in standalone or cluster mode, and provide REST APIs, command-line and web-ui.
+App Mesh is a `Multi-Tenant`, `Cloud Native`, `Micro Service` application management platform designed to manage, schedule, and monitor applications. Each app can be a specific microservice for service discovery or a standard app with replication. App Mesh ensures all defined applications run on time with the specified behavior and resource requests. The platform supports both standalone and cluster modes and provides REST APIs, a command-line interface, and a web UI.
 
-App Mesh is similar to Kubernetes but much more lightweight, supporting both container apps and native apps.
+App Mesh is similar to Kubernetes but is much more lightweight, supporting both containerized and native applications.
 
 <div align=center><img src="https://github.com/laoshanxi/app-mesh/raw/main/docs/source/diagram.jpg" align=center /></div>
 
 ## Features
 
 Feature | Description
 ---|---
-Application management | 1. Manage independent applications and guard the process running, similar with systemd but more flexible (long/short running, periodic long running, cron schedule, customized day time and error handling control) and comprehensive monitoring (number of starts, return code, error message, health-check) for both native and docker application. <br> 2. Use SDK/CLI run application on a remote host with sync/async mode and fetch result to client. <br> 3. Full control of application lifecycle (cgroup for resource limitation, specific OS user for execution user). <br> 4. Interactive application start support specify input data by pipe and environment variables.<br> 5. All functionality provides by [CLI](https://app-mesh.readthedocs.io/en/latest/CLI.html), [REST](https://app-mesh.readthedocs.io/en/latest/Development.html#rest-apis), [SDK](https://github.com/laoshanxi/app-mesh/tree/main/src/sdk) and [WebGUI](https://github.com/laoshanxi/app-mesh-ui) interface.<br>
+Application management | 1. Manage independent applications with flexible process control (long/short running, periodic, cron schedule, custom timings, error handling) and comprehensive monitoring (start counts, return codes, error messages, health checks) for both native and Docker applications. <br> 2. Run applications on remote hosts using SDK/CLI with sync/async modes and fetch results to the client. <br> 3. Full control over application lifecycle (cgroup resource limitation, specific OS user for execution). <br> 4. Support interactive application start with specific input data via pipe and environment variables. <br> 5. Access all functionalities via [CLI](https://app-mesh.readthedocs.io/en/latest/CLI.html), [REST](https://app-mesh.readthedocs.io/en/latest/Development.html#rest-apis), [SDK](https://github.com/laoshanxi/app-mesh/tree/main/src/sdk) and [WebGUI](https://github.com/laoshanxi/app-mesh-ui) interface.<br>
 Security |  ⚡️ [JWT authentication](https://app-mesh.readthedocs.io/en/latest/JWT.html) for CLI and REST interface <br> ⚡️ [LDAP support](https://app-mesh.readthedocs.io/en/latest/LDAP.html) <br> ⚡️ [Role based permission control](https://app-mesh.readthedocs.io/en/latest/USER_ROLE.html) <br> ⚡️ [Multi-factor authentication](https://app-mesh.readthedocs.io/en/latest/MFA.html)<br> SSL support (ECDH and secure ciphers) for REST http connection  <br> Multi-tenant support
-Cloud native | Schedule cloud level applications for running on multile hosts with resource size request.<br> ⚡️ [Prometheus Exporter (build-in)](https://app-mesh.readthedocs.io/en/latest/PROMETHEUS.html) <br> ⚡️ [Grafana SimpleJson datasource](https://app-mesh.readthedocs.io/en/latest/GrafanaDataSource.html) <br> ⚡️ [Grafana Loki](https://app-mesh.readthedocs.io/en/latest/Loki.html) <br>⚡️ [Dockerfile](https://github.com/laoshanxi/app-mesh/blob/main/Dockerfile)
+Cloud native | Schedule cloud-level applications to run on multiple hosts with resource size requests. <br> ⚡️ [Prometheus Exporter (build-in)](https://app-mesh.readthedocs.io/en/latest/PROMETHEUS.html) <br> ⚡️ [Grafana SimpleJson datasource](https://app-mesh.readthedocs.io/en/latest/GrafanaDataSource.html) <br> ⚡️ [Grafana Loki](https://app-mesh.readthedocs.io/en/latest/Loki.html) <br>⚡️ [Dockerfile](https://github.com/laoshanxi/app-mesh/blob/main/Dockerfile)
 Micro service application | ⚡️ [Consul micro-service cluster management](https://app-mesh.readthedocs.io/en/latest/CONSUL.html)
-Extra Features | Collect host/app resource usage <br> Remote run shell commands <br> Download/Upload files interface <br> Hot-update support `systemctl reload appmesh` <br> Bash completion <br> Reverse proxy <br> [Web GUI](https://github.com/laoshanxi/app-mesh-ui)
+Extra Features | Collect host/app resource usage <br> Remote shell command execution <br> File upload/download interface <br> Hot-update support `systemctl reload appmesh` <br> Bash completion <br> Reverse proxy <br> [Web GUI](https://github.com/laoshanxi/app-mesh-ui)
 Platform support | X86_64 <br> ARM32 <br> ARM64
 SDK | [Python](https://app-mesh.readthedocs.io/en/latest/api/appmesh_client.html) <br> [Golang](https://github.com/laoshanxi/app-mesh/blob/main/src/sdk/go/appmesh_client.go) <br> Swagger [OpenAPI Specification](https://raw.githubusercontent.com/laoshanxi/app-mesh/main/src/daemon/rest/openapi.yaml) `https://localhost:6060/swagger` 
 
 ## Getting started
 
-The [Installation doc](https://app-mesh.readthedocs.io/en/latest/Install.html) introduces how
-to install App Mesh via docker-compose or native way and setup App Mesh cluster.
+Refer to the [Installation doc](https://app-mesh.readthedocs.io/en/latest/Install.html) to learn how to install App Mesh via Docker Compose or natively and set up an App Mesh cluster.
 
 ## Documentation
 
 - [Read the Docs](https://app-mesh.readthedocs.io/)
 - [REST API](https://app-mesh.readthedocs.io/en/latest/Development.html#rest-apis)
 - [Command lines](https://app-mesh.readthedocs.io/en/latest/CLI.html)
 - [Security](https://app-mesh.readthedocs.io/en/latest/JWT.html)
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: appmesh Version: 1.1.8 Summary: Client SDK for App
+Metadata-Version: 2.1 Name: appmesh Version: 1.1.9 Summary: Client SDK for App
 Mesh Home-page: https://github.com/laoshanxi/app-mesh Author: laoshanxi Author-
 email: 178029200@qq.com License: MIT Keywords: appmesh AppMesh app-mesh
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown Requires-Dist:
 requests Requires-Dist: msgpack Requires-Dist: requests-toolbelt Requires-Dist:
 aniso8601 ï»¿[![language.badge]][language.url] [![standard.badge]]
@@ -13,74 +13,73 @@
 latest/?badge=latest) [![Join the chat at https://gitter.im/app-mesh/community]
 (https://badges.gitter.im/app-mesh/community.svg)](https://gitter.im/app-mesh/
 community?utm_source=badge&utm_medium=badge&utm_campaign=pr-
 badge&utm_content=badge) _[_C_o_v_e_r_i_t_y_ _S_c_a_n_ _B_u_i_l_d_ _S_t_a_t_u_s_][![OpenSSF Scorecard]
 (https://api.securityscorecards.dev/projects/github.com/laoshanxi/app-mesh/
 badge)](https://api.securityscorecards.dev/projects/github.com/laoshanxi/app-
 mesh) # App Mesh App Mesh is a `Multi-Tenant`, `Cloud Native`, `Micro Service`
-application management platform, used to manage, schedule and monitor
+application management platform designed to manage, schedule, and monitor
 applications. Each app can be a specific microservice for service discovery or
-a normal app with replication, the app-mesh will guarantee all defined
-applications run on time with defined behavior and resource requests. The
-platform can run in standalone or cluster mode, and provide REST APIs, command-
-line and web-ui. App Mesh is similar to Kubernetes but much more lightweight,
-supporting both container apps and native apps.
+a standard app with replication. App Mesh ensures all defined applications run
+on time with the specified behavior and resource requests. The platform
+supports both standalone and cluster modes and provides REST APIs, a command-
+line interface, and a web UI. App Mesh is similar to Kubernetes but is much
+more lightweight, supporting both containerized and native applications.
    [https://github.com/laoshanxi/app-mesh/raw/main/docs/source/diagram.jpg]
 ## Features Feature | Description ---|--- Application management | 1. Manage
-independent applications and guard the process running, similar with systemd
-but more flexible (long/short running, periodic long running, cron schedule,
-customized day time and error handling control) and comprehensive monitoring
-(number of starts, return code, error message, health-check) for both native
-and docker application.
-2. Use SDK/CLI run application on a remote host with sync/async mode and fetch
-result to client.
-3. Full control of application lifecycle (cgroup for resource limitation,
-specific OS user for execution user).
-4. Interactive application start support specify input data by pipe and
+independent applications with flexible process control (long/short running,
+periodic, cron schedule, custom timings, error handling) and comprehensive
+monitoring (start counts, return codes, error messages, health checks) for both
+native and Docker applications.
+2. Run applications on remote hosts using SDK/CLI with sync/async modes and
+fetch results to the client.
+3. Full control over application lifecycle (cgroup resource limitation,
+specific OS user for execution).
+4. Support interactive application start with specific input data via pipe and
 environment variables.
-5. All functionality provides by [CLI](https://app-mesh.readthedocs.io/en/
+5. Access all functionalities via [CLI](https://app-mesh.readthedocs.io/en/
 latest/CLI.html), [REST](https://app-mesh.readthedocs.io/en/latest/
 Development.html#rest-apis), [SDK](https://github.com/laoshanxi/app-mesh/tree/
 main/src/sdk) and [WebGUI](https://github.com/laoshanxi/app-mesh-ui) interface.
 Security | â¡ï¸ [JWT authentication](https://app-mesh.readthedocs.io/en/
 latest/JWT.html) for CLI and REST interface
 â¡ï¸ [LDAP support](https://app-mesh.readthedocs.io/en/latest/LDAP.html)
 â¡ï¸ [Role based permission control](https://app-mesh.readthedocs.io/en/
 latest/USER_ROLE.html)
 â¡ï¸ [Multi-factor authentication](https://app-mesh.readthedocs.io/en/latest/
 MFA.html)
 SSL support (ECDH and secure ciphers) for REST http connection
-Multi-tenant support Cloud native | Schedule cloud level applications for
-running on multile hosts with resource size request.
+Multi-tenant support Cloud native | Schedule cloud-level applications to run on
+multiple hosts with resource size requests.
 â¡ï¸ [Prometheus Exporter (build-in)](https://app-mesh.readthedocs.io/en/
 latest/PROMETHEUS.html)
 â¡ï¸ [Grafana SimpleJson datasource](https://app-mesh.readthedocs.io/en/
 latest/GrafanaDataSource.html)
 â¡ï¸ [Grafana Loki](https://app-mesh.readthedocs.io/en/latest/Loki.html)
 â¡ï¸ [Dockerfile](https://github.com/laoshanxi/app-mesh/blob/main/Dockerfile)
 Micro service application | â¡ï¸ [Consul micro-service cluster management]
 (https://app-mesh.readthedocs.io/en/latest/CONSUL.html) Extra Features |
 Collect host/app resource usage
-Remote run shell commands
-Download/Upload files interface
+Remote shell command execution
+File upload/download interface
 Hot-update support `systemctl reload appmesh`
 Bash completion
 Reverse proxy
 [Web GUI](https://github.com/laoshanxi/app-mesh-ui) Platform support | X86_64
 ARM32
 ARM64 SDK | [Python](https://app-mesh.readthedocs.io/en/latest/api/
 appmesh_client.html)
 [Golang](https://github.com/laoshanxi/app-mesh/blob/main/src/sdk/go/
 appmesh_client.go)
 Swagger [OpenAPI Specification](https://raw.githubusercontent.com/laoshanxi/
 app-mesh/main/src/daemon/rest/openapi.yaml) `https://localhost:6060/swagger` ##
-Getting started The [Installation doc](https://app-mesh.readthedocs.io/en/
-latest/Install.html) introduces how to install App Mesh via docker-compose or
-native way and setup App Mesh cluster. ## Documentation - [Read the Docs]
-(https://app-mesh.readthedocs.io/) - [REST API](https://app-
+Getting started Refer to the [Installation doc](https://app-
+mesh.readthedocs.io/en/latest/Install.html) to learn how to install App Mesh
+via Docker Compose or natively and set up an App Mesh cluster. ## Documentation
+- [Read the Docs](https://app-mesh.readthedocs.io/) - [REST API](https://app-
 mesh.readthedocs.io/en/latest/Development.html#rest-apis) - [Command lines]
 (https://app-mesh.readthedocs.io/en/latest/CLI.html) - [Security](https://app-
 mesh.readthedocs.io/en/latest/JWT.html) ## Comparison ### Standalone mode |
 Feature | App Mesh | [Supervisor](http://supervisord.org/) | [crontab](https://
 crontab.guru/) | | ------------------------ | -------- | ----------------------
 --------------- | -------------------------------- | | Accuracy | Seconds |
 Seconds | Minutes | | Language | C++11 | Python | C | | Web GUI | â | â | |
```

