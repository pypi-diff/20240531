# Comparing `tmp/oasysdb-0.5.1.tar.gz` & `tmp/oasysdb-0.6.0.tar.gz`

## Comparing `oasysdb-0.5.1.tar` & `oasysdb-0.6.0.tar`

### file list

```diff
@@ -1,63 +1,64 @@
--rw-r--r--   0        0        0     1540 1970-01-01 00:00:00.000000 oasysdb-0.5.1/Cargo.toml
--rw-r--r--   0     1001      127       30 2024-05-25 03:10:31.000000 oasysdb-0.5.1/.cargo/config.toml
--rw-r--r--   0     1001      127      167 2024-05-25 03:10:31.000000 oasysdb-0.5.1/.editorconfig
--rw-r--r--   0     1001      127       51 2024-05-25 03:10:31.000000 oasysdb-0.5.1/.env.example
--rw-r--r--   0     1001      127       33 2024-05-25 03:10:31.000000 oasysdb-0.5.1/.flake8
--rw-r--r--   0     1001      127      761 2024-05-25 03:10:31.000000 oasysdb-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0     1001      127      331 2024-05-25 03:10:31.000000 oasysdb-0.5.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0     1001      127      496 2024-05-25 03:10:31.000000 oasysdb-0.5.1/.github/ISSUE_TEMPLATE/do_chore.md
--rw-r--r--   0     1001      127      664 2024-05-25 03:10:31.000000 oasysdb-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0     1001      127     3048 2024-05-25 03:10:31.000000 oasysdb-0.5.1/.github/workflows/deploy-python.yml
--rw-r--r--   0     1001      127      477 2024-05-25 03:10:31.000000 oasysdb-0.5.1/.github/workflows/deploy-rust.yml
--rw-r--r--   0     1001      127     2340 2024-05-25 03:10:31.000000 oasysdb-0.5.1/.github/workflows/quality-check.yml
--rw-r--r--   0     1001      127      220 2024-05-25 03:10:31.000000 oasysdb-0.5.1/.gitignore
--rw-r--r--   0     1001      127       93 2024-05-25 03:10:31.000000 oasysdb-0.5.1/.prettierrc.yml
--rw-r--r--   0     1001      127    50679 2024-05-25 03:10:31.000000 oasysdb-0.5.1/Cargo.lock
--rw-r--r--   0     1001      127     1983 2024-05-25 03:10:31.000000 oasysdb-0.5.1/bench/main.rs
--rw-r--r--   0     1001      127      403 2024-05-25 03:10:31.000000 oasysdb-0.5.1/bench/utils.rs
--rw-r--r--   0     1001      127    10405 2024-05-25 03:10:31.000000 oasysdb-0.5.1/docs/changelog.md
--rw-r--r--   0     1001      127     5481 2024-05-25 03:10:31.000000 oasysdb-0.5.1/docs/code_of_conduct.md
--rw-r--r--   0     1001      127     5537 2024-05-25 03:10:31.000000 oasysdb-0.5.1/docs/contributing.md
--rw-r--r--   0     1001      127    10608 2024-05-25 03:10:31.000000 oasysdb-0.5.1/docs/guide.md
--rw-r--r--   0     1001      127     3866 2024-05-25 03:10:31.000000 oasysdb-0.5.1/docs/migrations/0.4.5-to-0.5.0.md
--rw-r--r--   0     1001      127      798 2024-05-25 03:10:31.000000 oasysdb-0.5.1/docs/pull_request_template.md
--rw-r--r--   0     1001      127      722 2024-05-25 03:10:31.000000 oasysdb-0.5.1/docs/security.md
--rw-r--r--   0     1001      127      453 2024-05-25 03:10:31.000000 oasysdb-0.5.1/examples/extract-metadata.rs
--rw-r--r--   0     1001      127      695 2024-05-25 03:10:31.000000 oasysdb-0.5.1/examples/measure-memory.rs
--rw-r--r--   0     1001      127      886 2024-05-25 03:10:31.000000 oasysdb-0.5.1/examples/quickstart.rs
--rw-r--r--   0     1001      127    10173 2024-05-25 03:10:31.000000 oasysdb-0.5.1/license
--rw-r--r--   0     1001      127      710 2024-05-25 03:10:31.000000 oasysdb-0.5.1/py/example.py
--rw-r--r--   0     1001      127       43 2024-05-25 03:10:31.000000 oasysdb-0.5.1/py/oasysdb/__init__.py
--rw-r--r--   0     1001      127     5150 2024-05-25 03:10:31.000000 oasysdb-0.5.1/py/oasysdb/collection.pyi
--rw-r--r--   0     1001      127     1456 2024-05-25 03:10:31.000000 oasysdb-0.5.1/py/oasysdb/database.pyi
--rw-r--r--   0     1001      127      119 2024-05-25 03:10:31.000000 oasysdb-0.5.1/py/oasysdb/prelude.pyi
--rw-r--r--   0     1001      127        0 2024-05-25 03:10:31.000000 oasysdb-0.5.1/py/oasysdb/py.typed
--rw-r--r--   0     1001      127      757 2024-05-25 03:10:31.000000 oasysdb-0.5.1/py/oasysdb/vector.pyi
--rw-r--r--   0     1001      127     7018 2024-05-25 03:10:31.000000 oasysdb-0.5.1/py/tests/test_collection.py
--rw-r--r--   0     1001      127     1593 2024-05-25 03:10:31.000000 oasysdb-0.5.1/py/tests/test_database.py
--rw-r--r--   0     1001      127      390 2024-05-25 03:10:31.000000 oasysdb-0.5.1/py/tests/test_vector.py
--rw-r--r--   0     1001      127    11126 2024-05-25 03:10:31.000000 oasysdb-0.5.1/readme.md
--rw-r--r--   0     1001      127       57 2024-05-25 03:10:31.000000 oasysdb-0.5.1/requirements.txt
--rw-r--r--   0     1001      127      104 2024-05-25 03:10:31.000000 oasysdb-0.5.1/rustfmt.toml
--rw-r--r--   0     1001      127     8382 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/db/database.rs
--rw-r--r--   0     1001      127      479 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/db/mod.rs
--rw-r--r--   0     1001      127    28500 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/func/collection.rs
--rw-r--r--   0     1001      127     2581 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/func/distance.rs
--rw-r--r--   0     1001      127     4240 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/func/err.rs
--rw-r--r--   0     1001      127     8913 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/func/metadata.rs
--rw-r--r--   0     1001      127      945 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/func/mod.rs
--rw-r--r--   0     1001      127    12980 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/func/utils.rs
--rw-r--r--   0     1001      127     3342 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/func/vector.rs
--rw-r--r--   0     1001      127     2380 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/lib.rs
--rw-r--r--   0     1001      127       13 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/main.rs
--rw-r--r--   0     1001      127      193 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/prelude/mod.rs
--rw-r--r--   0     1001      127     1060 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/tests/mod.rs
--rw-r--r--   0     1001      127     6205 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/tests/test_collection.rs
--rw-r--r--   0     1001      127     1566 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/tests/test_database.rs
--rw-r--r--   0     1001      127      505 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/tests/test_distance.rs
--rw-r--r--   0     1001      127      663 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/tests/test_metadata.rs
--rw-r--r--   0     1001      127      704 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/tests/test_vectorgen.rs
--rw-r--r--   0     1001      127      956 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/vectorgen/mod.rs
--rw-r--r--   0     1001      127     2533 2024-05-25 03:10:31.000000 oasysdb-0.5.1/src/vectorgen/openai.rs
--rw-r--r--   0     1001      127      646 2024-05-25 03:10:31.000000 oasysdb-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    11899 1970-01-01 00:00:00.000000 oasysdb-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1540 1970-01-01 00:00:00.000000 oasysdb-0.6.0/Cargo.toml
+-rw-r--r--   0     1001      127       30 2024-05-31 02:03:45.000000 oasysdb-0.6.0/.cargo/config.toml
+-rw-r--r--   0     1001      127      167 2024-05-31 02:03:45.000000 oasysdb-0.6.0/.editorconfig
+-rw-r--r--   0     1001      127       51 2024-05-31 02:03:45.000000 oasysdb-0.6.0/.env.example
+-rw-r--r--   0     1001      127       33 2024-05-31 02:03:45.000000 oasysdb-0.6.0/.flake8
+-rw-r--r--   0     1001      127      761 2024-05-31 02:03:45.000000 oasysdb-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      127      331 2024-05-31 02:03:45.000000 oasysdb-0.6.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0     1001      127      496 2024-05-31 02:03:45.000000 oasysdb-0.6.0/.github/ISSUE_TEMPLATE/do_chore.md
+-rw-r--r--   0     1001      127      664 2024-05-31 02:03:45.000000 oasysdb-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      127     3048 2024-05-31 02:03:45.000000 oasysdb-0.6.0/.github/workflows/deploy-python.yml
+-rw-r--r--   0     1001      127      477 2024-05-31 02:03:45.000000 oasysdb-0.6.0/.github/workflows/deploy-rust.yml
+-rw-r--r--   0     1001      127     2340 2024-05-31 02:03:45.000000 oasysdb-0.6.0/.github/workflows/quality-check.yml
+-rw-r--r--   0     1001      127      220 2024-05-31 02:03:45.000000 oasysdb-0.6.0/.gitignore
+-rw-r--r--   0     1001      127       93 2024-05-31 02:03:45.000000 oasysdb-0.6.0/.prettierrc.yml
+-rw-r--r--   0     1001      127    50679 2024-05-31 02:03:45.000000 oasysdb-0.6.0/Cargo.lock
+-rw-r--r--   0     1001      127     3101 2024-05-31 02:03:45.000000 oasysdb-0.6.0/bench/main.rs
+-rw-r--r--   0     1001      127      834 2024-05-31 02:03:45.000000 oasysdb-0.6.0/bench/utils.rs
+-rw-r--r--   0     1001      127    11464 2024-05-31 02:03:45.000000 oasysdb-0.6.0/docs/changelog.md
+-rw-r--r--   0     1001      127     5481 2024-05-31 02:03:45.000000 oasysdb-0.6.0/docs/code_of_conduct.md
+-rw-r--r--   0     1001      127     5537 2024-05-31 02:03:45.000000 oasysdb-0.6.0/docs/contributing.md
+-rw-r--r--   0     1001      127     9804 2024-05-31 02:03:45.000000 oasysdb-0.6.0/docs/guide.md
+-rw-r--r--   0     1001      127     3866 2024-05-31 02:03:45.000000 oasysdb-0.6.0/docs/migrations/0.4.5-to-0.5.0.md
+-rw-r--r--   0     1001      127      798 2024-05-31 02:03:45.000000 oasysdb-0.6.0/docs/pull_request_template.md
+-rw-r--r--   0     1001      127      722 2024-05-31 02:03:45.000000 oasysdb-0.6.0/docs/security.md
+-rw-r--r--   0     1001      127      453 2024-05-31 02:03:45.000000 oasysdb-0.6.0/examples/extract-metadata.rs
+-rw-r--r--   0     1001      127      695 2024-05-31 02:03:45.000000 oasysdb-0.6.0/examples/measure-memory.rs
+-rw-r--r--   0     1001      127     1654 2024-05-31 02:03:45.000000 oasysdb-0.6.0/examples/measure-recall.rs
+-rw-r--r--   0     1001      127      886 2024-05-31 02:03:45.000000 oasysdb-0.6.0/examples/quickstart.rs
+-rw-r--r--   0     1001      127    10173 2024-05-31 02:03:45.000000 oasysdb-0.6.0/license
+-rw-r--r--   0     1001      127      710 2024-05-31 02:03:45.000000 oasysdb-0.6.0/py/example.py
+-rw-r--r--   0     1001      127       43 2024-05-31 02:03:45.000000 oasysdb-0.6.0/py/oasysdb/__init__.py
+-rw-r--r--   0     1001      127     5122 2024-05-31 02:03:45.000000 oasysdb-0.6.0/py/oasysdb/collection.pyi
+-rw-r--r--   0     1001      127     1456 2024-05-31 02:03:45.000000 oasysdb-0.6.0/py/oasysdb/database.pyi
+-rw-r--r--   0     1001      127      119 2024-05-31 02:03:45.000000 oasysdb-0.6.0/py/oasysdb/prelude.pyi
+-rw-r--r--   0     1001      127        0 2024-05-31 02:03:45.000000 oasysdb-0.6.0/py/oasysdb/py.typed
+-rw-r--r--   0     1001      127      757 2024-05-31 02:03:45.000000 oasysdb-0.6.0/py/oasysdb/vector.pyi
+-rw-r--r--   0     1001      127     6848 2024-05-31 02:03:45.000000 oasysdb-0.6.0/py/tests/test_collection.py
+-rw-r--r--   0     1001      127     1593 2024-05-31 02:03:45.000000 oasysdb-0.6.0/py/tests/test_database.py
+-rw-r--r--   0     1001      127      390 2024-05-31 02:03:45.000000 oasysdb-0.6.0/py/tests/test_vector.py
+-rw-r--r--   0     1001      127    11126 2024-05-31 02:03:45.000000 oasysdb-0.6.0/readme.md
+-rw-r--r--   0     1001      127       57 2024-05-31 02:03:45.000000 oasysdb-0.6.0/requirements.txt
+-rw-r--r--   0     1001      127      104 2024-05-31 02:03:45.000000 oasysdb-0.6.0/rustfmt.toml
+-rw-r--r--   0     1001      127     8382 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/db/database.rs
+-rw-r--r--   0     1001      127      479 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/db/mod.rs
+-rw-r--r--   0     1001      127    27256 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/func/collection.rs
+-rw-r--r--   0     1001      127     1840 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/func/distance.rs
+-rw-r--r--   0     1001      127     4240 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/func/err.rs
+-rw-r--r--   0     1001      127     8913 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/func/metadata.rs
+-rw-r--r--   0     1001      127      945 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/func/mod.rs
+-rw-r--r--   0     1001      127    12339 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/func/utils.rs
+-rw-r--r--   0     1001      127     3342 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/func/vector.rs
+-rw-r--r--   0     1001      127     2380 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/lib.rs
+-rw-r--r--   0     1001      127       13 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/main.rs
+-rw-r--r--   0     1001      127      193 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/prelude/mod.rs
+-rw-r--r--   0     1001      127     1060 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/tests/mod.rs
+-rw-r--r--   0     1001      127     6198 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/tests/test_collection.rs
+-rw-r--r--   0     1001      127     1566 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/tests/test_database.rs
+-rw-r--r--   0     1001      127      501 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/tests/test_distance.rs
+-rw-r--r--   0     1001      127      663 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/tests/test_metadata.rs
+-rw-r--r--   0     1001      127      704 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/tests/test_vectorgen.rs
+-rw-r--r--   0     1001      127      956 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/vectorgen/mod.rs
+-rw-r--r--   0     1001      127     2533 2024-05-31 02:03:45.000000 oasysdb-0.6.0/src/vectorgen/openai.rs
+-rw-r--r--   0     1001      127      646 2024-05-31 02:03:45.000000 oasysdb-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0    11899 1970-01-01 00:00:00.000000 oasysdb-0.6.0/PKG-INFO
```

