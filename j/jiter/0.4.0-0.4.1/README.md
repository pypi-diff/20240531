# Comparing `tmp/jiter-0.4.0.tar.gz` & `tmp/jiter-0.4.1.tar.gz`

## Comparing `jiter-0.4.0.tar` & `jiter-0.4.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0     1001      127     1956 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/Cargo.toml
--rw-r--r--   0     1001      127     1091 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/LICENSE
--rw-r--r--   0     1001      127     6856 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/README.md
--rw-r--r--   0     1001      127    17519 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/bigints_array.json
--rw-r--r--   0     1001      127    19356 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/floats_array.json
--rwxr-xr-x   0     1001      127      530 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/generate_big.py
--rw-r--r--   0     1001      127    11882 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/main.rs
--rw-r--r--   0     1001      127    62332 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/massive_ints_array.json
--rw-r--r--   0     1001      127     2329 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/medium_response.json
--rw-r--r--   0     1001      127     1441 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/pass1.json
--rw-r--r--   0     1001      127       52 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/pass2.json
--rw-r--r--   0     1001      127     3726 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/python.rs
--rw-r--r--   0     1001      127      374 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/sentence.json
--rw-r--r--   0     1001      127     4801 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/short_numbers.json
--rw-r--r--   0     1001      127      700 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/string_array.json
--rw-r--r--   0     1001      127    90000 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/string_array_unique.json
--rw-r--r--   0     1001      127      600 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/true_array.json
--rw-r--r--   0     1001      127     1390 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/true_object.json
--rw-r--r--   0     1001      127      381 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/unicode.json
--rw-r--r--   0     1001      127      103 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/benches/x100.json
--rw-r--r--   0     1001      127       85 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/build.rs
--rw-r--r--   0     1001      127     9344 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/src/errors.rs
--rw-r--r--   0     1001      127    14540 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/src/jiter.rs
--rw-r--r--   0     1001      127     4756 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/src/lazy_index_map.rs
--rw-r--r--   0     1001      127      927 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/src/lib.rs
--rw-r--r--   0     1001      127    18219 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/src/number_decoder.rs
--rw-r--r--   0     1001      127     8845 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/src/parse.rs
--rw-r--r--   0     1001      127     1924 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/src/py_lossless_float.rs
--rw-r--r--   0     1001      127     7476 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/src/py_string_cache.rs
--rw-r--r--   0     1001      127    13185 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/src/python.rs
--rw-r--r--   0     1001      127     9760 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/src/simd_aarch64.rs
--rw-r--r--   0     1001      127    14539 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/src/string_decoder.rs
--rw-r--r--   0     1001      127    10261 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/src/value.rs
--rw-r--r--   0     1001      127    56025 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/tests/main.rs
--rw-r--r--   0     1001      127     2673 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter/tests/python.rs
--rw-r--r--   0     1001      127     6928 2024-05-22 19:38:29.000000 jiter-0.4.0/README.md
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 jiter-0.4.0/crates/jiter-python/Cargo.toml
--rw-r--r--   0     1001      127     2308 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter-python/README.md
--rw-r--r--   0     1001      127     2653 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter-python/bench.py
--rw-r--r--   0     1001      127     2329 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter-python/jiter.pyi
--rw-r--r--   0     1001      127       21 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter-python/requirements.txt
--rw-r--r--   0     1001      127     2175 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter-python/src/lib.rs
--rw-r--r--   0     1001      127       34 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter-python/tests/requirements.txt
--rw-r--r--   0     1001      127     7372 2024-05-22 19:38:29.000000 jiter-0.4.0/crates/jiter-python/tests/test_jiter.py
--rw-r--r--   0     1001      127    17759 2024-05-22 19:38:36.000000 jiter-0.4.0/Cargo.lock
--rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 jiter-0.4.0/Cargo.toml
--rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 jiter-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3625 1970-01-01 00:00:00.000000 jiter-0.4.0/PKG-INFO
+-rw-r--r--   0     1001      127     1973 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/Cargo.toml
+-rw-r--r--   0     1001      127     1091 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/LICENSE
+-rw-r--r--   0     1001      127     6856 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/README.md
+-rw-r--r--   0     1001      127    17519 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/bigints_array.json
+-rw-r--r--   0     1001      127    19356 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/floats_array.json
+-rwxr-xr-x   0     1001      127      530 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/generate_big.py
+-rw-r--r--   0     1001      127    11882 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/main.rs
+-rw-r--r--   0     1001      127    62332 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/massive_ints_array.json
+-rw-r--r--   0     1001      127     2329 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/medium_response.json
+-rw-r--r--   0     1001      127     1441 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/pass1.json
+-rw-r--r--   0     1001      127       52 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/pass2.json
+-rw-r--r--   0     1001      127     3726 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/python.rs
+-rw-r--r--   0     1001      127      374 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/sentence.json
+-rw-r--r--   0     1001      127     4801 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/short_numbers.json
+-rw-r--r--   0     1001      127      700 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/string_array.json
+-rw-r--r--   0     1001      127    90000 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/string_array_unique.json
+-rw-r--r--   0     1001      127      600 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/true_array.json
+-rw-r--r--   0     1001      127     1390 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/true_object.json
+-rw-r--r--   0     1001      127      381 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/unicode.json
+-rw-r--r--   0     1001      127      103 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/benches/x100.json
+-rw-r--r--   0     1001      127       85 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/build.rs
+-rw-r--r--   0     1001      127     9344 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/src/errors.rs
+-rw-r--r--   0     1001      127    14540 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/src/jiter.rs
+-rw-r--r--   0     1001      127     4756 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/src/lazy_index_map.rs
+-rw-r--r--   0     1001      127      927 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/src/lib.rs
+-rw-r--r--   0     1001      127    18219 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/src/number_decoder.rs
+-rw-r--r--   0     1001      127     8845 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/src/parse.rs
+-rw-r--r--   0     1001      127     1924 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/src/py_lossless_float.rs
+-rw-r--r--   0     1001      127     7476 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/src/py_string_cache.rs
+-rw-r--r--   0     1001      127    13185 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/src/python.rs
+-rw-r--r--   0     1001      127     9760 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/src/simd_aarch64.rs
+-rw-r--r--   0     1001      127    14579 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/src/string_decoder.rs
+-rw-r--r--   0     1001      127    12615 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/src/value.rs
+-rw-r--r--   0     1001      127    57576 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/tests/main.rs
+-rw-r--r--   0     1001      127     2673 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter/tests/python.rs
+-rw-r--r--   0     1001      127     6928 2024-05-31 16:19:31.000000 jiter-0.4.1/README.md
+-rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 jiter-0.4.1/crates/jiter-python/Cargo.toml
+-rw-r--r--   0     1001      127     2308 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter-python/README.md
+-rw-r--r--   0     1001      127     2653 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter-python/bench.py
+-rw-r--r--   0     1001      127     2329 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter-python/jiter.pyi
+-rw-r--r--   0     1001      127       21 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter-python/requirements.txt
+-rw-r--r--   0     1001      127     2175 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter-python/src/lib.rs
+-rw-r--r--   0     1001      127       34 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter-python/tests/requirements.txt
+-rw-r--r--   0     1001      127     7841 2024-05-31 16:19:31.000000 jiter-0.4.1/crates/jiter-python/tests/test_jiter.py
+-rw-r--r--   0     1001      127    18796 2024-05-31 16:19:42.000000 jiter-0.4.1/Cargo.lock
+-rw-r--r--   0        0        0      599 1970-01-01 00:00:00.000000 jiter-0.4.1/Cargo.toml
+-rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 jiter-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3625 1970-01-01 00:00:00.000000 jiter-0.4.1/PKG-INFO
```

### Comparing `jiter-0.4.0/crates/jiter/Cargo.toml` & `jiter-0.4.1/crates/jiter/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 [dependencies]
 num-bigint = "0.4.4"
 num-traits = "0.2.16"
 ahash = "0.8.0"
 smallvec = "1.11.0"
 pyo3 = { version = "0.21.0", optional = true }
 lexical-parse-float = { version = "0.8.5", features =  ["format"] }
