# Comparing `tmp/performica_prs-1.2.5.tar.gz` & `tmp/performica_prs-1.3.0.tar.gz`

## Comparing `performica_prs-1.2.5.tar` & `performica_prs-1.3.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      302 1970-01-01 00:00:00.000000 performica_prs-1.2.5/Cargo.toml
--rw-r--r--   0      501       20      840 2024-05-31 08:14:15.000000 performica_prs-1.2.5/src/boundaries.rs
--rw-r--r--   0      501       20      612 2024-05-31 08:14:15.000000 performica_prs-1.2.5/src/delta.rs
--rw-r--r--   0      501       20     3975 2024-05-31 08:14:15.000000 performica_prs-1.2.5/src/lib.rs
--rw-r--r--   0      501       20      548 2024-05-31 08:14:15.000000 performica_prs-1.2.5/src/minmax.rs
--rw-r--r--   0      501       20    13032 2024-05-31 08:14:15.000000 performica_prs-1.2.5/src/peerrank.rs
--rw-r--r--   0      501       20     1136 2024-05-31 08:14:15.000000 performica_prs-1.2.5/src/prs.rs
--rw-r--r--   0      501       20     1073 2024-05-31 08:14:15.000000 performica_prs-1.2.5/src/review.rs
--rw-r--r--   0      501       20     2235 2024-05-31 08:14:15.000000 performica_prs-1.2.5/src/row.rs
--rw-r--r--   0      501       20     1339 2024-05-31 08:14:15.000000 performica_prs-1.2.5/src/trend.rs
--rw-r--r--   0      501       20    15551 2024-05-31 08:14:15.000000 performica_prs-1.2.5/Cargo.lock
--rw-r--r--   0      501       20      131 2024-05-31 08:14:15.000000 performica_prs-1.2.5/pyproject.toml
--rw-r--r--   0        0        0       81 1970-01-01 00:00:00.000000 performica_prs-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0      292 1970-01-01 00:00:00.000000 performica_prs-1.3.0/Cargo.toml
+-rw-r--r--   0      501       20      840 2024-05-31 12:51:40.000000 performica_prs-1.3.0/src/boundaries.rs
+-rw-r--r--   0      501       20      734 2024-05-31 12:51:40.000000 performica_prs-1.3.0/src/delta.rs
+-rw-r--r--   0      501       20     3826 2024-05-31 12:51:40.000000 performica_prs-1.3.0/src/lib.rs
+-rw-r--r--   0      501       20      548 2024-05-31 12:51:40.000000 performica_prs-1.3.0/src/minmax.rs
+-rw-r--r--   0      501       20    13041 2024-05-31 12:51:40.000000 performica_prs-1.3.0/src/peerrank.rs
+-rw-r--r--   0      501       20     1287 2024-05-31 12:51:40.000000 performica_prs-1.3.0/src/prs.rs
+-rw-r--r--   0      501       20      666 2024-05-31 12:51:40.000000 performica_prs-1.3.0/src/py_bind.rs
+-rw-r--r--   0      501       20     1419 2024-05-31 12:51:40.000000 performica_prs-1.3.0/src/review.rs
+-rw-r--r--   0      501       20     2480 2024-05-31 12:51:40.000000 performica_prs-1.3.0/src/row.rs
+-rw-r--r--   0      501       20     1339 2024-05-31 12:51:40.000000 performica_prs-1.3.0/src/trend.rs
+-rw-r--r--   0      501       20    12670 2024-05-31 12:51:40.000000 performica_prs-1.3.0/Cargo.lock
+-rw-r--r--   0      501       20      151 2024-05-31 12:51:40.000000 performica_prs-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       82 1970-01-01 00:00:00.000000 performica_prs-1.3.0/PKG-INFO
```

### Comparing `performica_prs-1.2.5/src/boundaries.rs` & `performica_prs-1.3.0/src/boundaries.rs`

 * *Files identical despite different names*

### Comparing `performica_prs-1.2.5/src/lib.rs` & `performica_prs-1.3.0/src/lib.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,105 +1,101 @@
-use pyo3::exceptions;
-use pyo3_chrono::NaiveDate as PyNaiveDate;
 use std::collections::HashMap;
 
 use pyo3::prelude::*;
