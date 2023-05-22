# Comparing `tmp/blobtk-0.3.3.tar.gz` & `tmp/blobtk-0.3.5.tar.gz`

## Comparing `blobtk-0.3.3.tar` & `blobtk-0.3.5.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 blobtk-0.3.3/Cargo.toml
--rw-r--r--   0      501       20    59960 2023-05-17 09:24:31.000000 blobtk-0.3.3/Cargo.lock
--rw-r--r--   0      501       20      313 2023-05-17 09:24:31.000000 blobtk-0.3.3/pyproject.toml
--rw-r--r--   0      501       20     9018 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/bam.rs
--rw-r--r--   0      501       20    18356 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/blobdir.rs
--rw-r--r--   0      501       20     8832 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/cli.rs
--rw-r--r--   0      501       20      553 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/depth.rs
--rw-r--r--   0      501       20     1855 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/fasta.rs
--rw-r--r--   0      501       20     6177 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/fastq.rs
--rw-r--r--   0      501       20     1440 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/filter.rs
--rw-r--r--   0      501       20     2738 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/io.rs
--rw-r--r--   0      501       20      788 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/lib.rs
--rw-r--r--   0      501       20      659 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/main.rs
--rw-r--r--   0      501       20     4150 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/axis.rs
--rw-r--r--   0      501       20    22218 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/blob.rs
--rw-r--r--   0      501       20     5567 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/category.rs
--rw-r--r--   0      501       20     5730 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/chart.rs
--rw-r--r--   0      501       20    38034 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/component.rs
--rw-r--r--   0      501       20     5835 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/cumulative.rs
--rw-r--r--   0      501       20     4398 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/data.rs
--rw-r--r--   0      501       20    29932 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/snail.rs
--rw-r--r--   0      501       20     1020 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot/style.rs
--rw-r--r--   0      501       20    11606 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/plot.rs
--rw-r--r--   0      501       20     3172 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/python/depth.rs
--rw-r--r--   0      501       20     3518 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/python/filter.rs
--rw-r--r--   0      501       20     1879 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/python/utils.rs
--rw-r--r--   0      501       20      491 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/python.rs
--rw-r--r--   0      501       20     4497 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/taxonomy.rs
--rw-r--r--   0      501       20     8053 2023-05-17 09:24:31.000000 blobtk-0.3.3/src/utils.rs
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 blobtk-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1410 1970-01-01 00:00:00.000000 blobtk-0.3.5/Cargo.toml
+-rw-r--r--   0      501       20    60602 2023-05-22 15:31:33.000000 blobtk-0.3.5/Cargo.lock
+-rw-r--r--   0      501       20      313 2023-05-22 15:31:33.000000 blobtk-0.3.5/pyproject.toml
+-rw-r--r--   0      501       20     9018 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/bam.rs
+-rw-r--r--   0      501       20    20229 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/blobdir.rs
+-rw-r--r--   0      501       20     8857 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/cli.rs
+-rw-r--r--   0      501       20      541 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/depth.rs
+-rw-r--r--   0      501       20      723 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/error.rs
+-rw-r--r--   0      501       20     1855 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/fasta.rs
+-rw-r--r--   0      501       20     6177 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/fastq.rs
+-rw-r--r--   0      501       20     1416 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/filter.rs
+-rw-r--r--   0      501       20     2738 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/io.rs
+-rw-r--r--   0      501       20      824 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/lib.rs
+-rw-r--r--   0      501       20      650 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/main.rs
+-rw-r--r--   0      501       20     4174 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/axis.rs
+-rw-r--r--   0      501       20    22851 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/blob.rs
+-rw-r--r--   0      501       20     5567 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/category.rs
+-rw-r--r--   0      501       20     5730 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/chart.rs
+-rw-r--r--   0      501       20    38069 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/component.rs
+-rw-r--r--   0      501       20     5835 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/cumulative.rs
+-rw-r--r--   0      501       20     4422 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/data.rs
+-rw-r--r--   0      501       20    30467 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/snail.rs
+-rw-r--r--   0      501       20     1020 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot/style.rs
+-rw-r--r--   0      501       20    12399 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/plot.rs
+-rw-r--r--   0      501       20     3172 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/python/depth.rs
+-rw-r--r--   0      501       20     3518 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/python/filter.rs
+-rw-r--r--   0      501       20     1879 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/python/utils.rs
+-rw-r--r--   0      501       20      491 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/python.rs
+-rw-r--r--   0      501       20     4497 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/taxonomy.rs
+-rw-r--r--   0      501       20     8053 2023-05-22 15:31:33.000000 blobtk-0.3.5/src/utils.rs
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 blobtk-0.3.5/PKG-INFO
```

### Comparing `blobtk-0.3.3/Cargo.toml` & `blobtk-0.3.5/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "blobtk"
-version = "0.3.3"
+version = "0.3.5"
 edition = "2021"
 authors = [
     "Rich Challis <rc28@sanger.ac.uk>",
 ]
 license = "MIT"
 description = "Core utilities for BlobToolKit."
 homepage = "https://github.com/blobtoolkit/blobtk"
@@ -26,14 +26,15 @@
 [profile.release]
 strip = true
 lto = true
 codegen-units = 1
 panic = "abort"
 
 [dependencies]
+anyhow = "1.0.71"
 atty = "0.2.14"
 clap = { version = "4.0.29", features = [ "derive" ]}
 clap-num = "1.0.2"
 colorous = "1.0.10"
 coord_transforms = "1.4.0"
 flate2 = "1.0.25"
 glob = "0.3.1"
@@ -47,14 +48,16 @@
 rust-htslib = "0.40.2"
 rust_decimal = "1.29.1"
 serde = { version = "1.0.152", features= ["derive"] }
 serde-aux = "4.2.0"
 serde_json = "1.0.93"
 serde_with = "2.3.2"
 svg = "0.13.1"
+thiserror = "1.0.40"
 tiny-skia = "0.8.3"
 titlecase = "2.2.1"
 url = { version = "2.3.1", features = ["serde"] }
 usvg = "0.31.0"
 
 [build-dependencies]
 pyo3-build-config = "0.18.3"
+
```

### Comparing `blobtk-0.3.3/Cargo.lock` & `blobtk-0.3.5/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "anyhow"
+version = "1.0.71"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
+
+[[package]]
 name = "approx"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
 dependencies = [
  "num-traits",
 ]