+bitvec = "1.0.1"
 
 [features]
 python = ["dep:pyo3", "dep:pyo3-build-config"]
 
 [dev-dependencies]
 bencher = "0.1.5"
 paste = "1.0.7"
```

### Comparing `jiter-0.4.0/crates/jiter/LICENSE` & `jiter-0.4.1/crates/jiter/LICENSE`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/README.md` & `jiter-0.4.1/crates/jiter/README.md`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/benches/bigints_array.json` & `jiter-0.4.1/crates/jiter/benches/bigints_array.json`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/benches/floats_array.json` & `jiter-0.4.1/crates/jiter/benches/floats_array.json`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/benches/generate_big.py` & `jiter-0.4.1/crates/jiter/benches/generate_big.py`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/benches/main.rs` & `jiter-0.4.1/crates/jiter/benches/main.rs`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/benches/massive_ints_array.json` & `jiter-0.4.1/crates/jiter/benches/massive_ints_array.json`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/benches/medium_response.json` & `jiter-0.4.1/crates/jiter/benches/medium_response.json`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/benches/pass1.json` & `jiter-0.4.1/crates/jiter/benches/pass1.json`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/benches/python.rs` & `jiter-0.4.1/crates/jiter/benches/python.rs`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/benches/short_numbers.json` & `jiter-0.4.1/crates/jiter/benches/short_numbers.json`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/benches/string_array_unique.json` & `jiter-0.4.1/crates/jiter/benches/string_array_unique.json`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/benches/true_object.json` & `jiter-0.4.1/crates/jiter/benches/true_object.json`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/src/errors.rs` & `jiter-0.4.1/crates/jiter/src/errors.rs`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/src/jiter.rs` & `jiter-0.4.1/crates/jiter/src/jiter.rs`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/src/lazy_index_map.rs` & `jiter-0.4.1/crates/jiter/src/lazy_index_map.rs`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/src/lib.rs` & `jiter-0.4.1/crates/jiter/src/lib.rs`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/src/number_decoder.rs` & `jiter-0.4.1/crates/jiter/src/number_decoder.rs`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/src/parse.rs` & `jiter-0.4.1/crates/jiter/src/parse.rs`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/src/py_lossless_float.rs` & `jiter-0.4.1/crates/jiter/src/py_lossless_float.rs`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/src/py_string_cache.rs` & `jiter-0.4.1/crates/jiter/src/py_string_cache.rs`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/src/python.rs` & `jiter-0.4.1/crates/jiter/src/python.rs`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/src/simd_aarch64.rs` & `jiter-0.4.1/crates/jiter/src/simd_aarch64.rs`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter/src/string_decoder.rs` & `jiter-0.4.1/crates/jiter/src/string_decoder.rs`

 * *Files 0% similar despite different names*