### Comparing `oasysdb-0.5.1/Cargo.toml` & `oasysdb-0.6.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "oasysdb"
-version = "0.5.1"
+version = "0.6.0"
 edition = "2021"
 license = "Apache-2.0"
 readme = "readme.md"
 
 # Information.
 authors = ["Edwin Kys", "Oasys"]
 description = "Fast embedded vector database with incremental HNSW indexing."
```

### Comparing `oasysdb-0.5.1/.github/ISSUE_TEMPLATE/bug_report.md` & `oasysdb-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/.github/ISSUE_TEMPLATE/feature_request.md` & `oasysdb-0.6.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/.github/workflows/deploy-python.yml` & `oasysdb-0.6.0/.github/workflows/deploy-python.yml`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/.github/workflows/quality-check.yml` & `oasysdb-0.6.0/.github/workflows/quality-check.yml`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/Cargo.lock` & `oasysdb-0.6.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -833,15 +833,15 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "oasysdb"
-version = "0.5.1"
+version = "0.6.0"
 dependencies = [
  "bincode",
  "criterion",
  "dotenv",
  "futures",
  "jemalloc-ctl",
  "jemallocator",
```

### Comparing `oasysdb-0.5.1/bench/main.rs` & `oasysdb-0.6.0/bench/main.rs`

 * *Files 14% similar despite different names*

```diff
@@ -66,8 +66,44 @@
 criterion_group!(
     collection,
     bench_search_collection,
     bench_true_search_collection,
     bench_insert_to_collection
 );
 
-criterion_main!(collection);
+fn bench_save_collection_to_database(criterion: &mut Criterion) {
+    let id = "save collection to database";
+
+    // Setup the database and collection.
+    let collection = build_test_collection(DIMENSION, COLLECTION_SIZE);
+    let mut db = create_test_database(DIMENSION, COLLECTION_SIZE);
+
+    // Benchmark the save speed.
+    criterion.bench_function(id, |bencher| {
+        bencher.iter(|| {
+            black_box(db.save_collection("bench", &collection).unwrap());
+        })
+    });
+}
+
+fn bench_get_collection_from_database(criterion: &mut Criterion) {
+    let id = "get collection from database";
+    let db = create_test_database(DIMENSION, COLLECTION_SIZE);
+
+    // Benchmark the get speed.
+    // This is the operation that loads the collection into memory.
+    let routine = || {
+        black_box(db.get_collection("bench").unwrap());
+    };
+
+    criterion.bench_function(id, |b| b.iter(routine));
+}
+
+criterion_group! {
+    name = database;
+    config = Criterion::default().sample_size(10);
+    targets =
+        bench_save_collection_to_database,
+        bench_get_collection_from_database
+}
+
+criterion_main!(collection, database);
```

### Comparing `oasysdb-0.5.1/docs/changelog.md` & `oasysdb-0.6.0/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+# v0.6.0
+
+### What's Changed
+
+- **CONDITIONAL BREAKING CHANGE**: We remove support for dot distance metric and we replace cosine similarity with cosine distance metric. This change is made to make the distance metric consistent with the other distance metrics.
+- The default configuration for the collection (EF Construction and EF Search) is increased to a more sensible value according to the common real-world use cases. The default EF Construction is set to 128 and the default EF Search is set to 64.
+- We add a new script to measure the recall rate of the collection search functionality. And with this, we improve the search recall rate of OasysDB to match the recall rate of HNSWLib with the same configuration.
+
+  ```sh
+  cargo run --example measure-recall
+  ```
+
+- We add a new benchmark to measure the performance of saving and getting the collection. The benchmark can be run by running the command below.
+
+  ```sh
+  cargo bench
+  ```
+
+### Contributors
+
+- @edwinkys
+
+### Full Changelog
+
+https://github.com/oasysai/oasysdb/compare/v0.5.1...v0.6.0
+
 # v0.5.1
 
 ### What's Changed
 
 We add a new method `Collection.filter` to filter the vector records based on the metadata. This method returns a HashMap of the filtered vector records and their corresponding vector IDs. This implementation performs a linear search through the collection and thus might be slow for large datasets.
 
 This implementation includes support for the following metadata to filter:
```

### Comparing `oasysdb-0.5.1/docs/code_of_conduct.md` & `oasysdb-0.6.0/docs/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/docs/contributing.md` & `oasysdb-0.6.0/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/docs/guide.md` & `oasysdb-0.6.0/docs/guide.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,27 +113,16 @@
 
 ## Distance Metric
 
 For collections in OasysDB, you can specify the distance metric to use when calculating the distance between vectors. The distance metric is used mostly when inserting a new vector record into the collection and a bit when performing a search operation.
 
 As of the current version, OasysDB supports the following distance metrics:
 
-- [Euclidean](https://en.wikipedia.org/wiki/Euclidean_distance)
-- [Cosine Similarity](https://en.wikipedia.org/wiki/Cosine_similarity)
-- [Dot Product](https://en.wikipedia.org/wiki/Dot_product)
-
-### Cosine VS Normalized Cosine
-
-A lot of embedding models seem to recommend using cosine similarity as the distance metric. This is because cosine similarity is invariant to the magnitude of the vectors and only measures the angle between them which makes it easy to work with.
-
-With OasysDB, you can use the default **Cosine** or the **Normalized Cosine** distance metric.
-
-With the default Cosine, it will calculate both the dot product and the magnitude of the vectors to calculate the cosine similarity as you would expect.
-
-But for models that already normalize the vectors, you can use the Normalized Cosine distance metric. This will skip the magnitude calculation and only calculate the dot product which will result in a faster insert and search operation.
+- [Euclidean Distance](https://en.wikipedia.org/wiki/Euclidean_distance)
+- [Cosine Distance](https://en.wikipedia.org/wiki/Cosine_similarity#Cosine_distance)
 
 ## Relevancy Score
 
 Relevancy score is a big part of OasysDB. It allows you to essentially exclude vectors that are not relevant to your search query.
 
 Unlike other configurations, the relevancy score can be changed after the collection is created. I even encourage you to experiment with different relevancy scores to see what works best for your use case 😁
```

### Comparing `oasysdb-0.5.1/docs/migrations/0.4.5-to-0.5.0.md` & `oasysdb-0.6.0/docs/migrations/0.4.5-to-0.5.0.md`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/docs/pull_request_template.md` & `oasysdb-0.6.0/docs/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/docs/security.md` & `oasysdb-0.6.0/docs/security.md`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/examples/measure-memory.rs` & `oasysdb-0.6.0/examples/measure-memory.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/examples/quickstart.rs` & `oasysdb-0.6.0/examples/quickstart.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/license` & `oasysdb-0.6.0/license`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/py/example.py` & `oasysdb-0.6.0/py/example.py`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/py/oasysdb/collection.pyi` & `oasysdb-0.6.0/py/oasysdb/collection.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,15 @@
     - ef_construction: Nodes to consider during index construction.
     - ef_search: Nodes to consider during the search.
     - ml: Layer multiplier of the HNSW index.
     - distance: Distance metric function.
 
     Distance metrics:
     - euclidean
-    - dot
     - cosine
-    - norm_cosine
     """
 
     ef_construction: int
     ef_search: int
     ml: float
     distance: str
```

### Comparing `oasysdb-0.5.1/py/oasysdb/database.pyi` & `oasysdb-0.6.0/py/oasysdb/database.pyi`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/py/oasysdb/vector.pyi` & `oasysdb-0.6.0/py/oasysdb/vector.pyi`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/py/tests/test_collection.py` & `oasysdb-0.6.0/py/tests/test_collection.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 
 def test_create_config():
     default = Config.create_default()
 
     # Create config based on the default.
     config = Config(
-        ef_construction=40,
-        ef_search=15,
+        ef_construction=128,
+        ef_search=64,
         ml=0.2885,
         distance="euclidean"
     )
 
     assert config.ef_construction == default.ef_construction
     assert config.ef_search == default.ef_search
     assert config.ml == default.ml
@@ -209,20 +209,16 @@
     collection.insert_many(records)
 
     # Search for the record.
     query = Vector.random(dimension=DIMENSION)
     results = collection.search(query, n=k)
     true_results = collection.true_search(query, n=k)
 
-    # Sort result based on distance descending.
-    sort = sorted(results, key=lambda x: x.distance, reverse=True)
-
     for i in range(k):
         assert results[i].distance == true_results[i].distance
-        assert results[i].distance == sort[i].distance
 
 
 def test_collection_filter_text():
     collection = create_test_collection()
 
     # Insert records with text data.
     data = "OasysDB is awesome!"
```

### Comparing `oasysdb-0.5.1/py/tests/test_database.py` & `oasysdb-0.6.0/py/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/readme.md` & `oasysdb-0.6.0/readme.md`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/src/db/database.rs` & `oasysdb-0.6.0/src/db/database.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/src/func/collection.rs` & `oasysdb-0.6.0/src/func/collection.rs`

 * *Files 3% similar despite different names*

```diff
@@ -75,31 +75,31 @@
         distance: &str,
     ) -> Result<Self, Error> {
         let distance = Distance::from(distance)?;
         Ok(Self { ef_construction, ef_search, ml, distance })
     }
 
     /// Sets the distance calculation function.
-    /// * `distance`: Distance function, e.g. euclidean or dot.
+    /// * `distance`: Distance function, e.g. euclidean.
     pub fn set_distance(&mut self, distance: &str) -> Result<(), Error> {
         self.distance = Distance::from(distance)?;
         Ok(())
     }
 }
 
 impl Default for Config {
     /// Default configuration for the collection index.
-    /// * `ef_construction`: 40
-    /// * `ef_search`: 15
+    /// * `ef_construction`: 128
+    /// * `ef_search`: 64
     /// * `ml`: 0.2885
     /// * `distance`: euclidean
     fn default() -> Self {
         Self {
-            ef_construction: 40,
-            ef_search: 15,
+            ef_construction: 128,
+            ef_search: 64,
             ml: 0.2885,
             distance: Distance::Euclidean,
         }
     }
 }
 
 /// The collection of vector records with HNSW indexing.
@@ -350,42 +350,36 @@
             }
         };
 
         search.visited.resize_capacity(self.vectors.len());
         search.push(vector_id, vector, &self.vectors);
 
         for layer in LayerID(self.upper_layers.len()).descend() {
-            search.ef = if layer.is_zero() { self.config.ef_search } else { 5 };
+            search.ef = self.config.ef_search;
 
             if layer.0 == 0 {
                 let layer = self.base_layer.as_slice();
                 search.search(layer, vector, &self.vectors, M * 2);
             } else {
                 let layer = self.upper_layers[layer.0 - 1].as_slice();
                 search.search(layer, vector, &self.vectors, M);
-            }
-
-            if !layer.is_zero() {
                 search.cull();
             }
         }
 
         let map_result = |candidate: Candidate| {
             let id = candidate.vector_id.0;
             let distance = candidate.distance.0;
             let data = self.data[&candidate.vector_id].clone();
             SearchResult { id, distance, data }
         };
 
-        // Sort the search results by distance.
-        let res = search.iter().map(map_result).collect();
-        let sorted = self.sort_by_distance(res);
-
         // Truncate the list based on the relevancy score.
-        let mut relevant = self.truncate_irrelevant_result(sorted);
+        let res = search.iter().map(map_result).collect();
+        let mut relevant = self.truncate_irrelevant_result(res);
         relevant.truncate(n);
         Ok(relevant)
     }
 
     /// Searches the collection for the true nearest neighbors.
     /// * `vector`: Vector to search.
     /// * `n`: Number of neighbors to return.
@@ -404,19 +398,24 @@
         for (id, vec) in self.vectors.iter() {
             let distance = self.config.distance.calculate(vector, vec);
             let data = self.data[id].clone();
             let res = SearchResult { id: id.0, distance, data };
             nearest.push(res);
         }
 
-        // Sort the results by distance depending on the metric.
-        let sorted = self.sort_by_distance(nearest);
+        // Sort the results by distance in ascending order.
+        // The closest the distance, the better the match.
+        let sort_ascending = |a: &SearchResult, b: &SearchResult| {
+            a.distance.partial_cmp(&b.distance).unwrap()
+        };
+
+        nearest.par_sort_by(sort_ascending);
 
         // Remove irrelevant results and truncate the list.
-        let mut res = self.truncate_irrelevant_result(sorted);
+        let mut res = self.truncate_irrelevant_result(nearest);
         res.truncate(n);
         Ok(res)
     }
 
     /// Returns the number of vector records in the collection.
     pub fn len(&self) -> usize {
         self.count
@@ -787,54 +786,19 @@
         result: Vec<SearchResult>,
     ) -> Vec<SearchResult> {
         // Early return if the relevancy score is not set.
         if self.relevancy == -1.0 {
             return result;
         }
 
-        // For Euclidean distance, relevant results are those
-        // smaller than the relevancy score with best distance of 0.0.
-        if self.config.distance == Distance::Euclidean {
-            return result
-                .into_par_iter()
-                .filter(|r| r.distance <= self.relevancy)
-                .collect();
-        }
-
-        // For other distance metrics, like cosine similarity
-        // and dot product, the relevant results are above
-        // the relevancy score.
         result
             .into_par_iter()
-            .filter(|r| r.distance >= self.relevancy)
+            .filter(|r| r.distance <= self.relevancy)
             .collect()
     }
-
-    /// Sorts the search results by distance and distance metric.
-    fn sort_by_distance(&self, result: Vec<SearchResult>) -> Vec<SearchResult> {
-        let mut result = result;
-
-        // Sort the results by distance based on the metric.
-        // For Euclidean distance, sort in ascending order
-        // because the best distance is 0.0.
-        match self.config.distance {
-            Distance::Euclidean => {
-                result.sort_by(|a, b| {
-                    a.distance.partial_cmp(&b.distance).unwrap()
-                });
-            }
-            _ => {
-                result.sort_by(|a, b| {
-                    b.distance.partial_cmp(&a.distance).unwrap()
-                });
-            }
-        };
-
-        result
-    }
 }
 
 /// A record containing a vector and its associated data.
 #[cfg_attr(feature = "py", pyclass(module = "oasysdb.collection", get_all))]
 #[derive(Serialize, Deserialize, Clone, Debug)]
 pub struct Record {
     /// The vector embedding.
@@ -904,15 +868,15 @@
     pub fn many_random(dimension: usize, len: usize) -> Vec<Self> {
         (0..len).map(|_| Self::random(dimension)).collect()
     }
 }
 
 /// The collection nearest neighbor search result.
 #[cfg_attr(feature = "py", pyclass(module = "oasysdb.collection", get_all))]
-#[derive(Serialize, Deserialize, Debug)]
+#[derive(Serialize, Deserialize, Debug, PartialEq)]
 pub struct SearchResult {
     /// Vector ID.
     pub id: u32,
     /// Distance between the query to the collection vector.
     pub distance: f32,
     /// Data associated with the vector.
     pub data: Metadata,
```

### Comparing `oasysdb-0.5.1/src/func/distance.rs` & `oasysdb-0.6.0/src/func/distance.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,45 @@
 use super::*;
 
 /// The distance function used for similarity calculations.
 #[derive(Debug, Serialize, Deserialize, Clone, Copy)]
 #[derive(PartialEq, Eq, Hash, PartialOrd, Ord)]
 pub enum Distance {
-    /// Dot product function.
-    Dot,
     /// Euclidean distance function.
     Euclidean,
-    /// Cosine similarity function.
+    /// Cosine distance function (1 - Cosine similarity).
     Cosine,
-    /// Cosine function for normalized vectors.
-    NormCosine,
 }
 
 impl Distance {
     /// Creates a new distance function from a string.
     /// Available options:
-    /// * `dot`: Dot product function.
     /// * `euclidean`: Euclidean distance function.
     /// * `cosine`: Cosine similarity function.
-    /// * `norm_cosine`: Cosine function for normalized vectors.
     pub fn from(distance: &str) -> Result<Self, Error> {
         match distance {
-            "dot" => Ok(Distance::Dot),
             "euclidean" => Ok(Distance::Euclidean),
             "cosine" => Ok(Distance::Cosine),
-            "norm_cosine" => Ok(Distance::NormCosine),
             _ => Err(Error::invalid_distance()),
         }
     }
 
     /// Calculates the distance between two vectors.
     pub fn calculate(&self, a: &Vector, b: &Vector) -> f32 {
         assert_eq!(a.0.len(), b.0.len());
         match self {
-            Distance::Dot => Distance::dot(a, b),
             Distance::Euclidean => Distance::euclidean(a, b),
             Distance::Cosine => Distance::cosine(a, b),
-            Distance::NormCosine => Distance::dot(a, b),
         }
     }
 
     // List additional distance functions below.
 
-    fn dot(a: &Vector, b: &Vector) -> f32 {
-        f32::dot(&a.0, &b.0).unwrap() as f32
-    }
-
     fn cosine(a: &Vector, b: &Vector) -> f32 {
-        let dot = Self::dot(a, b);
-        let ma = a.0.iter().map(|x| x.powi(2)).sum::<f32>().sqrt();
-        let mb = b.0.iter().map(|y| y.powi(2)).sum::<f32>().sqrt();
-        dot / (ma * mb)
+        f32::cosine(&a.0, &b.0).unwrap() as f32
     }
 
     fn euclidean(a: &Vector, b: &Vector) -> f32 {
         let sq = f32::sqeuclidean(&a.0, &b.0).unwrap() as f32;
         sq.sqrt()
     }
 }
@@ -69,14 +52,12 @@
     }
 }
 
 #[cfg(feature = "py")]
 impl IntoPy<Py<PyAny>> for Distance {
     fn into_py(self, py: Python) -> Py<PyAny> {
         match self {
-            Distance::Dot => "dot".into_py(py),
             Distance::Euclidean => "euclidean".into_py(py),
             Distance::Cosine => "cosine".into_py(py),
-            Distance::NormCosine => "norm_cosine".into_py(py),
         }
     }
 }
```

### Comparing `oasysdb-0.5.1/src/func/err.rs` & `oasysdb-0.6.0/src/func/err.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/src/func/metadata.rs` & `oasysdb-0.6.0/src/func/metadata.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/src/func/mod.rs` & `oasysdb-0.6.0/src/func/mod.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/src/func/utils.rs` & `oasysdb-0.6.0/src/func/utils.rs`

 * *Files 1% similar despite different names*

```diff
@@ -231,17 +231,15 @@
 }
 
 #[derive(Clone)]
 pub struct Search {
     pub ef: usize,
     pub visited: Visited,
     candidates: BinaryHeap<Reverse<Candidate>>,
-    nearest: Vec<Candidate>,
-    working: Vec<Candidate>,
-    discarded: Vec<Candidate>,
+    nearest: Vec<Candidate>, // Ordered ascendingly by distance.
     distance: Distance,
 }
 
 impl Search {
     pub fn new(capacity: usize, distance: Distance) -> Self {
         let visited = Visited::with_capacity(capacity);
         Self { visited, distance, ..Default::default() }
@@ -252,38 +250,31 @@
         &mut self,
         layer: L,
         vector: &Vector,
         vectors: &HashMap<VectorID, Vector>,
         links: usize,
     ) {
         while let Some(Reverse(candidate)) = self.candidates.pop() {
-            // Skip candidates conditionally.
-            // For Euclidean metrics, skip candidate with larger distances
-            // because 0.0 is the smallest and best distance.
-            // For other metrics, the bigger the distance, the better.
-            if let Some(furthest) = self.nearest.last() {
-                if let Distance::Euclidean = self.distance {
-                    if candidate.distance > furthest.distance {
-                        break;
-                    }
-                } else if candidate.distance < furthest.distance {
+            if let Some(last) = self.nearest.last() {
+                if candidate.distance > last.distance {
                     break;
                 }
             }
 
             let layer_iter = layer.nearest_iter(&candidate.vector_id);
             for vector_id in layer_iter.take(links) {
                 self.push(&vector_id, vector, vectors);
             }
 
             self.nearest.truncate(self.ef);
         }
     }
 
-    /// Pushes a new neighbor candidate to the search object.
+    /// Creates and pushes a candidate to the nearest fieled
+    /// and candidates binary heap fields.
     pub fn push(
         &mut self,
         vector_id: &VectorID,
         vector: &Vector,
         vectors: &HashMap<VectorID, Vector>,
     ) {
         if !self.visited.insert(vector_id) {
@@ -321,16 +312,14 @@
     }
 
     /// Resets the search object data.
     pub fn reset(&mut self) {
         self.visited.clear();
         self.candidates.clear();
         self.nearest.clear();
-        self.working.clear();
-        self.discarded.clear();
     }
 
     /// Selects the nearest neighbors.
     pub fn select_simple(&mut self) -> &[Candidate] {
         &self.nearest
     }
 
@@ -341,17 +330,15 @@
 
 impl Default for Search {
     fn default() -> Self {
         Self {
             visited: Visited::with_capacity(0),
             candidates: BinaryHeap::new(),
             nearest: Vec::new(),
-            working: Vec::new(),
-            discarded: Vec::new(),
-            ef: 5,
+            ef: 64,
             distance: Distance::Euclidean,
         }
     }
 }
 
 pub struct SearchPool {
     pool: Mutex<Vec<(Search, Search)>>,
@@ -402,27 +389,25 @@
         let vector = &self.vectors[vector_id];
         let dist = self.config.distance;
 
         let (mut search, mut insertion) = self.search_pool.pop();
         insertion.ef = self.config.ef_construction;
 
         // Find the first valid vector ID to push.
-        let validator = |i: usize| self.vectors.get(&i.into()).is_some();
-        let valid_id = (0..self.vectors.len())
+        let validator = |i: u32| self.vectors.get(&i.into()).is_some();
+        let valid_id = (0..u32::MAX)
             .into_par_iter()
             .find_first(|i| validator(*i))
-            .unwrap();
+            .unwrap_or(0);
 
         search.reset();
         search.push(&valid_id.into(), vector, self.vectors);
 
         for current_layer in self.top_layer.descend() {
-            if current_layer <= *layer {
-                search.ef = self.config.ef_construction;
-            }
+            search.ef = self.config.ef_construction;
 
             // Find the nearest neighbor candidates.
             if current_layer > *layer {
                 let layer = layers[current_layer.0 - 1].as_slice();
                 search.search(layer, vector, self.vectors, M);
                 search.cull();
             } else {
@@ -430,30 +415,30 @@
                 break;
             }
         }
 
         // Select the neighbors.
         let candidates = {
             let candidates = search.select_simple();
-            &candidates[..Ord::min(candidates.len(), M)]
+            &candidates[..Ord::min(M, candidates.len())]
         };
 
         for (i, candidate) in candidates.iter().enumerate() {
             let vid = candidate.vector_id;
-            let old = &self.vectors[&vid];
+            let current = &self.vectors[&vid];
             let distance = candidate.distance;
 
             // Function to sort the vectors by distance.
             let ordering = |id: &VectorID| {
                 if !id.is_valid() {
-                    Ordering::Greater
-                } else {
-                    let other = &self.vectors[id];
-                    distance.cmp(&dist.calculate(old, other).into())
+                    return Ordering::Greater;
                 }
+
+                let other = &self.vectors[id];
+                distance.cmp(&dist.calculate(current, other).into())
             };
 
             // Find the correct index to insert at to keep the order.
             let index = self.base_layer[&vid]
                 .read()
                 .binary_search_by(ordering)
                 .unwrap_or_else(|error| error);
```

### Comparing `oasysdb-0.5.1/src/func/vector.rs` & `oasysdb-0.6.0/src/func/vector.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/src/lib.rs` & `oasysdb-0.6.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/src/tests/mod.rs` & `oasysdb-0.6.0/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/src/tests/test_collection.rs` & `oasysdb-0.6.0/src/tests/test_collection.rs`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     assert_eq!(list.len(), collection.len());
 }
 
 #[test]
 fn config_with_distance() {
     let ef = 10;
     let ml = 1.0;
-    for dist in vec!["cosine", "dot", "euclidean"] {
+    for dist in vec!["cosine", "euclidean"] {
         Config::new(ef, ef, ml, dist).unwrap();
     }
 }
 
 #[test]
 #[should_panic(expected = "Distance function not supported.")]
 fn config_with_distance_panic() {
```

### Comparing `oasysdb-0.5.1/src/tests/test_database.rs` & `oasysdb-0.6.0/src/tests/test_database.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/src/tests/test_metadata.rs` & `oasysdb-0.6.0/src/tests/test_metadata.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/src/tests/test_vectorgen.rs` & `oasysdb-0.6.0/src/tests/test_vectorgen.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/src/vectorgen/mod.rs` & `oasysdb-0.6.0/src/vectorgen/mod.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/src/vectorgen/openai.rs` & `oasysdb-0.6.0/src/vectorgen/openai.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/pyproject.toml` & `oasysdb-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oasysdb-0.5.1/PKG-INFO` & `oasysdb-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: oasysdb
-Version: 0.5.1
+Version: 0.6.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Database
 Classifier: Topic :: Text Processing :: Indexing
 Summary: Fast embedded vector database with incremental HNSW indexing.
 Keywords: embedded,vector,database,hnsw,ann
```

