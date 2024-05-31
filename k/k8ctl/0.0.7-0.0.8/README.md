# Comparing `tmp/k8ctl-0.0.7-py3-none-any.whl.zip` & `tmp/k8ctl-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 9385 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 24-May-30 12:19 k8ctl/__init__.py
--rw-r--r--  2.0 unx    16623 b- defN 24-May-30 12:19 k8ctl/k8ctl.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-30 12:19 k8ctl-0.0.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     1120 b- defN 24-May-30 12:19 k8ctl-0.0.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-30 12:19 k8ctl-0.0.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 24-May-30 12:19 k8ctl-0.0.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        6 b- defN 24-May-30 12:19 k8ctl-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      612 b- defN 24-May-30 12:19 k8ctl-0.0.7.dist-info/RECORD
-8 files, 29854 bytes uncompressed, 8319 bytes compressed:  72.1%
+Zip file size: 9952 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 24-May-31 05:44 k8ctl/__init__.py
+-rw-r--r--  2.0 unx     1267 b- defN 24-May-31 05:44 k8ctl/helper.py
+-rw-r--r--  2.0 unx    15464 b- defN 24-May-31 05:44 k8ctl/k8ctl.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-31 05:44 k8ctl-0.0.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-31 05:44 k8ctl-0.0.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 05:44 k8ctl-0.0.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 24-May-31 05:44 k8ctl-0.0.8.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 24-May-31 05:44 k8ctl-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      684 b- defN 24-May-31 05:44 k8ctl-0.0.8.dist-info/RECORD
+9 files, 30034 bytes uncompressed, 8780 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
 Filename: k8ctl/__init__.py
 Comment: 
 
+Filename: k8ctl/helper.py
+Comment: 
+
 Filename: k8ctl/k8ctl.py
 Comment: 
 
-Filename: k8ctl-0.0.7.dist-info/LICENSE
+Filename: k8ctl-0.0.8.dist-info/LICENSE
 Comment: 
 
-Filename: k8ctl-0.0.7.dist-info/METADATA
+Filename: k8ctl-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: k8ctl-0.0.7.dist-info/WHEEL
+Filename: k8ctl-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: k8ctl-0.0.7.dist-info/entry_points.txt
+Filename: k8ctl-0.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: k8ctl-0.0.7.dist-info/top_level.txt
+Filename: k8ctl-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: k8ctl-0.0.7.dist-info/RECORD
+Filename: k8ctl-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## k8ctl/k8ctl.py

