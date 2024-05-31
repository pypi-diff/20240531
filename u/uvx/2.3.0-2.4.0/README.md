# Comparing `tmp/uvx-2.3.0.tar.gz` & `tmp/uvx-2.4.0.tar.gz`

## Comparing `uvx-2.3.0.tar` & `uvx-2.4.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0     2405 1970-01-01 00:00:00.000000 uvx-2.3.0/Cargo.toml
--rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.3.0/.cargo/config.toml
--rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.3.0/.gitignore
--rw-rw-r--   0     1000     1000     2312 2024-05-28 15:59:54.000000 uvx-2.3.0/CHANGELOG.md
--rw-rw-r--   0     1000     1000    91955 2024-05-28 15:59:01.000000 uvx-2.3.0/Cargo.lock
--rw-rw-r--   0     1000     1000     2456 2024-05-15 08:49:40.000000 uvx-2.3.0/README.md
--rwxrwxr-x   0     1000     1000      251 2024-05-01 11:18:56.000000 uvx-2.3.0/build.sh
--rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.3.0/rustfmt.toml
--rw-rw-r--   0     1000     1000     1805 2024-05-28 15:27:09.000000 uvx-2.3.0/src/animate.rs
--rw-rw-r--   0     1000     1000    12927 2024-05-28 15:26:22.000000 uvx-2.3.0/src/cli.rs
--rw-rw-r--   0     1000     1000     3177 2024-05-28 15:22:30.000000 uvx-2.3.0/src/cmd.rs
--rw-rw-r--   0     1000     1000     1346 2024-05-15 07:59:15.000000 uvx-2.3.0/src/commands/activate.rs
--rw-rw-r--   0     1000     1000     3765 2024-05-28 15:21:04.000000 uvx-2.3.0/src/commands/changelog.rs
--rw-rw-r--   0     1000     1000     3634 2024-05-28 15:37:31.000000 uvx-2.3.0/src/commands/check.rs
--rw-rw-r--   0     1000     1000      897 2024-05-28 15:21:21.000000 uvx-2.3.0/src/commands/completions.rs
--rw-rw-r--   0     1000     1000     1154 2024-05-28 15:21:12.000000 uvx-2.3.0/src/commands/create.rs
--rw-rw-r--   0     1000     1000     2519 2024-05-28 15:13:17.000000 uvx-2.3.0/src/commands/ensurepath.rs
--rw-rw-r--   0     1000     1000     1681 2024-05-28 15:10:13.000000 uvx-2.3.0/src/commands/inject.rs
--rw-rw-r--   0     1000     1000     5108 2024-05-28 15:09:27.000000 uvx-2.3.0/src/commands/install.rs
--rw-rw-r--   0     1000     1000     2673 2024-05-28 15:08:04.000000 uvx-2.3.0/src/commands/list.rs
--rw-rw-r--   0     1000     1000      388 2024-05-28 13:58:35.000000 uvx-2.3.0/src/commands/mod.rs
--rw-rw-r--   0     1000     1000     2558 2024-05-28 15:05:56.000000 uvx-2.3.0/src/commands/reinstall.rs
--rw-rw-r--   0     1000     1000     1414 2024-05-28 15:05:34.000000 uvx-2.3.0/src/commands/reinstall_all.rs
--rw-rw-r--   0     1000     1000     4031 2024-05-28 15:05:14.000000 uvx-2.3.0/src/commands/run.rs
--rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.3.0/src/commands/runpip.rs
--rw-rw-r--   0     1000     1000     1227 2024-05-28 15:19:42.000000 uvx-2.3.0/src/commands/runpython.rs
--rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.3.0/src/commands/runuv.rs
--rw-rw-r--   0     1000     1000     3238 2024-05-28 14:57:28.000000 uvx-2.3.0/src/commands/self_update.rs
--rw-rw-r--   0     1000     1000     3793 2024-05-28 14:47:03.000000 uvx-2.3.0/src/commands/setup.rs
--rw-rw-r--   0     1000     1000     1674 2024-05-28 14:44:42.000000 uvx-2.3.0/src/commands/uninject.rs
--rw-rw-r--   0     1000     1000     2069 2024-05-28 14:44:00.000000 uvx-2.3.0/src/commands/uninstall.rs
--rw-rw-r--   0     1000     1000     1016 2024-05-28 14:42:57.000000 uvx-2.3.0/src/commands/uninstall_all.rs
--rw-rw-r--   0     1000     1000     4167 2024-05-28 14:42:29.000000 uvx-2.3.0/src/commands/upgrade.rs
--rw-rw-r--   0     1000     1000     1089 2024-05-28 14:41:07.000000 uvx-2.3.0/src/commands/upgrade_all.rs
--rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.3.0/src/helpers.rs
--rw-rw-r--   0     1000     1000     1934 2024-05-28 14:08:13.000000 uvx-2.3.0/src/main.rs
--rw-rw-r--   0     1000     1000    13211 2024-05-28 14:56:01.000000 uvx-2.3.0/src/metadata.rs
--rw-rw-r--   0     1000     1000     4372 2024-05-28 14:27:42.000000 uvx-2.3.0/src/pip.rs
--rw-rw-r--   0     1000     1000     3128 2024-05-28 14:26:39.000000 uvx-2.3.0/src/pypi.rs
--rw-rw-r--   0     1000     1000      487 2024-05-13 18:28:56.000000 uvx-2.3.0/src/shell/activate.sh
--rw-rw-r--   0     1000     1000     3691 2024-05-28 14:26:22.000000 uvx-2.3.0/src/symlinks.rs
--rw-rw-r--   0     1000     1000     3735 2024-05-28 14:24:57.000000 uvx-2.3.0/src/uv.rs
--rw-rw-r--   0     1000     1000     2806 2024-05-28 14:10:08.000000 uvx-2.3.0/src/venv.rs
--rw-rw-r--   0     1000     1000     1003 2024-05-01 11:26:34.000000 uvx-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     3093 1970-01-01 00:00:00.000000 uvx-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2476 1970-01-01 00:00:00.000000 uvx-2.4.0/Cargo.toml
+-rw-rw-r--   0     1000     1000       77 2024-04-15 17:07:31.000000 uvx-2.4.0/.cargo/config.toml
+-rw-rw-r--   0     1000     1000      686 2024-04-11 15:03:17.000000 uvx-2.4.0/.gitignore
+-rw-rw-r--   0     1000     1000     2545 2024-05-31 18:52:24.000000 uvx-2.4.0/CHANGELOG.md
+-rw-rw-r--   0     1000     1000    91967 2024-05-31 18:52:42.000000 uvx-2.4.0/Cargo.lock
+-rw-rw-r--   0     1000     1000     2456 2024-05-15 08:49:40.000000 uvx-2.4.0/README.md
+-rwxrwxr-x   0     1000     1000      251 2024-05-01 11:18:56.000000 uvx-2.4.0/build.sh
+-rw-rw-r--   0     1000     1000      106 2024-04-15 17:06:44.000000 uvx-2.4.0/rustfmt.toml
+-rw-rw-r--   0     1000     1000     1805 2024-05-28 15:27:09.000000 uvx-2.4.0/src/animate.rs
+-rw-rw-r--   0     1000     1000    13029 2024-05-31 18:46:37.000000 uvx-2.4.0/src/cli.rs
+-rw-rw-r--   0     1000     1000     3177 2024-05-28 15:22:30.000000 uvx-2.4.0/src/cmd.rs
+-rw-rw-r--   0     1000     1000     1346 2024-05-15 07:59:15.000000 uvx-2.4.0/src/commands/activate.rs
+-rw-rw-r--   0     1000     1000     3765 2024-05-28 15:21:04.000000 uvx-2.4.0/src/commands/changelog.rs
+-rw-rw-r--   0     1000     1000     3604 2024-05-31 17:56:29.000000 uvx-2.4.0/src/commands/check.rs
+-rw-rw-r--   0     1000     1000      897 2024-05-28 15:21:21.000000 uvx-2.4.0/src/commands/completions.rs
+-rw-rw-r--   0     1000     1000     1154 2024-05-28 15:21:12.000000 uvx-2.4.0/src/commands/create.rs
+-rw-rw-r--   0     1000     1000     2519 2024-05-28 15:13:17.000000 uvx-2.4.0/src/commands/ensurepath.rs
+-rw-rw-r--   0     1000     1000     1681 2024-05-28 15:10:13.000000 uvx-2.4.0/src/commands/inject.rs
+-rw-rw-r--   0     1000     1000     5108 2024-05-28 15:09:27.000000 uvx-2.4.0/src/commands/install.rs
+-rw-rw-r--   0     1000     1000     2752 2024-05-31 18:31:57.000000 uvx-2.4.0/src/commands/list.rs
+-rw-rw-r--   0     1000     1000      388 2024-05-28 13:58:35.000000 uvx-2.4.0/src/commands/mod.rs
+-rw-rw-r--   0     1000     1000     2960 2024-05-31 18:37:11.000000 uvx-2.4.0/src/commands/reinstall.rs
+-rw-rw-r--   0     1000     1000     1514 2024-05-31 18:46:24.000000 uvx-2.4.0/src/commands/reinstall_all.rs
+-rw-rw-r--   0     1000     1000     4031 2024-05-28 15:05:14.000000 uvx-2.4.0/src/commands/run.rs
+-rw-rw-r--   0     1000     1000      621 2024-04-24 20:39:59.000000 uvx-2.4.0/src/commands/runpip.rs
+-rw-rw-r--   0     1000     1000     1227 2024-05-28 15:19:42.000000 uvx-2.4.0/src/commands/runpython.rs
+-rw-rw-r--   0     1000     1000      527 2024-04-24 20:39:25.000000 uvx-2.4.0/src/commands/runuv.rs
+-rw-rw-r--   0     1000     1000     3238 2024-05-28 14:57:28.000000 uvx-2.4.0/src/commands/self_update.rs
+-rw-rw-r--   0     1000     1000     3793 2024-05-28 14:47:03.000000 uvx-2.4.0/src/commands/setup.rs
+-rw-rw-r--   0     1000     1000     1674 2024-05-28 14:44:42.000000 uvx-2.4.0/src/commands/uninject.rs
+-rw-rw-r--   0     1000     1000     2298 2024-05-31 18:31:41.000000 uvx-2.4.0/src/commands/uninstall.rs
+-rw-rw-r--   0     1000     1000     1106 2024-05-31 18:46:13.000000 uvx-2.4.0/src/commands/uninstall_all.rs
+-rw-rw-r--   0     1000     1000     4460 2024-05-31 18:49:49.000000 uvx-2.4.0/src/commands/upgrade.rs
+-rw-rw-r--   0     1000     1000     1306 2024-05-31 18:49:49.000000 uvx-2.4.0/src/commands/upgrade_all.rs
+-rw-rw-r--   0     1000     1000      962 2024-04-24 20:32:00.000000 uvx-2.4.0/src/helpers.rs
+-rw-rw-r--   0     1000     1000     1948 2024-05-31 18:31:41.000000 uvx-2.4.0/src/main.rs
+-rw-rw-r--   0     1000     1000    14018 2024-05-31 17:58:16.000000 uvx-2.4.0/src/metadata.rs
+-rw-rw-r--   0     1000     1000     4372 2024-05-28 14:27:42.000000 uvx-2.4.0/src/pip.rs
+-rw-rw-r--   0     1000     1000      418 2024-05-31 18:14:43.000000 uvx-2.4.0/src/promises.rs
+-rw-rw-r--   0     1000     1000     3128 2024-05-28 14:26:39.000000 uvx-2.4.0/src/pypi.rs
+-rw-rw-r--   0     1000     1000      487 2024-05-13 18:28:56.000000 uvx-2.4.0/src/shell/activate.sh
+-rw-rw-r--   0     1000     1000     3691 2024-05-28 14:26:22.000000 uvx-2.4.0/src/symlinks.rs
+-rw-rw-r--   0     1000     1000     3735 2024-05-28 14:24:57.000000 uvx-2.4.0/src/uv.rs
+-rw-rw-r--   0     1000     1000     2806 2024-05-28 14:10:08.000000 uvx-2.4.0/src/venv.rs
+-rw-rw-r--   0     1000     1000     1003 2024-05-01 11:26:34.000000 uvx-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3093 1970-01-01 00:00:00.000000 uvx-2.4.0/PKG-INFO
```

### Comparing `uvx-2.3.0/Cargo.toml` & `uvx-2.4.0/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 name = "uvx"
 description = "uvx: pipx for uv (🦀)"