-use pyo3::types::{PyDict, PyList};
+use pyo3::types::{PyDate, PyDict, PyList};
+use pyo3::wrap_pyfunction;
 
 use crate::boundaries::PeerRankScoreBoundaries;
 use crate::peerrank::PeerRankCalculator;
 use crate::prs::PeerRankScoreData;
+use crate::py_bind::DateWrap;
 use crate::review::Review;
 use crate::row::ExplodedRow;
 use crate::trend::_get_trend_type_values;
 
 pub mod boundaries;
 pub mod delta;
 pub mod minmax;
 pub mod peerrank;
 pub mod prs;
+mod py_bind;
 pub mod review;
 pub mod row;
 pub mod trend;
 
 #[pyclass]
 struct PeerRank {
     calculator: PeerRankCalculator,
 }
 
-fn get_float(kwargs: &PyDict, key: &str) -> f64 {
-    kwargs
-        .get_item(key)
-        .and_then(|o| o.extract::<f64>().ok())
-        .unwrap_or(0.)
+fn get_float(o_kwargs: Option<&Bound<'_, PyDict>>, key: &str) -> PyResult<f64> {
+    o_kwargs
+        .and_then(|kwargs| kwargs.get_item(key).ok().flatten())
+        .map::<Result<f64, _>, _>(|v| v.extract::<f64>())
+        .unwrap_or(Ok(0.))
 }
 
 #[pymethods]
 impl PeerRank {
     #[new]
-    #[args(kwargs = "**")]
-    #[allow(clippy::too_many_arguments)]
-    fn new(kwargs: Option<&PyDict>) -> PyResult<PeerRank> {
-        if let Some(kwargs) = kwargs {
-            let min_skill: f64 = get_float(kwargs, "min_skill");
-            let max_skill: f64 = get_float(kwargs, "max_skill");
-            let min_teamwork: f64 = get_float(kwargs, "min_teamwork");
-            let max_teamwork: f64 = get_float(kwargs, "max_teamwork");
-            let min_aggregate: f64 = get_float(kwargs, "min_aggregate");
-            let max_aggregate: f64 = get_float(kwargs, "max_aggregate");
-            let prs_by_employee_id: &PyDict = kwargs
-                .get_item("prs_by_employee_id")
-                .and_then(|o| o.downcast::<PyDict>().ok())
-                .unwrap();
-            Ok(PeerRank {
-                calculator: create_calculator(
-                    prs_by_employee_id,
-                    min_skill,
-                    max_skill,
-                    min_teamwork,
-                    max_teamwork,
-                    min_aggregate,
-                    max_aggregate,
-                ),
-            })
-        } else {
-            Err(PyErr::new::<exceptions::PyTypeError, _>(
-                "Invalid arguments",
-            ))
-        }
+    #[pyo3(signature = (prs_by_employee_id, **kwargs))]
+    fn py_new(
+        prs_by_employee_id: &Bound<'_, PyDict>,
+        kwargs: Option<&Bound<'_, PyDict>>,
+    ) -> PyResult<PeerRank> {
+        let min_skill: f64 = get_float(kwargs, "min_skill")?;
+        let max_skill: f64 = get_float(kwargs, "max_skill")?;
+        let min_teamwork: f64 = get_float(kwargs, "min_teamwork")?;
+        let max_teamwork: f64 = get_float(kwargs, "max_teamwork")?;
+        let min_aggregate: f64 = get_float(kwargs, "min_aggregate")?;
+        let max_aggregate: f64 = get_float(kwargs, "max_aggregate")?;
+
+        Ok(PeerRank {
+            calculator: create_calculator(
+                prs_by_employee_id,
+                min_skill,
+                max_skill,
+                min_teamwork,
+                max_teamwork,
+                min_aggregate,
+                max_aggregate,
+            ),
+        })
     }
 
     fn process_date(
         &mut self,
-        reviews_list: &PyList,
-        date: PyNaiveDate,
+        reviews_list: &Bound<'_, PyList>,
+        date: &Bound<'_, PyDate>,
     ) -> PyResult<(Vec<PeerRankScoreData>, Vec<ExplodedRow>)> {
         let reviews: Vec<Review> = reviews_list.iter().map(|i| i.extract().unwrap()).collect();
-        let exploded_rows_for_date = self.calculator.explode_date(&reviews, date);
+        let exploded_rows_for_date = self
+            .calculator
+            .explode_date(&reviews, &DateWrap::from_python(date));
         let prs = self.calculator.process_date(&exploded_rows_for_date);
         Ok((prs, exploded_rows_for_date))
     }
 
     fn get_prs(&mut self, employee_id: u32) -> PyResult<PeerRankScoreData> {
         Ok(self.calculator.get_prs(employee_id).clone())
     }
 }
 
 fn create_calculator(
-    prs_by_employee_id: &PyDict,
+    prs_by_employee_id: &Bound<'_, PyDict>,
     min_skill: f64,
     max_skill: f64,
     min_teamwork: f64,
     max_teamwork: f64,
     min_aggregate: f64,
     max_aggregate: f64,
 ) -> PeerRankCalculator {
     let mut _prs_by_employee_id = HashMap::new();
     for (k, v) in prs_by_employee_id.iter() {
-        let employee_id = FromPyObject::extract(k).unwrap();
+        let employee_id = FromPyObject::extract_bound(&k).unwrap();
         let prs = v.extract().unwrap();
         _prs_by_employee_id.insert(employee_id, prs);
     }
     PeerRankCalculator {
         prs_by_employee_id: _prs_by_employee_id,
         prs_boundaries: PeerRankScoreBoundaries::new(
             min_skill,
@@ -109,22 +105,22 @@
             min_aggregate,
             max_aggregate,
         ),
     }
 }
 
 #[pyfunction]
-fn get_trend_type_values(prs_values: &PyList, threshold: f64) -> Vec<i32> {
+fn get_trend_type_values(prs_values: &Bound<'_, PyList>, threshold: f64) -> Vec<i32> {
     let vec: Vec<f64> = prs_values.iter().map(|i| i.extract().unwrap()).collect();
     _get_trend_type_values(&vec, threshold)
 }
 
 /// This module implements the Peer Rank algorithm in Rust
 #[pymodule]
-fn prscalc(_py: Python, m: &PyModule) -> PyResult<()> {
+fn prscalc(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<PeerRank>()?;
     m.add_class::<PeerRankScoreData>()?;
     m.add_class::<Review>()?;
     m.add_class::<ExplodedRow>()?;
     m.add_function(wrap_pyfunction!(get_trend_type_values, m)?)?;
     Ok(())
 }
```

### Comparing `performica_prs-1.2.5/src/minmax.rs` & `performica_prs-1.3.0/src/minmax.rs`

 * *Files identical despite different names*

### Comparing `performica_prs-1.2.5/src/peerrank.rs` & `performica_prs-1.3.0/src/peerrank.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 use std::collections::HashMap;
 
 use itertools::Itertools;
 
 use crate::boundaries::PeerRankScoreBoundaries;
 use crate::delta::PeerRankScoreDeltaData;
 use crate::prs::PeerRankScoreData;
+use crate::py_bind::DateWrap;
 use crate::review::Review;
 use crate::row::ExplodedRow;
-use pyo3_chrono::NaiveDate as PyNaiveDate;
 
 static TOO_CLOSE: f64 = 5.;
 
 fn get_reviewer_weight(min_prs: f64, prs_range: f64, reviewer_prs: f64) -> f64 {
     if prs_range < f64::EPSILON {
         // give middle-of-the road weight to first reviews in type
         return 2.5;
@@ -105,16 +105,16 @@
                 .insert(prs.to_member_id, prs.clone());
         }
     }
 
     fn explode_group(
         &mut self,
         reviews: &[Review],
-        date: PyNaiveDate,
-        cycle: PyNaiveDate,
+        date: &DateWrap,
+        cycle: &DateWrap,
         content_type_id: u32,
         from_member_id: u32,
     ) -> Vec<ExplodedRow> {
         let mut result: Vec<ExplodedRow> = Vec::new();
         if reviews.len() < 2 {
             return result;
         }
@@ -217,16 +217,16 @@
                 * aggregate_reviewer_weight
                 * aggregate_spread_weight
                 * aggregate_expectation_weight;
 
             result.push(ExplodedRow {
                 content_type_id,
                 from_member_id,
-                date,
-                cycle,
+                _date: *date,
+                _cycle: *cycle,
                 id_1: review1.id,
                 id_2: review2.id,
                 to_member_id_1: review1.to_member_id,
                 to_member_id_2: review2.to_member_id,
                 skill_reviewer_weight,
                 skill_spread_weight,
                 skill_expectation_weight,
@@ -240,45 +240,45 @@
                 aggregate_expectation_weight,
                 aggregate_increment,
             })
         }
         result
     }
 
-    pub fn explode_date(&mut self, reviews: &[Review], date: PyNaiveDate) -> Vec<ExplodedRow> {
+    pub fn explode_date(&mut self, reviews: &[Review], date: &DateWrap) -> Vec<ExplodedRow> {
         let mut result: Vec<ExplodedRow> = Vec::new();
         if reviews.len() < 2 {
             return result;
         }
         let mut index = 0;
-        let mut cycle = reviews[0].cycle;
+        let mut cycle = reviews[0]._cycle;
         let mut content_type_id = reviews[0].content_type_id;
         let mut from_member_id = reviews[0].from_member_id;
         for (i, review) in reviews.iter().enumerate() {
-            if cycle != review.cycle
+            if cycle != review._cycle
                 || content_type_id != review.content_type_id
                 || from_member_id != review.from_member_id
             {
                 result.extend(self.explode_group(
                     &reviews[index..i],
                     date,
-                    cycle,
+                    &cycle,
                     content_type_id,
                     from_member_id,
                 ));
                 index = i;
-                cycle = review.cycle;
+                cycle = review._cycle;
                 content_type_id = review.content_type_id;
                 from_member_id = review.from_member_id;
             }
         }
         result.extend(self.explode_group(
             &reviews[index..],
             date,
-            cycle,
+            &cycle,
             content_type_id,
             from_member_id,
         ));
         result
     }
 
     pub fn process_date(
@@ -299,15 +299,15 @@
                 .entry(k)
                 .and_modify(|delta| {
                     delta.skill += row.skill_increment;
                     delta.teamwork += row.teamwork_increment;
                     delta.aggregate += row.aggregate_increment;
                 })
                 .or_insert_with(|| PeerRankScoreDeltaData {
-                    date: row.date,
+                    _date: row._date,
                     survey_request_id: row.id_1,
                     to_member_id: row.to_member_id_1,
                     teamwork: row.teamwork_increment,
                     skill: row.skill_increment,
                     aggregate: row.aggregate_increment,
                 });
 
@@ -316,15 +316,15 @@
                 .entry(k)
                 .and_modify(|delta| {
                     delta.skill -= row.skill_increment;
                     delta.teamwork -= row.teamwork_increment;
                     delta.aggregate -= row.aggregate_increment;
                 })
                 .or_insert_with(|| PeerRankScoreDeltaData {
-                    date: row.date,
+                    _date: row._date,
                     survey_request_id: row.id_2,
                     to_member_id: row.to_member_id_2,
                     teamwork: -row.teamwork_increment,
                     skill: -row.skill_increment,
                     aggregate: -row.aggregate_increment,
                 });
         }
@@ -349,15 +349,15 @@
                 .or_insert_with(|| {
                     let previous_prs = self.get_prs(delta.to_member_id);
                     PeerRankScoreData {
                         skill: previous_prs.skill + delta.skill,
                         teamwork: previous_prs.teamwork + delta.teamwork,
                         aggregate: previous_prs.aggregate + delta.aggregate,
                         to_member_id: delta.to_member_id,
-                        date: delta.date,
+                        _date: delta._date,
                         deltas: vec![delta.clone()],
                     }
                 });
         }
         new_prs.values().map(|d| d.to_owned()).collect()
     }
 }
```

### Comparing `performica_prs-1.2.5/src/row.rs` & `performica_prs-1.3.0/src/row.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,20 @@
+use crate::py_bind::DateWrap;
 use pyo3::prelude::*;
-use pyo3::types::PyList;
-use pyo3_chrono::NaiveDate as PyNaiveDate;
+use pyo3::types::{PyDate, PyList};
 
 #[pyclass]
 #[derive(Debug, Clone)]
 pub struct ExplodedRow {
     #[pyo3(get)]
     pub content_type_id: u32,
     #[pyo3(get)]
     pub from_member_id: u32,
-    #[pyo3(get)]
-    pub date: PyNaiveDate,
-    #[pyo3(get)]
-    pub cycle: PyNaiveDate,
+    pub _date: DateWrap,
+    pub _cycle: DateWrap,
     #[pyo3(get)]
     pub id_1: u32,
     #[pyo3(get)]
     pub id_2: u32,
     #[pyo3(get)]
     pub to_member_id_1: u32,
     #[pyo3(get)]
@@ -45,18 +43,28 @@
     pub aggregate_expectation_weight: f64,
     #[pyo3(get)]
     pub aggregate_increment: f64,
 }
 
 #[pymethods]
 impl ExplodedRow {
-    pub fn to_list<'p>(&self, py: Python<'p>) -> PyResult<&'p PyList> {
-        let result = PyList::new(py, vec![self.content_type_id, self.from_member_id]);
-        result.append(self.date)?;
-        result.append(self.cycle)?;
+    #[getter]
+    fn date<'py>(&self, py: Python<'py>) -> PyResult<Bound<'py, PyDate>> {
+        self._date.to_python(py)
+    }
+
+    #[getter]
+    fn cycle<'py>(&self, py: Python<'py>) -> PyResult<Bound<'py, PyDate>> {
+        self._cycle.to_python(py)
+    }
+
+    pub fn to_list<'py>(&self, py: Python<'py>) -> PyResult<Bound<'py, PyList>> {
+        let result = PyList::new_bound(py, vec![self.content_type_id, self.from_member_id]);
+        result.append(self.date(py)?)?;
+        result.append(self.cycle(py)?)?;
         result.append(self.id_1)?;
         result.append(self.id_2)?;
         result.append(self.to_member_id_1)?;
         result.append(self.to_member_id_2)?;
         result.append(self.skill_reviewer_weight)?;
         result.append(self.skill_spread_weight)?;
         result.append(self.skill_expectation_weight)?;
