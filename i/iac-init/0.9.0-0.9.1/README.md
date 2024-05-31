# Comparing `tmp/iac_init-0.9.0.tar.gz` & `tmp/iac_init-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iac_init-0.9.0.tar", max compression
+gzip compressed data, was "iac_init-0.9.1.tar", max compression
```

## Comparing `iac_init-0.9.0.tar` & `iac_init-0.9.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    16295 2024-05-30 05:48:09.408414 iac_init-0.9.0/LICENSE
--rw-r--r--   0        0        0        0 2024-05-30 05:48:09.408414 iac_init-0.9.0/README.md
--rw-r--r--   0        0        0      392 2024-05-30 05:48:09.408414 iac_init-0.9.0/iac_init/__init__.py
--rw-r--r--   0        0        0      162 2024-05-30 05:48:09.408414 iac_init-0.9.0/iac_init/__main__.py
--rw-r--r--   0        0        0    13438 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/cli/main.py
--rw-r--r--   0        0        0      228 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/cli/options.py
--rw-r--r--   0        0        0     1827 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/conf/__init__.py
--rw-r--r--   0        0        0     1166 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/conf/global_settings.py
--rw-r--r--   0        0        0     1583 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/scripts/ansible_tool.py
--rw-r--r--   0        0        0     2847 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/scripts/apic_connecton_tool.py
--rw-r--r--   0        0        0     7992 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/scripts/cimc_precheck_tool.py
--rw-r--r--   0        0        0      443 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/scripts/ssh_tool.py
--rw-r--r--   0        0        0     1871 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/scripts/telnet_tool.py
--rw-r--r--   0        0        0      336 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/scripts/thread_tool.py
--rw-r--r--   0        0        0     3778 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
--rw-r--r--   0        0        0     5040 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
--rw-r--r--   0        0        0     1860 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
--rw-r--r--   0        0        0     6989 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
--rw-r--r--   0        0        0     1370 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
--rw-r--r--   0        0        0     5598 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
--rw-r--r--   0        0        0     1516 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
--rw-r--r--   0        0        0     1607 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
--rw-r--r--   0        0        0     1553 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
--rw-r--r--   0        0        0      790 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
--rw-r--r--   0        0        0      197 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
--rw-r--r--   0        0        0      194 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
--rw-r--r--   0        0        0        0 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
--rw-r--r--   0        0        0     1557 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
--rw-r--r--   0        0        0     3527 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
--rw-r--r--   0        0        0     3585 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
--rw-r--r--   0        0        0     1656 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
--rw-r--r--   0        0        0        0 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
--rw-r--r--   0        0        0      181 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
--rw-r--r--   0        0        0      388 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/03-nac-tasks/aac_ansible/apic_deploy.yaml
--rw-r--r--   0        0        0      215 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/03-nac-tasks/aac_ansible/apic_test.yaml
--rw-r--r--   0        0        0      163 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/03-nac-tasks/aac_ansible/apic_validate.yaml
--rw-r--r--   0        0        0      237 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/03-nac-tasks/group_vars/aci.yaml.j2
--rw-r--r--   0        0        0        0 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/03-nac-tasks/host_vars/apic1/.gitkeep
--rw-r--r--   0        0        0      169 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/templates/03-nac-tasks/inventory.yaml.j2
--rw-r--r--   0        0        0      101 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/utils/exceptions.py
--rw-r--r--   0        0        0     4924 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/utils/functional.py
--rw-r--r--   0        0        0    14664 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/validator.py
--rw-r--r--   0        0        0     5269 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/yaml_conf/yaml.py
--rw-r--r--   0        0        0     5542 2024-05-30 05:48:09.412413 iac_init-0.9.0/iac_init/yaml_conf/yaml_writer.py
--rw-r--r--   0        0        0     1636 2024-05-30 05:48:09.416413 iac_init-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 iac_init-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    16295 2024-05-30 07:30:09.858110 iac_init-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1622 2024-05-30 07:30:09.858110 iac_init-0.9.1/README.md
+-rw-r--r--   0        0        0      392 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/__init__.py
+-rw-r--r--   0        0        0      162 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/__main__.py
+-rw-r--r--   0        0        0    13430 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/cli/main.py
+-rw-r--r--   0        0        0      228 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/cli/options.py
+-rw-r--r--   0        0        0     1829 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/conf/__init__.py
+-rw-r--r--   0        0        0     1199 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/conf/global_settings.py
+-rw-r--r--   0        0        0     1585 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/scripts/ansible_tool.py
+-rw-r--r--   0        0        0     2921 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/scripts/apic_connecton_tool.py
+-rw-r--r--   0        0        0     7958 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/scripts/cimc_precheck_tool.py
+-rw-r--r--   0        0        0      443 2024-05-30 07:30:09.858110 iac_init-0.9.1/iac_init/scripts/ssh_tool.py
+-rw-r--r--   0        0        0     1908 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/scripts/telnet_tool.py
+-rw-r--r--   0        0        0      415 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/scripts/thread_tool.py
+-rw-r--r--   0        0        0     3778 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh
+-rw-r--r--   0        0        0     5040 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64
+-rw-r--r--   0        0        0     1860 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     6989 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2
+-rw-r--r--   0        0        0     1370 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/files/.gitkeep
+-rw-r--r--   0        0        0     5598 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml
+-rw-r--r--   0        0        0     1516 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2
+-rw-r--r--   0        0        0     1607 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2
+-rw-r--r--   0        0        0     1553 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2
+-rw-r--r--   0        0        0      790 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/vars/.gitkeep
+-rw-r--r--   0        0        0      197 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/playbook_aci_switch_init.yaml
+-rw-r--r--   0        0        0      194 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/playbook_apic_init.yaml
+-rw-r--r--   0        0        0        0 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/files/.gitkeep
+-rw-r--r--   0        0        0     1557 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml
+-rw-r--r--   0        0        0     3527 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2
+-rw-r--r--   0        0        0     3585 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2
+-rw-r--r--   0        0        0     1656 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2
+-rw-r--r--   0        0        0        0 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/vars/.gitkeep
+-rw-r--r--   0        0        0      181 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/02-discover_apic/playbook_apic_discovery.yaml
+-rw-r--r--   0        0        0      388 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/03-nac_tasks/aac_ansible/apic_deploy.yaml
+-rw-r--r--   0        0        0      215 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/03-nac_tasks/aac_ansible/apic_test.yaml
+-rw-r--r--   0        0        0      163 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/03-nac_tasks/aac_ansible/apic_validate.yaml
+-rw-r--r--   0        0        0      237 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/03-nac_tasks/group_vars/aci.yaml.j2
+-rw-r--r--   0        0        0        0 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/03-nac_tasks/host_vars/apic1/.gitkeep
+-rw-r--r--   0        0        0      169 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/templates/03-nac_tasks/inventory.yaml.j2
+-rw-r--r--   0        0        0      101 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/utils/exceptions.py
+-rw-r--r--   0        0        0     4924 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/utils/functional.py
+-rw-r--r--   0        0        0    15022 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/validator.py
+-rw-r--r--   0        0        0     5304 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/yaml_conf/yaml.py
+-rw-r--r--   0        0        0     5586 2024-05-30 07:30:09.862110 iac_init-0.9.1/iac_init/yaml_conf/yaml_writer.py
+-rw-r--r--   0        0        0     1666 2024-05-30 07:30:09.866110 iac_init-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 iac_init-0.9.1/PKG-INFO
```

### Comparing `iac_init-0.9.0/LICENSE` & `iac_init-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/cli/main.py` & `iac_init-0.9.1/iac_init/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
+# Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 import os
 import sys
 import click
 import shutil
 import errorhandler
 import iac_init.validator
