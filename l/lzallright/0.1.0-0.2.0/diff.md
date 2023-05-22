# Comparing `tmp/lzallright-0.1.0.tar.gz` & `tmp/lzallright-0.2.0.tar.gz`

## Comparing `lzallright-0.1.0.tar` & `lzallright-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,22 @@
--rw-r--r--   0        0        0      235 1970-01-01 00:00:00.000000 lzallright-0.1.0/local_dependencies/lzokay-sys/Cargo.toml
--rw-r--r--   0     1001      123     1821 2023-05-07 23:13:49.000000 lzallright-0.1.0/local_dependencies/lzokay-sys/build.rs
--rw-r--r--   0     1001      123     1647 2023-05-07 23:13:49.000000 lzallright-0.1.0/local_dependencies/lzokay-sys/lzokay/CMakeLists.txt
--rw-r--r--   0     1001      123      107 2023-05-07 23:13:49.000000 lzallright-0.1.0/local_dependencies/lzokay-sys/lzokay/Config.cmake.in
--rw-r--r--   0     1001      123     1075 2023-05-07 23:13:49.000000 lzallright-0.1.0/local_dependencies/lzokay-sys/lzokay/LICENSE
--rw-r--r--   0     1001      123     1830 2023-05-07 23:13:49.000000 lzallright-0.1.0/local_dependencies/lzokay-sys/lzokay/README.md
--rw-r--r--   0     1001      123      204 2023-05-07 23:13:49.000000 lzallright-0.1.0/local_dependencies/lzokay-sys/lzokay/lzokay-c/CMakeLists.txt
--rw-r--r--   0     1001      123     1084 2023-05-07 23:13:49.000000 lzallright-0.1.0/local_dependencies/lzokay-sys/lzokay/lzokay-c/lzokay-c.cpp
--rw-r--r--   0     1001      123      566 2023-05-07 23:13:49.000000 lzallright-0.1.0/local_dependencies/lzokay-sys/lzokay/lzokay-c/lzokay-c.h
--rw-r--r--   0     1001      123    20622 2023-05-07 23:13:49.000000 lzallright-0.1.0/local_dependencies/lzokay-sys/lzokay/lzokay.cpp
--rw-r--r--   0     1001      123     2518 2023-05-07 23:13:49.000000 lzallright-0.1.0/local_dependencies/lzokay-sys/lzokay/lzokay.hpp
--rw-r--r--   0     1001      123     1268 2023-05-07 23:13:49.000000 lzallright-0.1.0/local_dependencies/lzokay-sys/lzokay/test.cpp
--rwxr-xr-x   0     1001      123     1277 2023-05-07 23:13:49.000000 lzallright-0.1.0/local_dependencies/lzokay-sys/src/lib.rs
--rw-r--r--   0     1001      123      164 2023-05-07 23:13:49.000000 lzallright-0.1.0/local_dependencies/lzokay-sys/wrapper.hpp
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 lzallright-0.1.0/Cargo.toml
--rw-r--r--   0     1001      123     4595 2023-05-07 23:13:49.000000 lzallright-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      799 2023-05-07 23:13:49.000000 lzallright-0.1.0/.github/workflows/Update.yml
--rw-r--r--   0     1001      123       33 2023-05-07 23:13:49.000000 lzallright-0.1.0/.gitignore
--rw-r--r--   0     1001      123     2255 2023-05-07 23:13:49.000000 lzallright-0.1.0/LICENSE
--rw-r--r--   0     1001      123      279 2023-05-07 23:13:49.000000 lzallright-0.1.0/README.md
--rw-r--r--   0     1001      123     1908 2023-05-07 23:13:49.000000 lzallright-0.1.0/benches/compress.rs
--rw-r--r--   0     1001      123    65747 2023-05-07 23:13:49.000000 lzallright-0.1.0/benches/lorem.txt
--rw-r--r--   0     1001      123       10 2023-05-07 23:15:09.000000 lzallright-0.1.0/dist/lzallright-0.1.0.tar.gz
--rw-r--r--   0     1001      123     5100 2023-05-07 23:13:49.000000 lzallright-0.1.0/flake.lock
--rw-r--r--   0     1001      123     6709 2023-05-07 23:13:49.000000 lzallright-0.1.0/flake.nix
--rw-r--r--   0     1001      123      459 2023-05-07 23:13:49.000000 lzallright-0.1.0/lzallright.pyi
--rw-r--r--   0     1001      123    27207 2023-05-07 23:13:49.000000 lzallright-0.1.0/pdm.lock
--rw-r--r--   0     1001      123       23 2023-05-07 23:13:49.000000 lzallright-0.1.0/pdm.toml
--rw-r--r--   0     1001      123      945 2023-05-07 23:13:49.000000 lzallright-0.1.0/pyproject.toml
--rw-r--r--   0     1001      123       51 2023-05-07 23:13:49.000000 lzallright-0.1.0/rust-toolchain.toml
--rw-r--r--   0     1001      123       71 2023-05-07 23:13:49.000000 lzallright-0.1.0/src/lib.rs
--rw-r--r--   0     1001      123     4068 2023-05-07 23:13:49.000000 lzallright-0.1.0/src/lzallright.rs
--rw-r--r--   0     1001      123     1291 2023-05-07 23:13:49.000000 lzallright-0.1.0/src/python.rs
--rw-r--r--   0     1001      123      295 2023-05-07 23:13:49.000000 lzallright-0.1.0/tests/test_roundtrip.py
--rw-r--r--   0     1001      123    22419 2023-05-07 23:13:49.000000 lzallright-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      668 1970-01-01 00:00:00.000000 lzallright-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 lzallright-0.2.0/local_dependencies/lzokay-sys/Cargo.toml
+-rw-r--r--   0     1001      123     2075 2023-05-22 14:41:09.000000 lzallright-0.2.0/local_dependencies/lzokay-sys/build.rs
+-rw-r--r--   0     1001      123    20622 2023-05-22 14:41:09.000000 lzallright-0.2.0/local_dependencies/lzokay-sys/lzokay/lzokay.cpp
+-rw-r--r--   0     1001      123     2518 2023-05-22 14:41:09.000000 lzallright-0.2.0/local_dependencies/lzokay-sys/lzokay/lzokay.hpp
+-rw-r--r--   0     1001      123     1268 2023-05-22 14:41:09.000000 lzallright-0.2.0/local_dependencies/lzokay-sys/lzokay/test.cpp
+-rwxr-xr-x   0     1001      123     1277 2023-05-22 14:41:09.000000 lzallright-0.2.0/local_dependencies/lzokay-sys/src/lib.rs
+-rw-r--r--   0     1001      123      164 2023-05-22 14:41:09.000000 lzallright-0.2.0/local_dependencies/lzokay-sys/wrapper.hpp
+-rw-r--r--   0        0        0     1062 1970-01-01 00:00:00.000000 lzallright-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      123     2255 2023-05-22 14:41:09.000000 lzallright-0.2.0/LICENSE
+-rw-r--r--   0     1001      123      279 2023-05-22 14:41:09.000000 lzallright-0.2.0/README.md
+-rw-r--r--   0     1001      123     1963 2023-05-22 14:41:09.000000 lzallright-0.2.0/benches/compress.rs
+-rw-r--r--   0     1001      123    65747 2023-05-22 14:41:09.000000 lzallright-0.2.0/benches/lorem.txt
+-rw-r--r--   0     1001      123      556 2023-05-22 14:41:09.000000 lzallright-0.2.0/lzallright.pyi
+-rw-r--r--   0     1001      123    43708 2023-05-22 14:41:09.000000 lzallright-0.2.0/pdm.lock
+-rw-r--r--   0     1001      123     1788 2023-05-22 14:41:09.000000 lzallright-0.2.0/pyproject.toml
+-rw-r--r--   0     1001      123       51 2023-05-22 14:41:09.000000 lzallright-0.2.0/rust-toolchain.toml
+-rw-r--r--   0     1001      123       71 2023-05-22 14:41:09.000000 lzallright-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      123     5496 2023-05-22 14:41:09.000000 lzallright-0.2.0/src/lzallright.rs
+-rw-r--r--   0     1001      123     1291 2023-05-22 14:41:09.000000 lzallright-0.2.0/src/python.rs
+-rw-r--r--   0     1001      123      976 2023-05-22 14:41:09.000000 lzallright-0.2.0/tests/test_python.py
+-rw-r--r--   0     1001      123    22419 2023-05-22 14:41:09.000000 lzallright-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 lzallright-0.2.0/PKG-INFO
```

### Comparing `lzallright-0.1.0/local_dependencies/lzokay-sys/build.rs` & `lzallright-0.2.0/local_dependencies/lzokay-sys/build.rs`

 * *Files 22% similar despite different names*

```diff
@@ -39,14 +39,23 @@
         println!(
             "cargo:rustc-link-search=native={}",
             String::from_utf8_lossy(&cpp_runtime_path)
                 .trim()
                 .strip_suffix(&cpp_runtime)
                 .expect("Failed to strip suffix"),
         );
