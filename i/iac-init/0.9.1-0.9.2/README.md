# Comparing `tmp/iac_init-0.9.1.tar.gz` & `tmp/iac_init-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.9.1.tar", max compression
+gzip compressed data, was "iac_init-0.9.2.tar", max compression
```

## Comparing `iac_init-0.9.1.tar` & `iac_init-0.9.2.tar`

### file list

```diff
@@ -1,49 +1,50 @@
--rw-r--r--   0        0        0    16295 2024-05-30 07:30:09.858110 iac_init-0.9.1/LICENSE
--rw-r--r--   0        0        0     1622 2024-05-30 07:30:09.858110 iac_init-0.9.1/README.md
--rw-r--r--   0        0        0      392 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/__main__.py
--rw-r--r--   0        0        0    13430 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/cli/main.py
--rw-r--r--   0        0        0      228 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/cli/options.py
--rw-r--r--   0        0        0     1829 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     1199 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0     1585 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2921 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     7958 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      443 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0     1908 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0      415 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/scripts/thread_tool.py
--rw-r--r--   0        0        0     3778 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6989 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1370 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1557 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/03-nac_tasks/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/03-nac_tasks/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/03-nac_tasks/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/03-nac_tasks/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/03-nac_tasks/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/03-nac_tasks/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4924 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/utils/functional.py
--rw-r--r--   0        0        0    15022 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/validator.py
--rw-r--r--   0        0        0     5304 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5586 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1666 2024-05-30 07:30:09.866110 iac_init-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 iac_init-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-31 04:43:00.083419 iac_init-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1622 2024-05-31 04:43:00.083419 iac_init-0.9.2/README.md
+-rw-r--r--   0        0        0      392 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/__main__.py
+-rw-r--r--   0        0        0    13220 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/cli/main.py
+-rw-r--r--   0        0        0      228 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/cli/options.py
+-rw-r--r--   0        0        0     1829 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     1199 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0     2064 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2697 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     7744 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      438 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/scripts/log_tool.py
+-rw-r--r--   0        0        0      443 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0     1694 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0      416 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/scripts/thread_tool.py
+-rw-r--r--   0        0        0     3778 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-05-31 04:43:00.083419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1557 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/03-nac_tasks/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/03-nac_tasks/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/03-nac_tasks/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/03-nac_tasks/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/03-nac_tasks/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/templates/03-nac_tasks/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4924 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    14879 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/validator.py
+-rw-r--r--   0        0        0     5090 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5382 2024-05-31 04:43:00.087419 iac_init-0.9.2/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1666 2024-05-31 04:43:00.087419 iac_init-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 iac_init-0.9.2/PKG-INFO
```

### Comparing `iac_init-0.9.1/LICENSE` & `iac_init-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/README.md` & `iac_init-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/cli/main.py` & `iac_init-0.9.2/iac_init/cli/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,45 +6,36 @@
 import sys
 import click
 import shutil
 import errorhandler
 import iac_init.validator
 
 from . import options
-from loguru import logger
 from iac_init.conf import settings
 from iac_init.yaml_conf import yaml_writer
+from iac_init.scripts.log_tool import log_tool
 from iac_init.scripts.thread_tool import MyThread
 from iac_init.scripts.ansible_tool import ansible_deploy_function
 
 error_handler = errorhandler.ErrorHandler()
+logger = log_tool()
 
 
 @click.command(context_settings=dict(help_option_names=["-h", "--help"]))
 @click.version_option(iac_init.__version__)
 @options.yaml_dir_path
 def main(
         data: str
 ) -> None:
     """A CLI tool to bootstrap and configure ACI fabric using ACI as Code."""
     output = settings.OUTPUT_BASE_DIR
 
     if os.path.exists(output) and os.path.isdir(output):
         shutil.rmtree(output)
 
