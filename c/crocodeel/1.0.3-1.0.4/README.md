# Comparing `tmp/crocodeel-1.0.3.tar.gz` & `tmp/crocodeel-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crocodeel-1.0.3.tar", max compression
+gzip compressed data, was "crocodeel-1.0.4.tar", max compression
```

## Comparing `crocodeel-1.0.3.tar` & `crocodeel-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0    35147 2024-05-06 16:01:16.847576 crocodeel-1.0.3/COPYING
--rw-r--r--   0        0        0     4273 2024-05-06 16:01:16.851576 crocodeel-1.0.3/README.md
--rw-r--r--   0        0        0       85 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/__init__.py
--rw-r--r--   0        0        0     1792 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/ab_table_utils.py
--rw-r--r--   0        0        0     2011 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/conta_event.py
--rw-r--r--   0        0        0     6776 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/crocodeel.py
--rw-r--r--   0        0        0      670 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/easy_wf.py
--rw-r--r--   0        0        0     1005 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/execution_description.py
--rw-r--r--   0        0        0   623880 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/models/crocodeel_rf_Mar2023.joblib
--rw-r--r--   0        0        0     6410 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/plot_conta.py
--rw-r--r--   0        0        0      731 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/rf_model.py
--rw-r--r--   0        0        0    16557 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/search_conta.py
--rw-r--r--   0        0        0   119253 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/test_data/mgs_profiles_test.tsv
--rw-r--r--   0        0        0    49550 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/test_data/results/contamination_events.pdf
--rw-r--r--   0        0        0     2051 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/test_data/results/contamination_events.tsv
--rw-r--r--   0        0        0     2008 2024-05-06 16:01:16.851576 crocodeel-1.0.3/crocodeel/test_install.py
--rw-r--r--   0        0        0     1377 2024-05-06 16:01:16.851576 crocodeel-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     5375 1970-01-01 00:00:00.000000 crocodeel-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-05-31 08:23:57.064046 crocodeel-1.0.4/COPYING
+-rw-r--r--   0        0        0     4273 2024-05-31 08:23:57.064046 crocodeel-1.0.4/README.md
+-rw-r--r--   0        0        0       85 2024-05-31 08:23:57.064046 crocodeel-1.0.4/crocodeel/__init__.py
+-rw-r--r--   0        0        0     1792 2024-05-31 08:23:57.064046 crocodeel-1.0.4/crocodeel/ab_table_utils.py
+-rw-r--r--   0        0        0     9263 2024-05-31 08:23:57.064046 crocodeel-1.0.4/crocodeel/common.py
+-rw-r--r--   0        0        0     2011 2024-05-31 08:23:57.064046 crocodeel-1.0.4/crocodeel/conta_event.py
+-rw-r--r--   0        0        0     8847 2024-05-31 08:23:57.064046 crocodeel-1.0.4/crocodeel/crocodeel.py
+-rw-r--r--   0        0        0      670 2024-05-31 08:23:57.064046 crocodeel-1.0.4/crocodeel/easy_wf.py
+-rw-r--r--   0        0        0     1435 2024-05-31 08:23:57.064046 crocodeel-1.0.4/crocodeel/execution_description.py
+-rw-r--r--   0        0        0   623880 2024-05-31 08:23:57.064046 crocodeel-1.0.4/crocodeel/models/crocodeel_rf_Mar2023.joblib
+-rw-r--r--   0        0        0     6412 2024-05-31 08:23:57.064046 crocodeel-1.0.4/crocodeel/plot_conta.py
+-rw-r--r--   0        0        0      731 2024-05-31 08:23:57.064046 crocodeel-1.0.4/crocodeel/rf_model.py
+-rw-r--r--   0        0        0     8371 2024-05-31 08:23:57.064046 crocodeel-1.0.4/crocodeel/search_conta.py
+-rw-r--r--   0        0        0   119253 2024-05-31 08:23:57.068046 crocodeel-1.0.4/crocodeel/test_data/mgs_profiles_test.tsv
+-rw-r--r--   0        0        0    49550 2024-05-31 08:23:57.068046 crocodeel-1.0.4/crocodeel/test_data/results/contamination_events.pdf
+-rw-r--r--   0        0        0     2051 2024-05-31 08:23:57.068046 crocodeel-1.0.4/crocodeel/test_data/results/contamination_events.tsv
+-rw-r--r--   0        0        0     2008 2024-05-31 08:23:57.068046 crocodeel-1.0.4/crocodeel/test_install.py
+-rw-r--r--   0        0        0     1377 2024-05-31 08:23:57.068046 crocodeel-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     5375 1970-01-01 00:00:00.000000 crocodeel-1.0.4/PKG-INFO
```

### Comparing `crocodeel-1.0.3/COPYING` & `crocodeel-1.0.4/COPYING`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.3/README.md` & `crocodeel-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.3/crocodeel/ab_table_utils.py` & `crocodeel-1.0.4/crocodeel/ab_table_utils.py`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.3/crocodeel/conta_event.py` & `crocodeel-1.0.4/crocodeel/conta_event.py`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.3/crocodeel/crocodeel.py` & `crocodeel-1.0.4/crocodeel/crocodeel.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import sys
 import argparse
 import logging
 import multiprocessing
 from importlib.metadata import version
 from crocodeel.execution_description import ExecutionDescription
-from crocodeel.search_conta import run_search_conta
+from crocodeel.search_conta import run_search_conta, run_search_conta_distrib
 from crocodeel.plot_conta import run_plot_conta, Defaults as plot_conta_defaults
 from crocodeel.easy_wf import run_easy_wf
 from crocodeel.test_install import run_test_install
 
 
 def set_logging() -> None:
     logger = logging.getLogger()
@@ -37,42 +37,118 @@
 
 def get_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="crocodeel")
     parser.add_argument(
         "-v", "--version", action="version", version=f"%(prog)s version { version("crocodeel")}"
     )
 
-
     subparsers = parser.add_subparsers(
         title="positional arguments",
-        help="Select subcommand",
+        help="Select command",
         dest="command",
         required=True,
     )
 
-    search_conta_parser = subparsers.add_parser(
+    easy_wf_parser = subparsers.add_parser(
+        "easy_wf",
+        help="Search cross-sample contamination and "
+        "create a PDF report in one command.",
+    )
+    easy_wf_parser.add_argument(
+        "-s",
+        dest="species_ab_table_fh",
+        type=argparse.FileType("r"),
+        required=True,
+        metavar='SPECIES_ABUNDANCE_TABLE',
+        help="Input TSV file giving the species abundance profiles in metagenomic samples",
+    )
+    easy_wf_parser.add_argument(
+       "-c",
+        dest="conta_events_fh",
+        type=argparse.FileType("w+"),
+        required=True,
+        metavar='CONTAMINATION_EVENTS_FILE',
+        help="Output TSV file listing all contamination events",
+    )
+    easy_wf_parser.add_argument(
+        "-r",
+        dest="pdf_report_fh",
+        type=argparse.FileType("wb"),
+        required=True,
+        metavar='PDF_REPORT_FILE',
+        help="Output PDF file with scatterplots for all contamination events",
+    )
+    easy_wf_parser.add_argument(
+        "--nproc",
+        dest="nproc",
+        type=nproc,
+        default=multiprocessing.cpu_count(),
+        help="Number of parallel processes to search for contaminations "
+        "(default: %(default)d)",
+    )
+
+    search_conta_distrib_parser = subparsers.add_parser(
         "search_conta", help="Search cross-sample contamination"
     )
-    search_conta_parser.add_argument(
+    search_conta_distrib_parser.add_argument(
         "-s",
         dest="species_ab_table_fh",
         type=argparse.FileType("r"),
         required=True,
         metavar='SPECIES_ABUNDANCE_TABLE',
         help="Input TSV file giving the species abundance profiles in metagenomic samples.",
     )
-    search_conta_parser.add_argument(
+    search_conta_distrib_parser.add_argument(
         "-c",
         dest="conta_events_fh",
         type=argparse.FileType("w"),
         required=True,
         metavar='CONTAMINATION_EVENTS_FILE',
         help="Output TSV file listing all contamination events.",
     )
-    search_conta_parser.add_argument(
+    search_conta_distrib_parser.add_argument(
+        "--nproc",
+        dest="nproc",
+        type=nproc,
+        default=multiprocessing.cpu_count(),
+        help="Number of parallel processes to search for contaminations "
+        "(default: %(default)d)",
+    )
+
+    search_conta_distrib_parser = subparsers.add_parser(
+        "search_conta_distrib", help="Search cross-sample contamination. "
+        "Command used in workflows to distribute computational load across multiple nodes."
+    )
+    search_conta_distrib_parser.add_argument(
+        "-s1",
+        dest="species_ab_table_fh",
+        type=argparse.FileType("r"),
+        required=True,
+        metavar='SPECIES_ABUNDANCE_TABLE',
+        help="Input TSV file giving the species abundance profiles in metagenomic samples."
+        " These samples are potential contamination sources.",
+    )
+    search_conta_distrib_parser.add_argument(
+        "-s2",
+        dest="species_ab_table_fh_2",
+        type=argparse.FileType("r"),
+        required=True,
+        metavar='SPECIES_ABUNDANCE_TABLE_2',
+        help="Input TSV file giving the species abundance profiles in metagenomic samples."
+        " These samples are potential contamination targets.",
+    )
+    search_conta_distrib_parser.add_argument(
+        "-c",
+        dest="conta_events_fh",
+        type=argparse.FileType("w"),
+        required=True,
+        metavar='CONTAMINATION_EVENTS_FILE',
+        help="Output TSV file listing all contamination events.",
+    )
+    search_conta_distrib_parser.add_argument(
         "--nproc",
         dest="nproc",
         type=nproc,
         default=multiprocessing.cpu_count(),
         help="Number of parallel processes to search for contaminations "
         "(default: %(default)d)",
     )
@@ -134,52 +210,14 @@
     plot_conta_parser.add_argument(
         "--color-conta-species",
         dest="color_conta_species",
         action="store_true",
         help="Use a different color for species introduced by contamination.",
     )
 
-    easy_wf_parser = subparsers.add_parser(
-        "easy_wf",
-        help="Search cross-sample contamination and "
-        "create a PDF report in one command.",
-    )
-    easy_wf_parser.add_argument(
-        "-s",
-        dest="species_ab_table_fh",
-        type=argparse.FileType("r"),
-        required=True,
-        metavar='SPECIES_ABUNDANCE_TABLE',
-        help="Input TSV file giving the species abundance profiles in metagenomic samples",
-    )
-    easy_wf_parser.add_argument(
-       "-c",
-        dest="conta_events_fh",
-        type=argparse.FileType("w+"),
-        required=True,
-        metavar='CONTAMINATION_EVENTS_FILE',
-        help="Output TSV file listing all contamination events",
-    )
-    easy_wf_parser.add_argument(
-        "-r",
-        dest="pdf_report_fh",
-        type=argparse.FileType("wb"),
-        required=True,
-        metavar='PDF_REPORT_FILE',
-        help="Output PDF file with scatterplots for all contamination events",
-    )
-    easy_wf_parser.add_argument(
-        "--nproc",
-        dest="nproc",
-        type=nproc,
-        default=multiprocessing.cpu_count(),
-        help="Number of parallel processes to search for contaminations "
-        "(default: %(default)d)",
-    )
-
     test_install_parser = subparsers.add_parser(
         "test_install", help="Test if %(prog)s is correctly installed "
         "and generates expected results"
     )
     test_install_parser.add_argument(
         "--keep",
         dest="keep_results",
@@ -195,18 +233,29 @@
     args = get_arguments()
 
     # Add comment line in output file describing execution context
     if args.command in ("search_conta","easy_wf"):
         exec_desc = ExecutionDescription(args.species_ab_table_fh.name)
         print(exec_desc, file = args.conta_events_fh)
 
-    if args.command == "search_conta":
+    if args.command == "search_conta_distrib":
+        exec_desc = ExecutionDescription(args.species_ab_table_fh.name,
+                                         args.species_ab_table_fh_2.name)
+        print(exec_desc, file = args.conta_events_fh)
+
+    if args.command == "easy_wf":
+        run_easy_wf(vars(args))
+    elif args.command == "search_conta":
         run_search_conta(vars(args))
+    elif args.command == "search_conta_distrib":
+        if args.species_ab_table_fh.name == args.species_ab_table_fh_2.name:
+            args.species_ab_table_fh_2.close()
+            run_search_conta(vars(args))
+        else:
+            run_search_conta_distrib(vars(args))
     elif args.command == "plot_conta":
         run_plot_conta(vars(args))
-    elif args.command == "easy_wf":
-        run_easy_wf(vars(args))
     elif args.command == "test_install":
         run_test_install(args.keep_results)
 
 if __name__ == "__main__":
     main()
```