+
+        println!(
+            "cargo:rustc-link-lib=static={}",
+            cpp_runtime
+                .chars()
+                .skip("lib".len())
+                .take(cpp_runtime.len() - "lib.a".len())
+                .collect::<String>()
+        );
     }
 
     #[cfg(target_os = "macos")]
     {
         println!("cargo:rustc-link-lib=dylib=c++");
         println!("cargo:rustc-link-lib=dylib=c++abi");
     }
```

### Comparing `lzallright-0.1.0/local_dependencies/lzokay-sys/lzokay/lzokay.cpp` & `lzallright-0.2.0/local_dependencies/lzokay-sys/lzokay/lzokay.cpp`

 * *Files identical despite different names*

### Comparing `lzallright-0.1.0/local_dependencies/lzokay-sys/lzokay/lzokay.hpp` & `lzallright-0.2.0/local_dependencies/lzokay-sys/lzokay/lzokay.hpp`

 * *Files identical despite different names*

### Comparing `lzallright-0.1.0/local_dependencies/lzokay-sys/lzokay/test.cpp` & `lzallright-0.2.0/local_dependencies/lzokay-sys/lzokay/test.cpp`

 * *Files identical despite different names*

### Comparing `lzallright-0.1.0/local_dependencies/lzokay-sys/src/lib.rs` & `lzallright-0.2.0/local_dependencies/lzokay-sys/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lzallright-0.1.0/LICENSE` & `lzallright-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lzallright-0.1.0/benches/compress.rs` & `lzallright-0.2.0/benches/compress.rs`

 * *Files 9% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 }
 
 fn bench_decompress(b: &mut Bencher<'_>) {
     Python::with_gil(|py| {
         let mut comp = LZOCompressor::new();
         let data = comp.compress(py, LOREM.into()).unwrap();
 
-        b.iter(|| LZOCompressor::decompress(py, black_box(data.as_bytes().into())));
+        b.iter(|| {
+            LZOCompressor::decompress(py, black_box(data.as_bytes().into()), Some(LOREM.len()))
+        });
     });
 }
 
 fn bench_compress_big(b: &mut Bencher<'_>) {
     let mut data = Vec::with_capacity(LOREM.len() * 100);
     for _ in 0..100 {
         data.extend_from_slice(LOREM);
@@ -38,17 +40,17 @@
     let mut data = Vec::with_capacity(LOREM.len() * 100);
     for _ in 0..100 {
         data.extend_from_slice(LOREM);
     }
 
     Python::with_gil(|py| {
         let mut comp = LZOCompressor::new();
-        let data = comp.compress(py, data[..].into()).unwrap();
+        let c = comp.compress(py, data[..].into()).unwrap();
 
-        b.iter(|| LZOCompressor::decompress(py, black_box(data.as_bytes().into())));
+        b.iter(|| LZOCompressor::decompress(py, black_box(c.as_bytes().into()), Some(data.len())));
     });
 }
 
 pub fn criterion_benchmark(c: &mut Criterion) {
     pyo3::prepare_freethreaded_python();
     c.bench_function("compress", bench_compress);
     c.bench_function("decompress", bench_decompress);
```