-    logger.add(
-        sink=os.path.join(
-            settings.OUTPUT_BASE_DIR,
-            'iac_init_log',
-            'iac_init_main.log'
-        ),
-        format='{time:YYYY-MM-DD HH:mm:ss} | {level} | {message}',
-        encoding='utf-8'
-    )
-
     validator = iac_init.validator.Validator(data, output)
 
     # Type single number or multiple numbers (1,2...)
     option_prompt = "Select single or multiple option(s) " \
                     "to init ACI Fabric:\n{}\nExample: (1,2,..)"\
         .format("\n".join([f"[{i + 1}]  {option}" for i, option
                            in enumerate(settings.DEFAULT_USER_OPTIONS)]))
```

### Comparing `iac_init-0.9.1/iac_init/conf/__init__.py` & `iac_init-0.9.2/iac_init/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/conf/global_settings.py` & `iac_init-0.9.2/iac_init/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.9.2/iac_init/scripts/apic_connecton_tool.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,17 @@
 # -*- coding: utf-8 -*-
 
 # Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
-import requests
-import os
 import json
 import urllib3
-from loguru import logger
-from iac_init.conf import settings
+import requests
+from iac_init.scripts.log_tool import log_tool
 
-# Rudy: need to check log setting
-logger.add(
-    sink=os.path.join(
-        settings.OUTPUT_BASE_DIR,
-        'iac_init_log',
-        'iac_init_main.log'
-    ),
-    format="{time} {level} {message}",
-    level="INFO"
-)
+logger = log_tool()
 
 urllib3.disable_warnings(
     urllib3.exceptions.InsecureRequestWarning
 )
 
 
 def get_health_status(APIC_IP, token):
```

### Comparing `iac_init-0.9.1/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.9.2/iac_init/scripts/cimc_precheck_tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,27 +4,17 @@
 
 import os
 import re
 import urllib3
 import requests
 import xml.etree.ElementTree as ET
 
-from loguru import logger
-from iac_init.conf import settings
+from iac_init.scripts.log_tool import log_tool
 
-# Rudy: need to check log setting
-logger.add(
-    sink=os.path.join(
-        settings.OUTPUT_BASE_DIR,
-        'iac_init_log',
-        'iac_init_main.log'
-    ),
-    format="{time} {level} {message}",
-    level="INFO"
-)
+logger = log_tool()
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 def cimc_api(CIMC_IP, data):
     try:
         cimc_url = f"https://{CIMC_IP}/nuova"
```

### Comparing `iac_init-0.9.1/iac_init/scripts/telnet_tool.py` & `iac_init-0.9.2/iac_init/scripts/telnet_tool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,16 @@
 # -*- coding: utf-8 -*-
 
 # Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
-import os
 import time
 import telnetlib
-from loguru import logger
-from iac_init.conf import settings
+from iac_init.scripts.log_tool import log_tool
 