-version = "2.3.0"
+version = "2.4.0"
 edition = "2021"
-categories = ["development-tools", "development-tools::build-utils", "virtualization", "external-ffi-bindings"]
+categories = ["development-tools", "development-tools::build-utils", "virtualization", "external-ffi-bindings", "command-line-interface", "command-line-utilities"]
 keywords = ["Python", "uv", "pip", "packaging"]
 repository = "https://github.com/robinvandernoord/uvx2"
 license = "MIT"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
@@ -49,14 +49,15 @@
 pep440_rs = { git = "https://github.com/astral-sh/uv.git", tag = "0.2.4" }
 pep508_rs = { git = "https://github.com/astral-sh/uv.git", tag = "0.2.4" }
 # install-wheel-rs = { git = "https://github.com/astral-sh/uv.git", tag = "0.2.4" }
 # distribution-types = { git = "https://github.com/astral-sh/uv.git", tag = "0.2.4" }
 
 # security bumps/pins:
 rustls = "0.23.8"
+futures = "0.3.30"
 
 [lints.clippy]
 # categories:
 pedantic = { level = "warn", priority = -1 }
 nursery = { level = "warn", priority = -1 }
 cargo = { level = "warn", priority = -1 }
 # specific ones:
```

### Comparing `uvx-2.3.0/.gitignore` & `uvx-2.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/CHANGELOG.md` & `uvx-2.4.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v2.4.0 (2024-05-31)
+
+### Features
+
+* speed up `uvx list` (+ `uvx check`) with Futures and filtering before running checks (instead of after)
+* speed up `upgrade-all`, `reinstall-all`, `upgrade-all` and allow filtering venv names
+
 ## v2.3.0 (2024-05-28)
 
 ### Feature
 
 * `uvx check` to perform checks (like uvx list does) and report any problems.
 
 ### Refactoring