```diff
@@ -114,14 +114,15 @@
                 b'b' => tape.push(b'\x08'),
                 b'f' => tape.push(b'\x0C'),
                 b'n' => tape.push(b'\n'),
                 b'r' => tape.push(b'\r'),
                 b't' => tape.push(b'\t'),
                 b'u' => {
                     let (c, new_index) = parse_escape(data, index)?;
+                    ascii_only = false;
                     index = new_index;
                     tape.extend_from_slice(c.encode_utf8(&mut [0_u8; 4]).as_bytes());
                 }
                 _ => return json_err!(InvalidEscape, index),
             }
             index += 1;
         } else {
```

### Comparing `jiter-0.4.0/crates/jiter/src/value.rs` & `jiter-0.4.1/crates/jiter/src/value.rs`

 * *Files 24% similar despite different names*

```diff
@@ -230,59 +230,132 @@
 
 /// like `take_value`, but nothing is returned, should be faster than `take_value`, useful when you don't care
 /// about the value, but just want to consume it
 pub(crate) fn take_value_skip(
     peek: Peek,
     parser: &mut Parser,
     tape: &mut Tape,
-    mut recursion_limit: u8,
+    recursion_limit: u8,
     allow_inf_nan: bool,
 ) -> JsonResult<()> {
     match peek {
         Peek::True => parser.consume_true(),
         Peek::False => parser.consume_false(),
         Peek::Null => parser.consume_null(),
-        Peek::String => {
-            parser.consume_string::<StringDecoderRange>(tape, false)?;
-            Ok(())
-        }
+        Peek::String => parser.consume_string::<StringDecoderRange>(tape, false).map(drop),
         Peek::Array => {
-            if let Some(peek_first) = parser.array_first()? {
-                check_recursion!(recursion_limit, parser.index,
-                    take_value_skip(peek_first, parser, tape, recursion_limit, allow_inf_nan)?;
-                );
-                while let Some(peek) = parser.array_step()? {
-                    check_recursion!(recursion_limit, parser.index,
-                        take_value_skip(peek, parser, tape, recursion_limit, allow_inf_nan)?;
-                    );
-                }
+            if let Some(next_peek) = parser.array_first()? {
+                take_value_skip_recursive(next_peek, ARRAY, parser, tape, recursion_limit, allow_inf_nan)
+            } else {
+                Ok(())
             }
-            Ok(())
         }
         Peek::Object => {
             if parser.object_first::<StringDecoderRange>(tape)?.is_some() {
-                let peek = parser.peek()?;
-                check_recursion!(recursion_limit, parser.index,
-                    take_value_skip(peek, parser, tape, recursion_limit, allow_inf_nan)?;
-                );
-                while parser.object_step::<StringDecoderRange>(tape)?.is_some() {
-                    let peek = parser.peek()?;
-                    check_recursion!(recursion_limit, parser.index,
-                        take_value_skip(peek, parser, tape, recursion_limit, allow_inf_nan)?;
-                    );
-                }
+                take_value_skip_recursive(parser.peek()?, OBJECT, parser, tape, recursion_limit, allow_inf_nan)
+            } else {
+                Ok(())
             }
-            Ok(())
         }
-        _ => {
-            if let Err(e) = parser.consume_number::<NumberRange>(peek.into_inner(), allow_inf_nan) {
+        _ => parser
+            .consume_number::<NumberRange>(peek.into_inner(), allow_inf_nan)
+            .map(drop)
+            .map_err(|e| {
                 if !peek.is_num() {
-                    Err(json_error!(ExpectedSomeValue, parser.index))
+                    json_error!(ExpectedSomeValue, parser.index)
                 } else {
-                    Err(e)
+                    e
                 }
-            } else {
-                Ok(())
+            }),
+    }
+}
+
+const ARRAY: bool = false;
+const OBJECT: bool = true;
+
+#[inline(never)] // this is an iterative algo called only from take_value_skip, no point in inlining
+fn take_value_skip_recursive(
+    mut peek: Peek,
+    mut current_recursion: bool,
+    parser: &mut Parser,
+    tape: &mut Tape,
+    recursion_limit: u8,
+    allow_inf_nan: bool,
+) -> JsonResult<()> {
+    let mut recursion_stack = bitvec::bitarr![0; 256];
+    let recursion_limit: usize = recursion_limit.into();
+    let mut current_recursion_depth = 0;
+
+    macro_rules! push_recursion {
+        ($next_peek:expr, $value:expr) => {
+            peek = $next_peek;
+            recursion_stack.set(
+                current_recursion_depth,
+                std::mem::replace(&mut current_recursion, $value),
+            );
+            current_recursion_depth += 1;
+            if current_recursion_depth >= recursion_limit {
+                return Err(json_error!(RecursionLimitExceeded, parser.index));
             }
-        }
+        };
+    }
+
+    loop {
+        match peek {
+            Peek::True => parser.consume_true()?,
+            Peek::False => parser.consume_false()?,
+            Peek::Null => parser.consume_null()?,
+            Peek::String => {
+                parser.consume_string::<StringDecoderRange>(tape, false)?;
+            }
+            Peek::Array => {
+                if let Some(next_peek) = parser.array_first()? {
+                    push_recursion!(next_peek, ARRAY);
+                    // immediately jump to process the first value in the array
+                    continue;
+                }
+            }
+            Peek::Object => {
+                if parser.object_first::<StringDecoderRange>(tape)?.is_some() {
+                    push_recursion!(parser.peek()?, OBJECT);
+                    // immediately jump to process the first value in the object
+                    continue;
+                }
+            }
+            _ => {
+                parser
+                    .consume_number::<NumberRange>(peek.into_inner(), allow_inf_nan)
+                    .map_err(|e| {
+                        if !peek.is_num() {
+                            json_error!(ExpectedSomeValue, parser.index)
+                        } else {
+                            e
+                        }
+                    })?;
+            }
+        };
+
+        // now try to advance position in the current array or object
+        peek = loop {
+            match current_recursion {
+                ARRAY => {
+                    if let Some(next_peek) = parser.array_step()? {
+                        break next_peek;
+                    }
+                }
+                OBJECT => {
+                    if parser.object_step::<StringDecoderRange>(tape)?.is_some() {
+                        break parser.peek()?;
+                    }
+                }
+            }
+
+            current_recursion_depth = match current_recursion_depth.checked_sub(1) {
+                Some(r) => r,
+                // no recursion left, we are done
+                None => return Ok(()),
+            };
+
+            current_recursion = recursion_stack[current_recursion_depth];
+        };
     }
 }
```