@@ -104,16 +110,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "blobtk"
-version = "0.3.3"
+version = "0.3.5"
 dependencies = [
+ "anyhow",
  "atty",
  "clap",
  "clap-num",
  "colorous",
  "coord_transforms",
  "flate2",
  "glob",
@@ -128,14 +135,15 @@
  "rust-htslib",
  "rust_decimal",
  "serde",
  "serde-aux",
  "serde_json",
  "serde_with",
  "svg",
+ "thiserror",
  "tiny-skia",
  "titlecase",
  "url",
  "usvg",
 ]
 
 [[package]]
@@ -154,37 +162,37 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0754613691538d51f329cce9af41d7b7ca150bc973056f1156611489475f54f7"
 dependencies = [
  "borsh-derive-internal",
  "borsh-schema-derive-internal",
  "proc-macro-crate",
  "proc-macro2",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "borsh-derive-internal"
 version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "afb438156919598d2c7bad7e1c0adf3d26ed3840dbc010db1a882a65583ca2fb"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "borsh-schema-derive-internal"
 version = "0.10.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "634205cc43f74a1b9046ef87c4540ebda95696ec0f315024860cad7c5b0f5ccd"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "buffer-redux"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2886ea01509598caac116942abd33ab5a88fa32acdf7e4abfa0fc489ca520c9"
@@ -214,15 +222,15 @@
 name = "bytecheck_derive"
 version = "0.6.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e31225543cb46f81a7e224762764f4a6a0f097b1db0b175f69e8065efaa42de5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "bytecount"
 version = "0.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c676a478f63e9fa2dd5368a42f28bba0d6c560b775f38583c8bbaa7fcd67c9c"
@@ -324,15 +332,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "684a277d672e91966334af371f1a7b5833f9aa00b07c84e92fbce95e00208ce8"
 dependencies = [
  "heck",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "783fe232adfca04f90f56201b26d79682d4cd2625e0bc7290b95123afe558ade"
@@ -450,15 +458,15 @@
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
 version = "1.0.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90201c1a650e95ccff1c8c0bb5a343213bdd317c6e600a93075bca2eff54ec97"
@@ -467,15 +475,15 @@
 name = "cxxbridge-macro"
 version = "1.0.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b75aed41bb2e6367cae39e6326ef817a851db13c13e4f3263714ca3cfb8de56"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "darling"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b750cb3417fd1b327431a470f388520309479ab0bf5e323505daf0290cd3850"
@@ -491,26 +499,26 @@
 checksum = "109c1ca6e6b7f82cc233a97004ea8ed7ca123a9af07a8230878fcfda9b158bf0"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "darling_macro"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a4aab4dbc9f7611d8b55048a3a16d2d010c2c8334e46304b40ac1cc14bf3b48e"
 dependencies = [
  "darling_core",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "data-url"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d7439c3735f405729d52c3fbbe4de140eaf938a1fe47d227c27f8254d4302a5"
@@ -519,15 +527,15 @@
 name = "derive-new"
 version = "0.5.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3418329ca0ad70234b9735dc4ceed10af4df60eff9c8e7b06cb5e520d92c3535"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "encode_unicode"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
@@ -1002,15 +1010,15 @@
 name = "nalgebra-macros"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01fcc0b8149b4632adc89ac3b7b31a12fb6099a0317a4eb2ebff574ef7de7218"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "needletail"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "db05a5ab397f64070d8c998fa0fbb84e484b81f95752af317dac183a82d9295d"
@@ -1198,15 +1206,15 @@
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro-error-attr"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1215,17 +1223,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "ptr_meta"
 version = "0.1.4"
@@ -1239,15 +1247,15 @@
 name = "ptr_meta_derive"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16b845dbfca988fa33db069c0e230574d15a3088f147a87b64c7589eb662c9ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06a3d8e8a46ab2738109347433cb7b96dffda2e4a218b03ef27090238886b147"
@@ -1288,39 +1296,39 @@
 version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bd44cf207476c6a9760c4653559be4f206efafb924d3e4cbf2721475fc0d6cc5"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc1f43d8e30460f36350d18631ccf85ded64c059829208fe680904c65bcd0a4c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -1443,15 +1451,15 @@
 name = "rkyv_derive"
 version = "0.7.41"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac1c672430eb41556291981f45ca900a0239ad007242d1cb4b4167af842db666"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "rosvgtree"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8cdb7996003c5cc8a8c2585b4ab6b422da64ad86a9c99cfa7ba320e15e8739f3"
@@ -1625,15 +1633,15 @@
 name = "serde_derive"
 version = "1.0.152"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.93"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cad406b69c91885b5107daf2c29572f6c8cdb3c66826821e286c533490c0bc76"
@@ -1664,15 +1672,15 @@
 version = "2.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "859011bddcc11f289f07f467cc1fe01c7a941daa4d8f6c40d4d1c92eb6d9319c"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "simba"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2f3fd720c48c53cace224ae62bef1bbff363a70c68c4802a78b5cc6159618176"
@@ -1747,15 +1755,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e385be0d24f186b4ce2f9982191e7101bb737312ad61c1f2f984f34bcf85d59"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "svg"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "02d815ad337e8449d2374d4248448645edfe74e699343dd5719139d93fa87112"
@@ -1788,14 +1796,25 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.16"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a6f671d4b5ffdb8eadec19c0ae67fe2639df8684bd7bc4b83d986b8db549cf01"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ae9980cab1db3fceee2f6c6f643d5d8de2997c58ee8d25fb0cc8a9e9e7348e5"
 
 [[package]]
 name = "termcolor"
@@ -1804,30 +1823,30 @@
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fb327af4685e4d03fa8cbcf1716380da910eeb2bb8be417e7f9fd3fb164f36f"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.16",
 ]
 
 [[package]]
 name = "time"
 version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
@@ -2095,15 +2114,15 @@
 checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2117,15 +2136,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.84"
```

### Comparing `blobtk-0.3.3/src/bam.rs` & `blobtk-0.3.5/src/bam.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.3/src/blobdir.rs` & `blobtk-0.3.5/src/blobdir.rs`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 use serde_aux::prelude::*;
 use serde_json;
 use serde_with::{serde_as, DefaultOnError};
 use titlecase::titlecase;
 use url::Url;
 
 use crate::cli;
-// use crate::io;
+use crate::error;
 
 pub use cli::PlotOptions;
 
 fn default_accession() -> String {
     "draft".to_string()
 }
 
@@ -70,24 +70,25 @@
     pub clamp: Option<f64>,
     pub preload: Option<bool>,
     pub active: Option<bool>,
     #[serde(rename = "set")]
     pub odb_set: Option<String>,
 }
 
-#[derive(Serialize, Deserialize, Debug, Clone)]
+#[derive(Serialize, Deserialize, Debug, Default, Clone)]
 pub struct PlotMeta {
     pub x: Option<String>,
     pub y: Option<String>,
     pub z: Option<String>,
     pub cat: Option<String>,
 }
 
 #[derive(Serialize, Deserialize, Debug)]
 pub struct TaxonMeta {
+    #[serde(default = "default_taxname")]
     pub name: String,
     pub class: Option<String>,
     pub family: Option<String>,
     pub genus: Option<String>,
     pub kingdom: Option<String>,
     pub order: Option<String>,
     pub phylum: Option<String>,
@@ -95,14 +96,18 @@
     #[serde(
         default = "default_taxid",
         deserialize_with = "deserialize_string_from_number"
     )]
     pub taxid: String,
 }
 
+fn default_taxname() -> String {
+    "unnamed".to_string()
+}
+
 fn default_taxid() -> String {
     "0".to_string()
 }
 
 #[derive(Serialize, Deserialize, Debug)]
 pub struct Meta {
     pub id: String,
@@ -112,28 +117,35 @@
     pub records: usize,
     #[serde(default = "default_revision")]
     pub revision: u8,
     #[serde(default = "default_version")]
     pub version: u8,
     pub assembly: AssemblyMeta,
     pub fields: Vec<FieldMeta>,
+    #[serde(default = "default_plotmeta")]
     pub plot: PlotMeta,
     pub taxon: TaxonMeta,
     pub field_list: Option<HashMap<String, FieldMeta>>,
     pub busco_list: Option<Vec<(String, usize, String)>>,
 }
 
 fn default_revision() -> u8 {
     0
 }
 
 fn default_version() -> u8 {
     1
 }
 
+fn default_plotmeta() -> PlotMeta {
+    PlotMeta {
+        ..Default::default()
+    }
+}
+
 #[derive(Serialize, Deserialize, Debug)]
 pub struct Field<T> {
     // pub meta: FieldMeta,
     pub values: Vec<T>,
     pub keys: Vec<String>,
     pub category_slot: Option<u8>,
     pub headers: Option<Vec<String>>,
@@ -194,17 +206,45 @@
 }
 
 #[derive(Deserialize, Debug, Clone, Serialize)]
 pub struct Keys {
     pub headers: String,
 }
 
-pub fn parse_blobdir(blobdir: &PathBuf) -> Meta {
-    let reader = file_reader(blobdir, "meta.json").unwrap();
-    let mut meta: Meta = serde_json::from_reader(reader).expect("unable to parse json");
+/// Parse a blobdir
+///
+/// # Examples
+///
+/// ```
+/// use std::path::PathBuf;
+/// # use crate::blobtk::blobdir::parse_blobdir;
+/// let meta = parse_blobdir(&PathBuf::from("test/minimal")).unwrap();
+/// assert_eq!(meta.taxon.name, "unnamed".to_string());
+/// ```
+
+pub fn parse_blobdir(blobdir: &PathBuf) -> Result<Meta, error::Error> {
+    let reader = match file_reader(blobdir, "meta.json") {
+        Some(r) => r,
+        None => {
+            return Err(error::Error::FileNotFound(format!(
+                "{}/meta.json",
+                &blobdir.to_str().unwrap()
+            )))
+        }
+    };
+    let mut meta: Meta = match serde_json::from_reader(reader) {
+        Ok(meta) => meta,
+        Err(err) => {
+            return Err(error::Error::SerdeError(format!(
+                "{}/meta.json {}",
+                &blobdir.to_str().unwrap(),
+                err.to_string()
+            )))
+        }
+    };
     let mut fields: HashMap<String, FieldMeta> = HashMap::new();
     let mut busco_fields: Vec<(String, usize, String)> = vec![];
     fn list_fields(
         field_list: &Vec<FieldMeta>,
         fields: &mut HashMap<String, FieldMeta>,
         busco_fields: &mut Vec<(String, usize, String)>,
         busco: bool,
@@ -292,15 +332,15 @@
         meta.record_type = if titlecase(&meta.assembly.level) == "Contig".to_string() {
             "contig".to_string()
         } else {
             "scaffold".to_string()
         };
     }
 
-    meta
+    Ok(meta)
 }
 
 pub fn parse_field_busco(id: String, blobdir: &PathBuf) -> Option<Vec<Vec<BuscoGene>>> {
     let reader = match file_reader(blobdir, &format!("{}.json", &id)) {
         Some(reader) => reader,
         None => return None,
     };
@@ -318,56 +358,83 @@
             });
         }
         values.push(val);
     }
     Some(values)
 }
 