-# Rudy: need to check log setting
-logger.add(
-    sink=os.path.join(
-        settings.OUTPUT_BASE_DIR,
-        'iac_init_log',
-        'iac_init_main.log'
-    ),
-    format="{time} {level} {message}",
-    level="INFO"
-)
+logger = log_tool()
 
 
 class TelnetClient:
     def __init__(
             self,
             telnet_ip,
             telnet_port,
@@ -34,15 +23,15 @@
         self.username = telnet_username
         self.password = telnet_password
 
     def login_host(self):
         try:
             self.tn.open(self.host_ip, self.port)
 
-        except:
+        except Exception:
             logger.error(
                 '{}:{} connected failed!'
                 .format(self.host_ip, self.port)
             )
             self.tn.close()
             return False
```

### Comparing `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.9.2/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.9.2/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.9.2/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.9.2/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.9.2/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/utils/functional.py` & `iac_init-0.9.2/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.1/iac_init/validator.py` & `iac_init-0.9.2/iac_init/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 # -*- coding: utf-8 -*-
 
 # Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 import os
 import re
 import time
+import yaml as pyyaml
 from ruamel import yaml
-
-from loguru import logger
 from typing import Any, Dict, List, Optional
 
 from iac_init.conf import settings
+from iac_init.scripts.log_tool import log_tool
 from iac_init.yaml_conf.yaml import load_yaml_files
 from iac_init.scripts.ssh_tool import check_ssh_connection
 from iac_init.scripts.apic_connecton_tool import apic_login
 from iac_init.scripts.cimc_precheck_tool import cimc_precheck
 from iac_init.scripts.telnet_tool import TelnetClient
 
-logger.add(sink=os.path.join(settings.OUTPUT_BASE_DIR,
-           'iac_init_log', 'iac_init_main.log'),
-           format='{time:YYYY-MM-DD HH:mm:ss} | {level} | {message}',
-           encoding='utf-8')
+logger = log_tool()
 
 
 class Validator:
     def __init__(self, data_path: str, output: str):
         self.data: Optional[Dict[str, Any]] = None
         self.data_path = data_path
         self.output = output
         self.global_policy = None
         self.errors: List[str] = []
         self._wrapped = self._validate_path
 
     def _validate_path(self):
-        '''Validate if user provided YAML directory exists'''
+        # Validate if user provided YAML directory exists
         if os.path.exists(self.data_path):
             if os.path.isdir(self.data_path):
                 pass
             else:
                 msg = "YAML directory must be a directory not a file: {}"\
                     .format(self.data_path)
                 logger.error(msg)
@@ -60,15 +57,15 @@
                 and \
                 (".yaml" in filename or ".yml" in filename):
             logger.info("Validated file: {} successfully.".format(filename))
 
             # YAML syntax validation
             try:
                 load_yaml_files([file_path])
-            except yaml.error.MarkedYAMLError as e:
+            except pyyaml.error.MarkedYAMLError as e:
                 line = 0
                 column = 0
                 if e.problem_mark is not None:
                     line = e.problem_mark.line + 1
                     column = e.problem_mark.column + 1
                 msg = "Syntax error '{}': Line {}, Column {} - {}".format(
                     file_path,
```

### Comparing `iac_init-0.9.1/iac_init/yaml_conf/yaml.py` & `iac_init-0.9.2/iac_init/yaml_conf/yaml.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,27 +4,17 @@
 
 import os
 import subprocess
 import importlib.util
 from typing import Any, Dict, List
 
 from ruamel import yaml
-from loguru import logger
-from iac_init.conf import settings
+from iac_init.scripts.log_tool import log_tool
 
-# Rudy: need to check log setting
-logger.add(
-    sink=os.path.join(
-        settings.OUTPUT_BASE_DIR,
-        'iac_init_log',
-        'iac_init_main.log'
-    ),
-    format="{time} {level} {message}",
-    level="INFO"
-)
+logger = log_tool()
 
 
 class VaultTag(yaml.YAMLObject):
     yaml_tag = "!vault"
 
     def __init__(self, v: str):
         self.value = v
```

### Comparing `iac_init-0.9.1/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.9.2/iac_init/yaml_conf/yaml_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,19 @@
 
 import json
 import os
 import pathlib
 import shutil
 
 from . import yaml
-from loguru import logger
 from typing import Any, Dict, List
+from iac_init.scripts.log_tool import log_tool
 from jinja2 import ChainableUndefined, Environment, FileSystemLoader
-from iac_init.conf import settings
 
-# Rudy: need to check log setting
-logger.add(
-    sink=os.path.join(
-        settings.OUTPUT_BASE_DIR,
-        'iac_init_log',
-        'iac_init_main.log'),
-    format="{time} {level} {message}", level="INFO")
+logger = log_tool()
 
 
 class YamlWriter:
     def __init__(
         self,
         data_paths: List[str],
     ) -> None:
```

### Comparing `iac_init-0.9.1/pyproject.toml` & `iac_init-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.9.1"
+version = "0.9.2"
 description = ""
 authors = ["Wang Xiao <xiawang3@cisco.com>", "Rudy Lei <shlei@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
```

### Comparing `iac_init-0.9.1/PKG-INFO` & `iac_init-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iac-init
-Version: 0.9.1
+Version: 0.9.2
 Summary: 
 Author: Wang Xiao
 Author-email: xiawang3@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

