# Comparing `tmp/kas-4.3.2.tar.gz` & `tmp/kas-4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kas-4.3.2.tar", last modified: Tue Apr  9 17:26:02 2024, max compression
+gzip compressed data, was "dist/kas-4.4.tar", last modified: Fri May 31 16:24:31 2024, max compression
```

## Comparing `kas-4.3.2.tar` & `kas-4.4.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-04-09 17:26:02.000000 kas-4.3.2/
--rw-r--r--   0 jan       (1000) users      (100)     2941 2024-04-09 17:26:02.000000 kas-4.3.2/PKG-INFO
--rw-r--r--   0 jan       (1000) users      (100)     1624 2023-04-08 06:54:12.000000 kas-4.3.2/README.rst
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-04-09 17:26:02.000000 kas-4.3.2/kas/
--rw-r--r--   0 jan       (1000) users      (100)     1527 2020-12-06 06:22:49.000000 kas-4.3.2/kas/__init__.py
--rw-r--r--   0 jan       (1000) users      (100)     1330 2021-09-13 11:52:25.000000 kas-4.3.2/kas/__main__.py
--rw-r--r--   0 jan       (1000) users      (100)     1422 2024-04-09 17:25:46.000000 kas-4.3.2/kas/__version__.py
--rw-r--r--   0 jan       (1000) users      (100)     7835 2024-02-13 09:50:23.000000 kas-4.3.2/kas/config.py
--rw-r--r--   0 jan       (1000) users      (100)     1455 2021-10-08 09:03:16.000000 kas-4.3.2/kas/configschema.py
--rw-r--r--   0 jan       (1000) users      (100)     4525 2022-10-28 05:38:25.000000 kas-4.3.2/kas/context.py
--rw-r--r--   0 jan       (1000) users      (100)    12489 2024-02-25 18:08:37.000000 kas-4.3.2/kas/includehandler.py
--rw-r--r--   0 jan       (1000) users      (100)     6532 2024-04-09 15:54:13.000000 kas-4.3.2/kas/kas.py
--rw-r--r--   0 jan       (1000) users      (100)     2794 2023-12-18 09:28:13.000000 kas-4.3.2/kas/kasusererror.py
--rw-r--r--   0 jan       (1000) users      (100)    14530 2024-04-09 15:54:13.000000 kas-4.3.2/kas/libcmds.py
--rw-r--r--   0 jan       (1000) users      (100)    13868 2024-03-13 06:22:05.000000 kas-4.3.2/kas/libkas.py
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-04-09 17:26:02.000000 kas-4.3.2/kas/plugins/
--rw-r--r--   0 jan       (1000) users      (100)     2014 2023-01-05 17:10:45.000000 kas-4.3.2/kas/plugins/__init__.py
--rw-r--r--   0 jan       (1000) users      (100)     4293 2024-02-25 18:08:37.000000 kas-4.3.2/kas/plugins/build.py
--rw-r--r--   0 jan       (1000) users      (100)     2352 2021-10-19 08:31:44.000000 kas-4.3.2/kas/plugins/checkout.py
--rw-r--r--   0 jan       (1000) users      (100)     8739 2023-12-18 09:28:13.000000 kas-4.3.2/kas/plugins/dump.py
--rw-r--r--   0 jan       (1000) users      (100)     5333 2023-10-20 17:38:55.000000 kas-4.3.2/kas/plugins/for_all_repos.py
--rw-r--r--   0 jan       (1000) users      (100)    18592 2024-02-25 18:08:37.000000 kas-4.3.2/kas/plugins/menu.py
--rw-r--r--   0 jan       (1000) users      (100)     4451 2023-05-19 05:17:03.000000 kas-4.3.2/kas/plugins/shell.py
--rw-r--r--   0 jan       (1000) users      (100)    23420 2024-04-09 15:54:13.000000 kas-4.3.2/kas/repos.py
--rw-r--r--   0 jan       (1000) users      (100)    10018 2024-02-13 09:50:23.000000 kas-4.3.2/kas/schema-kas.json
--rwxr-xr-x   0 jan       (1000) users      (100)    17993 2024-04-09 17:25:46.000000 kas-4.3.2/kas-container
-drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-04-09 17:26:02.000000 kas-4.3.2/kas.egg-info/
--rw-r--r--   0 jan       (1000) users      (100)     2941 2024-04-09 17:26:02.000000 kas-4.3.2/kas.egg-info/PKG-INFO
--rw-r--r--   0 jan       (1000) users      (100)      586 2024-04-09 17:26:02.000000 kas-4.3.2/kas.egg-info/SOURCES.txt
--rw-r--r--   0 jan       (1000) users      (100)        1 2024-04-09 17:26:02.000000 kas-4.3.2/kas.egg-info/dependency_links.txt
--rw-r--r--   0 jan       (1000) users      (100)       38 2024-04-09 17:26:02.000000 kas-4.3.2/kas.egg-info/entry_points.txt
--rw-r--r--   0 jan       (1000) users      (100)       96 2024-04-09 17:26:02.000000 kas-4.3.2/kas.egg-info/requires.txt
--rw-r--r--   0 jan       (1000) users      (100)        4 2024-04-09 17:26:02.000000 kas-4.3.2/kas.egg-info/top_level.txt
--rw-r--r--   0 jan       (1000) users      (100)       58 2021-11-29 10:53:59.000000 kas-4.3.2/pyproject.toml
--rw-r--r--   0 jan       (1000) users      (100)       38 2024-04-09 17:26:02.000000 kas-4.3.2/setup.cfg
--rw-r--r--   0 jan       (1000) users      (100)     3342 2024-03-02 08:32:56.000000 kas-4.3.2/setup.py
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-05-31 16:24:31.000000 kas-4.4/
+-rw-r--r--   0 jan       (1000) users      (100)     2939 2024-05-31 16:24:31.000000 kas-4.4/PKG-INFO
+-rw-r--r--   0 jan       (1000) users      (100)     1624 2023-04-08 06:54:12.000000 kas-4.4/README.rst
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-05-31 16:24:31.000000 kas-4.4/kas/
+-rw-r--r--   0 jan       (1000) users      (100)     1527 2020-12-06 06:22:49.000000 kas-4.4/kas/__init__.py
+-rw-r--r--   0 jan       (1000) users      (100)     1330 2021-09-13 11:52:25.000000 kas-4.4/kas/__main__.py
+-rw-r--r--   0 jan       (1000) users      (100)     1420 2024-05-31 16:23:43.000000 kas-4.4/kas/__version__.py
+-rw-r--r--   0 jan       (1000) users      (100)     8268 2024-05-06 13:31:07.000000 kas-4.4/kas/attestation.py
+-rw-r--r--   0 jan       (1000) users      (100)     8698 2024-05-06 13:31:07.000000 kas-4.4/kas/config.py
+-rw-r--r--   0 jan       (1000) users      (100)     1455 2021-10-08 09:03:16.000000 kas-4.4/kas/configschema.py
+-rw-r--r--   0 jan       (1000) users      (100)     4790 2024-05-28 05:20:33.000000 kas-4.4/kas/context.py
+-rw-r--r--   0 jan       (1000) users      (100)    12489 2024-02-25 18:08:37.000000 kas-4.4/kas/includehandler.py
+-rw-r--r--   0 jan       (1000) users      (100)     7225 2024-04-29 15:25:39.000000 kas-4.4/kas/kas.py
+-rw-r--r--   0 jan       (1000) users      (100)     3305 2024-05-06 13:31:07.000000 kas-4.4/kas/kasusererror.py
+-rw-r--r--   0 jan       (1000) users      (100)    16157 2024-05-14 13:30:56.000000 kas-4.4/kas/libcmds.py
+-rw-r--r--   0 jan       (1000) users      (100)    15602 2024-04-29 15:25:39.000000 kas-4.4/kas/libkas.py
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-05-31 16:24:31.000000 kas-4.4/kas/plugins/
+-rw-r--r--   0 jan       (1000) users      (100)     2014 2023-01-05 17:10:45.000000 kas-4.4/kas/plugins/__init__.py
+-rw-r--r--   0 jan       (1000) users      (100)     5982 2024-05-06 13:31:07.000000 kas-4.4/kas/plugins/build.py
+-rw-r--r--   0 jan       (1000) users      (100)     2352 2021-10-19 08:31:44.000000 kas-4.4/kas/plugins/checkout.py
+-rw-r--r--   0 jan       (1000) users      (100)    10226 2024-05-06 13:31:07.000000 kas-4.4/kas/plugins/dump.py
+-rw-r--r--   0 jan       (1000) users      (100)     5523 2024-05-06 13:31:07.000000 kas-4.4/kas/plugins/for_all_repos.py
+-rw-r--r--   0 jan       (1000) users      (100)    18554 2024-05-06 13:31:07.000000 kas-4.4/kas/plugins/menu.py
+-rw-r--r--   0 jan       (1000) users      (100)     4062 2024-04-29 15:25:39.000000 kas-4.4/kas/plugins/shell.py
+-rw-r--r--   0 jan       (1000) users      (100)    25635 2024-05-28 05:20:33.000000 kas-4.4/kas/repos.py
+-rw-r--r--   0 jan       (1000) users      (100)    10169 2024-05-06 13:31:07.000000 kas-4.4/kas/schema-kas.json
+-rwxr-xr-x   0 jan       (1000) users      (100)    18176 2024-05-31 16:23:43.000000 kas-4.4/kas-container
+drwxr-xr-x   0 jan       (1000) users      (100)        0 2024-05-31 16:24:31.000000 kas-4.4/kas.egg-info/
+-rw-r--r--   0 jan       (1000) users      (100)     2939 2024-05-31 16:24:30.000000 kas-4.4/kas.egg-info/PKG-INFO
+-rw-r--r--   0 jan       (1000) users      (100)      605 2024-05-31 16:24:31.000000 kas-4.4/kas.egg-info/SOURCES.txt
+-rw-r--r--   0 jan       (1000) users      (100)        1 2024-05-31 16:24:30.000000 kas-4.4/kas.egg-info/dependency_links.txt
+-rw-r--r--   0 jan       (1000) users      (100)       38 2024-05-31 16:24:30.000000 kas-4.4/kas.egg-info/entry_points.txt
+-rw-r--r--   0 jan       (1000) users      (100)       96 2024-05-31 16:24:30.000000 kas-4.4/kas.egg-info/requires.txt
+-rw-r--r--   0 jan       (1000) users      (100)        4 2024-05-31 16:24:30.000000 kas-4.4/kas.egg-info/top_level.txt
+-rw-r--r--   0 jan       (1000) users      (100)       58 2021-11-29 10:53:59.000000 kas-4.4/pyproject.toml
+-rw-r--r--   0 jan       (1000) users      (100)       38 2024-05-31 16:24:31.000000 kas-4.4/setup.cfg
+-rw-r--r--   0 jan       (1000) users      (100)     3342 2024-03-02 08:32:56.000000 kas-4.4/setup.py
```

### Comparing `kas-4.3.2/PKG-INFO` & `kas-4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kas
-Version: 4.3.2
+Version: 4.4
 Summary: Setup tool for bitbake based projects
 Home-page: https://github.com/siemens/kas
 Maintainer: Jan Kiszka
 Maintainer-email: jan.kiszka@siemens.com
 License: MIT
 Download-URL: https://github.com/siemens/kas/archive/{__version__}.tar.gz
 Description: Setup tool for bitbake based projects