```

### Comparing `performica_prs-1.2.5/src/trend.rs` & `performica_prs-1.3.0/src/trend.rs`

 * *Files identical despite different names*

### Comparing `performica_prs-1.2.5/Cargo.lock` & `performica_prs-1.3.0/Cargo.lock`

 * *Files 14% similar despite different names*

```diff
@@ -15,35 +15,35 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
-version = "1.3.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bumpalo"
-version = "3.12.0"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d261e256854913907f67ed06efbc3338dfe6179796deefc1ff763fc1aee5535"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "cc"
-version = "1.0.79"
+version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
+checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -58,474 +58,358 @@
  "js-sys",
  "num-traits",
  "wasm-bindgen",
  "windows-targets",
 ]
 
 [[package]]
-name = "codespan-reporting"
-version = "0.11.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3538270d33cc669650c4b093848450d380def10c331d38c768e34cac80576e6e"
-dependencies = [
- "termcolor",
- "unicode-width",
-]
-
-[[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
-
-[[package]]
-name = "cxx"
-version = "1.0.92"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a140f260e6f3f79013b8bfc65e7ce630c9ab4388c6a89c71e07226f49487b72"
-dependencies = [
- "cc",
- "cxxbridge-flags",
- "cxxbridge-macro",
- "link-cplusplus",
-]
-
-[[package]]
-name = "cxx-build"
-version = "1.0.92"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da6383f459341ea689374bf0a42979739dc421874f112ff26f829b8040b8e613"
-dependencies = [
- "cc",
- "codespan-reporting",
- "once_cell",
- "proc-macro2",
- "quote",
- "scratch",
- "syn",
-]
-
-[[package]]
-name = "cxxbridge-flags"
-version = "1.0.92"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90201c1a650e95ccff1c8c0bb5a343213bdd317c6e600a93075bca2eff54ec97"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
-name = "cxxbridge-macro"
-version = "1.0.92"
+name = "either"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b75aed41bb2e6367cae39e6326ef817a851db13c13e4f3263714ca3cfb8de56"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
-]
+checksum = "3dca9240753cf90908d7e4aac30f630662b02aebaa1b58a3cadabdb23385b58b"
 
 [[package]]
-name = "either"
-version = "1.6.1"
+name = "heck"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e78d4f1cc4ae33bbfc157ed5d5a5ef3bc29227303d595861deb238fcec4e9457"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.53"
+version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64c122667b287044802d6ce17ee2ddf13207ed924c712de9a66a5814d5b64765"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "winapi",
+ "windows-core",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "cxx",
- "cxx-build",
+ "cc",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.9"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
-
-[[package]]
-name = "instant"
-version = "0.1.12"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
-dependencies = [
- "cfg-if",
-]
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "itertools"
-version = "0.10.3"
+version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9a9d19fa1e79b6215ff29b9d6880b706147f16e9b1dbb1e4e5947b5b02bc5e3"
+checksum = "413ee7dfc52ee1a4949ceeb7dbc8a33f2d6c088194d9f922fb8318faf1f01186"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.61"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.141"
+version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3304a64d199bb964be99741b7a14d26972741915b3649639149b2479bb46f4b5"
-
-[[package]]
-name = "link-cplusplus"
-version = "1.0.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
-dependencies = [
- "cc",
-]
+checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "07af8b9cdd281b7915f413fa73f29ebd5d55d0d3f0155584dade1ff18cea1b17"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.15"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.12.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7709cef83f0c1f58f666e746a08b21e0085f7440fa6a29cc194d68aac97a4225"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.11.2"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
- "instant",
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.8.5"
+version = "0.9.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d76e8e1493bcac0d2766c42737f34458f1c8c50c0d23bcb24ea953affb273216"
+checksum = "1e401f977ab385c9e4e3ab30627d6f26d00e2c73eef317493c4ec6d468726cf8"
 dependencies = [
  "cfg-if",
- "instant",
  "libc",
  "redox_syscall",
  "smallvec",
- "winapi",
+ "windows-targets",
 ]
 
 [[package]]
 name = "performica-prs"
-version = "1.2.5"
+version = "1.3.0"
 dependencies = [
  "chrono",
  "itertools",
  "pyo3",
- "pyo3-chrono",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
+checksum = "a5e00b96a521718e08e03b1a622f01c8a8deb50719335de3f60b3b3950f069d8"
 dependencies = [
  "cfg-if",
+ "chrono",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
+checksum = "7883df5835fafdad87c0d888b266c8ec0f4c9ca48a5bed6bbb592e8dedee1b50"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
-name = "pyo3-chrono"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cc7b65b726673ac8acc9eadbc6f94295310c8cde2d0ee56f92ff5ad69707333"
-dependencies = [
- "chrono",
- "pyo3",
-]
-
-[[package]]
 name = "pyo3-ffi"
-version = "0.17.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
+checksum = "01be5843dc60b916ab4dad1dca6d20b9b4e6ddc8e15f50c47fe6d85f1fb97403"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
+checksum = "77b34069fc0682e11b31dbd10321cbf94808394c56fd996796ce45217dfac53c"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.3"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
+checksum = "08260721f32db5e1a5beae69a55553f56b99bd0e1c3e6e0a5e8851a9d0f5a85c"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.20"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3bcdf212e9776fbcb2d23ab029360416bb1706b1aea2d1a5ba002727cbcab804"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "scopeguard"
-version = "1.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
-
-[[package]]
-name = "scratch"
-version = "1.0.5"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1792db035ce95be60c3f8853017b3999209281c24e2ba5bc8e59bf97a0c590c1"
+checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "smallvec"
-version = "1.8.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc88c725d61fc6c3132893370cac4a0200e3fedf5da8331c570664b1987f5ca2"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "1.0.98"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c50aef8a904de4c23c788f104b7dddc7d6f79c647c7c8ce4cc8f73eb0ca773dd"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
-name = "termcolor"
-version = "1.2.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
-dependencies = [
- "winapi-util",
-]
-
-[[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
-
-[[package]]
-name = "unicode-width"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
+checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unindent"
-version = "0.1.9"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "52fee519a3e570f7df377a06a1a7775cdbfb7aa460be7e08de2b1f0e69973a44"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.84"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.84"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.84"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.84"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.84"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
-
-[[package]]
-name = "winapi"
-version = "0.3.9"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
-dependencies = [
- "winapi-i686-pc-windows-gnu",
- "winapi-x86_64-pc-windows-gnu",
-]
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
-name = "winapi-i686-pc-windows-gnu"
-version = "0.4.0"
+name = "windows-core"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
-
-[[package]]
-name = "winapi-util"
-version = "0.1.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70ec6ce85bb158151cae5e5c87f95a8e97d2c0c4b001223f33a334e3ce5de178"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "winapi",
+ "windows-targets",
 ]
 
 [[package]]
-name = "winapi-x86_64-pc-windows-gnu"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
-
-[[package]]
 name = "windows-targets"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
```