### Comparing `jiter-0.4.0/crates/jiter/tests/main.rs` & `jiter-0.4.1/crates/jiter/tests/main.rs`

 * *Files 2% similar despite different names*

```diff
@@ -958,14 +958,50 @@
         JsonValue::Array(v) => {
             assert_eq!(v.len(), 2000);
         }
         _ => panic!("expected array"),
     }
 }
 
+#[test]
+fn test_recursion_limit_skip_array() {
+    let json = (0..2000).map(|_| "[ ").collect::<String>();
+    let bytes = json.as_bytes();
+    let mut jiter = Jiter::new(bytes);
+    let e = jiter.next_skip().unwrap_err();
+    assert_eq!(
+        e.error_type,
+        JiterErrorType::JsonError(JsonErrorType::RecursionLimitExceeded)
+    );
+    let expected_index = JsonValue::parse(bytes, false).unwrap_err().index;
+    assert_eq!(e.index, expected_index);
+    assert_eq!(
+        e.description(&jiter),
+        format!("recursion limit exceeded at line 1 column {}", expected_index + 1)
+    );
+}
+
+#[test]
+fn test_recursion_limit_skip_object() {
+    let json = (0..2000).map(|_| "{\"a\": ").collect::<String>();
+    let bytes = json.as_bytes();
+    let mut jiter = Jiter::new(bytes);
+    let e = jiter.next_skip().unwrap_err();
+    assert_eq!(
+        e.error_type,
+        JiterErrorType::JsonError(JsonErrorType::RecursionLimitExceeded)
+    );
+    let expected_index = JsonValue::parse(bytes, false).unwrap_err().index;
+    assert_eq!(e.index, expected_index);
+    assert_eq!(
+        e.description(&jiter),
+        format!("recursion limit exceeded at line 1 column {}", expected_index + 1)
+    );
+}
+
 macro_rules! number_bytes {
     ($($name:ident: $json:literal => $expected:expr;)*) => {
         $(
             paste::item! {
                 #[test]
                 fn [< $name >]() {
                     let mut jiter = Jiter::new($json);
@@ -1590,7 +1626,20 @@
     assert_eq!(jiter.next_str().unwrap(), "foo");
     let e = jiter.array_step().unwrap_err();
     assert_eq!(
         e.error_type,
         JiterErrorType::JsonError(JsonErrorType::EofWhileParsingList)
     );
 }
+
+#[test]
+fn test_unicode_roundtrip() {
+    // '"中文"'
+    let json_bytes = b"\"\\u4e2d\\u6587\"";
+    let value = JsonValue::parse(json_bytes, false).unwrap();
+    let cow = match value {
+        JsonValue::Str(s) => s,
+        _ => panic!("expected string"),
+    };
+    assert_eq!(cow, "中文");
+    assert!(matches!(cow, Cow::Owned(_)));
+}
```