```

### Comparing `kas-4.3.2/README.rst` & `kas-4.4/README.rst`

 * *Files identical despite different names*

### Comparing `kas-4.3.2/kas/__init__.py` & `kas-4.4/kas/__init__.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.2/kas/__main__.py` & `kas-4.4/kas/__main__.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.2/kas/__version__.py` & `kas-4.4/kas/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 # SOFTWARE.
 """
     This module contains the version of kas.
 """
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) Siemens AG, 2017-2020'
 
-__version__ = '4.3.2'
+__version__ = '4.4'
 
 # Please update docs/format-changelog.rst when changing the file version.
-__file_version__ = 16
+__file_version__ = 17
 __compatible_file_version__ = 1
```

### Comparing `kas-4.3.2/kas/config.py` & `kas-4.4/kas/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,30 +21,33 @@
 # SOFTWARE.
 """
     This module contains the implementation of the kas configuration.
 """
 
 import os
 import json
+from pathlib import Path
 from .repos import Repo
 from .includehandler import IncludeHandler, IncludeException
+from .kasusererror import ArtifactNotFoundError
 
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) Siemens AG, 2017-2021'
 
 CONFIG_YAML_FILE = '.config.yaml'
 
 
 class Config:
     """
         Implements the kas configuration based on config files.
     """
     def __init__(self, ctx, filename, target=None, task=None):
         self._override_target = target
         self._override_task = task