### Comparing `crocodeel-1.0.3/crocodeel/easy_wf.py` & `crocodeel-1.0.4/crocodeel/easy_wf.py`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.3/crocodeel/execution_description.py` & `crocodeel-1.0.4/crocodeel/execution_description.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,36 @@
 from socket import gethostname
 from getpass import getuser
 from datetime import datetime
 from importlib.metadata import version
 from pathlib import Path
+from typing import Optional
 from crocodeel.rf_model import RandomForestModel
 
 class ExecutionDescription:
-    def __init__(self, species_ab_table_path : str) -> None:
+    def __init__(self, species_ab_table_path : str, species_ab_table_2_path : Optional[str] = None) -> None:
         self.software_version = version('crocodeel')
         self.rf_model_version = RandomForestModel.get_version()
         self.hostname = gethostname()
         self.username = getuser()
         self.datetime = datetime.now().replace(microsecond=0).isoformat()
         self.species_ab_table_path = Path(species_ab_table_path).resolve()
+        self.species_ab_table_2_path = (
+            Path(species_ab_table_2_path).resolve() if species_ab_table_2_path else None
+        )
 
     def __str__(self) -> str:
-        return (
+        exec_desc_str = (
             f"# crocodeel version: {self.software_version}"
             f" | rf_model_version: {self.rf_model_version}"
             f" | hostname: {self.hostname}"
             f" | username: {self.username}"
             f" | datetime: {self.datetime}"
             f" | species_ab_table: {self.species_ab_table_path}"
         )
+
+        if self.species_ab_table_2_path:
+            exec_desc_str = (
+                exec_desc_str + f" | species_ab_table_2: {self.species_ab_table_2_path}"
+            )
+
+        return exec_desc_str
```

### Comparing `crocodeel-1.0.3/crocodeel/models/crocodeel_rf_Mar2023.joblib` & `crocodeel-1.0.4/crocodeel/models/crocodeel_rf_Mar2023.joblib`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.3/crocodeel/plot_conta.py` & `crocodeel-1.0.4/crocodeel/plot_conta.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,8 +174,8 @@
                         self._create_plot(
                             self.conta_events[global_plot_id], axs[plot_id]
                         )
                     else:
                         axs[plot_id].axis("off")
                 plt.tight_layout()
                 fig.savefig(pdf, format="pdf")
-                plt.close(fig)
+                plt.close('all')
```

### Comparing `crocodeel-1.0.3/crocodeel/rf_model.py` & `crocodeel-1.0.4/crocodeel/rf_model.py`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.3/crocodeel/test_data/mgs_profiles_test.tsv` & `crocodeel-1.0.4/crocodeel/test_data/mgs_profiles_test.tsv`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.3/crocodeel/test_data/results/contamination_events.pdf` & `crocodeel-1.0.4/crocodeel/test_data/results/contamination_events.pdf`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.3/crocodeel/test_data/results/contamination_events.tsv` & `crocodeel-1.0.4/crocodeel/test_data/results/contamination_events.tsv`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.3/crocodeel/test_install.py` & `crocodeel-1.0.4/crocodeel/test_install.py`

 * *Files identical despite different names*

### Comparing `crocodeel-1.0.3/pyproject.toml` & `crocodeel-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crocodeel"
-version = "1.0.3"
+version = "1.0.4"
 description = "CroCoDeEL is a tool that detects cross-sample (aka well-to-well) contamination in shotgun metagenomic data"
 authors = [
     "Lindsay Goulet <lindsay.goulet@inrae.fr>",
     "Florian Plaza Oñate <florian.plaza-onate@inrae.fr>",
     "Edi Prifti <edi.prifti@ird.fr>",
     "Eugeni Belda <eugeni.belda@ird.fr>",
     "Emmanuelle Le Chatelier <emmanuelle.le-chatelier@inrae.fr>",
```

### Comparing `crocodeel-1.0.3/PKG-INFO` & `crocodeel-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crocodeel
-Version: 1.0.3
+Version: 1.0.4
 Summary: CroCoDeEL is a tool that detects cross-sample (aka well-to-well) contamination in shotgun metagenomic data
 Home-page: https://github.com/metagenopolis/CroCoDeEL
 License: GPL-3.0-or-later
 Keywords: Metagenomics
 Author: Lindsay Goulet
 Author-email: lindsay.goulet@inrae.fr
 Requires-Python: >=3.12
```