@@ -21,110 +21,111 @@
 
 @click.command(context_settings=dict(help_option_names=["-h", "--help"]))
 @click.version_option(iac_init.__version__)
 @options.yaml_dir_path
 def main(
         data: str
 ) -> None:
-    """A CLI tool to perform APIC initialize."""
+    """A CLI tool to bootstrap and configure ACI fabric using ACI as Code."""
     output = settings.OUTPUT_BASE_DIR
 
     if os.path.exists(output) and os.path.isdir(output):
         shutil.rmtree(output)
 
     logger.add(
         sink=os.path.join(
             settings.OUTPUT_BASE_DIR,
             'iac_init_log',
-            'iac-init-main.log'
+            'iac_init_main.log'
         ),
         format='{time:YYYY-MM-DD HH:mm:ss} | {level} | {message}',
         encoding='utf-8'
     )
 
     validator = iac_init.validator.Validator(data, output)
 
-    # Type single number or multiple number (1,2...)
-    option_prompt = "Select single or multiple options " \
-                    "to init APIC:\n{}\nExample: (1,2,..)"\
+    # Type single number or multiple numbers (1,2...)
+    option_prompt = "Select single or multiple option(s) " \
+                    "to init ACI Fabric:\n{}\nExample: (1,2,..)"\
         .format("\n".join([f"[{i + 1}]  {option}" for i, option
                            in enumerate(settings.DEFAULT_USER_OPTIONS)]))
     option_choice = click.prompt(
         click.style(option_prompt, fg='green'),
         type=validator.validate_choices)
     if not option_choice:
         exit()
 
-    # Type "yes" or "no" to preform APIC initiator
-    option_prompt = "\nAre you sure proceed init following Procedures!?\n{}\n"\
+    # Type "yes" or "no" to confirm
+    option_prompt = "\nAre you sure to proceed with following option(s)?\n{}\n"\
         .format("\n".join([f"[{i}]  {settings.DEFAULT_USER_OPTIONS[int(i)-1]}"
                            for i in option_choice]))
     option_proceed = click.prompt(
         click.style(option_prompt, fg='green'),
         type=click.Choice(['yes', 'no'], case_sensitive=False)
     )
     validator._validate_bool(option_proceed)
 
     error = validator._wrapped()
     if error:
+        logger.error("Option(s) validated failed, exiting...")
         exit()
-    logger.info("Initial Validation of Yamls Directory Success!!")
+    logger.info("Option(s) validated.")
 
     for option in option_choice:
-        logger.info("Start proceeding step {}.".format(option))
+        logger.info("Start processing step {}.".format(option))
         if int(option) in [1]:
             error = validator.validate_ssh_telnet_connection()
             if error:
                 exit()
             yaml_path = validator.validate_yaml_exist(
                 settings.DEFAULT_DATA_PATH
             )
             if not yaml_path:
                 exit()
             error = validator.validate_cimc_precheck()
             if error:
                 exit()
+            # Rudy: If only 1, this might not need to check
             option_yaml_path = validator.validate_yaml_exist(
                 settings.DATA_PATH[int(option)-1]
             )
             if not option_yaml_path:
                 exit()
             try:
                 writer = yaml_writer.YamlWriter([yaml_path])
                 writer.write(settings.TEMPLATE_DIR[int(option) - 1], output)
