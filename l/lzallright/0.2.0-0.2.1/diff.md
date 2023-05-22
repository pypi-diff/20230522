# Comparing `tmp/lzallright-0.2.0.tar.gz` & `tmp/lzallright-0.2.1.tar.gz`

## Comparing `lzallright-0.2.0.tar` & `lzallright-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 lzallright-0.2.0/local_dependencies/lzokay-sys/Cargo.toml
--rw-r--r--   0     1001      123     2075 2023-05-22 14:41:09.000000 lzallright-0.2.0/local_dependencies/lzokay-sys/build.rs
--rw-r--r--   0     1001      123    20622 2023-05-22 14:41:09.000000 lzallright-0.2.0/local_dependencies/lzokay-sys/lzokay/lzokay.cpp
--rw-r--r--   0     1001      123     2518 2023-05-22 14:41:09.000000 lzallright-0.2.0/local_dependencies/lzokay-sys/lzokay/lzokay.hpp
--rw-r--r--   0     1001      123     1268 2023-05-22 14:41:09.000000 lzallright-0.2.0/local_dependencies/lzokay-sys/lzokay/test.cpp
--rwxr-xr-x   0     1001      123     1277 2023-05-22 14:41:09.000000 lzallright-0.2.0/local_dependencies/lzokay-sys/src/lib.rs
--rw-r--r--   0     1001      123      164 2023-05-22 14:41:09.000000 lzallright-0.2.0/local_dependencies/lzokay-sys/wrapper.hpp
--rw-r--r--   0        0        0     1062 1970-01-01 00:00:00.000000 lzallright-0.2.0/Cargo.toml
--rw-r--r--   0     1001      123     2255 2023-05-22 14:41:09.000000 lzallright-0.2.0/LICENSE
--rw-r--r--   0     1001      123      279 2023-05-22 14:41:09.000000 lzallright-0.2.0/README.md
--rw-r--r--   0     1001      123     1963 2023-05-22 14:41:09.000000 lzallright-0.2.0/benches/compress.rs
--rw-r--r--   0     1001      123    65747 2023-05-22 14:41:09.000000 lzallright-0.2.0/benches/lorem.txt
--rw-r--r--   0     1001      123      556 2023-05-22 14:41:09.000000 lzallright-0.2.0/lzallright.pyi
--rw-r--r--   0     1001      123    43708 2023-05-22 14:41:09.000000 lzallright-0.2.0/pdm.lock
--rw-r--r--   0     1001      123     1788 2023-05-22 14:41:09.000000 lzallright-0.2.0/pyproject.toml
--rw-r--r--   0     1001      123       51 2023-05-22 14:41:09.000000 lzallright-0.2.0/rust-toolchain.toml
--rw-r--r--   0     1001      123       71 2023-05-22 14:41:09.000000 lzallright-0.2.0/src/lib.rs
--rw-r--r--   0     1001      123     5496 2023-05-22 14:41:09.000000 lzallright-0.2.0/src/lzallright.rs
--rw-r--r--   0     1001      123     1291 2023-05-22 14:41:09.000000 lzallright-0.2.0/src/python.rs
--rw-r--r--   0     1001      123      976 2023-05-22 14:41:09.000000 lzallright-0.2.0/tests/test_python.py
--rw-r--r--   0     1001      123    22419 2023-05-22 14:41:09.000000 lzallright-0.2.0/Cargo.lock
--rw-r--r--   0        0        0      793 1970-01-01 00:00:00.000000 lzallright-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 lzallright-0.2.1/local_dependencies/lzokay-sys/Cargo.toml
+-rw-r--r--   0     1001      123     2075 2023-05-22 15:24:20.000000 lzallright-0.2.1/local_dependencies/lzokay-sys/build.rs
+-rw-r--r--   0     1001      123    20622 2023-05-22 15:24:20.000000 lzallright-0.2.1/local_dependencies/lzokay-sys/lzokay/lzokay.cpp
+-rw-r--r--   0     1001      123     2518 2023-05-22 15:24:20.000000 lzallright-0.2.1/local_dependencies/lzokay-sys/lzokay/lzokay.hpp
+-rw-r--r--   0     1001      123     1268 2023-05-22 15:24:20.000000 lzallright-0.2.1/local_dependencies/lzokay-sys/lzokay/test.cpp
+-rwxr-xr-x   0     1001      123     1277 2023-05-22 15:24:20.000000 lzallright-0.2.1/local_dependencies/lzokay-sys/src/lib.rs
+-rw-r--r--   0     1001      123      164 2023-05-22 15:24:20.000000 lzallright-0.2.1/local_dependencies/lzokay-sys/wrapper.hpp
+-rw-r--r--   0        0        0     1030 1970-01-01 00:00:00.000000 lzallright-0.2.1/Cargo.toml
+-rw-r--r--   0     1001      123     2255 2023-05-22 15:24:20.000000 lzallright-0.2.1/LICENSE
+-rw-r--r--   0     1001      123      279 2023-05-22 15:24:20.000000 lzallright-0.2.1/README.md
+-rw-r--r--   0     1001      123     1963 2023-05-22 15:24:20.000000 lzallright-0.2.1/benches/compress.rs
+-rw-r--r--   0     1001      123    65747 2023-05-22 15:24:20.000000 lzallright-0.2.1/benches/lorem.txt
+-rw-r--r--   0     1001      123      556 2023-05-22 15:24:20.000000 lzallright-0.2.1/lzallright.pyi
+-rw-r--r--   0     1001      123    43708 2023-05-22 15:24:20.000000 lzallright-0.2.1/pdm.lock
+-rw-r--r--   0     1001      123     1788 2023-05-22 15:24:20.000000 lzallright-0.2.1/pyproject.toml
+-rw-r--r--   0     1001      123       51 2023-05-22 15:24:20.000000 lzallright-0.2.1/rust-toolchain.toml
+-rw-r--r--   0     1001      123       71 2023-05-22 15:24:20.000000 lzallright-0.2.1/src/lib.rs
+-rw-r--r--   0     1001      123     5496 2023-05-22 15:24:20.000000 lzallright-0.2.1/src/lzallright.rs
+-rw-r--r--   0     1001      123     1291 2023-05-22 15:24:20.000000 lzallright-0.2.1/src/python.rs
+-rw-r--r--   0     1001      123      976 2023-05-22 15:24:20.000000 lzallright-0.2.1/tests/test_python.py
+-rw-r--r--   0     1001      123    22419 2023-05-22 15:24:20.000000 lzallright-0.2.1/Cargo.lock
+-rw-r--r--   0        0        0      787 1970-01-01 00:00:00.000000 lzallright-0.2.1/PKG-INFO
```

### Comparing `lzallright-0.2.0/local_dependencies/lzokay-sys/build.rs` & `lzallright-0.2.1/local_dependencies/lzokay-sys/build.rs`

 * *Files identical despite different names*

### Comparing `lzallright-0.2.0/local_dependencies/lzokay-sys/lzokay/lzokay.cpp` & `lzallright-0.2.1/local_dependencies/lzokay-sys/lzokay/lzokay.cpp`

 * *Files identical despite different names*

### Comparing `lzallright-0.2.0/local_dependencies/lzokay-sys/lzokay/lzokay.hpp` & `lzallright-0.2.1/local_dependencies/lzokay-sys/lzokay/lzokay.hpp`

 * *Files identical despite different names*

### Comparing `lzallright-0.2.0/local_dependencies/lzokay-sys/lzokay/test.cpp` & `lzallright-0.2.1/local_dependencies/lzokay-sys/lzokay/test.cpp`

 * *Files identical despite different names*

### Comparing `lzallright-0.2.0/local_dependencies/lzokay-sys/src/lib.rs` & `lzallright-0.2.1/local_dependencies/lzokay-sys/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lzallright-0.2.0/Cargo.toml` & `lzallright-0.2.1/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [package]
 name = "lzallright"
 authors= ["László Vaskó <1771332+vlaci@users.noreply.github.com>"]