### Comparing `jiter-0.4.0/crates/jiter/tests/python.rs` & `jiter-0.4.1/crates/jiter/tests/python.rs`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/README.md` & `jiter-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter-python/Cargo.toml` & `jiter-0.4.1/crates/jiter-python/Cargo.toml`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter-python/README.md` & `jiter-0.4.1/crates/jiter-python/README.md`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter-python/bench.py` & `jiter-0.4.1/crates/jiter-python/bench.py`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter-python/jiter.pyi` & `jiter-0.4.1/crates/jiter-python/jiter.pyi`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter-python/src/lib.rs` & `jiter-0.4.1/crates/jiter-python/src/lib.rs`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/crates/jiter-python/tests/test_jiter.py` & `jiter-0.4.1/crates/jiter-python/tests/test_jiter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from decimal import Decimal
 
 import jiter
 import pytest
 from math import inf
 from dirty_equals import IsFloatNan
 
@@ -235,7 +236,21 @@
     assert repr(f) == 'LosslessFloat(123.456789123456789e45)'
 
 
 def test_lossless_floats_int():
     v = jiter.from_json(b'123', lossless_floats=True)
     assert isinstance(v, int)
     assert v == 123
+
+
+def test_unicode_roundtrip():
+    original = ['中文']
+    json_data = json.dumps(original).encode()
+    assert jiter.from_json(json_data) == original
+    assert json.loads(json_data) == original
+
+
+def test_unicode_roundtrip_ensure_ascii():
+    original = {'name': '中文'}
+    json_data = json.dumps(original, ensure_ascii=False).encode()
+    assert jiter.from_json(json_data, cache_mode=False) == original
+    assert json.loads(json_data) == original
```

### Comparing `jiter-0.4.0/Cargo.lock` & `jiter-0.4.1/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,26 @@
 [[package]]
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
+name = "bitvec"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
+dependencies = [
+ "funty",
+ "radium",
+ "tap",
+ "wyz",
+]
+
+[[package]]
 name = "cc"
 version = "1.0.98"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "41c270e7540d725e65ac7f1b212ac8ce349719624d7bcff99f8e2e488e8cf03f"
 dependencies = [
  "jobserver",
  "libc",
@@ -90,16 +102,22 @@
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
+name = "funty"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
+
+[[package]]
 name = "fuzz"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "indexmap",
  "jiter",
  "libfuzzer-sys",
  "num-bigint",
  "num-traits",
  "serde",
@@ -149,33 +167,34 @@
 name = "itoa"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jiter"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "ahash",
  "bencher",
+ "bitvec",
  "codspeed-bencher-compat",
  "lexical-parse-float",
  "num-bigint",
  "num-traits",
  "paste",
  "pyo3",
  "pyo3-build-config",
  "serde",
  "serde_json",
  "smallvec",
 ]
 
 [[package]]
 name = "jiter-python"
