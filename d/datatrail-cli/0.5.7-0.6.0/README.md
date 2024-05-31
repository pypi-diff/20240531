# Comparing `tmp/datatrail_cli-0.5.7.tar.gz` & `tmp/datatrail_cli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatrail_cli-0.5.7.tar", max compression
+gzip compressed data, was "datatrail_cli-0.6.0.tar", max compression
```

## Comparing `datatrail_cli-0.5.7.tar` & `datatrail_cli-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1080 2024-05-10 18:29:48.263562 datatrail_cli-0.5.7/LICENSE
--rw-r--r--   0        0        0     3558 2024-05-10 18:29:48.263562 datatrail_cli-0.5.7/README.md
--rw-r--r--   0        0        0      214 2024-05-10 18:29:48.271562 datatrail_cli-0.5.7/dtcli/__init__.py
--rw-r--r--   0        0        0     4759 2024-05-10 18:29:48.271562 datatrail_cli-0.5.7/dtcli/clear.py
--rw-r--r--   0        0        0     1437 2024-05-10 18:29:48.271562 datatrail_cli-0.5.7/dtcli/cli.py
--rw-r--r--   0        0        0     4037 2024-05-10 18:29:48.271562 datatrail_cli-0.5.7/dtcli/config.py
--rw-r--r--   0        0        0     1062 2024-05-10 18:29:48.271562 datatrail_cli-0.5.7/dtcli/config.yaml
--rw-r--r--   0        0        0     4101 2024-05-10 18:29:48.271562 datatrail_cli-0.5.7/dtcli/ls.py
--rw-r--r--   0        0        0     8086 2024-05-10 18:29:48.271562 datatrail_cli-0.5.7/dtcli/ps.py
--rw-r--r--   0        0        0     4799 2024-05-10 18:29:48.271562 datatrail_cli-0.5.7/dtcli/pull.py
--rw-r--r--   0        0        0    15878 2024-05-10 18:29:48.271562 datatrail_cli-0.5.7/dtcli/src/functions.py
--rw-r--r--   0        0        0     9241 2024-05-10 18:29:48.271562 datatrail_cli-0.5.7/dtcli/utilities/cadcclient.py
--rw-r--r--   0        0        0     3206 2024-05-10 18:29:48.271562 datatrail_cli-0.5.7/dtcli/utilities/utilities.py
--rw-r--r--   0        0        0     1073 2024-05-10 18:29:48.275562 datatrail_cli-0.5.7/pyproject.toml
--rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 datatrail_cli-0.5.7/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-05-31 19:18:51.369402 datatrail_cli-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3558 2024-05-31 19:18:51.369402 datatrail_cli-0.6.0/README.md
+-rw-r--r--   0        0        0      214 2024-05-31 19:18:51.377402 datatrail_cli-0.6.0/dtcli/__init__.py
+-rw-r--r--   0        0        0     4759 2024-05-31 19:18:51.377402 datatrail_cli-0.6.0/dtcli/clear.py
+-rw-r--r--   0        0        0     1473 2024-05-31 19:18:51.377402 datatrail_cli-0.6.0/dtcli/cli.py
+-rw-r--r--   0        0        0     4037 2024-05-31 19:18:51.377402 datatrail_cli-0.6.0/dtcli/config.py
+-rw-r--r--   0        0        0     1062 2024-05-31 19:18:51.377402 datatrail_cli-0.6.0/dtcli/config.yaml
+-rw-r--r--   0        0        0     4101 2024-05-31 19:18:51.377402 datatrail_cli-0.6.0/dtcli/ls.py
+-rw-r--r--   0        0        0     8316 2024-05-31 19:18:51.377402 datatrail_cli-0.6.0/dtcli/ps.py
+-rw-r--r--   0        0        0     4799 2024-05-31 19:18:51.377402 datatrail_cli-0.6.0/dtcli/pull.py
+-rw-r--r--   0        0        0     5133 2024-05-31 19:18:51.377402 datatrail_cli-0.6.0/dtcli/scout.py
+-rw-r--r--   0        0        0    15953 2024-05-31 19:18:51.381402 datatrail_cli-0.6.0/dtcli/src/functions.py
+-rw-r--r--   0        0        0    12468 2024-05-31 19:18:51.381402 datatrail_cli-0.6.0/dtcli/utilities/cadcclient.py
+-rw-r--r--   0        0        0     3582 2024-05-31 19:18:51.381402 datatrail_cli-0.6.0/dtcli/utilities/utilities.py
+-rw-r--r--   0        0        0     1073 2024-05-31 19:18:51.381402 datatrail_cli-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 datatrail_cli-0.6.0/PKG-INFO
```

### Comparing `datatrail_cli-0.5.7/LICENSE` & `datatrail_cli-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.7/README.md` & `datatrail_cli-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.7/dtcli/clear.py` & `datatrail_cli-0.6.0/dtcli/clear.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.7/dtcli/cli.py` & `datatrail_cli-0.6.0/dtcli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Datatrail Command Line Interface."""
 
 import click
 from click_aliasing import ClickAliasedGroup
 from pkg_resources import get_distribution
 from rich import console, pretty
 
-from dtcli import clear, config, ls, ps, pull
+from dtcli import clear, config, ls, ps, pull, scout
 from dtcli.utilities import utilities
 
 pretty.install()
 terminal = console.Console()
 
 
 # Main CLI
@@ -32,19 +32,20 @@
     )
     terminal.print(
         f"datatrail-server {'0.1.1'}",
         style="green",
     )
 
 
+cli.add_command(clear.clear)
+cli.add_command(config.config)
 cli.add_command(ls.list, aliases=["ls"])
 cli.add_command(ps.ps)
 cli.add_command(pull.pull)
-cli.add_command(clear.clear)
-cli.add_command(config.config)
+cli.add_command(scout.scout)
 
 
 def check_version() -> None:
     """Check if CLI is latest release."""
     if not utilities.cli_is_latest_release():
         current_version = get_distribution("datatrail-cli").version
         latest_version = utilities.get_latest_released_version()
```

### Comparing `datatrail_cli-0.5.7/dtcli/config.py` & `datatrail_cli-0.6.0/dtcli/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
     Args:
         config (Path, optional): Configuration. Defaults to CONFIG.
 
     Returns:
         Dict[str, Any]: Configuration.
     """
     try:
-        with open(CONFIG.as_posix()) as stream:
+        with open(config.as_posix()) as stream:
             configuration = yaml.safe_load(stream)
         if key:
             return configuration[key]
         return configuration
     except Exception as exception:
         log.exception(exception)
         configuration = None
```

### Comparing `datatrail_cli-0.5.7/dtcli/config.yaml` & `datatrail_cli-0.6.0/dtcli/config.yaml`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.7/dtcli/ls.py` & `datatrail_cli-0.6.0/dtcli/ls.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.7/dtcli/ps.py` & `datatrail_cli-0.6.0/dtcli/ps.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,14 +64,18 @@
             ctx.invoke(list)
             return None
     except Exception as e:
         error_console.print(e)
         return None
     try:
         files, policies = functions.ps(scope, dataset, verbose, quiet)
+        if isinstance(files, str) or isinstance(policies, str):
+            error_console.print("Error: files = ", files)
+            error_console.print("Error: policies = ", policies)
+            return None
     except Exception as e:
         error_console.print(e)
         return None
 
     if show_files and files:
         # Files table
         file_table = create_files_table(dataset, scope, files)
@@ -79,14 +83,15 @@
         with console.pager():
             logger.debug("Showing file table.")
             console.print(file_table)
         return None
 
     if files and ("error" in files.keys()):
         error_console.print(files["error"])
+        return None
 
     # Info table
     elif files:
         if len(files["file_replica_locations"]) < 1:
             unregistered_info = functions.get_unregistered_dataset(dataset, scope)
             if unregistered_info:
                 console.print(
```

### Comparing `datatrail_cli-0.5.7/dtcli/pull.py` & `datatrail_cli-0.6.0/dtcli/pull.py`

 * *Files identical despite different names*

### Comparing `datatrail_cli-0.5.7/dtcli/src/functions.py` & `datatrail_cli-0.6.0/dtcli/src/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -82,21 +82,22 @@
         try:
             url = server + f"/query/dataset/children/{scope}/{dataset}"
             logger.debug(f"URL: {url}")
             r = requests.get(url)
             logger.debug(f"Status: {r.status_code}.")
             response = utilities.decode_response(r)
             logger.debug(f"Reponse: {response}")
-            if "object has no attribute" in response:
-                return {"error": f"The dataset {dataset} has no children."}
+            utilities.validate_request_response(response, dataset, scope)
             return {"datasets": response["contains"]}  # type: ignore
         except requests.exceptions.ConnectionError as e:
             logger.error(e)
             return {"error": "Datatrail Server at CHIME is not responding."}