### Comparing `lzallright-0.1.0/benches/lorem.txt` & `lzallright-0.2.0/benches/lorem.txt`

 * *Files identical despite different names*

### Comparing `lzallright-0.1.0/src/lzallright.rs` & `lzallright-0.2.0/src/lzallright.rs`

 * *Files 18% similar despite different names*

```diff
@@ -28,16 +28,16 @@
             lzokay_sys::EResult::Error => EResult::Error,
             lzokay_sys::EResult::InputNotConsumed => EResult::InputNotConsumed,
             _ => unreachable!(),
         }
     }
 }
 
-create_exception!(module, LZOError, pyo3::exceptions::PyException);
-create_exception!(module, InputNotConsumed, LZOError);
+create_exception!(lzallright, LZOError, pyo3::exceptions::PyException);
+create_exception!(lzallright, InputNotConsumed, LZOError);
 
 #[pyclass(unsendable)]
 pub struct LZOCompressor {
     dict: UniquePtr<lzokay_sys::DictBase>,
 }
 
 #[pymethods]
@@ -72,16 +72,24 @@
                 Ok(unsafe { py.from_owned_ptr(PyBytes_FromObject(dst.as_ptr())) })
             }
             e => Err(LZOError::new_err(EResult::from(e))),
         }
     }
 
     #[staticmethod]
-    pub fn decompress<'a>(py: Python<'a>, data: Buffer) -> PyResult<&'a PyBytes> {
-        let size = 2 * data.len();
+    pub fn decompress<'a>(
+        py: Python<'a>,
+        data: Buffer,
+        output_size_hint: Option<usize>,
+    ) -> PyResult<&'a PyBytes> {
+        let size = if let Some(size) = output_size_hint {
+            size
+        } else {
+            2 * data.len()
+        };
         let mut decompressed_size = 0usize;
         let mut result;
         let dst = PyByteArray::new_with(py, size, |_| Ok(()))?;
         loop {
             let dst_bytes = unsafe { dst.as_bytes_mut() };
             result = py.allow_threads(|| unsafe {
                 lzokay_sys::decompress(
@@ -89,55 +97,93 @@
                     data.len(),
                     dst_bytes.as_mut_ptr(),
                     dst_bytes.len(),
                     &mut decompressed_size,
                 )
             });
             if result == lzokay_sys::EResult::OutputOverrun {
-                dst.resize(2 * size)?;
+                dst.resize(2 * dst.len())?;
                 continue;
             }
             break;
         }
         dst.resize(decompressed_size)?;
+
+        let rv = unsafe { py.from_owned_ptr::<PyBytes>(PyBytes_FromObject(dst.as_ptr())) };
         match result {
-            lzokay_sys::EResult::Success => {
-                Ok(unsafe { py.from_owned_ptr(PyBytes_FromObject(dst.as_ptr())) })
+            lzokay_sys::EResult::Success => Ok(rv),
+            lzokay_sys::EResult::InputNotConsumed => {
+                Err(InputNotConsumed::new_err::<(_, Py<PyBytes>)>((
+                    EResult::InputNotConsumed,
+                    rv.into(),
+                )))
             }
             e => Err(LZOError::new_err(EResult::from(e))),
         }
     }
 }
 
 impl Default for LZOCompressor {
     fn default() -> Self {
         Self::new()
     }
 }
 
 #[pymodule]
-fn lzallright(_py: Python, m: &PyModule) -> PyResult<()> {
+fn lzallright(py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<LZOCompressor>()?;
     m.add_class::<EResult>()?;
+    m.add("LZOError", py.get_type::<LZOError>())?;
+    m.add("InputNotConsumed", py.get_type::<InputNotConsumed>())?;
     Ok(())
 }
 
 #[cfg(test)]
 mod test {
+    use pyo3::types::PyType;
+
     use super::*;
 
     pub const LOREM: &[u8] = include_bytes!("../benches/lorem.txt");
 
     #[test]
     fn test_roundtrip() {
         pyo3::prepare_freethreaded_python();
 
         Python::with_gil(|py| {
             let mut comp = LZOCompressor::new();
             let compressed = comp.compress(py, LOREM.into()).unwrap();
 
-            let out = LZOCompressor::decompress(py, compressed.as_bytes().into()).unwrap();
+            let out =
+                LZOCompressor::decompress(py, compressed.as_bytes().into(), Some(LOREM.len()))
+                    .unwrap();
 
             assert_eq!(out.as_bytes(), LOREM);
         });
     }
+
+    #[test]
+    fn test_decompress_invalid_data() {
+        pyo3::prepare_freethreaded_python();
+
+        Python::with_gil(|py| {
+            let err = LZOCompressor::decompress(py, LOREM.into(), None).unwrap_err();
+            assert!(err.get_type(py).is(PyType::new::<LZOError>(py)));
+        });
+    }
+
+    #[test]
+    fn test_big_compression_ratio() {
+        // https://github.com/vlaci/lzallright/issues/12
+        pyo3::prepare_freethreaded_python();
+
+        Python::with_gil(|py| {
+            let mut comp = LZOCompressor::new();
+            let data = [0u8; 65536];
+            let compressed = comp.compress(py, data[..].into()).unwrap();
+
+            let out = LZOCompressor::decompress(py, compressed.as_bytes().into(), None).unwrap();
+
+            assert_eq!(out.as_bytes(), data);
+        });
+    }
 }
```