+        self._build_dir = ctx.build_dir
         self._config = {}
         if not filename:
             filename = os.path.join(ctx.kas_work_dir, CONFIG_YAML_FILE)
 
         self.filenames = [os.path.abspath(configfile)
                           for configfile in filename.split(':')]
         top_repo_path = Repo.get_root_path(
@@ -215,7 +218,24 @@
             Returns the multiconfig array as bitbake string
         """
         multiconfigs = set()
         for target in self.get_bitbake_targets():
             if target.startswith('multiconfig:') or target.startswith('mc:'):
                 multiconfigs.add(target.split(':')[1])
         return ' '.join(multiconfigs)
+
+    def get_artifacts(self, missing_ok=True):
+        """
+            Returns the found artifacts after glob expansion, relative
+            to the build_dir as a list of tuples (name, path).
+            If missing_ok=False, raises an ArtifactNotFoundError if no
+            artifact for a given name is found.
+        """
+        arts = self._config.get('artifacts', {})
+        foundfiles = []
+        for name, art in arts.items():
+            files = list(Path(self._build_dir).glob(art))
+            if not missing_ok and len(files) == 0:
+                raise ArtifactNotFoundError(name, art)
+            foundfiles.extend([(name, f) for f in files])
+        return [(n, f.relative_to(self._build_dir))
+                for n, f in foundfiles]
```

### Comparing `kas-4.3.2/kas/configschema.py` & `kas-4.4/kas/configschema.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.2/kas/context.py` & `kas-4.4/kas/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 # SOFTWARE.
 """
     This module contains the implementation of the kas context.
 """
 
 import os
 import logging
+from kas.kasusererror import KasUserError
 
 try:
     import distro
 
     def get_distro_id_base():
         """
             Returns a compatible distro id.
@@ -74,14 +75,18 @@
         work_dir = os.environ.get('KAS_WORK_DIR', os.getcwd())
         self.__kas_work_dir = os.path.abspath(work_dir)
         build_dir = os.environ.get('KAS_BUILD_DIR',
                                    os.path.join(self.__kas_work_dir, 'build'))
         self.__kas_build_dir = os.path.abspath(build_dir)
         ref_dir = os.environ.get('KAS_REPO_REF_DIR', None)
         self.__kas_repo_ref_dir = os.path.abspath(ref_dir) if ref_dir else None
+        clone_depth = os.environ.get('KAS_CLONE_DEPTH', '0')
+        if not clone_depth.isdigit():
+            raise KasUserError('KAS_CLONE_DEPTH must be a number')
+        self.repo_clone_depth = max(int(clone_depth), 0)
         self.setup_initial_environ()
         self.config = None
         self.args = args
 
     def setup_initial_environ(self):
         """
             Sets the environment variables for processes that are
```

### Comparing `kas-4.3.2/kas/includehandler.py` & `kas-4.4/kas/includehandler.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.2/kas/kas.py` & `kas-4.4/kas/kas.py`

 * *Files 12% similar despite different names*

```diff
@@ -137,20 +137,40 @@
                                  'critical'],
                         default=f'{default_log_level}',
                         help=f'Set log level (default: {default_log_level})')
 
     subparser = parser.add_subparsers(help='sub command help', dest='cmd')
 
     for plugin in plugins.all():
-        plugin_parser = subparser.add_parser(plugin.name, help=plugin.helpmsg)
+        plugin_parser = subparser.add_parser(
+            plugin.name,
+            help=plugin.helpmsg,
+            formatter_class=ArgumentChoicesHelpFormatter)
         plugin.setup_parser(plugin_parser)
 
     return parser
 
 
+class ArgumentChoicesHelpFormatter(argparse.HelpFormatter):
+    """Help message formatter which adds choices to argument help.
+
+    If the default METAVAR is used, this will do nothing, as the default
+    METAVAR shows the available choices already. If the METAVAR is
+    overridden, and %(choice)s is not present in the help string, add
+    them.
+    """
+
+    def _get_help_string(self, action):
+        help = action.help
+        if action.choices and action.metavar is not None:
+            if "%(choices)" not in action.help:
+                help += " Possible choices: %(choices)s."
+        return help
+
+
 def kas(argv):
     """
         The actual main entry point of kas.
     """
     create_logger()
 
     parser = kas_get_argparser()
```

### Comparing `kas-4.3.2/kas/kasusererror.py` & `kas-4.4/kas/kasusererror.py`

 * *Files 17% similar despite different names*

```diff
@@ -62,7 +62,23 @@
 
 class ArgsCombinationError(KasUserError):
     """
     Invalid combination of CLI arguments provided
     """
     def __init__(self, message):
         super().__init__(f'Invalid combination of arguments: {message}')
+
+
+class ArtifactNotFoundError(KasUserError, FileNotFoundError):
+    """
+    A configured artifact is not found (or the glob matches 0 elements).
+    """
+    def __init__(self, name, artifact):
+        super().__init__(f'No artifact found for {name}:"{artifact}"')
+
+
+class MissingModuleError(KasUserError):
+    """
+    An optional module is missing for the requested operation
+    """
+    def __init__(self, module, operation) -> None:
+        super().__init__(f'Module "{module}" is required for: {operation}')
```

### Comparing `kas-4.3.2/kas/libcmds.py` & `kas-4.4/kas/libcmds.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,14 +176,43 @@
 
     def __del__(self):
         shutil.rmtree(self.tmpdirname)
 
     def __str__(self):
         return 'setup_home'
 
+    @staticmethod
+    def _on_ci():
+        """
+            Detects if we are running on a CI system.
+            Returns the name of the CI system or None.
+        """
+        if os.environ.get('GITHUB_ACTIONS', False) == 'true':
+            return 'GitHub Actions'
+        elif os.environ.get('GITLAB_CI', False) == 'true':
+            return 'GitLab CI'
+        return None
+
+    @staticmethod
+    def _ssh_config_present():
+        """
+            Checks if any file in the .ssh dir exists or
+            any manual ssh config option is set.
+        """
+        ssh_vars = ['SSH_PRIVATE_KEY', 'SSH_PRIVATE_KEY_FILE', 'SSH_AUTH_SOCK']
+        if any(e in os.environ for e in ssh_vars):
+            return True
+
+        ssh_path = os.path.expanduser('~/.ssh')
+        if os.path.isdir(ssh_path):
+            with os.scandir(ssh_path) as it:
+                if any(it):
+                    return True
+        return False
+
     def _setup_netrc(self):
         if os.environ.get('NETRC_FILE', False):
             shutil.copy(os.environ['NETRC_FILE'],
                         self.tmpdirname + "/.netrc")
         if os.environ.get('CI_SERVER_HOST', False) \
                 and os.environ.get('CI_JOB_TOKEN', False):
             with open(self.tmpdirname + '/.netrc', 'a') as fds:
@@ -218,17 +247,16 @@
             shutil.copy(os.environ['AWS_WEB_IDENTITY_TOKEN_FILE'],
                         webid_token_file)
 
     def _setup_gitconfig(self):
         gitconfig_host = os.environ.get('GITCONFIG_FILE', False)
         gitconfig_kas = self.tmpdirname + '/.gitconfig'
 
-        # when running in the github ci, always try to read the gitconfig
-        if not gitconfig_host and \
-           os.environ.get('GITHUB_ACTIONS', False) == 'true':
+        # on supported CI systems, always try to read the gitconfig
+        if not gitconfig_host and self._on_ci():
             gitconfig_host = os.path.expanduser('~/.gitconfig')
 
         if gitconfig_host and os.path.exists(gitconfig_host):
             shutil.copy(gitconfig_host, gitconfig_kas)
 
         with GitConfigParser(gitconfig_kas, read_only=False) as config:
             # overwrite user as kas operates git
@@ -239,17 +267,31 @@
             if os.environ.get('GIT_CREDENTIAL_HELPER', False):
                 config['credential'] = {
                     'helper': os.environ.get('GIT_CREDENTIAL_HELPER')
                 }
                 if os.environ.get('GIT_CREDENTIAL_USEHTTPPATH', False):
                     config['credential']['useHttpPath'] = \
                         os.environ.get('GIT_CREDENTIAL_USEHTTPPATH')
+            # in GitLab CI, add ssh -> https rewrites if no config is present
+            ci_server = os.environ.get('CI_SERVER_HOST', False)
+            if self._on_ci() == 'GitLab CI' and ci_server and \
+                    not self._ssh_config_present() and \
+                    not os.path.exists(gitconfig_host):
+                logging.debug('Adding GitLab CI ssh -> https rewrites')
+                section = f'url "https://{ci_server}/"'
+                config.add_value(section, 'insteadOf',
+                                 f'git@{ci_server}:')
+                config.add_value(section, 'insteadOf',
+                                 f'ssh://git@{ci_server}/')
             config.write()
 
     def execute(self, ctx):
+        ci = self._on_ci()
+        if ci:
+            logging.info(f'Running on {ci}')
         def_umask = os.umask(0o077)
         self._setup_netrc()
         self._setup_gitconfig()
         self._setup_aws_creds()
         os.umask(def_umask)
 
         ctx.environ['HOME'] = self.tmpdirname
```

### Comparing `kas-4.3.2/kas/libkas.py` & `kas-4.4/kas/libkas.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """
     This module contains the core implementation of kas.
 """
 
+import argparse
 import re
 import os
 import sys
 import logging
 import tempfile
 import asyncio
 import errno
@@ -402,35 +403,83 @@
         if content != generated_content:
             logging.warning("%s already exists, "
                             "not touching it to disable StrictHostKeyChecking",
                             ssh_config)
 
 
 def setup_parser_common_args(parser):
+    from kas.libcmds import Macro
+
     parser.add_argument('config',
                         help='Config file(s), separated by colon. Using '
                         '.config.yaml in KAS_WORK_DIR if none is specified.',
                         nargs='?')
     parser.add_argument('--skip',
-                        help='Skip build steps',
-                        default=[])
+                        help='Skip build steps. To skip more than one step, '
+                        'use this argument multiple times.',
+                        default=[],
+                        action='append',
+                        metavar='STEP',
+                        choices=[str(c) for c in Macro().setup_commands])
     parser.add_argument('--force-checkout', action='store_true',
                         help='Always checkout the desired commit/branch/tag '
                         'of each repository, discarding any local changes')
     parser.add_argument('--update', action='store_true',
                         help='Pull new upstream changes to the desired '
                         'branch even if it is already checked out locally')
 
 
 def setup_parser_preserve_env_arg(parser):
     parser.add_argument('-E', '--preserve-env',
                         help='Keep current user environment block',
                         action='store_true')
 
 
+class ExtendConstAction(argparse._AppendConstAction):
+    """Add an 'extend_const' action similar to 'append_const'.
+
+    Based on the existing 'append_const' and 'extend' actions.
+    """
+    def __init__(self, option_strings, dest, const, default=None,
+                 required=False, help=None, metavar=None):
+        super(argparse._AppendConstAction, self).__init__(
+            option_strings=option_strings, dest=dest, nargs=0, const=const,
+            default=default, required=required, help=help, metavar=metavar)
+
+    def __call__(self, parser, namespace, values, option_string=None):
+        items = getattr(namespace, self.dest, None)
+        if items is None:
+            items = []
+
+        if isinstance(items, list):
+            items = items[:]
+        else:
+            import copy
+            items = copy.copy(items)
+
+        items.extend(self.const)
+        setattr(namespace, self.dest, items)
+
+
+def setup_parser_keep_config_unchanged_arg(parser):
+    # Skip the tasks which would change the config of the build
+    # environment
+    steps = [
+        'setup_dir',
+        'finish_setup_repos',
+        'repos_apply_patches',
+        'write_bbconfig',
+    ]
+    parser.add_argument('-k', '--keep-config-unchanged',
+                        help='Skip steps that change the configuration',
+                        action=ExtendConstAction,
+                        dest='skip',
+                        const=steps)
+
+
 def run_handle_preserve_env_arg(ctx, os, args, SetupHome):
     if args.preserve_env:
         # Warn if there's any settings that setup_home would apply
         # but are now ignored
         for var in SetupHome.ENV_VARS:
             if var in os.environ:
                 logging.warning('Environment variable "%s" ignored '
```

### Comparing `kas-4.3.2/kas/plugins/__init__.py` & `kas-4.4/kas/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.2/kas/plugins/build.py` & `kas-4.4/kas/plugins/shell.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,108 +16,105 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """
-    This plugin implements the ``kas build`` command.
+    This plugin implements the ``kas shell`` command.
 
     When this command is executed, kas will checkout repositories, setup the
-    build environment and then invoke bitbake to build the targets selected
-    in the chosen config file.
+    build environment and then start a shell in the build environment. This
+    can be used to manually run ``bitbake`` with custom command line options
+    or to execute other commands such as ``runqemu``.
 
-    For example, to build the configuration described in the file
+    For example, to start a shell in the build environment for the file
     ``kas-project.yml`` you could run::
 
-        kas build kas-project.yml
+        kas shell kas-project.yml
+
+    Or to invoke qemu to test an image which has been built::
+
+        kas shell kas-project.yml -c 'runqemu'
 """
 
 import logging
+import os
 import subprocess
-import sys
 from kas.context import create_global_context
 from kas.config import Config
-from kas.libkas import find_program, run_cmd
-from kas.libcmds import Macro, Command
+from kas.libcmds import Macro, Command, SetupHome
 from kas.libkas import setup_parser_common_args
+from kas.libkas import setup_parser_keep_config_unchanged_arg
+from kas.libkas import setup_parser_preserve_env_arg
+from kas.libkas import run_handle_preserve_env_arg
 from kas.kasusererror import CommandExecError
 
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) Siemens AG, 2017-2018'
 
 
-class Build:
+class Shell:
     """
-        This class implements the build plugin for kas.
+        Implements a kas plugin that opens a shell within the kas environment.
     """
 
-    name = 'build'
-    helpmsg = (
-        'Checks out all necessary repositories and builds using bitbake as '
-        'specified in the configuration file.'
-    )
+    name = 'shell'
+    helpmsg = 'Run a shell in the build environment.'
 
     @classmethod
     def setup_parser(cls, parser):
         """
-            Setup the argument parser for the build plugin
+            Setup the argument parser for the shell plugin
         """
 
         setup_parser_common_args(parser)
-        parser.add_argument('extra_bitbake_args',
-                            nargs='*',
-                            help='Extra arguments to pass to bitbake '
-                                 '(typically requires separation via \'--\')')
-        parser.add_argument('--target',
-                            action='append',
-                            help='Select target to build')
-        parser.add_argument('-c', '--cmd', '--task', dest='task',
-                            help='Select which task should be executed')
+        setup_parser_preserve_env_arg(parser)
+        setup_parser_keep_config_unchanged_arg(parser)
+        parser.add_argument('-c', '--command',
+                            help='Run command',
+                            default='')
 
     def run(self, args):
         """
-            Executes the build command of the kas plugin.
+            Runs this kas plugin
         """
 
-        if args.config and args.config.startswith('-'):
-            args.extra_bitbake_args.insert(0, args.config)
-            args.config = None
-
         ctx = create_global_context(args)
-        ctx.config = Config(ctx, args.config, args.target, args.task)
+        ctx.config = Config(ctx, args.config)
+
+        run_handle_preserve_env_arg(ctx, os, args, SetupHome)
 
         macro = Macro()
-        macro.add(BuildCommand(args.extra_bitbake_args))
+        macro.add(ShellCommand(args.command))
         macro.run(ctx, args.skip)
 
 
-class BuildCommand(Command):
+class ShellCommand(Command):
     """
-        Implements the bitbake build step.
+        This class implements the command that starts a shell.
     """
 
-    def __init__(self, extra_bitbake_args):
+    def __init__(self, cmd):
         super().__init__()
-        self.extra_bitbake_args = extra_bitbake_args
+        self.cmd = []
+        if cmd:
+            self.cmd = cmd
 
     def __str__(self):
-        return 'build'
+        return 'shell'
 
     def execute(self, ctx):
-        """
-            Executes the bitbake build command.
-        """
-        # Start bitbake build of image
-        bitbake = find_program(ctx.environ['PATH'], 'bitbake')
-        cmd = [bitbake, '-c', ctx.config.get_bitbake_task()] \
-            + self.extra_bitbake_args + ctx.config.get_bitbake_targets()
-        if sys.stdout.isatty():
-            logging.info('%s$ %s', ctx.build_dir, ' '.join(cmd))
-            ret = subprocess.call(cmd, env=ctx.environ, cwd=ctx.build_dir)
-            if ret != 0:
-                raise CommandExecError(cmd, ret)
-        else:
-            run_cmd(cmd, cwd=ctx.build_dir, liveupdate=True)
+        logging.info("To start the default build, run: bitbake -c %s %s",
+                     ctx.config.get_bitbake_task(),
+                     ' '.join(ctx.config.get_bitbake_targets()))
+        cmd = [ctx.environ.get('SHELL', '/bin/sh')]
+        if self.cmd:
+            cmd.append('-c')
+            cmd.append(self.cmd)
+        ret = subprocess.call(cmd, env=ctx.environ, cwd=ctx.build_dir)
+        if ret != 0:
+            logging.error('Shell returned non-zero exit status')
+            raise CommandExecError(cmd, ret, True)
 
 
-__KAS_PLUGINS__ = [Build]
+__KAS_PLUGINS__ = [Shell]
```

### Comparing `kas-4.3.2/kas/plugins/checkout.py` & `kas-4.4/kas/plugins/checkout.py`

 * *Files identical despite different names*

### Comparing `kas-4.3.2/kas/plugins/dump.py` & `kas-4.4/kas/plugins/dump.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # kas - setup tool for bitbake based projects
 #
-# Copyright (c) Siemens AG, 2017-2023
+# Copyright (c) Siemens AG, 2017-2024
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -32,14 +32,20 @@
     When running with ``--lock``, a locking spec is created which only contains
     the exact commit of each repository. This can be used to pin the commit of
     floating branches and tags, while still keeping an easy update path. When
     combining with ``--inplace``, a lockfile is created next to the first file
     on the kas cmdline. For details on the locking support, see
     :class:`kas.includehandler.IncludeHandler`.
 
+    When running with ``--resolve-local``, VCS tracking information of the root
+    repo (the one with the kas-project.yml) is added to the output. The
+    generated file can be used as single input to kas to reproduce the build
+    environment. If the root repo is not under version control or contains
+    uncommitted changes, a warning is emitted.
+
     Please note:
 
     - the dumped config is semantically identical but not bit-by-bit identical
     - all referenced repositories are checked out to resolve cross-repo configs
     - all branches are resolved before patches are applied
 
     For example, to get a single config representing the final build config of
@@ -62,14 +68,15 @@
 
     Note, that the lockfiles should be checked-in into the VCS.
 """
 
 import sys
 import json
 import yaml
+import logging
 from typing import TypeVar, TextIO
 from collections import OrderedDict
 from kas.context import get_context
 from kas.plugins.checkout import Checkout
 from kas.kasusererror import KasUserError, ArgsCombinationError
 
 __license__ = 'MIT'
@@ -158,14 +165,17 @@
         parser.add_argument('--indent',
                             type=int,
                             default=4,
                             help='Line indent (# of spaces, default: 4)')
         parser.add_argument('--resolve-refs',
                             action='store_true',
                             help='Replace floating refs with exact SHAs')
+        parser.add_argument('--resolve-local',
+                            action='store_true',
+                            help='Add tracking information of root repo')
         lk_or_env.add_argument('--resolve-env',
                                action='store_true',
                                help='Set env defaults to captured env value')
         lk_or_env.add_argument('--lock',
                                action='store_true',
                                help='Create lockfile with exact SHAs')
         parser.add_argument('-i', '--inplace',
@@ -186,14 +196,17 @@
         config_expanded = {'header': {'version': schema_v}} if args.lock \
             else ctx.config.get_config()
         repos = ctx.config.get_repos()
         output = IoTarget(target=sys.stdout, managed=False)
 
         if args.inplace and not args.lock:
             raise ArgsCombinationError('--inplace requires --lock')
+        if args.resolve_local and args.lock:
+            raise ArgsCombinationError(
+                '--resolve-local cannot be used with --lock')
 
         if args.lock:
             args.resolve_refs = True
             # when locking, only consider repos managed by kas
             repos = [r for r in repos if not r.operations_disabled]
             config_expanded['overrides'] = \
                 {'repos': {r.name: {'commit': r.revision} for r in repos}}
@@ -203,20 +216,34 @@
             output = IoTarget(target=lockfile, managed=True)
 
         # includes are already expanded, delete the key
         if 'includes' in config_expanded['header']:
             del config_expanded['header']['includes']
 
         if args.resolve_refs and not args.lock:
-            for r in repos:
+            for r in filter(lambda r: not r.operations_disabled, repos):
                 if r.commit or r.branch or r.tag:
                     config_expanded['repos'][r.name]['commit'] = r.revision
                 elif r.refspec:
                     config_expanded['repos'][r.name]['refspec'] = r.revision
 
+        if args.resolve_local:
+            for r in filter(lambda r: r.operations_disabled and r.name, repos):
+                if r.revision:
+                    if r.dirty:
+                        logging.warning(f'Repository {r.name} (root repo) '
+                                        'contains uncommitted changes.')
+                    if config_expanded['repos'][r.name] is None:
+                        config_expanded['repos'][r.name] = {}
+                    config_expanded['repos'][r.name]['url'] = r.url
+                    config_expanded['repos'][r.name]['commit'] = r.revision
+                else:
+                    logging.warning(f'Repository {r.name} (root repo) '
+                                    'is not under version control.')
+
         if args.resolve_env and 'env' in config_expanded:
             config_expanded['env'] = ctx.config.get_environment()
 
         with IoTargetMonitor(output) as f:
             if args.format == 'json':
                 json.dump(config_expanded, f, indent=args.indent)
                 f.write('\n')
```

### Comparing `kas-4.3.2/kas/plugins/for_all_repos.py` & `kas-4.4/kas/plugins/for_all_repos.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 import logging
 import os
 import subprocess
 from kas.context import create_global_context
 from kas.config import Config
 from kas.libcmds import Macro, Command, SetupHome
 from kas.libkas import setup_parser_common_args
+from kas.libkas import setup_parser_keep_config_unchanged_arg
 from kas.libkas import setup_parser_preserve_env_arg
 from kas.libkas import run_handle_preserve_env_arg
 from kas.kasusererror import CommandExecError
 
 __license__ = 'MIT'
 __copyright__ = 'Copyright (c) Siemens AG, 2017-2018'
 
@@ -87,14 +88,15 @@
         'Runs a specified command in all checked out repositories.'
     )
 
     @classmethod
     def setup_parser(cls, parser):
         setup_parser_common_args(parser)
         setup_parser_preserve_env_arg(parser)
+        setup_parser_keep_config_unchanged_arg(parser)
         parser.add_argument('command',
                             help='Command to be executed as a string.')
 
     def run(self, args):
         ctx = create_global_context(args)
         ctx.config = Config(ctx, args.config)
 
@@ -116,15 +118,16 @@
     def execute(self, ctx):
         for repo in ctx.config.get_repos():
             env = {
                 **ctx.environ,
                 'KAS_REPO_NAME': repo.name,
                 'KAS_REPO_PATH': repo.path,
                 'KAS_REPO_URL': '' if repo.operations_disabled else repo.url,
-                'KAS_REPO_COMMIT': repo.commit or '',
+                'KAS_REPO_COMMIT': '' if repo.operations_disabled
+                                   else (repo.commit or ''),
                 'KAS_REPO_BRANCH': repo.branch or '',
                 'KAS_REPO_TAG': repo.tag or '',
                 'KAS_REPO_REFSPEC': repo.refspec or '',
             }
             logging.info('%s$ %s', repo.path, self.command)
             retcode = subprocess.call(self.command, shell=True, cwd=repo.path,
                                       env=env)
```

### Comparing `kas-4.3.2/kas/plugins/menu.py` & `kas-4.4/kas/plugins/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 from kas import __version__, __file_version__
 from kas.context import create_global_context
 from kas.config import CONFIG_YAML_FILE
 from kas.repos import Repo
 from kas.includehandler import load_config as load_config_yaml, \
     SOURCE_DIR_OVERRIDE_KEY, SOURCE_DIR_HOST_OVERRIDE_KEY
 from kas.plugins.build import Build
-from kas.kasusererror import KasUserError
+from kas.kasusererror import KasUserError, MissingModuleError
 
 try:
     from snack import SnackScreen, EntryWindow, ButtonChoiceWindow, \
         ButtonBar, Listbox, GridFormHelp
     HAVE_NEWT = True
 except ImportError:
     HAVE_NEWT = False  # will be reported in run()
@@ -96,18 +96,14 @@
 SOURCE_DIR_HOST_ENV_KEY = '_KAS_REPO_DIR_HOST'
 
 
 class VariableTypeError(KasUserError):
     pass
 
 
-class MissingModuleError(KasUserError):
-    pass
-
-
 class KConfigLoadError(KasUserError):
     """
     The KConfig file could not be found or is invalid
     """
     pass
 
 
@@ -259,16 +255,15 @@
     def dump_kconf_warnings(self):
         if len(self.kconf.warnings) > 0:
             logging.warning("\n".join(self.kconf.warnings))
             self.kconf.warnings = []
 
     def run(self, args):
         if not HAVE_NEWT:
-            raise MissingModuleError(
-                'Menu plugin requires \'python3-newt\' distribution package.')
+            raise MissingModuleError('python3-newt', 'Menu plugin')
 
         ctx = create_global_context(args)
 
         kconfig_file = os.path.abspath(args.kconfig)
         try:
             self.kconf = Kconfig(kconfig_file, warn_to_stderr=False)
         except (KconfigError, FileNotFoundError) as err:
@@ -294,14 +289,15 @@
 
             build_args = Args()
             build_args.config = None
             build_args.target = None
             build_args.task = None
             build_args.extra_bitbake_args = []
             build_args.skip = None
+            build_args.provenance = False
 
             Build().run(build_args)
 
 
 class Menuconfig():
     def __init__(self, kconf):
         self.kconf = kconf
```

### Comparing `kas-4.3.2/kas/repos.py` & `kas-4.4/kas/repos.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,17 @@
         self.tag = tag
         self.branch = branch
         self.refspec = refspec
         self._layers = layers
         self._patches = patches
         self.operations_disabled = disable_operations
 
+        if not self.url:
+            self.resolve_local()
+
     @property
     def layers(self):
         return [os.path.join(self.path, layer).rstrip(os.sep + '.')
                 for layer in self._layers]
 
     @property
     def qualified_name(self):
@@ -131,14 +134,22 @@
             (_, output) = run_cmd(self.resolve_branch_cmd(),
                                   cwd=self.path, fail=False)
             if output:
                 return output.strip()
             return branch
         return None
 
+    @property
+    def dirty(self):
+        if not self.url:
+            return True
+        (_, output) = run_cmd(self.is_dirty_cmd(),
+                              cwd=self.path, fail=False)
+        return bool(output)
+
     def __str__(self):
         if self.commit and (self.tag or self.branch):
             refspec = f'{self.commit}({self.tag or self.branch})'
         else:
             refspec = self.commit or self.tag or self.branch or self.refspec
 
         return f'{self.url}:{refspec} ' \
@@ -222,15 +233,14 @@
                 path = os.path.join(get_context().kas_work_dir, name)
         elif not os.path.isabs(path):
             # Relative pathes are assumed to start from work_dir
             path = os.path.join(get_context().kas_work_dir, path)
 
         if url is None:
             # No version control operation on repository
-            url = path
             disable_operations = True
 
         if repo_type == 'git':
             return GitRepo(name, url, path, commit, tag, branch, refspec,
                            layers, patches, disable_operations)
         if repo_type == 'hg':
             if not shutil.which('hg'):
@@ -348,18 +358,15 @@
         if self.operations_disabled \
             or (self.commit is None and self.tag is None
                 and self.branch is None and self.refspec is None):
             return
 
         if not get_context().force_checkout:
             # Check if repos is dirty
-            (_, output) = run_cmd(self.is_dirty_cmd(),
-                                  cwd=self.path,
-                                  fail=False)
-            if output:
+            if self.dirty:
                 logging.warning('Repo %s is dirty - no checkout', self.name)
                 return
 
         if self.tag and self.branch:
             raise RepoRefError(
                 f'Both tag "{self.tag}" and branch "{self.branch}" '
                 f'cannot be specified for repository "{self.name}"')
@@ -383,15 +390,17 @@
             (retc, output) = run_cmd(self.resolve_branch_cmd(),
                                      cwd=self.path,
                                      fail=False)
             if retc:
                 raise RepoRefError(
                     f'Branch "{self.branch}" cannot be found '
                     f'in repository "{self.name}"')
-            if self.commit:
+            # check if branch contains the requested commit.
+            # skip check on shallow clones, as branch information is missing
+            if self.commit and not get_context().repo_clone_depth:
                 (_, output) = run_cmd(self.branch_contains_ref(),
                                       cwd=self.path,
                                       fail=False)
                 if not output.strip():
                     raise RepoRefError(
                         f'Branch "{self.branch}" in '
                         f'repository "{self.name}" does not contain '
@@ -479,29 +488,60 @@
                 cmd, cwd=self.path, fail=False)
             if retc:
                 raise PatchApplyError('Could not commit patch changes. repo: '
                                       f'{self.name}, vcs output: {output})')
 
         return 0
 
+    def resolve_local(self):
+        (retc, output) = run_cmd(self.get_remote_url_cmd(),
+                                 cwd=self.path, fail=False)
+        if retc == 0:
+            self.url = output.strip()
+
+        (retc, output) = run_cmd(self.get_commit_cmd(),
+                                 cwd=self.path, fail=False)
+        if retc == 0:
+            self.commit = output.strip()
+        if self.url and self.commit:
+            logging.debug('Repository %s resolved to %s @ %s',
+                          self.name, self.url, self.commit)
+
 
 class GitRepo(RepoImpl):
     """
         Provides the git functionality for a Repo.
     """
 
+    @staticmethod
+    def get_type():
+        return 'git'
+
     def remove_ref_prefix(self, ref):
         ref_prefix = 'refs/'
         return ref[ref.startswith(ref_prefix) and len(ref_prefix):]
 
     def add_cmd(self):
         return ['git', 'add', '-A']
 
     def clone_cmd(self, srcdir, createref):
         cmd = ['git', 'clone', '-q']
+
+        depth = get_context().repo_clone_depth
+        if depth:
+            if self.refspec:
+                logging.warning('Shallow cloning is not supported for legacy '
+                                f'refspec on repository "{self.name}". '
+                                'Performing full clone.')
+            else:
+                cmd.extend(['--depth', str(depth)])
+                if self.branch:
+                    cmd.extend(['--branch',
+                                self.remove_ref_prefix(self.branch)])
+
         if createref:
             cmd.extend([self.effective_url, '--bare', srcdir])
         elif srcdir:
             cmd.extend([srcdir, '--reference', srcdir, self.path])
         else:
             cmd.extend([self.effective_url, self.path])
         return cmd
@@ -514,19 +554,30 @@
         branch = self.branch or self.refspec
         if branch and branch.startswith('refs/'):
             branch = 'remotes/origin/' + self.remove_ref_prefix(branch)
         return ['git', 'cat-file', '-t', self.commit or self.tag or branch]
 
     def fetch_cmd(self):
         cmd = ['git', 'fetch', '-q']
+
+        depth = 0 if self.refspec else get_context().repo_clone_depth
+        if depth:
+            cmd.extend(['--depth', str(depth)])
+
         if self.tag:
-            cmd.append('--tags')
+            cmd.extend(['origin', f'+{self.tag}:refs/tags/{self.tag}'])
+            return cmd
+
+        # only fetch this commit (branch information is lost)
+        if depth and self.commit:
+            cmd.extend(['origin', self.commit])
+            return cmd
 
         branch = self.branch or self.refspec
-        if branch and branch.startswith('refs/'):
+        if branch and (branch.startswith('refs/') or depth):
             branch = self.remove_ref_prefix(branch)
             cmd.extend(['origin', f'+{branch}:refs/remotes/origin/{branch}'])
 
         return cmd
 
     def is_dirty_cmd(self):
         return ['git', 'status', '-s']
@@ -559,20 +610,30 @@
 
     def apply_patches_file_cmd(self, path):
         return ['git', 'apply', '--whitespace=nowarn', path]
 
     def set_remote_url_cmd(self):
         return ['git', 'remote', 'set-url', 'origin', self.effective_url]
 
+    def get_remote_url_cmd(self):
+        return ['git', 'remote', 'get-url', 'origin']
+
+    def get_commit_cmd(self):
+        return ['git', 'rev-parse', '--verify', 'HEAD']
+
 
 class MercurialRepo(RepoImpl):
     """
         Provides the hg functionality for a Repo.
     """
 
+    @staticmethod
+    def get_type():
+        return 'mercurial'
+
     def add_cmd(self):
         return ['hg', 'add']
 
     def clone_cmd(self, srcdir, createref):
         # Mercurial does not support repo references (object caches)
         if createref:
             return ['true']
@@ -616,7 +677,13 @@
         return ['hg', 'branch', '-f', f'patched-{refspec}']
 
     def apply_patches_file_cmd(self, path):
         return ['hg', 'import', '--no-commit', path]
 
     def set_remote_url_cmd(self):
         raise NotImplementedError()
+
+    def get_remote_url_cmd(self):
+        return ['hg', 'paths', 'default']
+
+    def get_commit_cmd(self):
+        return ['hg', 'log', '-r', '.', '--template', '{node}\n']
```

### Comparing `kas-4.3.2/kas/schema-kas.json` & `kas-4.4/kas/schema-kas.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9963235294117647%*

 * *Differences: {"'properties'": "{'artifacts': OrderedDict([('type', 'object'), ('additionalProperties', "*

 * *                 "OrderedDict([('type', ['string'])]))])}"}*

```diff
@@ -6,14 +6,22 @@
     "properties": {
         "_source_dir": {
             "type": "string"
         },
         "_source_dir_host": {
             "type": "string"
         },
+        "artifacts": {
+            "additionalProperties": {
+                "type": [
+                    "string"
+                ]
+            },
+            "type": "object"
+        },
         "bblayers_conf_header": {
             "additionalProperties": {
                 "type": "string"
             },
             "type": "object"
         },
         "build_system": {
```

### Comparing `kas-4.3.2/kas-container` & `kas-4.4/kas-container`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/bin/sh
 #
 # kas - setup tool for bitbake based projects
 #
-# Copyright (c) Siemens AG, 2018-2022
+# Copyright (c) Siemens AG, 2018-2024
 #
 # Authors:
 #  Jan Kiszka <jan.kiszka@siemens.com>
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
@@ -23,14 +23,19 @@
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 set -e
 
+KAS_IMAGE_VERSION_DEFAULT="4.4"
+KAS_CONTAINER_IMAGE_PATH_DEFAULT="ghcr.io/siemens/kas"
+KAS_CONTAINER_IMAGE_NAME_DEFAULT="kas"
+KAS_CONTAINER_SELF_NAME="$(basename "$0")"
+
 usage()
 {
 	SELF="${KAS_CONTAINER_SELF_NAME}"
 	printf "%b" "Usage: ${SELF} [OPTIONS] { build | shell } [KASOPTIONS] [KASFILE]\n"
 	printf "%b" "       ${SELF} [OPTIONS] { checkout | dump } [KASOPTIONS] [KASFILE]\n"
 	printf "%b" "       ${SELF} [OPTIONS] for-all-repos [KASOPTIONS] [KASFILE] COMMAND\n"
 	printf "%b" "       ${SELF} [OPTIONS] { clean | cleansstate | cleanall} [KASFILE]\n"
@@ -140,19 +145,14 @@
 		if [ "$1" = "cleanall" ]; then
 			DL_DIR=${DL_DIR:-${KAS_BUILD_DIR}/downloads}
 			trace rm -rf "${DL_DIR}"
 		fi
 	fi
 }
 
-KAS_IMAGE_VERSION_DEFAULT="4.3.2"
-KAS_CONTAINER_IMAGE_PATH_DEFAULT="ghcr.io/siemens/kas"
-KAS_CONTAINER_IMAGE_NAME_DEFAULT="kas"
-KAS_CONTAINER_SELF_NAME="$(basename "$0")"
-
 set_container_image_var() {
 	KAS_IMAGE_VERSION="${KAS_IMAGE_VERSION:-${KAS_IMAGE_VERSION_DEFAULT}}"
 	KAS_CONTAINER_IMAGE_NAME="${KAS_CONTAINER_IMAGE_NAME:-${KAS_CONTAINER_IMAGE_NAME_DEFAULT}}"
 	KAS_CONTAINER_IMAGE_PATH="${KAS_CONTAINER_IMAGE_PATH:-${KAS_CONTAINER_IMAGE_PATH_DEFAULT}}"
 	KAS_CONTAINER_IMAGE_DEFAULT="${KAS_CONTAINER_IMAGE_PATH}/${KAS_CONTAINER_IMAGE_NAME}:${KAS_IMAGE_VERSION}"
 	KAS_CONTAINER_IMAGE="${KAS_CONTAINER_IMAGE:-${KAS_CONTAINER_IMAGE_DEFAULT}}"
 }
@@ -326,23 +326,30 @@
 KAS_EXTRA_BITBAKE_ARGS=0
 
 # parse kas sub-command options
 while [ $# -gt 0 ] && [ $KAS_EXTRA_BITBAKE_ARGS -eq 0 ]; do
 	case "$1" in
 	--skip|--target|--task)
 		KAS_OPTIONS="${KAS_OPTIONS} $1 $2"
-		shift 2
+		shift 1
+		shift 1 || KAS_OPTIONS="--help"
 		;;
 	-c|--cmd|--command)
 		KAS_BITBAKE_C_OPTION_ARGS="$2"