-                logger.info("Generate Step {} working directory forder"
-                            " in {} Success!!"
+                logger.info("Generate step {} working directory in {} successfully."
                             .format(option, output))
 
                 dir_path = os.path.join(
                     output,
                     os.path.basename(settings.TEMPLATE_DIR[int(option)-1]),
                     'aci_switch_reimage',
                     'vars'
                 )
                 if os.path.exists(dir_path) and os.path.isdir(dir_path):
                     yaml_cp_output_path = os.path.join(dir_path, 'main.yml')
                     shutil.copy(option_yaml_path, yaml_cp_output_path)
-                    logger.info("Copied Yaml file to {} success."
+                    logger.info("Copied switch YAML file to {} successfully."
                                 .format(yaml_cp_output_path))
 
                 dir_path = os.path.join(
                     output,
                     os.path.basename(settings.TEMPLATE_DIR[int(option)-1]),
                     'apic_reimage',
                     'vars'
                 )
                 if os.path.exists(dir_path) and os.path.isdir(dir_path):
                     yaml_cp_output_path = os.path.join(dir_path, 'main.yml')
                     shutil.copy(option_yaml_path, yaml_cp_output_path)
-                    logger.info("Copied Yaml file to {} success."
+                    logger.info("Copied APIC YAML file to {} successfully."
                                 .format(yaml_cp_output_path))
 
             except Exception as e:
-                msg = "Generate working directory fail, detail: {}".format(e)
+                msg = "Generate working directory failed.\nDetail: {}".format(e)
                 logger.error(msg)
                 exit()
 
             try:
                 playbook_dir_apic = os.path.join(
                     os.getcwd(),
                     output,
@@ -154,35 +155,35 @@
                         playbook_dir_switch,
                         settings.ANSIBLE_STEP[4],
                         option,
                         None,
                         True)
                 )
 
-                logger.info("Wipe aci fabric start pls wait, "
-                            "check log for detail.")
+                logger.info("ACI fabric bootstrap in progress, "
+                            "check APIC/switch logs for detail.")
 
                 thread1.start()
                 thread2.start()
 
                 thread1.join()
                 thread2.join()
 
                 if thread1.get_result() and thread2.get_result():
-                    logger.info("Wipe aci fabric Success proceed.")
+                    logger.info("ACI fabric bootstrap is successfully.")
                 else:
                     logger.error(
-                        "Exist iac-init tool Step 1 failed "
-                        "pls check log for detail"
+                        "ACI fabric bootstrap failed, "
+                        "check APIC/switch logs for detail."
                     )
                     exit()
 
             except Exception as e:
-                msg = "Run Step 1 wipe aci fabric ansible-playbook" \
-                      " failed detail:\nError: {}".format(e)
+                msg = "Run Step 1 ACI fabric bootstrap ansible-playbook" \
+                      " failed.\nDetail: {}".format(e)
                 logger.error(msg)
                 exit()
 
         elif int(option) in [2]:
             yaml_path = validator.validate_yaml_exist(
                 settings.DEFAULT_DATA_PATH
             )
@@ -196,34 +197,34 @@
             )
             if not option_yaml_path:
                 exit()
             try:
                 writer = yaml_writer.YamlWriter([yaml_path])
                 writer.write(settings.TEMPLATE_DIR[int(option)-1], output)
                 logger.info(
-                    "Generate Step {} working directory forder in {} Success!!"
+                    "Generate step {} working directory in {} successfully."
                     .format(option, output)
                 )
 
                 dir_path = os.path.join(
                     output,
                     os.path.basename(settings.TEMPLATE_DIR[int(option)-1]),
                     'apic_discovery',
                     'vars'
                 )
                 if os.path.exists(dir_path) and os.path.isdir(dir_path):
                     yaml_cp_output_path = os.path.join(dir_path, 'main.yml')
                     shutil.copy(option_yaml_path, yaml_cp_output_path)
                     logger.info(
-                        "Copied Yaml file to {} success."
+                        "Copied APIC YAML file to {} successfully."
                         .format(yaml_cp_output_path)
                     )
 
             except Exception as e:
-                msg = "Generate working directory fail, detail: {}".format(e)
+                msg = "Generate working directory failed.\nDetail: {}".format(e)
                 logger.error(msg)
                 exit()
 
             try:
                 playbook_dir = os.path.join(
                     os.getcwd(),
                     output,
@@ -234,25 +235,22 @@
                 run_result = ansible_deploy_function(
                     playbook_dir=playbook_dir,
                     step_name=settings.ANSIBLE_STEP[5],
                     option=option,
                     quiet=False
                 )
                 if run_result:
-                    logger.info("Run step 2 APIC discovery "
-                                "ansible-playbook successfully.")
+                    logger.info("APIC init successfully.")
                 else:
-                    msg = "Run Step 2 APIC discovery ansible-playbook failed"
-                    logger.error(msg)
+                    logger.error("APIC init failed!")
                     exit()
 
             except Exception as e:
-                msg = "Run Step 2 APIC discovery " \
-                      "ansible-playbook fail detail:\nError: {}"\
-                    .format(e)
+                msg = "Run Step 2 APIC init ansible-playbook" \
+                      " failed.\nDetail: {}".format(e)
                 logger.error(msg)
                 exit()
 
         elif int(option) in [3]:
             error = validator.validate_apic_aaa_connection()
             if error:
                 exit()
@@ -269,15 +267,15 @@
             try:
                 writer = yaml_writer.YamlWriter([yaml_path])
                 writer.write(
                     settings.TEMPLATE_DIR[int(option)-1],
                     output
                 )
                 logger.info(
-                    "Generate Step {} working directory forder in {} Success!!"
+                    "Generate step {} working directory in {} successfully."
                     .format(option, output)
                 )
                 dir_path = os.path.join(
                     output,
                     os.path.basename(settings.TEMPLATE_DIR[int(option)-1]),
                     'host_vars',
                     'apic1'
@@ -291,15 +289,15 @@
                         option_yaml_path,
                         yaml_cp_output_path
                     )
                     if not result:
                         exit()
 
             except Exception as e:
-                msg = "Generate working directory fail, detail: {}"\
+                msg = "Generate working directory failed.\nDetail: {}"\
                     .format(e)
                 logger.error(msg)
                 exit()
 
             try:
                 inventory_path = os.path.join(
                     os.getcwd(),
@@ -360,16 +358,16 @@
                     quiet=False
                 )
 
                 if not test_result:
                     exit()
 
             except Exception as e:
-                msg = "Run NAC ansible-playbook fail detail:\nError: {}"\
-                    .format(e)
+                msg = "Run Step 3 NaC ansible-playbook" \
+                      " failed.\nDetail: {}".format(e)
                 logger.error(msg)
                 exit()
 
 
 def exit() -> None:
     if error_handler.fired:
         sys.exit(1)
```

### Comparing `iac_init-0.9.0/iac_init/conf/__init__.py` & `iac_init-0.9.1/iac_init/conf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
-# Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
+# Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 from iac_init.conf import global_settings
 from iac_init.utils.functional import LazyObject, empty
 
-ENVIRONMENT_VARIABLE = "IAC_INIT_SETTINGS_MODULE"
+# ENVIRONMENT_VARIABLE = "IAC_INIT_SETTINGS_MODULE"
 
 
 class SettingsReference(str):
     """
     String subclass which references a current settings value. It's treated as
     the value in memory but serializes to a settings.NAME attribute reference.
     """
```

### Comparing `iac_init-0.9.0/iac_init/conf/global_settings.py` & `iac_init-0.9.1/iac_init/conf/global_settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
+# Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 import os.path
 from pathlib import Path
 
 BASE_DIR = Path(__file__).resolve().parent.parent
 
 OUTPUT_BASE_DIR = os.path.join(os.getcwd(), "iac_init_output_working_dir")
@@ -23,26 +23,27 @@
     "00-global_policy.yml",
     "nac_data",
 ]
 
 TEMPLATE_DIR = [
     os.path.join(BASE_DIR, "templates", "01-wipe_aci_fabric"),
     os.path.join(BASE_DIR, "templates", "02-discover_apic"),
-    os.path.join(BASE_DIR, "templates", "03-nac-tasks"),
+    os.path.join(BASE_DIR, "templates", "03-nac_tasks"),
 ]
 
 OUTPUT_DIR = [
     os.path.join(OUTPUT_BASE_DIR, "01-wipe_aci_fabric"),
     os.path.join(OUTPUT_BASE_DIR, "02-discover_apic"),
-    os.path.join(OUTPUT_BASE_DIR, "03-nac-tasks"),
+    os.path.join(OUTPUT_BASE_DIR, "03-nac_tasks"),
 ]
 
 os.environ["iac_init_option_1"] = OUTPUT_DIR[0]
 os.environ["iac_init_option_2"] = OUTPUT_DIR[1]
 
+# Rudy: sync the step name later
 ANSIBLE_STEP = [
     'iac-validate',
     'deploy',
     'iac-test',
     'wipe_apic',
     'wipe_switch',
     'apic_setup'
```

### Comparing `iac_init-0.9.0/iac_init/scripts/ansible_tool.py` & `iac_init-0.9.1/iac_init/scripts/ansible_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
+# Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 import re
 import os
 from ansible_runner import run
 from iac_init.conf import settings
 
 
@@ -16,15 +16,15 @@
     from logging.handlers import RotatingFileHandler
 
     logger = logging.getLogger(playbook_dir)
     logger.setLevel(logging.INFO)
     log_formatter = logging.Formatter('%(message)s')
     log_file = os.path.join(settings.OUTPUT_BASE_DIR,
                             'iac_init_log',
-                            'iac-init-{}-{}.log'.format(option, step_name))
+                            'iac_init_{}_{}.log'.format(option, step_name))
     file_handler = RotatingFileHandler(
         log_file,
         maxBytes=30*1024*1024,
         backupCount=0
     )
 
     file_handler.setFormatter(log_formatter)
@@ -40,15 +40,15 @@
     runner = run(playbook=playbook_dir,
                  inventory=inventory_path,
                  verbosity=5,
                  quiet=True,
                  event_handler=callback)
 
     if runner.status == "successful":
-        logger.info("Successfully finish Step {}: {}"
+        logger.info("Successfully finished Step {}: {}"
                     .format(option, step_name.upper()))
         return True
 
     else:
         logger.error("Failed run Step {}: {}"
                      .format(option, step_name.upper()))
         return False
```

### Comparing `iac_init-0.9.0/iac_init/scripts/apic_connecton_tool.py` & `iac_init-0.9.1/iac_init/scripts/apic_connecton_tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 
-# Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
+# Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 import requests
 import os
 import json
 import urllib3
 from loguru import logger
 from iac_init.conf import settings
 
+# Rudy: need to check log setting
 logger.add(
     sink=os.path.join(
         settings.OUTPUT_BASE_DIR,
         'iac_init_log',
-        'iac-init-main.log'
+        'iac_init_main.log'
     ),
     format="{time} {level} {message}",
     level="INFO"
 )
 
 urllib3.disable_warnings(
     urllib3.exceptions.InsecureRequestWarning
@@ -42,27 +43,27 @@
             return_data = response.json()
             for item in return_data['imdata']:
                 health_status.append(
                     item['infraWiNode']['attributes']['health']
                 )
             for status in health_status:
                 if status != "fully-fit":
-                    msg = "Error: APIC {} Health Check fail(Not fully-fix)!!"\
+                    msg = "APIC {} Health Check failed(Not fully-fit)!"\
                         .format(APIC_IP)
                     logger.error(msg)
                     return False
             return True
         else:
             return False
     except Exception as e:
         msg = "{}".format(e)
         logger.error(msg)
         return False
 
-
+# Rudy: discuss AAA domain later
 def apic_login(APIC_IP, APIC_USERNAME, APIC_PASSWORD):
     try:
         apic_login_url = f"https://{APIC_IP}/api/aaaLogin.json"
         headers = {
             'accept': 'application/json',
             'Content-Type': 'application/json',
         }
@@ -84,18 +85,18 @@
 
         if response.status_code == 200:
             res_json = response.json()
             token = res_json["imdata"][0]["aaaLogin"]["attributes"]["token"]
             if token:
                 return get_health_status(APIC_IP, token)
             else:
-                msg = "Error: APIC {} Connection Fail!!".format(APIC_IP)
+                msg = "APIC {} connected failed(no token)!".format(APIC_IP)
                 logger.error(msg)
                 return False
         else:
-            msg = "Error: APIC {} Connection Fail!!".format(APIC_IP)
+            msg = "APIC {} connected failed(not 200 response)!".format(APIC_IP)
             logger.error(msg)
             return False
     except Exception as e:
         msg = "{}".format(e)
         logger.error(msg)
         return False
```

### Comparing `iac_init-0.9.0/iac_init/scripts/cimc_precheck_tool.py` & `iac_init-0.9.1/iac_init/scripts/cimc_precheck_tool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 # -*- coding: utf-8 -*-
 
-# Copyright: (c) 2022, Rudy Lei <shlei@cisco.com>
-
-# This is for APIC CIMC pre check,
-# run this pre check when option 1 is selected,
-# apply this for all APICs.
-
+# Copyright: (c) 2024, Rudy Lei <shlei@cisco.com>
 
 import os
 import re
 import urllib3
 import requests
 import xml.etree.ElementTree as ET
 
 from loguru import logger
 from iac_init.conf import settings
 
+# Rudy: need to check log setting
 logger.add(
     sink=os.path.join(
         settings.OUTPUT_BASE_DIR,
         'iac_init_log',
-        'iac-init-main.log'
+        'iac_init_main.log'
     ),
     format="{time} {level} {message}",
     level="INFO"
 )
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
@@ -43,15 +39,15 @@
             data=data,
             verify=False
         )
 
         if response.status_code == 200:
             return response
         else:
-            msg = f"Error: CIMC {CIMC_IP} Connection Fail!!"
+            msg = f"APIC CIMC {CIMC_IP} connected failed!"
             logger.error(msg)
             return False
     except Exception as e:
         msg = "{}".format(e)
         logger.error(msg)
         return False
 
@@ -59,32 +55,32 @@
 def cimc_login(CIMC_IP, CIMC_USERNAME, CIMC_PASSWORD):
     try:
         data = f"<aaaLogin inName='{CIMC_USERNAME}' " \
                f"inPassword='{CIMC_PASSWORD}'></aaaLogin>"
         response = cimc_api(CIMC_IP, data)
         token = ET.fromstring(response.text).attrib['outCookie']
         if token:
-            logger.info(f"Login token: {token}")
+            logger.info(f"CIMC Login token: {token}")
             return token
         else:
-            msg = f"Error: CIMC {CIMC_IP} Login Fail!!"
+            msg = f"CIMC {CIMC_IP} Login failed!"
             logger.error(msg)
             return False
 
     except Exception as e:
         msg = "{}".format(e)
         logger.error(msg)
         return False
 
 
 def cimc_logout(CIMC_IP, token):
     try:
         data = f"<aaaLogout cookie='{token}'inCookie='{token}'> </aaaLogout>"
         cimc_api(CIMC_IP, data)
-        logger.info(f"Logout {token} successfully!")
+        logger.info(f"Logout CIMC {CIMC_IP} with token {token} successfully.")
 
     except Exception as e:
         msg = "{}".format(e)
         logger.error(msg)
         return False
 
 
@@ -92,15 +88,15 @@
     try:
         firmware_data = f'''
         <!-- firmware version -->
         <configResolveDn cookie="{token}" inHierarchical='false'
         dn="sys/rack-unit-1/mgmt/fw-system"/>
         '''
         firmware_response = cimc_api(CIMC_IP, firmware_data)
-        logger.info(firmware_response.text)
+        # logger.info(firmware_response.text)
         firmware_version = ET.fromstring(
             firmware_response.text).find(
             './/firmwareRunning').attrib['version']
         logger.info(f"Current Firmware version is: {firmware_version}")
 
         fault_data = f'''
         <!-- fault info -->
@@ -113,21 +109,21 @@
 
         tpm_data = f'''
         <!-- TPM status -->
         <configResolveClass cookie="{token}"
         inHierarchical='false' classId='equipmentTpm'/>
         '''
         tpm_response = cimc_api(CIMC_IP, tpm_data)
-        logger.info(tpm_response.text)
+        # logger.info(tpm_response.text)
         tpm_status = ET.fromstring(tpm_response.text).find(
             './/equipmentTpm').attrib['enabledStatus']
         logger.info(f"Current TPM status is: {tpm_status}")
 
         if "enable" not in tpm_status:
-            logger.error("TPM is not enabled!!")
+            logger.error(f"CIMC {CIMC_IP}: TPM is not enabled!")
             return False
 
         return True
 
     except Exception as e:
         msg = "{}".format(e)
         logger.error(msg)
@@ -138,15 +134,15 @@
     try:
         cimc_mapping_data = f'''
         <!-- Retrieve CIMC mapping -->
         <configResolveClass cookie="{token}"
         inHierarchical='false' classId='commVMediaMap'/>
         '''
         cimc_mapping_response = cimc_api(CIMC_IP, cimc_mapping_data)
-        logger.info(cimc_mapping_response.text)
+        # logger.info(cimc_mapping_response.text)
         if re.search(r'commVMediaMap volumeName', cimc_mapping_response.text):
             existing_mapping = ET.fromstring(
                 cimc_mapping_response.text).find(
                 './/commVMediaMap').attrib['volumeName']
             logger.info(f"Removing existing mapping: {existing_mapping}")
             cimc_mapping_clear_data = f'''
             <!-- CIMC mapping clear -->
@@ -168,15 +164,15 @@
 
         cimc_boot_data = f'''
         <!-- Retrieve CIMC boot order -->
         <configResolveClass cookie="{token}"
         inHierarchical='false' classId='lsbootVMedia'/>
         '''
         cimc_boot_data_response = cimc_api(CIMC_IP, cimc_boot_data)
-        logger.info(cimc_boot_data_response.text)
+        # logger.info(cimc_boot_data_response.text)
         if re.search(r'lsbootVMedia name', cimc_boot_data_response.text):
             existing_bootorder = ET.fromstring(
                 cimc_boot_data_response.text).find(
                 './/lsbootVMedia').attrib['name']
             logger.info(f"Removing existing boot order: {existing_bootorder}")
             cimc_bootorder_clear_data = f'''
             <!-- CIMC boot order clear -->
@@ -228,28 +224,28 @@
 
 
 def cimc_precheck(CIMC_IP, CIMC_USERNAME, CIMC_PASSWORD):
     try:
         token = cimc_login(CIMC_IP, CIMC_USERNAME, CIMC_PASSWORD)
         health_check_result = cimc_health_check(CIMC_IP, token)
         if not health_check_result:
-            logger.error("CIMC health check failed!!")
+            logger.error("CIMC health check failed!")
             return False
 
         logger.info("CIMC health check pass!")
 
         cimc_mapping_clean_result = cimc_mapping_clean(
             CIMC_IP,
             token
         )
         if not cimc_mapping_clean_result:
-            logger.error("CIMC mapping clean failed!!")
+            logger.error("CIMC mapping clean failed!")
             return False
 
-        logger.info("CIMC mapping clean successfully!")
+        logger.info("CIMC mapping clean successfully.")
         logger.info("Powering down CIMC...")
         power_down_cimc(CIMC_IP, token)
         cimc_logout(CIMC_IP, token)
         return True
 
     except Exception as e:
         msg = "{}".format(e)
```

### Comparing `iac_init-0.9.0/iac_init/scripts/telnet_tool.py` & `iac_init-0.9.1/iac_init/scripts/telnet_tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 
-# Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
+# Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 import os
 import time
 import telnetlib
 from loguru import logger
 from iac_init.conf import settings
 
+# Rudy: need to check log setting
 logger.add(
     sink=os.path.join(
         settings.OUTPUT_BASE_DIR,
         'iac_init_log',
-        'iac-init-main.log'
+        'iac_init_main.log'
     ),
     format="{time} {level} {message}",
     level="INFO"
 )
 
 
 class TelnetClient:
@@ -34,37 +35,37 @@
         self.password = telnet_password
 
     def login_host(self):
         try:
             self.tn.open(self.host_ip, self.port)
 
         except:
-            logger.warning(
-                '{}:{} Network Connection Issue'
+            logger.error(
+                '{}:{} connected failed!'
                 .format(self.host_ip, self.port)
             )
             self.tn.close()
             return False
 
         self.tn.read_until(b'login: ', timeout=10)
         self.tn.write(self.username.encode('ascii') + b'\n')
         self.tn.read_until(b'Password: ', timeout=10)
         self.tn.write(self.password.encode('ascii') + b'\n')
         time.sleep(2)
         command_result = self.tn.read_very_eager()\
             .decode('ascii')
-        print(command_result)
+        # print(command_result)
         if 'Login incorrect' not in command_result:
             logger.info(
-                '{}:{} Login Success!!'
+                'Login {}:{} successfully.'
                 .format(self.host_ip, self.port)
             )
             self.tn.write(b"exit\n")
             self.tn.close()
             return True
         else:
-            logger.warning(
-                '{}:{} Login Failed wrong username or password'
+            logger.error(
+                'Login {}:{} failed due to wrong username or password!'
                 .format(self.host_ip, self.port)
             )
             self.tn.close()
             return False
```

### Comparing `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh` & `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge.sh`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64` & `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/files/aci_switch_reiamge_sh_base64`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml` & `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2` & `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2` & `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/aci_switch_reimage/templates/aci_switch_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml` & `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2` & `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2` & `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2` & `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2` & `iac_init-0.9.1/iac_init/templates/01-wipe_aci_fabric/apic_reimage/templates/apic_reimage_post_check.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml` & `iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2` & `iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery4.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2` & `iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery5.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2` & `iac_init-0.9.1/iac_init/templates/02-discover_apic/apic_discovery/templates/apic_discovery6.exp.jinja2`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/utils/functional.py` & `iac_init-0.9.1/iac_init/utils/functional.py`

 * *Files identical despite different names*

### Comparing `iac_init-0.9.0/iac_init/validator.py` & `iac_init-0.9.1/iac_init/validator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 
-# Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
+# Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 import os
 import re
 import time
 from ruamel import yaml
 
 from loguru import logger
@@ -14,56 +14,56 @@
 from iac_init.yaml_conf.yaml import load_yaml_files
 from iac_init.scripts.ssh_tool import check_ssh_connection
 from iac_init.scripts.apic_connecton_tool import apic_login
 from iac_init.scripts.cimc_precheck_tool import cimc_precheck
 from iac_init.scripts.telnet_tool import TelnetClient
 
 logger.add(sink=os.path.join(settings.OUTPUT_BASE_DIR,
-           'iac_init_log', 'iac-init-main.log'),
+           'iac_init_log', 'iac_init_main.log'),
            format='{time:YYYY-MM-DD HH:mm:ss} | {level} | {message}',
            encoding='utf-8')
 
 
 class Validator:
     def __init__(self, data_path: str, output: str):
         self.data: Optional[Dict[str, Any]] = None
         self.data_path = data_path
         self.output = output
         self.global_policy = None
         self.errors: List[str] = []
         self._wrapped = self._validate_path
 
     def _validate_path(self):
-        '''Validate if user provided yaml directory exist'''
+        '''Validate if user provided YAML directory exists'''
         if os.path.exists(self.data_path):
             if os.path.isdir(self.data_path):
                 pass
             else:
-                msg = "Yaml Directory must be a directory not a file.: {}"\
+                msg = "YAML directory must be a directory not a file: {}"\
                     .format(self.data_path)
                 logger.error(msg)
                 self.errors.append(msg)
                 return True
         else:
-            msg = "Yaml Directory not exist.: {}".format(self.data_path)
+            msg = "YAML Directory doesn't exist: {}".format(self.data_path)
             logger.error(msg)
             self.errors.append(msg)
             return True
 
-        logger.info("Loaded Yaml directory: {}".format(self.data_path))
+        logger.info("Loaded YAML directory: {}".format(self.data_path))
 
         return self._validate_yaml()
 
     def _validate_syntax_file(self, file_path: str):
         """Run syntactic validation for a single file"""
         filename = os.path.basename(file_path)
         if os.path.isfile(file_path) \
                 and \
                 (".yaml" in filename or ".yml" in filename):
-            logger.info("Validate file: {}".format(filename))
+            logger.info("Validated file: {} successfully.".format(filename))
 
             # YAML syntax validation
             try:
                 load_yaml_files([file_path])
             except yaml.error.MarkedYAMLError as e:
                 line = 0
                 column = 0
@@ -84,15 +84,15 @@
             for filename in files:
                 self._validate_syntax_file(os.path.join(dir, filename))
                 if settings.DEFAULT_DATA_PATH == filename:
                     self.global_policy = os.path.join(dir, filename)
         if self.global_policy:
             settings.global_policy = load_yaml_files([self.global_policy])
         else:
-            msg = "Configuration File {} not fount"\
+            msg = "Configuration File {} is missing!"\
                 .format(settings.DEFAULT_DATA_PATH)
             logger.error(msg)
             self.errors.append(msg)
             return True
 
         return self._load_connnection_info()
 
@@ -152,30 +152,30 @@
             return True
 
     def _validate_ip(self):
         pattern = r'^((25[0-5]|2[0-4]\d|[01]?\d\d?)\.)' \
                   r'{3}(25[0-5]|2[0-4]\d|[01]?\d\d?)$'
         fail_ip_list = []
         if self.total_ip_list:
-            msg = "Validate Error: " \
-                  "Below IP can not meet IP Address Format.\n"
+            msg = "Validation Error: " \
+                  "Below IP(s) can not meet IP Address Format!\n"
             for ip in self.total_ip_list:
                 p = re.compile(pattern)
                 if not p.match(ip):
                     fail_ip_list.append(ip)
                     msg = msg + "{}".format(ip)
 
             if fail_ip_list:
                 logger.error(msg)
                 self.errors.append(msg)
                 return True
             else:
                 return self._validate_image_version()
         else:
-            msg = "Validate error: Pls provide APIC/Switch IP configuration"
+            msg = "Validation error: APIC/Switch IP configuration is missing!"
             logger.error(msg)
             self.errors.append(msg)
             return True
 
     def _validate_image_version(self):
         try:
             global_policy = settings.global_policy['fabric']['global_policies']
@@ -183,54 +183,54 @@
             image64 = global_policy['switch_image64']
 
             pattern_32 = r"^(.+)\.bin"
             pattern_64 = r'(.+)-cs_64.bin'
 
             if image32 == image64:
                 if not image32.endswith(".bin"):
-                    msg = "Validate error: Image name must end with .bin."
+                    msg = "Validation error: Image name must end with .bin."
                     logger.error(msg)
                     return True
             else:
                 if not re.match(pattern_32, image32).group(1) == \
                        re.match(pattern_64, image64).group(1):
-                    msg = "Validate error: switch_image32 and " \
-                          "switch_image64 checking failed."
+                    msg = "Validation error: switch_image32 and " \
+                          "switch_image64 are not in same release!"
                     logger.error(msg)
                     return True
 
         except Exception as e:
-            msg = "Validate error: Yaml configuration switch_image32 and " \
-                  "switch_image64 checking failed."
+            msg = "Validation error: YAML configuration switch_image32 and " \
+                  "switch_image64 checking failed!"
             logger.error(msg)
             msg = e
             logger.error(msg)
             self.errors.append(str(msg))
             return True
 
     def validate_ssh_telnet_connection(self):
-        apic_error_msg = "Validate error: APIC CIMC SSH Fail.\n"
+        apic_error_msg = "Validation error: APIC CIMC SSH failed!\n"
         apic_fail_list = []
 
         for ip in self.cimc_address:
-            logger.info("Start SSH Connection Validate for {}, "
-                        "timeout 5 minustes".format(ip))
+            logger.info("Start SSH connection validation for {}, "
+                        "timeout 5 minutes".format(ip))
             connection_state = check_ssh_connection(
                 ip,
                 self.apic_cimc_credential[0],
                 self.apic_cimc_credential[1]
             )
             if not connection_state:
                 apic_fail_list.append(ip)
 
-        switch_error_msg = "Validate error: Switch Telnet Fail.\n"
+        switch_error_msg = "Validation error: Switch Telnet failed!\n"
         switch_fail_list = []
 
         for data in self.switch_list:
-            logger.info("Start Telnet Connection Validate for {}:{}"
+            logger.info("Start Telnet connection validation for {}:{}"
                         .format(data[0], data[1]))
             connection = TelnetClient(
                 data[0],
                 data[1],
                 self.aci_local_credential[0],
                 self.aci_local_credential[1]
             )
@@ -256,20 +256,22 @@
         if not apic_fail_list and switch_fail_list:
             switch_error_msg += ",".join(switch_fail_list)
 
             logger.error(switch_error_msg)
             self.errors.append(switch_error_msg)
             return True
 
-        logger.info("APIC CIMC SSH Connection and "
-                    "Switch Telnet Connection Success.")
+        logger.info("APIC CIMC SSH connection and "
+                    "Switch Telnet connection validate successfully.")
         return
 
     def validate_apic_aaa_connection(self):
-        apic_error_msg = "Validate error: APIC AAA Login Fail.\n"
+        # Rudy: Need to update AAA login code later
+        # (it's default domain at this moment)
+        apic_error_msg = "Validatation error: APIC Login failed!\n"
         apic_fail_list = []
 
         for ip in self.apic_address:
             start_time = time.time()
             if apic_fail_list:
                 apic_fail_list = list[set(apic_fail_list)]
                 apic_error_msg += ",".join(apic_fail_list)
@@ -287,51 +289,54 @@
                     ip,
                     self.aci_local_credential[0],
                     self.aci_local_credential[1]
                 )
                 if not connection_state:
                     apic_fail_list.append(ip)
                     logger.info("Attempt to validate {} "
-                                "APIC AAA Login Connection {}th,"
-                                " timeout 15 min."
+                                "APIC Login Connection {}th,"
+                                " timeout 15 mins."
                                 .format(ip, i))
                     i += 1
                     time.sleep(3)
                 else:
                     break
 
-        logger.info("APIC AAA Login Connection Success.")
+        logger.info("APIC Login validates successfully.")
         return
 
     def validate_choices(self, value):
         from iac_init.conf import settings
         choices = value.split(',')
         valid_choices = list(str(i) for i in
                              range(1, len(settings.DEFAULT_USER_OPTIONS)+1)
                              )
         for choice in choices:
             if choice not in valid_choices:
-                msg = '{} is not a valid choice'.format(choice)
+                msg = '{} is not a valid choice!'.format(choice)
                 logger.error(msg)
                 self.errors.append(msg)
                 return
         self.choices = sorted(choices, key=lambda x: int(x))
         self.options = value
         return self.choices
 
     # This function is used for option 1 and 2.
+    # Rudy: seems this is used for all options
     def validate_yaml_exist(self, yamlfile):
         for dir, _, files in os.walk(self.data_path):
             for filename in files:
                 if yamlfile == filename:
                     self.yaml_path = os.path.join(dir, filename)
         if self.yaml_path:
+            msg = "YAML file {} validated successfully.".format(yamlfile)
+            logger.info(msg)
             return self.yaml_path
         else:
-            msg = "Validate Error: Yaml File {} not fount".format(yamlfile)
+            msg = "Validation error: YAML file {} is missing!".format(yamlfile)
             logger.error(msg)
             self.errors.append(msg)
             return False
 
     # This function is used for option 3.
     def validate_yaml_dir_exist(self, yaml_dir):
         try:
@@ -340,30 +345,30 @@
             if os.path.exists(folder_path) and os.path.isdir(folder_path):
                 for dir, _, files in os.walk(folder_path):
                     for filename in files:
                         option3_yaml_path = os.path.join(dir, filename)
                         if option3_yaml_path:
                             self.file_dir_list.append(option3_yaml_path)
             else:
-                msg = "Validate Error: Directory {} not exist."\
+                msg = "Validation Error: Directory {} doesn't exist!"\
                     .format(folder_path)
                 logger.error(msg)
                 self.errors.append(msg)
                 return False
 
             if self.file_dir_list:
                 return self.file_dir_list
             else:
-                msg = "Validate Error: No file fount in dir: {}"\
+                msg = "Validation Error: No file found in dir: {}"\
                     .format(folder_path)
                 logger.error(msg)
                 self.errors.append(msg)
                 return False
         except Exception as e:
-            msg = "Validate Error: {}".format(e)
+            msg = "Validation Error: {}".format(e)
             logger.error(msg)
             self.errors.append(msg)
             return False
 
     def validate_cimc_precheck(self):
         cimc_username = self.apic_cimc_credential[0]
         cimc_password = self.apic_cimc_credential[1]
@@ -371,19 +376,19 @@
         for cimc_ip in self.cimc_address:
             error = cimc_precheck(cimc_ip, cimc_username, cimc_password)
             result[cimc_ip] = error
 
         result_state = True
         for cimc_ip, test_result in result.items():
             if test_result:
-                msg = "{} pre-check success\n".format(cimc_ip)
+                msg = "APIC CIMC {} pre-check successfully.\n".format(cimc_ip)
                 logger.info(msg)
             else:
                 result_state = False
-                msg = "{} pre-check fail\n".format(cimc_ip)
+                msg = "APIC CIMC {} pre-check failed!\n".format(cimc_ip)
                 logger.error(msg)
 
         if result_state:
             return False
         return True
 
     def _validate_bool(self, bool):
```

### Comparing `iac_init-0.9.0/iac_init/yaml_conf/yaml.py` & `iac_init-0.9.1/iac_init/yaml_conf/yaml.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # -*- coding: utf-8 -*-
 
-# Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
+# Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 import os
 import subprocess
 import importlib.util
 from typing import Any, Dict, List
 
 from ruamel import yaml
 from loguru import logger
 from iac_init.conf import settings
 
+# Rudy: need to check log setting
 logger.add(
     sink=os.path.join(
         settings.OUTPUT_BASE_DIR,
         'iac_init_log',
-        'iac-init-main.log'
+        'iac_init_main.log'
     ),
     format="{time} {level} {message}",
     level="INFO"
 )
 
 
 class VaultTag(yaml.YAMLObject):
@@ -68,15 +69,15 @@
 
     @classmethod
     def from_yaml(cls, loader: Any, node: Any) -> str:
         return str(cls(node.value))
 
 
 def load_yaml_files(paths: List[str]) -> Dict[str, Any]:
-    """Load all yaml files from a provided directory."""
+    """Load all YAML files from a provided directory."""
 
     def _load_file(file_path: str, data: Dict[str, Any]) -> None:
         with open(file_path, "r") as file:
             if ".yaml" in file_path or ".yml" in file_path:
                 data_yaml = file.read()
                 y = yaml.YAML()
                 y.preserve_quotes = True  # type: ignore
@@ -100,15 +101,15 @@
                         )
     return result
 
 
 def merge_list_item(
     source_item: Any, destination: List[Any], merge_list_items: bool = True
 ) -> None:
-    """Merge item into list."""
+    """Merge items into list."""
     if isinstance(source_item, dict) and merge_list_items:
         # check if we have an item in destination with matching primitives
         for dest_item in destination:
             match = True
             comparison = False
             unique_source = False
             unique_dest = False
```

### Comparing `iac_init-0.9.0/iac_init/yaml_conf/yaml_writer.py` & `iac_init-0.9.1/iac_init/yaml_conf/yaml_writer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 # -*- coding: utf-8 -*-
 
-# Copyright: (c) 2022, Wang Xiao <xiawang3@cisco.com>
+# Copyright: (c) 2024, Wang Xiao <xiawang3@cisco.com>
 
 import json
 import os
 import pathlib
 import shutil
 
 from . import yaml
 from loguru import logger
 from typing import Any, Dict, List
 from jinja2 import ChainableUndefined, Environment, FileSystemLoader
 from iac_init.conf import settings
 
+# Rudy: need to check log setting
 logger.add(
     sink=os.path.join(
         settings.OUTPUT_BASE_DIR,
         'iac_init_log',
-        'iac-init-main.log'),
+        'iac_init_main.log'),
     format="{time} {level} {message}", level="INFO")
 
 
 class YamlWriter:
     def __init__(
         self,
         data_paths: List[str],
     ) -> None:
-        logger.info("Loading yaml files from {}".format(data_paths[0]))
+        logger.info("Loading YAML files from {}".format(data_paths[0]))
         self.data = yaml.load_yaml_files(data_paths)
         self.filters: Dict[str, Any] = {}
 
     def render_template(
             self,
             template_path: str,
             output_path: str,
             env: Environment,
             **kwargs: Any
     ) -> None:
         """Render single robot jinja template"""
-        logger.info("Render ansible playbook template: {}"
+        logger.info("Render Ansible playbook template: {}"
                     .format(template_path))
         # create output directory if it does not exist yet
         pathlib.Path(os.path.dirname(output_path))\
             .mkdir(parents=True, exist_ok=True)
 
         template = env.get_template(template_path)
         # json roundtrip should be safe
@@ -115,29 +116,29 @@
                             output_path,
                             os.path.basename(templates_path),
                             rel
                         )
 
                         self.o_path = os.path.join(o_dir, filename)
                         self.render_template(t_path, self.o_path, env)
-                        logger.info("Generate working file success: {}"
+                        logger.info("Generate working file successfully: {}"
                                     .format(self.o_path))
                 except Exception as e:
                     logger.error("Generate working file failed: {}"
                                  .format(self.o_path))
                     logger.error("Error: {}".format(e))
                     exit()
             else:
                 try:
                     rel = os.path.relpath(dir, templates_path)
                     rel = rel.replace("\\", "/")
                     self.o_dir = self._fix_duplicate_path(
                         output_path, os.path.basename(templates_path), rel
                     )
                     pathlib.Path(self.o_dir).mkdir(parents=True, exist_ok=True)
-                    logger.info("Generate working directory success: {}"
+                    logger.info("Generate working directory successfully: {}"
                                 .format(self.o_dir))
                 except Exception as e:
                     logger.error("Generate working directory failed: {}"
                                  .format(self.o_dir))
                     logger.error("Error: {}".format(e))
                     exit()
```

### Comparing `iac_init-0.9.0/pyproject.toml` & `iac_init-0.9.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "iac-init"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
-authors = ["Wang Xiao <xiawang3@cisco.com>"]
+authors = ["Wang Xiao <xiawang3@cisco.com>", "Rudy Lei <shlei@cisco.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 iac-init = "iac_init.cli.main:main"
 
 [tool.poetry.dependencies]
 click = "^8.0.4"
```