```diff
@@ -1,61 +1,19 @@
 import click
 import subprocess
 import os
-# import helper
+import helper
 # import logging
 
 rancher_url = os.getenv("RANCHER_URL")
 
 # log = logging.getLogger(__name__)
 # log.setLevel(logging.DEBUG)
 # log.addHandler(logging.StreamHandler())
 
-## helper functions
-
-def check_token_validlity():
-    '''
-    Check if the token is still valid
-    '''
-    result = subprocess.run("kubectl get po", shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
-
-    return result.returncode
-
-def list_env(app):
-    '''
-    List all environment variables
-    '''
-    cmd = """kubectl get secret {}""".format(app) + ''' -o jsonpath="{.data}" '''
-    cmd2= cmd + """ | jq -r 'to_entries|map("\(.key)=\(.value | @base64d)")|.[]' """
-
-    result = subprocess.run(cmd, shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.PIPE)
-
-    # checking whether the secret exists
-    if result.returncode != 0:
-        print("Failed to list the environment variables. May be app not found")
-        return 404
-    
-    result2 = subprocess.run(cmd2, shell=True, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE, input=result.stdout)
-
-    return result2.stdout.decode('utf-8').strip()
-
-def current_cluster():
-    '''
-    Get the current cluster
-    '''
-    cmd = "kubectl config current-context"
-    result = subprocess.run(cmd, shell=True, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-
-    return result.stdout.decode('utf-8').strip()
-
-
-def hello_world():
-    print("Hello World")
-
-
 ## Program starts here
 
 @click.group()
 def k8ctl():
     '''
     k8ctl is a command line tool for managing rancher multicluster kubernetes environments
     '''
@@ -177,15 +135,15 @@
         click.echo(f"No")
         return 1
     elif dummy == cluster:
         current_cluster.returncode = 0
     else:
         current_cluster.returncode = 1
 
-    if current_cluster.returncode == 0 and check_token_validlity() == 0:
+    if current_cluster.returncode == 0 and helper.check_token_validlity() == 0:
         click.echo(f"Already logged into {cluster}")
         return 0
     
     elif result.returncode != 0:
         click.echo(f"Cluster {cluster} config not found")
 
         subprocess.run(f"touch ~/.kube/{cluster}", shell=True, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
@@ -197,15 +155,15 @@
             click.echo("Failed to switch to the cluster")
             return 1
         else:
             click.echo(f"{cluster} config is stored in ~/.kube/")
             
     copy_config = subprocess.run(f"cp ~/.kube/{cluster} ~/.kube/config", shell=True, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
     
-    if check_token_validlity() != 0:
+    if helper.check_token_validlity() != 0:
         click.echo("Token has expired. So, logging in again")
 
         subprocess.run(f"> ~/.kube/{cluster}", shell=True, check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
 
         with open(os.path.expanduser(f"~/.kube/{cluster}"), "w") as f:
             config_write = subprocess.run(f"rancher cluster kf {cluster}", shell=True, stdout=f, stderr=subprocess.PIPE, text=True)
         
@@ -267,15 +225,15 @@
             try:
                 env_vars.append(input())
             except EOFError:
                 break
 
     env_vars = dict([env_var.split('=', 1) for env_var in env_vars])
 
-    last_env = list_env(app).strip()
+    last_env = helper.list_env(app).strip()
     last_env = dict([env.split('=', 1) for env in last_env.split('\n')])
 
     for key, value in env_vars.items():
         last_env[key] = value
 
     with open("/tmp/env_{}.env".format(app), "w") as f:
         for key, value in last_env.items():
@@ -368,15 +326,15 @@
 @click.option('--app', '-a', prompt=True, help='The application name to deploy', required=True)
 def psql(app):
     '''
     Connect to the application database
     '''
 
     # get the db url
-    env_vars = list_env(app)
+    env_vars = helper.list_env(app)
     if env_vars == 404:
         return
 
     # split with first '='
     env_vars = dict([env_var.split('=', 1) for env_var in env_vars.split('\n')])
 
     if "DASHBOARD_DB_URL" not in env_vars and "DB_URL" not in env_vars and "DATABASE_URL" not in env_vars:
@@ -416,15 +374,16 @@
     '''
     Connect to the application with bash
     '''
     result = os.system(f"kubectl exec -it $(kubectl get po --sort-by='.status.startTime' --field-selector=status.phase==Running -l app={app}"+" | awk 'NR ==2 {print $1}' ) -- bash")
 
     if result != 0:
         click.echo("Failed to connect to the bash")
-
+    elif result == 530:
+        click.echo("Exited from the bash")
 
 ## Restart group
 @restart.command(name='web')
 @click.option('--app', '-a', prompt=True, help='The application name to restart the web services', required=True)
 def restart_app(app):
     '''
     Restart the application
```

## Comparing `k8ctl-0.0.7.dist-info/LICENSE` & `k8ctl-0.0.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `k8ctl-0.0.7.dist-info/METADATA` & `k8ctl-0.0.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: k8ctl
-Version: 0.0.7
+Version: 0.0.8
 Author: Kishorekarthik P
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click
 
 # k8ctl
```

## Comparing `k8ctl-0.0.7.dist-info/RECORD` & `k8ctl-0.0.8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 k8ctl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-k8ctl/k8ctl.py,sha256=xR8J0mzr4dkG4n06vYU9N0oHFZkSgJtBq_rSW6q_69U,16623
-k8ctl-0.0.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-k8ctl-0.0.7.dist-info/METADATA,sha256=wqzCMCaGRAD5SKE-AqYJrPWbSXamHDZztXPfd5ZpZrw,1120
-k8ctl-0.0.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-k8ctl-0.0.7.dist-info/entry_points.txt,sha256=snE4Lt3gioSbGG7Chpv4NxhrWV_Z8wI7MVBB6zauFGo,44
-k8ctl-0.0.7.dist-info/top_level.txt,sha256=MWKRJ9qlnCPm7r_pIheyUtZ4LqaWZ21y0H-O_NFS3Bw,6
-k8ctl-0.0.7.dist-info/RECORD,,
+k8ctl/helper.py,sha256=2nMeY-wUhN0EpYsDeyiMbOfL8SSxD8bF31yFVpQNZIY,1267
+k8ctl/k8ctl.py,sha256=FT1KWxcMNMhl8vwIDaNvCFB6F2HWeuyt9BVJ2xfL3nc,15464
+k8ctl-0.0.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+k8ctl-0.0.8.dist-info/METADATA,sha256=mVSajIceuULU8RgRMMmBmwD1-UaACVbftFZMOAzspec,1120
+k8ctl-0.0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+k8ctl-0.0.8.dist-info/entry_points.txt,sha256=snE4Lt3gioSbGG7Chpv4NxhrWV_Z8wI7MVBB6zauFGo,44
+k8ctl-0.0.8.dist-info/top_level.txt,sha256=MWKRJ9qlnCPm7r_pIheyUtZ4LqaWZ21y0H-O_NFS3Bw,6
+k8ctl-0.0.8.dist-info/RECORD,,
```