-version = "0.4.0"
+version = "0.4.1"
 dependencies = [
  "jiter",
  "pyo3",
 ]
 
 [[package]]
 name = "jobserver"
@@ -290,17 +309,17 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "parking_lot"
-version = "0.12.2"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e4af0ca4f6caed20e900d564c242b8e5d4903fdacf31d3daf527b66fe6f42fb"
+checksum = "f1bf18183cf54e8d6059647fc3063646a1801cf30896933ec2311622cc4b9a27"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
@@ -325,17 +344,17 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.83"
+version = "1.0.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b33eb56c327dec362a9e55b3ad14f9d2f0904fb5a5b03b513ab5465399e9f43"
+checksum = "ec96c6a92621310b51366f1e28d05ef11489516e93be030060e5fc12024a49d6"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.21.2"
@@ -406,14 +425,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
+name = "radium"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
+
+[[package]]
 name = "redox_syscall"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "469052894dcb553421e483e4209ee581a45100d31b4018de03e5a7ad86374a7e"
 dependencies = [
  "bitflags",
 ]
@@ -428,26 +453,26 @@
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
 name = "serde"
-version = "1.0.202"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "226b61a0d411b2ba5ff6d7f73a476ac4f8bb900373459cd00fab8512828ba395"
+checksum = "7253ab4de971e72fb7be983802300c30b5a7f0c2e56fab8abfc6a214307c0094"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.202"
+version = "1.0.203"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
+checksum = "500cbc0ebeb6f46627f50f3f5811ccf6bf00643be300b4c3eabc0ef55dc5b5ba"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
@@ -472,24 +497,30 @@
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
 name = "syn"
-version = "2.0.65"
+version = "2.0.66"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d2863d96a84c6439701d7a38f9de935ec562c8832cc55d1dde0f513b52fad106"
+checksum = "c42f3f41a2de00b01c0aaad383c5a45241efc8b2d1eda5661812fda5f3cdcff5"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "tap"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "unicode-ident"
@@ -642,14 +673,23 @@
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
+name = "wyz"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
+dependencies = [
+ "tap",
+]
+
+[[package]]
 name = "zerocopy"
 version = "0.7.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ae87e3fcd617500e5d106f0380cf7b77f3c6092aae37191433159dda23cfb087"
 dependencies = [
  "zerocopy-derive",
 ]
```

### Comparing `jiter-0.4.0/Cargo.toml` & `jiter-0.4.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [workspace]
 members = ["crates/jiter-python"]
 resolver = "2"
 
 [workspace.package]
 authors = ["Samuel Colvin <samuel@pydantic.dev>"]
-version = "0.4.0"
+version = "0.4.1"
 edition = "2021"
 license = "MIT"
 keywords = ["JSON", "parsing", "deserialization", "iter"]
 categories = ["parser-implementations", "parsing"]
 homepage = "https://github.com/pydantic/jiter/"
 repository = "https://github.com/pydantic/jiter/"
```

### Comparing `jiter-0.4.0/pyproject.toml` & `jiter-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jiter-0.4.0/PKG-INFO` & `jiter-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jiter
-Version: 0.4.0
+Version: 0.4.1
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