-
+        except Exception as e:
+            logger.error(e)
+            return {"error": e}
     else:
         return {}
 
 
 def ps(
     scope: str,
     dataset: str,
@@ -138,25 +139,25 @@
 
         logger.info(f"Getting policy for {dataset} in {scope}.")
         url: str = str(base_url) + f"/query/dataset/{scope}/{dataset}"
         logger.debug(f"URL: {url}")
         r = requests.get(url)
         logger.debug(f"Status: {r.status_code}.")
         policy_response = utilities.decode_response(r)
-        if ("object has no attribute" in policy_response) and (
-            "error" in files_response
-        ):
-            raise Exception(files_response["error"])
-        elif "error" in files_response:
+        utilities.validate_request_response(policy_response, dataset, scope)
+        if "error" in files_response:
             return None, policy_response  # type: ignore
         return files_response, policy_response  # type: ignore
 
     except requests.exceptions.ConnectionError as e:
         logger.error(e)
         raise ConnectionError("Datatrail Server at CHIME is not responding.")
+    except Exception as e:
+        logger.error(e)
+        raise Exception(e)
 
 
 def get_dataset_file_info(
     scope: str,
     dataset: str,
     verbose: int = 0,
     quiet: bool = False,
@@ -188,20 +189,22 @@
         logger.debug(f"Payload: {payload}")
         url = str(base_url) + "/query/dataset/find"
         logger.debug(f"URL: {url}")
         r = requests.post(url, json=payload)
         logger.debug(f"Status: {r.status_code}.")
         logger.debug("Decoding response.")
         response = utilities.decode_response(r)
-        if "object has no attribute" in response:
-            return {"error": f"Could not find {dataset} {scope} in Datatrail."}
+        utilities.validate_request_response(response, dataset, scope)
         return response  # type: ignore
     except requests.exceptions.ConnectionError as e:
         logger.error(e)
         return {"error": "Datatrail Server at CHIME is not responding."}
+    except Exception as e:
+        logger.error(e)
+        return {"error": e}
 
 
 def find_missing_dataset_files(
     scope: str, dataset: str, root_path: Optional[str] = None, verbose: int = 0
 ) -> Dict:
     """List missing files for a dataset.
 
@@ -385,29 +388,31 @@
     logger.debug("Loading configuration.")
     try:
         config = procure()
         server = config["server"]
         logger.debug(f"Server: {server}")
         logger.debug("Configuration loaded successfully.")
     except Exception:
-        logger.error(
-            "No configuration file found. Create one with `datatrail config init`."
-        )
         logger.error("No config. Create one with `datatrail config init`.")
         return None
     # Query Datatrail Central Server.
     logger.info(f"Querying Datatrail for {dataset} {scope}.")
     payload = {"name": dataset, "scope": scope}
     url = server + "/query/dataset/find"
     logger.debug(f"URL: {url}")
     try:
         r = requests.post(url, json=payload)
         dataset_locations = utilities.decode_response(r)  # type: ignore
+        utilities.validate_request_response(dataset_locations, dataset, scope)
     except ConnectionError:
         return "The Datatrail Central Server at CHIME at is not reachable!!!"
+    except Exception as e:
+        logger.error(e)
+        return None
+
     # Build data paths.
     if dataset_locations["file_replica_locations"].get("minoc"):  # type: ignore
         file_uris = dataset_locations["file_replica_locations"]["minoc"]  # type: ignore
         file_paths = [f.replace("cadc:CHIMEFRB/", "") for f in file_uris]
 
         common_path = os.path.commonprefix(file_paths).replace("//", "/")
         if common_path[-1] != "/":
```

### Comparing `datatrail_cli-0.5.7/dtcli/utilities/cadcclient.py` & `datatrail_cli-0.6.0/dtcli/utilities/cadcclient.py`

 * *Files 18% similar despite different names*

```diff
@@ -248,7 +248,119 @@
         timeout=timeout,
         data_only=True,
         no_column_names=True,
     )
     content = buffer.getvalue()
     sys.stdout = sys.__stdout__
     return float(content.split("\n")[0])
+
+
+def dataset_md5s(
+    directory: str,
+    namespace: str = "cadc:CHIMEFRB",
+    timeout: int = 60,
+    verbose: int = 0,
+) -> Dict[str, str]:
+    """Get list of files in a directory.
+
+    Args:
+        directory (str): Directory to get the size of.
+        certfile (str, optional): Certificate file. Defaults to None.
+        namespace (str, optional): Minoc Namespace. Defaults to "cadc:CHIMEFRB".
+        timeout (int, optional): Timeout. Defaults to 60.
+        verbose (int, optional): Verbosity. Defaults to 0.
+
+    Returns:
+        Dict[str, str]: Dictionary of file paths and their md5 checksums.
+
+    Example:
+        >>> dataset_md5s("data/gbo/baseband/raw/2024/01/10/astro_350955086")
+    """
+    # Set logging level.
+    logger.setLevel("WARNING")
+    if verbose == 1:
+        logger.setLevel("INFO")
+    elif verbose > 1:
+        logger.setLevel("DEBUG")
+
+    query = f"select uri,contentChecksum from inventory.Artifact where uri like '{namespace}/{directory}%'"  # noqa
+    query = query.replace("//", "/")
+    logger.info(f"Running query: {query}")
+    buffer = StringIO()
+    sys.stdout = buffer
+    _, _, queryClient = _connect()
+    queryClient.query(  # type: ignore
+        query=query,
+        output_file=None,
+        response_format="csv",
+        tmptable=None,
+        lang="ADQL",
+        timeout=timeout,
+        data_only=True,
+        no_column_names=True,
+    )
+    content = buffer.getvalue()
+    sys.stdout = sys.__stdout__
+    paths = []
+    md5s = []
+    for line in content.split("\n"):
+        if line == "":
+            continue
+        path = line.split(",")[0].replace(namespace + "/", "")
+        try:
+            md5 = line.split(",")[1].replace("md5:", "")
+        except IndexError:
+            md5 = ""
+        paths.append(path)
+        md5s.append(md5)
+    data: Dict[str, str] = {}
+    for p, m in zip(paths, md5s):
+        data[p] = m
+    return data
+
+
+def query(
+    query: str,
+    namespace: str = "cadc:CHIMEFRB",
+    timeout: int = 60,
+    verbose: int = 0,
+) -> List[Any]:
+    """Get list of files in a directory.
+
+    Args:
+        query (str): SQL query.
+        certfile (str, optional): Certificate file. Defaults to None.
+        namespace (str, optional): Minoc Namespace. Defaults to "cadc:CHIMEFRB".
+        timeout (int, optional): Timeout. Defaults to 60.
+        verbose (int, optional): Verbosity. Defaults to 0.
+
+    Returns:
+        List[str]: List of files in the directory.
+
+    Example:
+        >>> size("/data/chime/intensity/raw/2023/01/01/")
+    """
+    # Set logging level.
+    logger.setLevel("WARNING")
+    if verbose == 1:
+        logger.setLevel("INFO")
+    elif verbose > 1:
+        logger.setLevel("DEBUG")
+
+    query = query.replace("//", "/")
+    logger.info(f"Running query: {query}")
+    buffer = StringIO()
+    sys.stdout = buffer
+    _, _, queryClient = _connect()
+    queryClient.query(  # type: ignore
+        query=query,
+        output_file=None,
+        response_format="csv",
+        tmptable=None,
+        lang="ADQL",
+        timeout=timeout,
+        data_only=True,
+        no_column_names=True,
+    )
+    content = buffer.getvalue()
+    sys.stdout = sys.__stdout__
+    return [line.split(",") for line in content.split("\n")]
```

### Comparing `datatrail_cli-0.5.7/dtcli/utilities/utilities.py` & `datatrail_cli-0.6.0/dtcli/utilities/utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,31 @@
         return response.json()
     elif response.status_code in [503]:
         raise requests.exceptions.ConnectionError("Service not responding.")
     else:
         return response.text
 
 
+def validate_request_response(
+    request_response: Any,
+    dataset: str,
+    scope: str,
+) -> None:
+    """Validate the response of a request.
+
+    Args:
+        request_response (Any): response to validate
+
+    Returns:
+        None
+    """
+    if "object has no attribute" in request_response:
+        raise Exception(f"Could not find {dataset} {scope} in Datatrail.")
+
+
 def split(data: List[Any], count: int) -> List[List[Any]]:
     """Split a list into batches.
 
     Args:
         data (List[Any]): List to split.
         count (int): Number of batches to split into.
```

### Comparing `datatrail_cli-0.5.7/pyproject.toml` & `datatrail_cli-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datatrail-cli"
-version = "0.5.7"
+version = "0.6.0"
 description = "CHIME/FRB Datatrail CLI"
 authors = ["CHIME FRB Project Office"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "dtcli" }]
 
 [tool.poetry.dependencies]
```

### Comparing `datatrail_cli-0.5.7/PKG-INFO` & `datatrail_cli-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrail-cli
-Version: 0.5.7
+Version: 0.6.0
 Summary: CHIME/FRB Datatrail CLI
 License: MIT
 Author: CHIME FRB Project Office
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datatrail-cli Version: 0.5.7 Summary: CHIME/FRB
+Metadata-Version: 2.1 Name: datatrail-cli Version: 0.6.0 Summary: CHIME/FRB
 Datatrail CLI License: MIT Author: CHIME FRB Project Office Requires-Python:
 >=3.8.1,<4.0.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: cadcdata (>=2.5.0,<3.0.0) Requires-Dist: cadctap
 (>=0.9.11,<0.10.0) Requires-Dist: cadcutils (>=1.5.1.1,<2.0.0.0) Requires-Dist:
```