### Comparing `lzallright-0.1.0/src/python.rs` & `lzallright-0.2.0/src/python.rs`

 * *Files identical despite different names*

### Comparing `lzallright-0.1.0/Cargo.lock` & `lzallright-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -312,25 +312,25 @@
 checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "lzallright"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "criterion",
  "cxx",
  "lzokay-sys",
  "pyo3",
 ]
 
 [[package]]
 name = "lzokay-sys"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
 name = "memchr"
```

### Comparing `lzallright-0.1.0/PKG-INFO` & `lzallright-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: lzallright
-Version: 0.1.0
+Version: 0.2.0
 License-File: LICENSE
-Summary: 
+Home-Page: https://github.com/pydantic/pydantic-core
 Author: László Vaskó <1771332+vlaci@users.noreply.github.com>
 Author-email: László Vaskó <1771332+vlaci@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/vlaci/lzallright
+Project-URL: Repository, https://github.com/vlaci/lzallright
+Project-URL: Changelog, https://github.com/vlaci/pyperscan/blob/main/CHANGELOG.md
 
 # lzallright
 
 A Python 3.8+ binding for [LZ👌](https://github.com/jackoalan/lzokay) library which is
 
 > A minimal, C++14 implementation of the
 > [LZO compression format](http://www.oberhumer.com/opensource/lzo/).
```