-version= "0.2.0"
+version= "0.2.1"
 edition= "2021"
 license= "MIT"
-homepage= "https://github.com/pydantic/pydantic-core"
-repository= "https://github.com/pydantic/pydantic-core.git"
+homepage= "https://github.com/vlaci/lzallright"
+repository= "https://github.com/vlaci/lzallright"
 readme= "README.md"
 
 include = [
     "/pyproject.toml",
     "/pdm.lock",
     "/README.md",
     "/LICENSE",
@@ -39,14 +39,14 @@
 harness = false
 
 [workspace]
 resolver = "2"
 members = ["local_dependencies/lzokay-sys"]
 
 [workspace.package]
-version = "0.2.0"
+version = "0.2.1"
 authors = ["László Vaskó <1771332+vlaci@users.noreply.github.com>"]
 license = "MIT"
 edition = "2021"
-homepage = "https://github.com/pydantic/pydantic-core"
-repository = "https://github.com/pydantic/pydantic-core.git"
+repository = "https://github.com/vlaci/lzallright"
+homepage = "https://github.com/vlaci/lzallright"
 readme = "README.md"
```

### Comparing `lzallright-0.2.0/LICENSE` & `lzallright-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lzallright-0.2.0/benches/compress.rs` & `lzallright-0.2.1/benches/compress.rs`

 * *Files identical despite different names*

### Comparing `lzallright-0.2.0/benches/lorem.txt` & `lzallright-0.2.1/benches/lorem.txt`

 * *Files identical despite different names*

### Comparing `lzallright-0.2.0/lzallright.pyi` & `lzallright-0.2.1/lzallright.pyi`

 * *Files identical despite different names*

### Comparing `lzallright-0.2.0/pdm.lock` & `lzallright-0.2.1/pdm.lock`

 * *Files identical despite different names*

### Comparing `lzallright-0.2.0/pyproject.toml` & `lzallright-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lzallright-0.2.0/src/lzallright.rs` & `lzallright-0.2.1/src/lzallright.rs`

 * *Files identical despite different names*

### Comparing `lzallright-0.2.0/src/python.rs` & `lzallright-0.2.1/src/python.rs`

 * *Files identical despite different names*

### Comparing `lzallright-0.2.0/tests/test_python.py` & `lzallright-0.2.1/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `lzallright-0.2.0/Cargo.lock` & `lzallright-0.2.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -312,25 +312,25 @@
 checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "lzallright"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "criterion",
  "cxx",
  "lzokay-sys",
  "pyo3",
 ]
 
 [[package]]
 name = "lzokay-sys"
-version = "0.2.0"
+version = "0.2.1"
 dependencies = [
  "cxx",
  "cxx-build",
 ]
 
 [[package]]
 name = "memchr"
```

### Comparing `lzallright-0.2.0/PKG-INFO` & `lzallright-0.2.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: lzallright
-Version: 0.2.0
+Version: 0.2.1
 License-File: LICENSE
-Home-Page: https://github.com/pydantic/pydantic-core
+Home-Page: https://github.com/vlaci/lzallright
 Author: László Vaskó <1771332+vlaci@users.noreply.github.com>
 Author-email: László Vaskó <1771332+vlaci@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Repository, https://github.com/vlaci/lzallright
 Project-URL: Changelog, https://github.com/vlaci/pyperscan/blob/main/CHANGELOG.md
```