```

### Comparing `uvx-2.3.0/Cargo.lock` & `uvx-2.4.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3309,22 +3309,23 @@
  "once_cell",
  "owo-colors",
  "rustc-hash",
 ]
 
 [[package]]
 name = "uvx"
-version = "2.3.0"
+version = "2.4.0"
 dependencies = [
  "anstyle",
  "chrono",
  "clap",
  "clap_complete",
  "configparser",
  "directories",
+ "futures",
  "home",
  "itertools 0.13.0",
  "owo-colors",
  "pep440_rs",
  "pep508_rs",
  "regex",
  "reqwest",
```

### Comparing `uvx-2.3.0/README.md` & `uvx-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/animate.rs` & `uvx-2.4.0/src/animate.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/cli.rs` & `uvx-2.4.0/src/cli.rs`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,16 @@
 pub struct UninstallAllOptions {
     #[clap(
         short = 'f',
         long,
         help = "Remove executable with the same name (in ~/.local/bin) even if related venv was not found."
     )]
     pub force: bool,
+
+    pub venv_names: Vec<String>,
 }
 
 #[derive(Debug, Parser)]
 pub struct ReinstallOptions {
     pub package: String,
     #[clap(long, help = PYTHON_HELP_TEXT)]
     pub python: Option<String>,
@@ -191,24 +193,28 @@
         help = "Don't include previously injected libraries in reinstall"
     )]
     pub without_injected: bool,
     #[clap(long, help = "Run without `uv` cache")]
     pub no_cache: bool,
     #[clap(long, short, help = "(Re)install as editable")]
     pub editable: bool,
+
+    pub venv_names: Vec<String>,
 }
 
 #[derive(Debug, Parser)]
 pub struct UpgradeAllOptions {
     #[clap(short = 'f', long, help = "Ignore previous version constraint")]
     pub force: bool,
     #[clap(long, help = "Don't also upgrade injected packages")]
     pub skip_injected: bool,
     #[clap(long, help = "Run without `uv` cache")]
     pub no_cache: bool,
+
+    pub venv_names: Vec<String>,
 }
 
 #[derive(Debug, Parser)]
 pub struct RunOptions {
     pub package_name: String,
     #[clap(long, help = "Run without `uv` cache")]
     pub no_cache: bool,
```

### Comparing `uvx-2.3.0/src/cmd.rs` & `uvx-2.4.0/src/cmd.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/activate.rs` & `uvx-2.4.0/src/commands/activate.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/changelog.rs` & `uvx-2.4.0/src/commands/changelog.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/check.rs` & `uvx-2.4.0/src/commands/check.rs`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,19 @@
         // Display outdated issues
         if !self.outdated.is_empty() {
             println!("{}", "\n🔶 Outdated:".bold().yellow());
             for issue in &self.outdated {
                 println!("  - {}", issue.red());
             }
 
-            println!("{}", "💡 Tip: you can use `uvx upgrade <package>` to update a specific environment.".blue());
+            println!(
+                "{}",
+                "💡 Tip: you can use `uvx upgrade <package>` to update a specific environment."
+                    .blue()
+            );
         }
 
         // Display script issues
         if !self.scripts.is_empty() {
             println!("{}", "\n🔶 Missing Scripts:".bold().yellow());
             for (script, problems) in &self.scripts {
                 println!("  - {}", format!("{script}:").red().bold());
@@ -91,19 +95,15 @@
     }
 }
 
 impl Process for CheckOptions {
     async fn process(self) -> Result<i32, String> {
         let config = self.to_metadataconfig();
 
-        let mut items = list_packages(&config).await?;
-
-        if !self.venv_names.is_empty() {
-            items.retain(|k| self.venv_names.contains(&k.name));
-        }
+        let items = list_packages(&config, Some(&self.venv_names)).await?;
 
         let mut issues = Issues::new();
 
         for metadata in items {
             let invalid_scripts = metadata.invalid_scripts();
             if !self.skip_scripts && !invalid_scripts.is_empty() {
                 issues
```

### Comparing `uvx-2.3.0/src/commands/completions.rs` & `uvx-2.4.0/src/commands/completions.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/create.rs` & `uvx-2.4.0/src/commands/create.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/ensurepath.rs` & `uvx-2.4.0/src/commands/ensurepath.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/inject.rs` & `uvx-2.4.0/src/commands/inject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/install.rs` & `uvx-2.4.0/src/commands/install.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/list.rs` & `uvx-2.4.0/src/commands/list.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 use std::fs::ReadDir;
 
 use crate::cli::{ListOptions, Process};
 use crate::helpers::ResultToString;
 use crate::metadata::{get_venv_dir, LoadMetadataConfig, Metadata};
-use owo_colors::OwoColorize;
+use crate::promises::handle_promises;
 
-async fn read_from_folder(
+async fn read_from_folder_filtered(
     metadata_dir: ReadDir,
     config: &LoadMetadataConfig,
+    filter_names: &[String],
 ) -> Vec<Metadata> {
-    let mut result: Vec<Metadata> = vec![];
+    let mut promises = vec![];
 
     for dir in metadata_dir.flatten() {
-        if let Some(metadata) = Metadata::for_dir(&dir.path(), config).await {
-            result.push(metadata);
-        } else {
-            let venv_name = dir.file_name().into_string().unwrap_or_default();
+        let venv_name = dir.file_name().into_string().unwrap_or_default();
 
-            eprintln!("! metadata for '{}' could not be read!", venv_name.red());
+        if !filter_names.is_empty() && !filter_names.contains(&venv_name) {
+            continue;
         }
+
+        promises.push(
+            Metadata::for_owned_dir(dir.path(), config), // no .await so its a future (requires ownership of dir_path)
+        );
     }
 
-    result
+    handle_promises(promises).await
 }
 
 impl ListOptions {
     pub fn process_json(
         self,
         items: &Vec<Metadata>,
     ) -> Result<i32, String> {
@@ -46,37 +49,36 @@
             updates_check: !self.skip_updates,
             updates_prereleases: self.show_prereleases,
             updates_ignore_constraints: self.ignore_constraints,
         }
     }
 }
 
-pub async fn list_packages(config: &LoadMetadataConfig) -> Result<Vec<Metadata>, String> {
+pub async fn list_packages(
+    config: &LoadMetadataConfig,
+    filter_names: Option<&[String]>,
+) -> Result<Vec<Metadata>, String> {
     let venv_dir_path = get_venv_dir();
 
     // no tokio::fs because ReadDir.flatten doesn't exist then.
     let must_exist = if let Ok(dir) = std::fs::read_dir(&venv_dir_path) {
         dir
     } else {
         std::fs::create_dir_all(&venv_dir_path).map_err_to_string()?;
         std::fs::read_dir(&venv_dir_path).map_err_to_string()?
     };
 
-    Ok(read_from_folder(must_exist, config).await)
+    Ok(read_from_folder_filtered(must_exist, config, filter_names.unwrap_or(&[])).await)
 }
 
 impl Process for ListOptions {
     async fn process(self) -> Result<i32, String> {
         let config = self.to_metadataconfig();
 
-        let mut items = list_packages(&config).await?;
-
-        if !self.venv_names.is_empty() {
-            items.retain(|k| self.venv_names.contains(&k.name));
-        }
+        let items = list_packages(&config, Some(&self.venv_names)).await?;
 
         if self.json {
             return self.process_json(&items);
         }
 
         for metadata in items {
             if self.verbose {
```

### Comparing `uvx-2.3.0/src/commands/reinstall.rs` & `uvx-2.4.0/src/commands/reinstall.rs`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,34 @@
     cli::{Process, ReinstallOptions},
     commands::{install::install_package, uninstall::uninstall_package},
     metadata::{venv_path, Metadata},
     pip::parse_requirement,
     uv::ExtractInfo,
 };
 
+/// Version of `reinstall` that can be used with Futures
+pub async fn reinstall_owned(
+    install_spec: String,
+    python: Option<&String>,
+    force: bool,
+    with_injected: bool,
+    no_cache: bool,
+    editable: bool,
+) -> Result<String, String> {
+    reinstall(
+        &install_spec,
+        python,
+        force,
+        with_injected,
+        no_cache,
+        editable,
+    )
+    .await
+}
+
 pub async fn reinstall(
     install_spec: &str,
     python: Option<&String>,
     force: bool,
     with_injected: bool,
     no_cache: bool,
     editable: bool,
```

### Comparing `uvx-2.3.0/src/commands/reinstall_all.rs` & `uvx-2.4.0/src/commands/uninstall_all.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,40 @@
-use crate::cli::{Process, ReinstallAllOptions};
+use crate::cli::{Process, UninstallAllOptions};
 use crate::commands::list::list_packages;
-use crate::commands::reinstall::reinstall;
+use crate::commands::uninstall::uninstall_package_owned;
 use crate::metadata::LoadMetadataConfig;
-use owo_colors::OwoColorize;
+use crate::promises::handle_promises;
 
-pub async fn reinstall_all(
-    python: Option<&String>,
+pub async fn uninstall_all(
     force: bool,
-    without_injected: bool,
-    no_cache: bool,
-    editable: bool,
+    venv_names: &[String],
 ) -> Result<(), String> {
-    let mut all_ok = true;
+    let mut promises = vec![];
 
-    for meta in list_packages(&LoadMetadataConfig::none()).await? {
-        match reinstall(
-            &meta.name,
-            python,
-            force,
-            !without_injected,
-            no_cache,
-            editable,
-        )
-        .await
-        {
-            Ok(msg) => {
-                println!("{msg}");
-            },
-            Err(msg) => {
-                eprintln!("{}", msg.red());
-                all_ok = false;
-            },
-        }
+    for meta in list_packages(&LoadMetadataConfig::none(), Some(venv_names)).await? {
+        promises.push(uninstall_package_owned(meta.name, force));
     }
 
+    let promise_len = promises.len();
+    let results = handle_promises(promises).await;
+    let all_ok = promise_len == results.len();
+
+    for msg in results {
+        eprintln!("{msg}");
+    }
     if all_ok {
         Ok(())
     } else {
         Err(String::from(
-            "⚠️ Not all packages were properly reinstalled!",
+            "⚠️ Not all packages were properly uninstalled!",
         ))
     }
 }
 
-impl Process for ReinstallAllOptions {
+impl Process for UninstallAllOptions {
     async fn process(self) -> Result<i32, String> {
-        match reinstall_all(
-            self.python.as_ref(),
-            self.force,
-            self.without_injected,
-            self.no_cache,
-            self.editable,
-        )
-        .await
-        {
+        match uninstall_all(self.force, &self.venv_names).await {
             Ok(()) => Ok(0),
             Err(msg) => Err(msg),
         }
     }
 }
```

### Comparing `uvx-2.3.0/src/commands/run.rs` & `uvx-2.4.0/src/commands/run.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/runpip.rs` & `uvx-2.4.0/src/commands/runpip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/runpython.rs` & `uvx-2.4.0/src/commands/runpython.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/runuv.rs` & `uvx-2.4.0/src/commands/runuv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/self_update.rs` & `uvx-2.4.0/src/commands/self_update.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/setup.rs` & `uvx-2.4.0/src/commands/setup.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/uninject.rs` & `uvx-2.4.0/src/commands/uninject.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/commands/uninstall.rs` & `uvx-2.4.0/src/commands/uninstall.rs`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 use owo_colors::OwoColorize;
 
 use crate::cli::{Process, UninstallOptions};
 use crate::metadata::{venv_path, LoadMetadataConfig, Metadata};
 use crate::symlinks::{find_symlinks, remove_symlink, remove_symlinks};
 use crate::venv::{activate_venv, remove_venv};
 
+/// Version of `uninstall_package` that can be used with Futures
+pub async fn uninstall_package_owned(
+    package_name: String,
+    force: bool,
+) -> Result<String, String> {
+    uninstall_package(&package_name, force).await
+}
+
 pub async fn uninstall_package(
     package_name: &str,
     force: bool,
 ) -> Result<String, String> {
     let (requirement, _) = parse_requirement(package_name).await?;
     let requirement_name = requirement.name.to_string();
```

### Comparing `uvx-2.3.0/src/commands/upgrade.rs` & `uvx-2.4.0/src/commands/upgrade.rs`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,24 @@
     .await?;
 
     let new_version = update_metadata(metadata, requirement, environ, version).await?;
 
     Ok(build_msg(&old_version, &new_version, metadata))
 }
 
+/// Version of `upgrade_package` that can be used with Futures
+pub async fn upgrade_package_owned(
+    install_spec: String,
+    force: bool,
+    no_cache: bool,
+    skip_injected: bool,
+) -> Result<String, String> {
+    upgrade_package(&install_spec, force, no_cache, skip_injected).await
+}
+
 pub async fn upgrade_package(
     install_spec: &str,
     force: bool,
     no_cache: bool,
     skip_injected: bool,
 ) -> Result<String, String> {
     // No virtualenv for '{package_name}', stopping. Use 'uvx install' instead.
```

### Comparing `uvx-2.3.0/src/helpers.rs` & `uvx-2.4.0/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/main.rs` & `uvx-2.4.0/src/main.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 mod animate;
 mod cli;
 mod cmd;
 mod commands;
 mod helpers;
 mod metadata;
 mod pip;
+mod promises;
 mod pypi;
 mod symlinks;
 mod uv;
 mod venv;
 
 use std::io;
```

### Comparing `uvx-2.3.0/src/metadata.rs` & `uvx-2.4.0/src/metadata.rs`

 * *Files 2% similar despite different names*

```diff
@@ -163,14 +163,38 @@
         };
 
         self.fill_python(venv);
 
         Some(())
     }
 
+    /// like `for_dir` but with an owned dirname Pathbuf instead of &Path
+    /// (required to work with Futures) -> also returns a Result which is more useful with a future
+    pub async fn for_owned_dir(
+        dirname: PathBuf,
+        config: &LoadMetadataConfig,
+    ) -> Result<Self, String> {
+        let meta_path = dirname.join(".metadata");
+
+        Self::for_file(&meta_path, config).await.map_or_else(
+            || {
+                let venv_name = dirname
+                    .file_name()
+                    .and_then(|fname| fname.to_str())
+                    .unwrap_or_default();
+
+                Err(format!(
+                    "Metadata for '{}' could not be loaded.",
+                    venv_name.red()
+                ))
+            },
+            Ok,
+        )
+    }
+
     pub async fn for_dir(
         dirname: &Path,
         config: &LoadMetadataConfig,
     ) -> Option<Self> {
         let meta_path = dirname.join(".metadata");
 
         Self::for_file(&meta_path, config).await
@@ -179,15 +203,16 @@
     pub async fn for_requirement(
         requirement: &Requirement,
         config: &LoadMetadataConfig,
     ) -> Self {
         let requirement_name = requirement.name.to_string();
         let venv_dir = venv_path(&requirement_name);
 
-        (Self::for_dir(&venv_dir, config).await)
+        Self::for_dir(&venv_dir, config)
+            .await
             .map_or_else(|| Self::find(requirement), |meta| meta)
     }
 
     pub async fn for_file(
         filename: &Path,
         config: &LoadMetadataConfig,
     ) -> Option<Self> {
```

### Comparing `uvx-2.3.0/src/pip.rs` & `uvx-2.4.0/src/pip.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/pypi.rs` & `uvx-2.4.0/src/pypi.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/symlinks.rs` & `uvx-2.4.0/src/symlinks.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/uv.rs` & `uvx-2.4.0/src/uv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/src/venv.rs` & `uvx-2.4.0/src/venv.rs`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/pyproject.toml` & `uvx-2.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uvx-2.3.0/PKG-INFO` & `uvx-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uvx
-Version: 2.3.0
+Version: 2.4.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Requires-Dist: uv
 Requires-Dist: pip
```