-		shift 2
+		shift 1
+		shift 1 || KAS_OPTIONS="--help"
 		;;
 	-E|--preserve-env)
 		fatal_error "$1 is not supported with ${KAS_CONTAINER_SELF_NAME}"
 		;;
+	--provenance)
+		KAS_OPTIONS="${KAS_OPTIONS} $1 $2"
+		shift 1
+		shift 1 || KAS_OPTIONS="--help"
+		;;
 	--)
 		KAS_EXTRA_BITBAKE_ARGS=$#
 		;;
 	-*)
 		KAS_OPTIONS="${KAS_OPTIONS} $1"
 		shift 1
 		;;
@@ -535,15 +542,15 @@
 		fatal_error "Passed KAS_REPO_REF_DIR '${KAS_REPO_REF_DIR}' is not a directory"
 	fi
 	set -- "$@" \
 		-v "$(readlink -fv "${KAS_REPO_REF_DIR}")":/repo-ref:rw \
 		-e KAS_REPO_REF_DIR=/repo-ref
 fi
 
-for var in TERM KAS_DISTRO KAS_MACHINE KAS_TARGET KAS_TASK \
+for var in TERM KAS_DISTRO KAS_MACHINE KAS_TARGET KAS_TASK KAS_CLONE_DEPTH \
            KAS_PREMIRRORS DISTRO_APT_PREMIRRORS BB_NUMBER_THREADS PARALLEL_MAKE \
            GIT_CREDENTIAL_USEHTTPPATH; do
 	if [ -n "$(eval echo \$${var})" ]; then
 		set -- "$@" -e "${var}=$(eval echo \"\$${var}\")"
 	fi
 done
```

### Comparing `kas-4.3.2/kas.egg-info/PKG-INFO` & `kas-4.4/kas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kas
-Version: 4.3.2
+Version: 4.4
 Summary: Setup tool for bitbake based projects
 Home-page: https://github.com/siemens/kas
 Maintainer: Jan Kiszka
 Maintainer-email: jan.kiszka@siemens.com
 License: MIT
 Download-URL: https://github.com/siemens/kas/archive/{__version__}.tar.gz
 Description: Setup tool for bitbake based projects
```

### Comparing `kas-4.3.2/kas.egg-info/SOURCES.txt` & `kas-4.4/kas.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.rst
 kas-container
 pyproject.toml
 setup.py
 kas/__init__.py
 kas/__main__.py
 kas/__version__.py
+kas/attestation.py
 kas/config.py
 kas/configschema.py
 kas/context.py
 kas/includehandler.py
 kas/kas.py
 kas/kasusererror.py
 kas/libcmds.py
```

### Comparing `kas-4.3.2/setup.py` & `kas-4.4/setup.py`

 * *Files identical despite different names*