-pub fn parse_field_cat(id: String, blobdir: &PathBuf) -> Option<Vec<(String, usize)>> {
+pub fn parse_field_cat(
+    id: String,
+    blobdir: &PathBuf,
+) -> Result<Vec<(String, usize)>, error::Error> {
     let reader = match file_reader(blobdir, &format!("{}.json", &id)) {
         Some(reader) => reader,
-        None => return None,
+        None => {
+            return Err(error::Error::FileNotFound(format!(
+                "{}/{}.json",
+                &blobdir.to_str().unwrap(),
+                &id
+            )))
+        }
     };
     let field: Field<usize> = serde_json::from_reader(reader).expect("unable to parse json");
     let mut values: Vec<(String, usize)> = vec![];
     let keys = field.keys.clone();
     for value in field.values() {
         values.push((keys[*value].clone(), *value))
     }
-    Some(values)
+    Ok(values)
 }
 
-pub fn parse_field_float(id: String, blobdir: &PathBuf) -> Option<Vec<f64>> {
+pub fn parse_field_float(id: String, blobdir: &PathBuf) -> Result<Vec<f64>, error::Error> {
     let reader = match file_reader(blobdir, &format!("{}.json", &id)) {
         Some(reader) => reader,
-        None => return None,
+        None => {
+            return Err(error::Error::FileNotFound(format!(
+                "{}/{}.json",
+                &blobdir.to_str().unwrap(),
+                &id
+            )))
+        }
     };
     let field: Field<f64> = serde_json::from_reader(reader).expect("unable to parse json");
     let values = field.values().clone();
-    Some(values)
+    Ok(values)
 }
 
-pub fn parse_field_int(id: String, blobdir: &PathBuf) -> Option<Vec<usize>> {
+pub fn parse_field_int(id: String, blobdir: &PathBuf) -> Result<Vec<usize>, error::Error> {
     let reader = match file_reader(blobdir, &format!("{}.json", &id)) {
         Some(reader) => reader,
-        None => return None,
+        None => {
+            return Err(error::Error::FileNotFound(format!(
+                "{}/{}.json",
+                &blobdir.to_str().unwrap(),
+                &id
+            )))
+        }
     };
     let field: Field<usize> = serde_json::from_reader(reader).expect("unable to parse json");
     let values = field.values().clone();
-    Some(values)
+    Ok(values)
 }
 
-pub fn parse_field_string(id: String, blobdir: &PathBuf) -> Option<Vec<String>> {
+pub fn parse_field_string(id: String, blobdir: &PathBuf) -> Result<Vec<String>, error::Error> {
     let reader = match file_reader(blobdir, &format!("{}.json", &id)) {
         Some(reader) => reader,
-        None => return None,
+        None => {
+            return Err(error::Error::FileNotFound(format!(
+                "{}/{}.json",
+                &blobdir.to_str().unwrap(),
+                &id
+            )))
+        }
     };
     let field: Field<String> = serde_json::from_reader(reader).expect("unable to parse json");
     let values = field.values().clone();
-    Some(values)
+    Ok(values)
 }
 
 pub fn parse_filters(
     options: &cli::PlotOptions,
     plot_meta: Option<&HashMap<String, String>>,
 ) -> HashMap<String, Filter> {
     let mut filters = options.filter.clone();
@@ -565,43 +632,48 @@
     output
 }
 
 pub fn get_plot_values(
     meta: &Meta,
     blobdir: &PathBuf,
     plot_map: &HashMap<String, String>,
-) -> (HashMap<String, Vec<f64>>, Vec<(String, usize)>) {
+) -> Result<(HashMap<String, Vec<f64>>, Vec<(String, usize)>), error::Error> {
     let mut plot_values = HashMap::new();
     let mut cat_values = vec![];
     let field_list = meta.field_list.clone().unwrap();
     for (axis, id) in plot_map {
         let field_meta_option = field_list.get(id);
         match field_meta_option {
             Some(field_meta) => {
                 let field = field_meta.clone();
                 match field.datatype {
                     Some(Datatype::Float) => {
-                        let values = parse_field_float(field_meta.id.clone(), blobdir).unwrap();
+                        let values = parse_field_float(field_meta.id.clone(), blobdir)?;
                         plot_values.insert(axis.clone(), values);
                     }
                     Some(Datatype::Integer) => {
-                        let values: Vec<f64> = parse_field_int(field_meta.id.clone(), blobdir)
-                            .unwrap()
+                        let values: Vec<f64> = parse_field_int(field_meta.id.clone(), blobdir)?
                             .iter()
                             .map(|x| x.clone() as f64)
                             .collect();
                         plot_values.insert(axis.clone(), values);
                     }
                     Some(Datatype::String) => {
                         if field.data.is_some() {
-                            cat_values = parse_field_cat(field_meta.id.clone(), blobdir).unwrap();
+                            cat_values = parse_field_cat(field_meta.id.clone(), blobdir)?;
                         }
                     }
                     Some(_) => (),
                     None => (),
                 }
             }
-            None => (),
+            None => {
+                if axis == "cat" && id == "_" {
+                    cat_values = vec![("blank".to_string(), 0); meta.records]
+                } else {
+                    ()
+                }
+            }
         };
     }
-    (plot_values, cat_values)
+    Ok((plot_values, cat_values))
 }
```

### Comparing `blobtk-0.3.3/src/cli.rs` & `blobtk-0.3.5/src/cli.rs`

 * *Files 1% similar despite different names*

```diff
@@ -159,16 +159,17 @@
     )]
     pub fastq_out: bool,
     /// Path to output list of read IDs
     #[arg(long = "read-list", short = 'O', value_name = "TXT")]
     pub read_list: Option<PathBuf>,
 }
 
-#[derive(ValueEnum, Clone, Debug)]
+#[derive(ValueEnum, Clone, Debug, Default)]
 pub enum View {
+    #[default]
     Blob,
     Cumulative,
     Snail,
 }
 
 #[derive(ValueEnum, Clone, Debug)]
 pub enum Origin {
@@ -185,24 +186,24 @@
 }
 
 fn less_than_5(s: &str) -> Result<f64, String> {
     Ok(number_range(&format!("{}", s.parse::<f64>().unwrap() * 10.0), 2, 50)? as f64 / 10.0)
 }
 
 /// Options to pass to `blobtk plot`
-#[derive(Parser, Debug)]
+#[derive(Parser, Debug, Default)]
 #[pyclass]
 pub struct PlotOptions {
     /// Path to BlobDir directory
     #[arg(long, short = 'd')]
     pub blobdir: PathBuf,
     /// View to plot
     #[arg(long, short = 'v')]
     #[clap(value_enum)]
-    pub view: Option<View>,
+    pub view: View,
     /// Output filename
     #[arg(long, short = 'o', default_value_t = String::from("output.svg"))]
     pub output: String,
     #[arg(long, short = 'f')]
     pub filter: Vec<String>,
     /// Segment count for snail plot
     #[arg(long, short = 's', default_value_t = 1000)]
```

### Comparing `blobtk-0.3.3/src/fasta.rs` & `blobtk-0.3.5/src/fasta.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.3/src/fastq.rs` & `blobtk-0.3.5/src/fastq.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.3/src/filter.rs` & `blobtk-0.3.5/src/filter.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 //!
 //! Invoked by calling:
 //! `blobtk filter <args>`
 
-use std::error::Error;
 use std::io::ErrorKind;
 
 use crate::bam;
 use crate::cli;
 use crate::fasta;
 use crate::fastq;
 use crate::io;
 
 pub use cli::FilterOptions;
 
 /// Execute the `filter` subcommand from `blobtk`.
 /// Pass a list of sequence names and a BAM file to generate
 /// a list of read names and filtered FASTA/FASTQ files.
-pub fn filter(options: &cli::FilterOptions) -> Result<(), Box<dyn Error>> {
+pub fn filter(options: &cli::FilterOptions) -> Result<(), anyhow::Error> {
     let seq_names = io::get_list(&options.list_file);
     if seq_names.is_empty() {
         return Ok(());
     }
     fasta::subsample(
         &seq_names,
         &options.fasta,
```

### Comparing `blobtk-0.3.3/src/io.rs` & `blobtk-0.3.5/src/io.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.3/src/lib.rs` & `blobtk-0.3.5/src/lib.rs`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,17 @@
 
 /// The BlobTk Command Line Interface.
 pub mod cli;
 
 /// Summarise windowed coverage depth.
 pub mod depth;
 
+/// Error handline.
+pub mod error;
+
 /// Functions for processing FASTA files.
 pub mod fasta;
 
 /// Functions for processing FASTQ files.
 pub mod fastq;
 
 /// Filter files based on a list of sequence IDs.
```

### Comparing `blobtk-0.3.3/src/plot/axis.rs` & `blobtk-0.3.5/src/plot/axis.rs`

 * *Files 2% similar despite different names*

```diff
@@ -63,17 +63,18 @@
             "bottom" => Ok(Position::BOTTOM),
             "left" => Ok(Position::LEFT),
             _ => Err(()),
         }
     }
 }
 
-#[derive(Clone, Debug, PartialEq, ValueEnum)]
+#[derive(Clone, Debug, Default, PartialEq, ValueEnum)]
 pub enum Scale {
     LINEAR,
+    #[default]
     SQRT,
     LOG,
 }
 
 impl FromStr for Scale {
     type Err = ();
     fn from_str(input: &str) -> Result<Scale, Self::Err> {
```

### Comparing `blobtk-0.3.3/src/plot/blob.rs` & `blobtk-0.3.5/src/plot/blob.rs`

 * *Files 4% similar despite different names*

```diff
@@ -244,14 +244,22 @@
         && x_meta.scale.clone().unwrap() == "scaleLog".to_string()
     {
         x_domain[0] = default_clamp;
         Some(default_clamp)
     } else {
         None
     };
+    if x_domain[0] == x_domain[1] {
+        if x_domain[0] == 0.0 {
+            x_domain[1] += 0.1;
+        } else {
+            x_domain[0] /= 0.1;
+            x_domain[1] *= 0.1;
+        }
+    }
     let x_axis = AxisOptions {
         position: Position::BOTTOM,
         height: dimensions.height + dimensions.padding[0] + dimensions.padding[2],
         label: axes["x"].clone(),
         padding: [dimensions.padding[3], dimensions.padding[1]],
         offset: dimensions.height + dimensions.padding[0] + dimensions.padding[2],
         scale: Scale::from_str(&x_meta.scale.unwrap()).unwrap(),
@@ -282,14 +290,23 @@
         && y_meta.scale.clone().unwrap() == "scaleLog".to_string()
     {
         y_domain[0] = default_clamp;
         Some(default_clamp)
     } else {
         None
     };
+
+    if y_domain[0] == y_domain[1] {
+        if y_domain[0] == 0.0 {
+            y_domain[1] += 0.1;
+        } else {
+            y_domain[0] /= 2.0;
+            y_domain[1] *= 2.0;
+        }
+    }
     let y_axis = AxisOptions {
         position: Position::LEFT,
         height: dimensions.width + dimensions.padding[1] + dimensions.padding[3],
         label: axes["y"].clone(),
         padding: [dimensions.padding[2], dimensions.padding[0]],
         scale: Scale::from_str(&y_meta.scale.unwrap()).unwrap(),
         domain: y_domain,
@@ -297,18 +314,27 @@
         clamp: y_clamp,
         rotate: true,
         ..Default::default()
     };
     let y_scaled = scale_values(&blob_data.y, &y_axis);
 
     let z_meta = fields[axes["z"].as_str()].clone();
+    let mut z_domain = z_meta.range.unwrap().clone();
+    if z_domain[0] == z_domain[1] {
+        if z_domain[0] == 0.0 {
+            z_domain[1] += 0.1;
+        } else {
+            z_domain[0] /= 2.0;
+            z_domain[1] *= 2.0;
+        }
+    }
     let z_axis = AxisOptions {
         label: axes["z"].clone(),
         scale: options.scale_function.clone(),
-        domain: z_meta.range.unwrap(),
+        domain: z_domain,
         range: [2.0, 2.0 + dimensions.height / 15.0 * options.scale_factor],
         ..Default::default()
     };
     let z_scaled = scale_values(&blob_data.z, &z_axis);
 
     let mut points = vec![];
     let cat_order = blob_data.cat_order.clone();
```

### Comparing `blobtk-0.3.3/src/plot/category.rs` & `blobtk-0.3.5/src/plot/category.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.3/src/plot/chart.rs` & `blobtk-0.3.5/src/plot/chart.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.3/src/plot/component.rs` & `blobtk-0.3.5/src/plot/component.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use std::cmp::max;
 use std::f64::consts::PI;
 
 use coord_transforms::d2::polar2cartesian;
 use coord_transforms::prelude::*;
 use num_integer::div_rem;
 use svg::node::element::path::Data;
 use svg::node::element::{Circle, Group, Line, Path, Rectangle, Text};
@@ -475,15 +476,15 @@
                             &options,
                             &options.major_ticks.as_ref().unwrap(),
                         ));
                         i = i * step;
                     }
                 }
                 TickStatus::Minor => {
-                    let mut i = 10u32.pow((power.abs() - 1) as u32) as f64;
+                    let mut i = 10u32.pow((max(0, power.abs() - 1)) as u32) as f64;
                     if power < 0 {
                         i = 1.0 / i;
                     }
                     if min_value.clone() < 0.0 {
                         i = -i
                     }
                     while i <= domain[1].clone() {
@@ -603,15 +604,15 @@
                     String::new()
                 };
                 ticks.push(set_tick(i, label, &domain, &range, &status, &scale));
                 i = i * 10.0;
             }
         }
         TickStatus::Minor => {
-            let mut i = 10u32.pow((power.abs() - 1) as u32) as f64;
+            let mut i = 10u32.pow((max(0, power.abs() - 1)) as u32) as f64;
             if power < 0 {
                 i = 1.0 / i;
             }
             if min_value.clone() < 0.0 {
                 i = -i
             }
             while i <= max_value.clone() {
```

### Comparing `blobtk-0.3.3/src/plot/cumulative.rs` & `blobtk-0.3.5/src/plot/cumulative.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.3/src/plot/data.rs` & `blobtk-0.3.5/src/plot/data.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 use clap::ValueEnum;
 use svg::node::element::path::Data;
 
 use super::axis::{AxisName, AxisOptions, Position};
 use super::category::Category;
 
-#[derive(Clone, Debug, ValueEnum)]
+#[derive(Clone, Debug, Default, ValueEnum)]
 pub enum Reducer {
+    #[default]
     Sum,
     Max,
     Min,
     Count,
     Mean,
 }
```

### Comparing `blobtk-0.3.3/src/plot/snail.rs` & `blobtk-0.3.5/src/plot/snail.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use std::cmp::Ordering;
+use std::cmp::{self, Ordering};
 use std::collections::HashSet;
 use std::f64::consts::PI;
 
 use serde;
 use serde::{Deserialize, Serialize};
 use svg::node::element::{Group, Line, Path, Rectangle, Text};
 use svg::Document;
@@ -143,23 +143,31 @@
 
 pub fn snail_stats(
     length_values: &Vec<usize>,
     gc_values: &Vec<f64>,
     n_vals: &Option<Vec<f64>>,
     ncount_values: &Vec<usize>,
     busco_values: &Vec<Vec<blobdir::BuscoGene>>,
-    busco_total: usize,
-    busco_lineage: String,
+    busco_total: Option<usize>,
+    busco_lineage: Option<String>,
     id: String,
     record_type: String,
     options: &cli::PlotOptions,
 ) -> SnailStats {
     let span = length_values.iter().sum();
     let n = ncount_values.iter().sum();
     let mut new_vals = vec![];
+    let busco_total = match busco_total {
+        Some(total) => total,
+        None => 0,
+    };
+    let busco_lineage = match busco_lineage {
+        Some(lineage) => lineage,
+        None => "".to_string(),
+    };
     let n_values = match n_vals {
         Some(vals) => vals,
         None => {
             for (i, length) in length_values.iter().enumerate() {
                 new_vals.push(ncount_values[i] as f64 / length.clone() as f64);
             }
             &new_vals
@@ -178,20 +186,22 @@
     let mut scaffold_index: usize = 0;
     let mut scaffold_sum: usize = length_values[order[scaffold_index]];
     let mut gc_span = gc_values[order[scaffold_index]]
         * ((length_values[order[scaffold_index]] - ncount_values[order[scaffold_index]]) as f64);
     let mut at_span = (1.0 - gc_values[order[scaffold_index]])
         * ((length_values[order[scaffold_index]] - ncount_values[order[scaffold_index]]) as f64);
     let mut n_span = ncount_values[order[scaffold_index]];
-    count_buscos(
-        &busco_values[order[scaffold_index]],
-        &mut busco_frag,
-        &mut busco_list,
-        &mut busco_dup,
-    );
+    if !busco_values.is_empty() {
+        count_buscos(
+            &busco_values[order[scaffold_index]],
+            &mut busco_frag,
+            &mut busco_list,
+            &mut busco_dup,
+        );
+    }
 
     let mut binned_scaffold_lengths: Vec<usize> = vec![];
     let mut binned_scaffold_counts: Vec<usize> = vec![];
     for _ in 0..options.segments {
         position += segment;
         let mut gcs: Vec<f64> = vec![gc_values[order[scaffold_index]] * 100.0];
         let mut ns: Vec<f64> = vec![n_values[order[scaffold_index]] * 100.0];
@@ -204,20 +214,22 @@
             gc_span += gc_values[order[scaffold_index]]
                 * ((length_values[order[scaffold_index]] - ncount_values[order[scaffold_index]])
                     as f64);
             at_span += (1.0 - gc_values[order[scaffold_index]])
                 * ((length_values[order[scaffold_index]] - ncount_values[order[scaffold_index]])
                     as f64);
             n_span += ncount_values[order[scaffold_index]];
-            count_buscos(
-                &busco_values[order[scaffold_index]],
-                &mut busco_frag,
-                &mut busco_list,
-                &mut busco_dup,
-            );
+            if !busco_values.is_empty() {
+                count_buscos(
+                    &busco_values[order[scaffold_index]],
+                    &mut busco_frag,
+                    &mut busco_list,
+                    &mut busco_dup,
+                );
+            }
         }
         binned_scaffold_counts.push(scaffold_index + 1);
         binned_scaffold_lengths.push(length_values[order[scaffold_index]]);
         gcs.sort_by(|a, b| a.partial_cmp(b).unwrap_or(Ordering::Equal));
         binned_gcs.push(SummaryStats {
             min: gcs[0],
             max: gcs[gcs.len() - 1],
@@ -673,15 +685,15 @@
     }
 
     let mut major_length_tick_group = Group::new();
     let mut major_length_gridline_group = Group::new();
 
     for (i, tick) in major_length_ticks.iter().enumerate() {
         let tick = tick.clone();
-        let label = if i < major_length_ticks.len() - 3 {
+        let label = if i < cmp::max(major_length_ticks.len(), 3) - 3 {
             Text::new()
         } else {
             tick.label
         };
         major_length_tick_group = major_length_tick_group.add(tick.path).add(label);
         let arc_data = arc_path(
             -1.0 * tick.position,
@@ -722,18 +734,23 @@
 
     let scale_legend = scale_stats_legend(&snail_stats, &options)
         .set("transform", format!("translate({},{})", 5, 900));
 
     let dataset_legend = dataset_name_legend(&snail_stats, &options)
         .set("transform", format!("translate({},{})", 5, 990));
 
-    let busc_stats_legend = busco_stats_legend(&snail_stats, &options)
-        .set("transform", format!("translate({},{})", 630, 25));
-
-    let busco_group = busco_plot(snail_stats).set("transform", "translate(910, 170)");
+    let (busc_stats_legend, busco_group) = if snail_stats.busco_total() >= 1 {
+        (
+            busco_stats_legend(&snail_stats, &options)
+                .set("transform", format!("translate({},{})", 630, 25)),
+            busco_plot(snail_stats).set("transform", "translate(910, 170)"),
+        )
+    } else {
+        (Group::new(), Group::new())
+    };
 
     let group = Group::new()
         .set("transform", "translate(500, 525)")
         .add(scaf_count_path)
         .add(major_count_gridline_group)
         .add(scaf_length_path)
         .add(gc_prop_path)
```

### Comparing `blobtk-0.3.3/src/plot/style.rs` & `blobtk-0.3.5/src/plot/style.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.3/src/plot.rs` & `blobtk-0.3.5/src/plot.rs`

 * *Files 7% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 //! Invoked by calling:
 //! `blobtk plot <args>`
 
 use std::collections::HashMap;
 use std::path::PathBuf;
 use std::str::FromStr;
 
+use anyhow;
+
 use crate::blobdir;
 use crate::cli;
+use crate::error;
 use crate::plot::blob::BlobData;
 use crate::plot::cumulative::CumulativeData;
 // use crate::io;
 
 use clap::ValueEnum;
 pub use cli::PlotOptions;
 use colorous;
@@ -86,76 +89,87 @@
             "png" => Ok(Suffix::PNG),
             "svg" => Ok(Suffix::SVG),
             _ => Err(()),
         }
     }
 }
 
-#[derive(ValueEnum, Clone, Debug)]
+#[derive(ValueEnum, Clone, Debug, Default)]
 pub enum ShowLegend {
+    #[default]
     Default,
     Full,
     Compact,
     None,
 }
 
-pub fn plot_snail(meta: &blobdir::Meta, options: &cli::PlotOptions) {
-    // let busco_list = meta.busco_list.clone().unwrap();
-    let busco_field = meta.busco_list.clone().unwrap()[0].clone();
-    let busco_values = blobdir::parse_field_busco(busco_field.0, &options.blobdir).unwrap();
-    let busco_total = busco_field.1;
-    let busco_lineage = busco_field.2;
-    let gc_values = blobdir::parse_field_float("gc".to_string(), &options.blobdir).unwrap();
-    let length_values = blobdir::parse_field_int("length".to_string(), &options.blobdir).unwrap();
+/// Make a snail plot
+pub fn plot_snail(meta: &blobdir::Meta, options: &cli::PlotOptions) -> Result<(), anyhow::Error> {
+    let gc_values = blobdir::parse_field_float("gc".to_string(), &options.blobdir)?;
+    let length_values = blobdir::parse_field_int("length".to_string(), &options.blobdir)?;
     let n_values = blobdir::parse_field_float("n".to_string(), &options.blobdir);
-    let ncount_values = blobdir::parse_field_int("ncount".to_string(), &options.blobdir).unwrap();
+    let ncount_values = blobdir::parse_field_int("ncount".to_string(), &options.blobdir)?;
     let id = meta.id.clone();
     let record_type = meta.record_type.clone();
 
     let filters = blobdir::parse_filters(&options, None);
     let wanted_indices = blobdir::set_filters(filters, &meta, &options.blobdir);
 
     let gc_filtered = blobdir::apply_filter_float(&gc_values, &wanted_indices);
     let n_filtered = match n_values {
-        None => None,
-        Some(values) => Some(blobdir::apply_filter_float(&values, &wanted_indices)),
+        Ok(values) => Some(blobdir::apply_filter_float(&values, &wanted_indices)),
+        Err(_) => None,
     };
     let length_filtered = blobdir::apply_filter_int(&length_values, &wanted_indices);
     let ncount_filtered = blobdir::apply_filter_int(&ncount_values, &wanted_indices);
-    let busco_filtered = blobdir::apply_filter_busco(&busco_values, &wanted_indices);
+    let busco_list = meta.busco_list.clone();
+    let (busco_total, busco_lineage, busco_filtered) = match busco_list {
+        Some(list) if !list.is_empty() => {
+            let busco_field = list[0].clone();
+            let busco_values = blobdir::parse_field_busco(busco_field.0, &options.blobdir).unwrap();
+            let busco_total = busco_field.1;
+            let busco_lineage = busco_field.2;
+            let busco_filtered = blobdir::apply_filter_busco(&busco_values, &wanted_indices);
+            (Some(busco_total), Some(busco_lineage), busco_filtered)
+        }
+        _ => (None, None, vec![]),
+    };
 
     let snail_stats = snail::snail_stats(
         &length_filtered,
         &gc_filtered,
         &n_filtered,
         &ncount_filtered,
         &busco_filtered,
         busco_total,
         busco_lineage,
         id,
         record_type,
         &options,
     );
     let document: Document = snail::svg(&snail_stats, &options);
-    save_by_suffix(options, document);
+    save_by_suffix(options, document)?;
+    Ok(())
 }
 
-fn save_by_suffix(options: &PlotOptions, document: Document) {
-    let suffix = Suffix::from_str(
-        PathBuf::from(options.output.as_str())
-            .extension()
-            .unwrap()
-            .to_str()
-            .unwrap(),
-    )
-    .unwrap();
+fn save_by_suffix(options: &PlotOptions, document: Document) -> Result<(), error::Error> {
+    let output_str = options.output.as_str();
+    let suffix_str = PathBuf::from(output_str)
+        .extension()
+        .unwrap()
+        .to_str()
+        .unwrap()
+        .to_string();
+    let suffix = Suffix::from_str(&suffix_str);
     match suffix {
-        Suffix::PNG => save_png(&document, &options),
-        Suffix::SVG => save_svg(&document, &options),
-    }
+        Ok(Suffix::PNG) => save_png(&document, &options),
+        Ok(Suffix::SVG) => save_svg(&document, &options),
+        Err(_) => return Err(error::Error::InvalidImageSuffix(suffix_str)),
+    };
+    Ok(())
 }
 
 /// Convert a colorous::Color to 6 digit hex string
 /// # Examples
 ///
 /// ```
 /// # use colorous::Color;
@@ -214,40 +228,65 @@
                 color_list[i] = hexcode;
             }
         }
     }
     color_list
 }
 
-pub fn plot_blob(meta: &blobdir::Meta, options: &cli::PlotOptions) {
-    // let busco_list = meta.busco_list.clone().unwrap();
-    let mut plot_meta: HashMap<String, String> = HashMap::new();
-    if options.x_field.is_some() {
-        plot_meta.insert("x".to_string(), options.x_field.clone().unwrap());
+fn insert_hashmap_option(
+    hash: &mut HashMap<String, String>,
+    tag: String,
+    primary: Option<String>,
+    secondary: Option<String>,
+    tertiary: Option<String>,
+) -> Result<(), error::Error> {
+    if primary.is_some() {
+        hash.insert(tag, primary.unwrap());
+    } else if secondary.is_some() {
+        hash.insert(tag, secondary.unwrap());
+    } else if tertiary.is_some() {
+        hash.insert(tag, tertiary.unwrap());
     } else {
-        plot_meta.insert("x".to_string(), meta.plot.x.clone().unwrap());
+        return Err(error::Error::AxisNotDefined(tag));
     }
-    if options.y_field.is_some() {
-        plot_meta.insert("y".to_string(), options.y_field.clone().unwrap());
-    } else {
-        plot_meta.insert("y".to_string(), meta.plot.y.clone().unwrap());
-    }
-    if options.z_field.is_some() {
-        plot_meta.insert("z".to_string(), options.z_field.clone().unwrap());
-    } else {
-        plot_meta.insert("z".to_string(), meta.plot.z.clone().unwrap());
-    }
-    if options.cat_field.is_some() {
-        plot_meta.insert("cat".to_string(), options.cat_field.clone().unwrap());
-    } else {
-        plot_meta.insert("cat".to_string(), meta.plot.cat.clone().unwrap());
-    }
-    // TODO: handle empty values
+    Ok(())
+}
+
+pub fn plot_blob(meta: &blobdir::Meta, options: &cli::PlotOptions) -> Result<(), anyhow::Error> {
+    let mut plot_meta: HashMap<String, String> = HashMap::new();
+    insert_hashmap_option(
+        &mut plot_meta,
+        "x".to_string(),
+        options.x_field.clone(),
+        meta.plot.x.clone(),
+        None,
+    )?;
+    insert_hashmap_option(
+        &mut plot_meta,
+        "y".to_string(),
+        options.y_field.clone(),
+        meta.plot.y.clone(),
+        None,
+    )?;
+    insert_hashmap_option(
+        &mut plot_meta,
+        "z".to_string(),
+        options.z_field.clone(),
+        meta.plot.z.clone(),
+        None,
+    )?;
+    insert_hashmap_option(
+        &mut plot_meta,
+        "cat".to_string(),
+        options.cat_field.clone(),
+        meta.plot.cat.clone(),
+        Some("_".to_string()),
+    )?;
 
-    let (plot_values, cat_values) = blobdir::get_plot_values(&meta, &options.blobdir, &plot_meta);
+    let (plot_values, cat_values) = blobdir::get_plot_values(&meta, &options.blobdir, &plot_meta)?;
 
     let palette = set_palette(&options.palette, &options.color, options.cat_count);
 
     let (cat_order, cat_indices) = category::set_cat_order(
         &cat_values,
         &plot_values["z"],
         &options.cat_order,
@@ -310,26 +349,33 @@
         scatter_data,
         x_bins,
         y_bins,
         max_bin,
         max_bin,
         &options,
     );
-    save_by_suffix(options, document);
+    save_by_suffix(options, document)?;
+    Ok(())
 }
 
-pub fn plot_cumulative(meta: &blobdir::Meta, options: &cli::PlotOptions) {
+pub fn plot_cumulative(
+    meta: &blobdir::Meta,
+    options: &cli::PlotOptions,
+) -> Result<(), anyhow::Error> {
     let mut plot_meta: HashMap<String, String> = HashMap::new();
     plot_meta.insert("z".to_string(), "length".to_string());
-    if options.cat_field.is_some() {
-        plot_meta.insert("cat".to_string(), options.cat_field.clone().unwrap());
-    } else {
-        plot_meta.insert("cat".to_string(), meta.plot.cat.clone().unwrap());
-    }
-    let (plot_values, cat_values) = blobdir::get_plot_values(&meta, &options.blobdir, &plot_meta);
+
+    insert_hashmap_option(
+        &mut plot_meta,
+        "cat".to_string(),
+        options.cat_field.clone(),
+        meta.plot.cat.clone(),
+        Some("_".to_string()),
+    )?;
+    let (plot_values, cat_values) = blobdir::get_plot_values(&meta, &options.blobdir, &plot_meta)?;
 
     let palette = set_palette(&options.palette, &options.color, options.cat_count);
 
     let (cat_order, cat_indices) = category::set_cat_order(
         &cat_values,
         &plot_values["z"],
         &options.cat_order,
@@ -351,22 +397,22 @@
     let dimensions = Dimensions {
         ..Default::default()
     };
 
     let cumulative_lines = cumulative::cumulative_lines(&cumulative_data, &dimensions, &options);
 
     let document: Document = cumulative::plot(dimensions, cumulative_lines, &options);
-    save_by_suffix(options, document);
+    save_by_suffix(options, document)?;
+    Ok(())
 }
 
 /// Execute the `plot` subcommand from `blobtk`.
-pub fn plot(options: &cli::PlotOptions) -> Result<(), Box<dyn std::error::Error>> {
-    let meta = blobdir::parse_blobdir(&options.blobdir);
+pub fn plot(options: &cli::PlotOptions) -> Result<(), anyhow::Error> {
+    let meta = blobdir::parse_blobdir(&options.blobdir)?;
     let view = &options.view;
     match view {
-        Some(cli::View::Blob) => plot_blob(&meta, &options),
-        Some(cli::View::Cumulative) => plot_cumulative(&meta, &options),
-        Some(cli::View::Snail) => plot_snail(&meta, &options),
-        _ => (),
+        cli::View::Blob => plot_blob(&meta, &options)?,
+        cli::View::Cumulative => plot_cumulative(&meta, &options)?,
+        cli::View::Snail => plot_snail(&meta, &options)?,
     }
     Ok(())
 }
```

### Comparing `blobtk-0.3.3/src/python/depth.rs` & `blobtk-0.3.5/src/python/depth.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.3/src/python/filter.rs` & `blobtk-0.3.5/src/python/filter.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.3/src/python/utils.rs` & `blobtk-0.3.5/src/python/utils.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.3/src/taxonomy.rs` & `blobtk-0.3.5/src/taxonomy.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 //!
 //! Invoked by calling:
 //! `blobtk taxonomy <args>`
 
 use std::collections::HashMap;
 
+use anyhow;
+
 use serde;
 use serde::{de::Error, Deserialize, Deserializer};
 
 use crate::cli;
 use crate::io;
 
 pub use cli::TaxonomyOptions;
@@ -96,15 +98,15 @@
             names,
             scientific_name: None,
         })
     }
 }
 
 /// Execute the `taxonomy` subcommand from `blobtk`.
-pub fn taxonomy(options: &cli::TaxonomyOptions) -> Result<(), Box<dyn std::error::Error>> {
+pub fn taxonomy(options: &cli::TaxonomyOptions) -> Result<(), anyhow::Error> {
     let nodes_file = match options.taxdump.clone() {
         Some(mut d) => {
             d.push("nodes.dmp");
             d
         }
         None => return Ok(()),
     };
```

### Comparing `blobtk-0.3.3/src/utils.rs` & `blobtk-0.3.5/src/utils.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.3.3/PKG-INFO` & `blobtk-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blobtk
-Version: 0.3.3
+Version: 0.3.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Core utilities for BlobToolKit.
 Keywords: bioinformatics,blobtoolkit,genome,genomics
 Home-Page: https://github.com/blobtoolkit/blobtk
 Author: Rich Challis <rc28@sanger.ac.uk>
```

