# Comparing `tmp/pyscan_rs-0.1.1.tar.gz` & `tmp/pyscan_rs-0.1.2.tar.gz`

## Comparing `pyscan_rs-0.1.1.tar` & `pyscan_rs-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,27 @@
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pyscan_rs-0.1.1/Cargo.toml
--rw-r--r--   0        0        0      834 2023-05-16 11:24:31.000000 pyscan_rs-0.1.1/.github/FUNDING.yml
--rw-r--r--   0        0        0      872 2023-05-16 11:24:31.000000 pyscan_rs-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      615 2023-05-16 11:24:31.000000 pyscan_rs-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     2428 2023-05-16 10:26:25.000000 pyscan_rs-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      756 2023-05-15 14:06:10.000000 pyscan_rs-0.1.1/.gitignore
--rw-r--r--   0        0        0      504 2023-05-17 11:34:32.000000 pyscan_rs-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0     5355 2023-05-16 11:24:31.000000 pyscan_rs-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1280 2023-05-16 11:24:31.000000 pyscan_rs-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    38864 2023-05-17 11:27:36.000000 pyscan_rs-0.1.1/Cargo.lock
--rw-r--r--   0        0        0     1086 2023-05-16 11:24:31.000000 pyscan_rs-0.1.1/LICENSE
--rw-r--r--   0        0        0     2718 2023-05-17 11:45:20.000000 pyscan_rs-0.1.1/README.md
--rw-r--r--   0        0        0      201 2023-05-16 11:24:31.000000 pyscan_rs-0.1.1/SECURITY.md
--rw-r--r--   0        0        0     8746 2023-04-22 10:47:51.000000 pyscan_rs-0.1.1/osv_schema.json
--rw-r--r--   0        0        0      367 2023-05-16 07:21:52.000000 pyscan_rs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 13:16:26.000000 pyscan_rs-0.1.1/python/pyscan/__init__.py
--rw-r--r--   0        0        0      913 2023-05-15 13:49:45.000000 pyscan_rs-0.1.1/python/pyscan/__main__.py
--rw-r--r--   0        0        0     2517 2023-05-17 11:28:49.000000 pyscan_rs-0.1.1/src/main.rs
--rw-r--r--   0        0        0     2570 2023-05-17 11:24:08.000000 pyscan_rs-0.1.1/src/parser/extractor.rs
--rw-r--r--   0        0        0     5553 2023-05-15 12:17:36.000000 pyscan_rs-0.1.1/src/parser/mod.rs
--rw-r--r--   0        0        0     1791 2023-05-16 04:24:12.000000 pyscan_rs-0.1.1/src/parser/structs.rs
--rw-r--r--   0        0        0     4908 2023-05-17 10:45:05.000000 pyscan_rs-0.1.1/src/scanner/api.rs
--rw-r--r--   0        0        0     4301 2023-05-17 11:16:03.000000 pyscan_rs-0.1.1/src/scanner/mod.rs
--rw-r--r--   0        0        0     4505 2023-05-16 04:29:05.000000 pyscan_rs-0.1.1/src/scanner/models.rs
--rw-r--r--   0        0        0      431 2023-05-17 11:27:51.000000 pyscan_rs-0.1.1/src/utils.rs
--rw-r--r--   0        0        0      623 2023-05-16 01:39:11.000000 pyscan_rs-0.1.1/test/pyproject.toml
--rw-r--r--   0        0        0       62 2023-05-15 02:54:22.000000 pyscan_rs-0.1.1/test/requirements.txt
--rw-r--r--   0        0        0      195 2023-04-24 05:12:56.000000 pyscan_rs-0.1.1/test/something.py
--rw-r--r--   0        0        0     3376 1970-01-01 00:00:00.000000 pyscan_rs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pyscan_rs-0.1.2/Cargo.toml
+-rw-r--r--   0        0        0      834 2023-05-16 11:24:31.000000 pyscan_rs-0.1.2/.github/FUNDING.yml
+-rw-r--r--   0        0        0      872 2023-05-16 11:24:31.000000 pyscan_rs-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      615 2023-05-16 11:24:31.000000 pyscan_rs-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2662 2023-05-17 11:57:45.000000 pyscan_rs-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      756 2023-05-15 14:06:10.000000 pyscan_rs-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1507 2023-05-22 12:59:21.000000 pyscan_rs-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0     5355 2023-05-16 11:24:31.000000 pyscan_rs-0.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1280 2023-05-16 11:24:31.000000 pyscan_rs-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    38864 2023-05-22 08:00:37.000000 pyscan_rs-0.1.2/Cargo.lock
+-rw-r--r--   0        0        0     1086 2023-05-16 11:24:31.000000 pyscan_rs-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3046 2023-05-22 07:58:55.000000 pyscan_rs-0.1.2/README.md
+-rw-r--r--   0        0        0      201 2023-05-16 11:24:31.000000 pyscan_rs-0.1.2/SECURITY.md
+-rw-r--r--   0        0        0     8746 2023-04-22 10:47:51.000000 pyscan_rs-0.1.2/osv_schema.json
+-rw-r--r--   0        0        0      367 2023-05-16 07:21:52.000000 pyscan_rs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 13:16:26.000000 pyscan_rs-0.1.2/python/pyscan/__init__.py
+-rw-r--r--   0        0        0      913 2023-05-15 13:49:45.000000 pyscan_rs-0.1.2/python/pyscan/__main__.py
+-rw-r--r--   0        0        0     4182 2023-05-21 04:54:34.000000 pyscan_rs-0.1.2/src/docker/mod.rs
+-rw-r--r--   0        0        0     3749 2023-05-21 04:44:58.000000 pyscan_rs-0.1.2/src/main.rs
+-rw-r--r--   0        0        0     2594 2023-05-21 05:27:06.000000 pyscan_rs-0.1.2/src/parser/extractor.rs
+-rw-r--r--   0        0        0     5381 2023-05-21 05:26:22.000000 pyscan_rs-0.1.2/src/parser/mod.rs
+-rw-r--r--   0        0        0     1795 2023-05-20 04:05:11.000000 pyscan_rs-0.1.2/src/parser/structs.rs
+-rw-r--r--   0        0        0     4737 2023-05-20 04:05:14.000000 pyscan_rs-0.1.2/src/scanner/api.rs
+-rw-r--r--   0        0        0     3354 2023-05-21 04:33:52.000000 pyscan_rs-0.1.2/src/scanner/mod.rs
+-rw-r--r--   0        0        0     4505 2023-05-16 04:29:05.000000 pyscan_rs-0.1.2/src/scanner/models.rs
+-rw-r--r--   0        0        0     4462 2023-05-20 04:06:07.000000 pyscan_rs-0.1.2/src/utils.rs
+-rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 pyscan_rs-0.1.2/PKG-INFO
```

### Comparing `pyscan_rs-0.1.1/Cargo.toml` & `pyscan_rs-0.1.2/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyscan"
-version = "0.1.1"
+version = "0.1.2"
 edition = "2021"
 authors = ["Aswin <aswinsnair@protonmail.com>"]
 license = "MIT"
 description = "Python dependency vulnerability scanner"
 readme = "README.md"
 homepage = "https://github.com/aswinnnn/pyscan"
 repository = "https://github.com/aswinnnn/pyscan"
```

### Comparing `pyscan_rs-0.1.1/.github/FUNDING.yml` & `pyscan_rs-0.1.2/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `pyscan_rs-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `pyscan_rs-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.1/.gitignore` & `pyscan_rs-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.1/CODE_OF_CONDUCT.md` & `pyscan_rs-0.1.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.1/CONTRIBUTING.md` & `pyscan_rs-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.1/Cargo.lock` & `pyscan_rs-0.1.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -766,15 +766,15 @@
 checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pyscan"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "chrono",
  "clap",
  "console",
  "lazy_static",
  "pep-508",
  "regex",
```

### Comparing `pyscan_rs-0.1.1/LICENSE` & `pyscan_rs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.1/README.md` & `pyscan_rs-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,80 @@
 <h1 align="center"> 🐍 Pyscan </h1>
 
-![CI](https://github.com/aswinnnn/pyscan/actions/workflows/CI.yml/badge.svg) ![Liscense](https://img.shields.io/github/license/aswinnnn/pyscan?color=ff64b4) [![PyPI](https://img.shields.io/pypi/v/pyscan-rs?color=ff69b4)](https://pypi.org/project/pyscan-rs) [![](https://img.shields.io/crates/v/pyscan?color=ff64b4)](https://crates.io/pyscan) [![GitHub issues](https://img.shields.io/github/issues/aswinnnn/pyscan.svg?color=ff69b4)](https://GitHub.com/aswinnnn/pyscan/issues/) [![Top Language](https://img.shields.io/github/languages/top/aswinnnn/pyscan?color=ff69b4)](https://img.shields.io/github/languages/top/aswinnnn/pyscan)
+![CI](https://github.com/aswinnnn/pyscan/actions/workflows/CI.yml/badge.svg) ![Liscense](https://img.shields.io/github/license/aswinnnn/pyscan?color=ff64b4) [![PyPI](https://img.shields.io/pypi/v/pyscan-rs?color=ff69b4)](https://pypi.org/project/pyscan-rs) [![](https://img.shields.io/crates/v/pyscan?color=ff64b4)](https://crates.io/crates/pyscan) [![GitHub issues](https://img.shields.io/github/issues/aswinnnn/pyscan.svg?color=ff69b4)](https://GitHub.com/aswinnnn/pyscan/issues/) [![Top Language](https://img.shields.io/github/languages/top/aswinnnn/pyscan?color=ff69b4)](https://img.shields.io/github/languages/top/aswinnnn/pyscan)
 
 <h4 align="center"> 
 
 <img src="https://media.discordapp.net/attachments/1002212458502557718/1107648562004758538/pyscan.png?width=779&height=206">
 
 </h4>
 
 <h5 align="center"> <i>A dependency vulnerability scanner for your python projects, straight from the terminal.</i> </h5>
 
-+ 🚀 blazingly fast and efficient scanner that can be used to scan large projects fairly quickly.
-+ 🤖 automatically uses `requirements.txt`, `pyproject.toml` or straight from the source code (though not reccomended)
-+ 🧑‍💻 easy to use, and can be integrated into existing build processes.
-+ 💽 In its very early alpha stage, so some features may not work correctly. PRs and issue makers welcome.
++ 🚀 blazingly fast scanner that can be used within large projects quickly.
++ 🤖 automatically uses `requirements.txt`, `pyproject.toml` or, the source code (highly discouraged)
++ 🧑‍💻 can be integrated into existing build processes.
++ 💽 In its alpha stage, some features may not work correctly. PRs and issue makers welcome.
 
 ## 🕊️ Install
 
 ```bash
-pip install pyscan-rs
+> pip install pyscan-rs
 ```
 look out for the "-rs" part
 or
 
 ```bash
-cargo install pyscan
+> cargo install pyscan
 ```
 
-or check out the [releases](https://github.com/aswinnnn/pyscan/releases).
+check out the [releases](https://github.com/aswinnnn/pyscan/releases).
 
 ## 🐇 Usage
 
-Go to your python source directory (or wherever you keep your requirements.txt/pyproject.toml) and run:
+Go to your python source directory (or wherever you keep your `requirements.txt`/`pyproject.toml`) and run:
 
 ```bash
-pyscan
+> pyscan
 ```
 or
 ```bash
-pyscan -d path/to/src
+> pyscan -d path/to/src
 ```
 
-that should get the thing going.
+## Docker
+
+Pyscan can scan inside docker images given you provide the correct path inside. This is still in its early stage and may break easily.
+
+```bash
+> pyscan docker -n my-docker-image -p /path/inside/container/to/source
+```
+
+by <i>"source"</i> I mean `requirements.txt`, `pyproject.toml` or your python files.
+
+<br>
 Here's the order of precedence for a "source" file:
 
-+ requirements.txt
-+ pyproject.toml
-+ your python source code (.py) [highly not reccomended]
++ `requirements.txt`
++ `pyproject.toml`
++ your python source code (`.py`) [highly discouraged]
 
-Any dependencies without a specified version defaults to its latest stable version. **Make sure you version-ize your requirements** and use proper [pep-508 syntax](https://peps.python.org/pep-0508/).
+Pyscan will find dependency versions from `pip` if not provided within the source file. Even though, **Make sure you version-ize your requirements** and use proper [pep-508 syntax](https://peps.python.org/pep-0508/).
 
 ## 🦀 Note
 
 pyscan uses [OSV](https://osv.dev) as its database for now. There are plans to add a few more.
 
-pyscan doesn't make sure your code is safe from everything. Use all resources available to you like Dependabot and other github features.
+pyscan doesn't make sure your code is safe from everything. Use all resources available to you like Dependabot, `pip-audit` or trivy.
 
 ## 🐰 Todo
 
 - [x] get it working.
-- [ ] add  tests.
-- [ ] more advisory databases.
-- [ ] query individual dependencies.
+- [ ] add  tests. [coming soon]
+- [x] query individual python packages. [v0.1.1]
 - [ ] perfomance optimizations.
+- [x] scan docker images [v0.1.2]
+- [ ] scan code health. [coming soon]
 
 ## 🐹 Sponsor
 
 While not coding, I am a broke high school student with nothing else to do. I appreciate all the help I'm worthy of.
```

### Comparing `pyscan_rs-0.1.1/osv_schema.json` & `pyscan_rs-0.1.2/osv_schema.json`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.1/python/pyscan/__main__.py` & `pyscan_rs-0.1.2/python/pyscan/__main__.py`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.1/src/main.rs` & `pyscan_rs-0.1.2/src/parser/extractor.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,158 +1,163 @@
-00000000: 7573 6520 7374 643a 3a7b 7061 7468 3a3a  use std::{path::
-00000010: 5061 7468 4275 662c 2070 726f 6365 7373  PathBuf, process
-00000020: 3a3a 6578 6974 7d3b 0d0a 7573 6520 636c  ::exit};..use cl
-00000030: 6170 3a3a 7b50 6172 7365 722c 2053 7562  ap::{Parser, Sub
-00000040: 636f 6d6d 616e 647d 3b0d 0a6d 6f64 2075  command};..mod u
-00000050: 7469 6c73 3b0d 0a6d 6f64 2070 6172 7365  tils;..mod parse
-00000060: 723b 0d0a 6d6f 6420 7363 616e 6e65 723b  r;..mod scanner;
-00000070: 0d0a 0d0a 7573 6520 7374 643a 3a65 6e76  ....use std::env
-00000080: 3b0d 0a0d 0a75 7365 2063 7261 7465 3a3a  ;....use crate::
-00000090: 7b75 7469 6c73 3a3a 6765 745f 7665 7273  {utils::get_vers
-000000a0: 696f 6e2c 2070 6172 7365 723a 3a73 7472  ion, parser::str
-000000b0: 7563 7473 3a3a 4465 7065 6e64 656e 6379  ucts::Dependency
-000000c0: 2c20 7363 616e 6e65 723a 3a61 7069 3a3a  , scanner::api::
-000000d0: 4f73 767d 3b0d 0a0d 0a23 5b64 6572 6976  Osv};....#[deriv
-000000e0: 6528 5061 7273 6572 2c20 4465 6275 6729  e(Parser, Debug)
-000000f0: 5d0d 0a23 5b63 6f6d 6d61 6e64 2861 7574  ]..#[command(aut
-00000100: 686f 723d 2261 7377 696e 6e6e 6e22 2c76  hor="aswinnnn",v
-00000110: 6572 7369 6f6e 3d22 302e 312e 3122 2c61  ersion="0.1.1",a
-00000120: 626f 7574 3d22 7079 7468 6f6e 2064 6570  bout="python dep
-00000130: 656e 6465 6e63 7920 7675 6c6e 6572 6162  endency vulnerab
-00000140: 696c 6974 7920 7363 616e 6e65 722e 2229  ility scanner.")
-00000150: 5d0d 0a73 7472 7563 7420 436c 6920 7b0d  ]..struct Cli {.
-00000160: 0a0d 0a20 2020 202f 2f2f 2070 6174 6820  ...    /// path 
-00000170: 746f 2073 6f75 7263 652e 2069 6620 6e6f  to source. if no
-00000180: 7420 7072 6f76 6964 6564 2069 7420 7769  t provided it wi
-00000190: 6c6c 2075 7365 2074 6865 2063 7572 7265  ll use the curre
-000001a0: 6e74 2064 6972 6563 746f 7279 2e0d 0a20  nt directory... 
-000001b0: 2020 2023 5b61 7267 286c 6f6e 672c 7368     #[arg(long,sh
-000001c0: 6f72 742c 6465 6661 756c 745f 7661 6c75  ort,default_valu
-000001d0: 653d 4e6f 6e65 2c76 616c 7565 5f6e 616d  e=None,value_nam
-000001e0: 653d 2244 4952 4543 544f 5259 2229 5d0d  e="DIRECTORY")].
-000001f0: 0a20 2020 2064 6972 3a20 4f70 7469 6f6e  .    dir: Option
-00000200: 3c50 6174 6842 7566 3e2c 0d0a 0d0a 2020  <PathBuf>,....  
-00000210: 2020 2f2f 2f20 7365 6172 6368 2066 6f72    /// search for
-00000220: 2061 2073 696e 676c 6520 7061 636b 6167   a single packag
-00000230: 652c 2064 6f20 2270 7973 6361 6e20 7061  e, do "pyscan pa
-00000240: 636b 6167 6520 2d2d 6865 6c70 2220 666f  ckage --help" fo
-00000250: 7220 6d6f 7265 0d0a 2020 2020 235b 636f  r more..    #[co
-00000260: 6d6d 616e 6428 7375 6263 6f6d 6d61 6e64  mmand(subcommand
-00000270: 295d 0d0a 2020 2020 7061 636b 6167 653a  )]..    package:
-00000280: 204f 7074 696f 6e3c 5375 6243 6f6d 6d61   Option<SubComma
-00000290: 6e64 3e2c 0d0a 0d0a 2020 2020 2f2f 2f20  nd>,....    /// 
-000002a0: 736b 6970 3a20 736b 6970 2074 6865 2067  skip: skip the g
-000002b0: 6976 656e 2064 6174 6162 6173 6573 0d0a  iven databases..
-000002c0: 2020 2020 2f2f 2f20 6578 2e20 7079 7363      /// ex. pysc
-000002d0: 616e 202d 7320 6f73 762c 736e 796b 0d0a  an -s osv,snyk..
-000002e0: 2020 2020 2f2f 2f20 6869 6464 656e 2064      /// hidden d
-000002f0: 7565 2074 6f20 6f6e 6c79 2068 6176 696e  ue to only havin
-00000300: 6720 6f6e 6520 6461 7461 6261 7365 2066  g one database f
-00000310: 6f72 206e 6f77 2e0d 0a20 2020 2023 5b61  or now...    #[a
-00000320: 7267 2873 686f 7274 2c20 6c6f 6e67 2c20  rg(short, long, 
-00000330: 7661 6c75 655f 6465 6c69 6d69 7465 723d  value_delimiter=
-00000340: 272c 272c 2076 616c 7565 5f6e 616d 653d  ',', value_name=
-00000350: 2256 414c 312c 5641 4c32 2c56 414c 332e  "VAL1,VAL2,VAL3.
-00000360: 2e2e 222c 2068 6964 653d 7472 7565 295d  ..", hide=true)]
-00000370: 0d0a 2020 2020 736b 6970 3a20 5665 633c  ..    skip: Vec<
-00000380: 5374 7269 6e67 3e0d 0a0d 0a7d 0d0a 0d0a  String>....}....
-00000390: 235b 6465 7269 7665 2853 7562 636f 6d6d  #[derive(Subcomm
-000003a0: 616e 642c 2044 6562 7567 2c20 436c 6f6e  and, Debug, Clon
-000003b0: 6529 5d0d 0a65 6e75 6d20 5375 6243 6f6d  e)]..enum SubCom
-000003c0: 6d61 6e64 207b 0d0a 2020 2020 2f2f 2f20  mand {..    /// 
-000003d0: 7175 6572 7920 666f 7220 6120 7369 6e67  query for a sing
-000003e0: 6c65 2070 7974 686f 6e20 7061 636b 6167  le python packag
-000003f0: 650d 0a20 2020 2050 6163 6b61 6765 207b  e..    Package {
-00000400: 0d0a 2020 2020 2020 2020 2f2f 2f20 6e61  ..        /// na
-00000410: 6d65 206f 6620 7468 6520 7061 636b 6167  me of the packag
-00000420: 650d 0a20 2020 2020 2020 2023 5b61 7267  e..        #[arg
-00000430: 286c 6f6e 672c 7368 6f72 7429 5d0d 0a20  (long,short)].. 
-00000440: 2020 2020 2020 206e 616d 653a 2053 7472         name: Str
-00000450: 696e 672c 0d0a 0d0a 2020 2020 2020 2020  ing,....        
-00000460: 2f2f 2f20 7665 7273 696f 6e20 6f66 2074  /// version of t
-00000470: 6865 2070 6163 6b61 6765 2028 6966 206e  he package (if n
-00000480: 6f74 2070 726f 7669 6465 642c 2074 6865  ot provided, the
-00000490: 206c 6174 6573 7420 7374 6162 6c65 2077   latest stable w
-000004a0: 696c 6c20 6265 2075 7365 6429 0d0a 2020  ill be used)..  
-000004b0: 2020 2020 2020 235b 6172 6728 6c6f 6e67        #[arg(long
-000004c0: 2c20 7368 6f72 742c 2064 6566 6175 6c74  , short, default
-000004d0: 5f76 616c 7565 3d4e 6f6e 6529 5d0d 0a20  _value=None)].. 
-000004e0: 2020 2020 2020 2076 6572 7369 6f6e 3a20         version: 
-000004f0: 4f70 7469 6f6e 3c53 7472 696e 673e 0d0a  Option<String>..
-00000500: 2020 2020 7d0d 0a7d 0d0a 0d0a 666e 206d      }..}....fn m
-00000510: 6169 6e28 2920 7b0d 0a20 2020 206c 6574  ain() {..    let
-00000520: 2061 7267 7320 3d20 436c 693a 3a70 6172   args = Cli::par
-00000530: 7365 2829 3b0d 0a0d 0a20 2020 206d 6174  se();....    mat
-00000540: 6368 2061 7267 732e 7061 636b 6167 6520  ch args.package 
-00000550: 7b0d 0a20 2020 2020 2020 202f 2f20 7375  {..        // su
-00000560: 6263 6f6d 6d61 6e64 2070 6163 6b61 6765  bcommand package
-00000570: 0d0a 0d0a 2020 2020 2020 2020 536f 6d65  ....        Some
-00000580: 2853 7562 436f 6d6d 616e 643a 3a50 6163  (SubCommand::Pac
-00000590: 6b61 6765 207b 206e 616d 652c 2076 6572  kage { name, ver
-000005a0: 7369 6f6e 207d 2920 3d3e 207b 0d0a 2020  sion }) => {..  
-000005b0: 2020 2020 2020 2020 2020 6c65 7420 6f73            let os
-000005c0: 7620 3d20 4f73 763a 3a6e 6577 2829 2e65  v = Osv::new().e
-000005d0: 7870 6563 7428 2243 616e 6e6f 7420 6163  xpect("Cannot ac
-000005e0: 6365 7373 2074 6865 2041 5049 2074 6f20  cess the API to 
-000005f0: 6765 7420 7468 6520 6c61 7465 7374 2070  get the latest p
-00000600: 6163 6b61 6765 2076 6572 7369 6f6e 2e22  ackage version."
-00000610: 293b 0d0a 2020 2020 2020 2020 2020 2020  );..            
-00000620: 6c65 7420 7665 7273 696f 6e20 3d20 6966  let version = if
-00000630: 206c 6574 2053 6f6d 6528 7629 203d 2076   let Some(v) = v
-00000640: 6572 7369 6f6e 207b 767d 2065 6c73 6520  ersion {v} else 
-00000650: 7b6f 7376 2e67 6574 5f6c 6174 6573 745f  {osv.get_latest_
-00000660: 7061 636b 6167 655f 7665 7273 696f 6e28  package_version(
-00000670: 6e61 6d65 2e63 6c6f 6e65 2829 290d 0a20  name.clone()).. 
-00000680: 2020 2020 2020 2020 2020 202e 6578 7065             .expe
-00000690: 6374 2822 4572 726f 7220 696e 2072 6574  ct("Error in ret
-000006a0: 7269 7669 6e67 2073 7461 626c 6520 7665  riving stable ve
-000006b0: 7273 696f 6e20 6672 6f6d 2041 5049 2229  rsion from API")
-000006c0: 7d3b 0d0a 0d0a 2020 2020 2020 2020 2020  };....          
-000006d0: 2020 6c65 7420 6465 7020 3d20 4465 7065    let dep = Depe
-000006e0: 6e64 656e 6379 207b 6e61 6d65 3a20 6e61  ndency {name: na
-000006f0: 6d65 2c20 7665 7273 696f 6e3a 2053 6f6d  me, version: Som
-00000700: 6528 7665 7273 696f 6e29 2c20 636f 6d70  e(version), comp
-00000710: 6172 6174 6f72 3a20 4e6f 6e65 7d3b 0d0a  arator: None};..
-00000720: 2020 2020 2020 2020 2020 2020 2f2f 2073              // s
-00000730: 7461 7274 2829 2066 726f 6d20 7363 616e  tart() from scan
-00000740: 6e65 7220 6f6e 6c79 2061 6363 6570 7473  ner only accepts
-00000750: 2056 6563 3c44 6570 656e 6465 6e63 793e   Vec<Dependency>
-00000760: 2073 6f0d 0a20 2020 2020 2020 2020 2020   so..           
-00000770: 206c 6574 2076 6465 7020 3d20 7665 6321   let vdep = vec!
-00000780: 5b64 6570 5d3b 0d0a 0d0a 2020 2020 2020  [dep];....      
-00000790: 2020 2020 2020 6c65 7420 5f72 6573 203d        let _res =
-000007a0: 2073 6361 6e6e 6572 3a3a 7374 6172 7428   scanner::start(
-000007b0: 7664 6570 293b 0d0a 2020 2020 2020 2020  vdep);..        
-000007c0: 2020 2020 6578 6974 2830 290d 0a0d 0a20      exit(0).... 
-000007d0: 2020 2020 2020 207d 2c0d 0a20 2020 2020         },..     
-000007e0: 2020 204e 6f6e 6520 3d3e 2028 290d 0a20     None => ().. 
-000007f0: 2020 207d 0d0a 0d0a 2020 2020 7072 696e     }....    prin
-00000800: 746c 6e21 2822 7079 7363 616e 2076 7b7d  tln!("pyscan v{}
-00000810: 207c 2062 7920 4173 7769 6e20 2867 6974   | by Aswin (git
-00000820: 6875 622e 636f 6d2f 6173 7769 6e6e 6e6e  hub.com/aswinnnn
-00000830: 2922 2c20 6765 745f 7665 7273 696f 6e28  )", get_version(
-00000840: 2929 3b20 2020 200d 0a20 2020 202f 2f20  ));    ..    // 
-00000850: 7072 696e 746c 6e21 2822 7b3a 3f7d 222c  println!("{:?}",
-00000860: 2061 7267 7329 3b0d 0a0d 0a20 2020 202f   args);....    /
-00000870: 2f20 2d2d 2d20 6769 7669 6e67 2063 6f6e  / --- giving con
-00000880: 7472 6f6c 2074 6f20 7061 7273 6572 2073  trol to parser s
-00000890: 7461 7274 7320 6865 7265 202d 2d2d 0d0a  tarts here ---..
-000008a0: 0d0a 2020 2020 2f2f 2069 6620 6120 6469  ..    // if a di
-000008b0: 7265 6374 6f72 7920 7061 7468 2069 7320  rectory path is 
-000008c0: 7072 6f76 6964 6564 0d0a 2020 2020 6966  provided..    if
-000008d0: 206c 6574 2053 6f6d 6528 6469 7229 203d   let Some(dir) =
-000008e0: 2061 7267 732e 6469 7220 7b20 7061 7273   args.dir { pars
-000008f0: 6572 3a3a 7363 616e 5f64 6972 2864 6972  er::scan_dir(dir
-00000900: 2e61 735f 7061 7468 2829 2920 7d20 0d0a  .as_path()) } ..
-00000910: 0d0a 2020 2020 2f2f 2069 6620 6e6f 742c  ..    // if not,
-00000920: 2075 7365 2063 7764 0d0a 2020 2020 656c   use cwd..    el
-00000930: 7365 2069 6620 6c65 7420 4f6b 2864 6972  se if let Ok(dir
-00000940: 2920 3d20 656e 763a 3a63 7572 7265 6e74  ) = env::current
-00000950: 5f64 6972 2829 207b 2070 6172 7365 723a  _dir() { parser:
-00000960: 3a73 6361 6e5f 6469 7228 6469 722e 6173  :scan_dir(dir.as
-00000970: 5f70 6174 6828 2929 207d 200d 0a20 2020  _path()) } ..   
-00000980: 2065 6c73 6520 7b65 7072 696e 746c 6e21   else {eprintln!
-00000990: 2822 7468 6520 6769 7665 6e20 6469 7265  ("the given dire
-000009a0: 6374 6f72 7920 6973 2065 6d70 7479 2e22  ctory is empty."
-000009b0: 297d 3b20 2f2f 2065 7272 2077 6865 6e20  )}; // err when 
-000009c0: 6469 7220 6973 2065 6d70 7479 0d0a 0d0a  dir is empty....
-000009d0: 0d0a 0d0a 7d                             ....}
+00000000: 2f2f 2f20 666f 7220 7468 6520 7061 7273  /// for the pars
+00000010: 6572 206d 6f64 756c 652c 2065 7874 7261  er module, extra
+00000020: 6374 6f72 2e72 7320 6973 2074 6865 2062  ctor.rs is the b
+00000030: 6163 6b62 6f6e 6520 6f66 2061 6c6c 2070  ackbone of all p
+00000040: 6172 7369 6e67 0d0a 2f2f 2f20 6974 2074  arsing../// it t
+00000050: 616b 6573 2061 2053 7472 696e 6720 616e  akes a String an
+00000060: 6420 6120 6d75 7461 626c 6520 7265 6665  d a mutable refe
+00000070: 7265 6e63 6520 746f 2061 2056 6563 3c44  rence to a Vec<D
+00000080: 6570 656e 6465 6e63 793e 2e0d 0a2f 2f2f  ependency>...///
+00000090: 2053 7472 696e 6720 6973 2074 6865 2063   String is the c
+000000a0: 6f6e 7465 6e74 7320 6f66 2061 2073 6f75  ontents of a sou
+000000b0: 7263 6520 6669 6c65 2c20 7768 696c 6520  rce file, while 
+000000c0: 7468 6520 6d75 7420 7265 6620 7665 6374  the mut ref vect
+000000d0: 6f72 2077 696c 6c0d 0a2f 2f2f 2062 6520  or will../// be 
+000000e0: 7573 6564 2074 6f20 636f 6c6c 6563 7420  used to collect 
+000000f0: 7468 6520 6465 7065 6e64 656e 6369 6573  the dependencies
+00000100: 2074 6861 7420 7765 2068 6176 6520 6578   that we have ex
+00000110: 7472 6163 7465 6420 6672 6f6d 2074 6865  tracted from the
+00000120: 2063 6f6e 7465 6e74 732e 0d0a 0d0a 7573   contents.....us
+00000130: 6520 6c61 7a79 5f73 7461 7469 633a 3a6c  e lazy_static::l
+00000140: 617a 795f 7374 6174 6963 3b0d 0a75 7365  azy_static;..use
+00000150: 2072 6567 6578 3a3a 5265 6765 783b 0d0a   regex::Regex;..
+00000160: 7573 6520 7065 705f 3530 383a 3a7b 7365  use pep_508::{se
+00000170: 6c66 2c20 5370 6563 7d3b 0d0a 7573 6520  lf, Spec};..use 
+00000180: 7375 7065 723a 3a73 7472 7563 7473 3a3a  super::structs::
+00000190: 7b44 6570 656e 6465 6e63 797d 3b0d 0a75  {Dependency};..u
+000001a0: 7365 2074 6f6d 6c3a 3a54 6162 6c65 3b0d  se toml::Table;.
+000001b0: 0a0d 0a70 7562 2066 6e20 6578 7472 6163  ...pub fn extrac
+000001c0: 745f 696d 706f 7274 735f 7079 7468 6f6e  t_imports_python
+000001d0: 2874 6578 743a 2053 7472 696e 672c 2069  (text: String, i
+000001e0: 6d70 3a20 266d 7574 2056 6563 3c44 6570  mp: &mut Vec<Dep
+000001f0: 656e 6465 6e63 793e 2920 7b0d 0a20 2020  endency>) {..   
+00000200: 206c 617a 795f 7374 6174 6963 2120 7b0d   lazy_static! {.
+00000210: 0a20 2020 2020 2020 2073 7461 7469 6320  .        static 
+00000220: 7265 6620 494d 504f 5254 5f52 4547 4558  ref IMPORT_REGEX
+00000230: 203a 2052 6567 6578 203d 2052 6567 6578   : Regex = Regex
+00000240: 3a3a 6e65 7728 0d0a 2020 2020 2020 2020  ::new(..        
+00000250: 2020 2020 2020 2020 7222 5e5c 732a 283f          r"^\s*(?
+00000260: 3a66 726f 6d7c 696d 706f 7274 295c 732b  :from|import)\s+
+00000270: 285c 772b 283f 3a5c 732a 2c5c 732a 5c77  (\w+(?:\s*,\s*\w
+00000280: 2b29 2a29 220d 0a20 2020 2020 2020 2020  +)*)"..         
+00000290: 2020 2029 2e75 6e77 7261 7028 293b 0d0a     ).unwrap();..
+000002a0: 2020 2020 7d0d 0a0d 0a20 2020 2066 6f72      }....    for
+000002b0: 2078 2069 6e20 494d 504f 5254 5f52 4547   x in IMPORT_REG
+000002c0: 4558 2e66 696e 645f 6974 6572 2826 7465  EX.find_iter(&te
+000002d0: 7874 2920 7b0d 0a20 2020 2020 2020 206c  xt) {..        l
+000002e0: 6574 206d 6174 203d 2078 2e61 735f 7374  et mat = x.as_st
+000002f0: 7228 292e 746f 5f73 7472 696e 6728 293b  r().to_string();
+00000300: 0d0a 2020 2020 2020 2020 6c65 7420 6d61  ..        let ma
+00000310: 7420 3d20 6d61 742e 7265 706c 6163 656e  t = mat.replacen
+00000320: 2822 696d 706f 7274 222c 2022 222c 2031  ("import", "", 1
+00000330: 292e 7472 696d 2829 2e74 6f5f 7374 7269  ).trim().to_stri
+00000340: 6e67 2829 3b0d 0a0d 0a20 2020 2020 2020  ng();....       
+00000350: 2069 6d70 2e70 7573 6828 4465 7065 6e64   imp.push(Depend
+00000360: 656e 6379 207b 206e 616d 653a 206d 6174  ency { name: mat
+00000370: 2c20 7665 7273 696f 6e3a 204e 6f6e 652c  , version: None,
+00000380: 2063 6f6d 7061 7261 746f 723a 204e 6f6e   comparator: Non
+00000390: 6520 7d29 0d0a 0d0a 2020 2020 7d0d 0a7d  e })....    }..}
+000003a0: 0d0a 0d0a 7075 6220 666e 2065 7874 7261  ....pub fn extra
+000003b0: 6374 5f69 6d70 6f72 7473 5f72 6571 7328  ct_imports_reqs(
+000003c0: 7465 7874 3a20 5374 7269 6e67 2c20 696d  text: String, im
+000003d0: 703a 2026 6d75 7420 5665 633c 4465 7065  p: &mut Vec<Depe
+000003e0: 6e64 656e 6379 3e29 207b 0d0a 2020 2020  ndency>) {..    
+000003f0: 2f2f 2072 6571 7569 7265 6d65 6e74 732e  // requirements.
+00000400: 7478 7420 7573 6573 2061 2050 4550 2035  txt uses a PEP 5
+00000410: 3038 2070 6172 7365 7220 746f 2070 6172  08 parser to par
+00000420: 7365 2064 6570 656e 6465 6e63 6965 7320  se dependencies 
+00000430: 6163 636f 7264 696e 676c 790d 0a20 2020  accordingly..   
+00000440: 202f 2f20 796f 7520 6d69 6768 7420 7468   // you might th
+00000450: 696e 6b20 6974 7320 6a75 7374 2061 2074  ink its just a t
+00000460: 6578 7420 6669 6c65 2c20 6275 7420 4927  ext file, but I'
+00000470: 6d20 676f 6e6e 6120 6465 636c 696e 6520  m gonna decline 
+00000480: 7265 696e 7665 6e74 696e 6720 7468 6520  reinventing the 
+00000490: 7768 6565 6c0d 0a20 2020 202f 2f20 6a75  wheel..    // ju
+000004a0: 7374 2074 6f20 7061 7273 6520 2272 6571  st to parse "req
+000004b0: 7565 7374 7320 3e3d 2032 2e30 2e38 220d  uests >= 2.0.8".
+000004c0: 0a20 2020 200d 0a20 2020 206c 6574 2070  .    ..    let p
+000004d0: 6172 7365 6420 3d20 7065 705f 3530 383a  arsed = pep_508:
+000004e0: 3a70 6172 7365 2874 6578 742e 6173 5f73  :parse(text.as_s
+000004f0: 7472 2829 293b 0d0a 0d0a 2020 2020 6966  tr());....    if
+00000500: 2020 6c65 7420 4f6b 2864 6570 2920 3d20    let Ok(dep) = 
+00000510: 7061 7273 6564 207b 0d0a 2020 2020 2020  parsed {..      
+00000520: 2020 6c65 7420 646e 616d 6520 3d20 6465    let dname = de
+00000530: 702e 6e61 6d65 2e74 6f5f 7374 7269 6e67  p.name.to_string
+00000540: 2829 3b0d 0a20 2020 2020 2020 202f 2f20  ();..        // 
+00000550: 7072 696e 746c 6e21 2822 7b3a 3f7d 222c  println!("{:?}",
+00000560: 2064 6570 2e63 6c6f 6e65 2829 293b 0d0a   dep.clone());..
+00000570: 2020 2020 2020 2020 6966 206c 6574 2053          if let S
+00000580: 6f6d 6528 7665 7229 203d 2064 6570 2e73  ome(ver) = dep.s
+00000590: 7065 6320 7b0d 0a20 2020 2020 2020 2020  pec {..         
+000005a0: 2020 2069 6620 6c65 7420 5370 6563 3a3a     if let Spec::
+000005b0: 5665 7273 696f 6e28 7665 7273 7065 6329  Version(verspec)
+000005c0: 203d 2076 6572 207b 0d0a 2020 2020 2020   = ver {..      
+000005d0: 2020 2020 2020 2020 2020 666f 7220 7620            for v 
+000005e0: 696e 2076 6572 7370 6563 207b 0d0a 2020  in verspec {..  
+000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000600: 2020 2f2f 2070 7973 6361 6e20 6f6e 6c79    // pyscan only
+00000610: 2074 616b 6573 2074 6865 2066 6972 7374   takes the first
+00000620: 2076 6572 7369 6f6e 2073 7065 6320 666f   version spec fo
+00000630: 756e 6420 666f 7220 7468 6520 6465 7065  und for the depe
+00000640: 6e64 656e 6379 0d0a 2020 2020 2020 2020  ndency..        
+00000650: 2020 2020 2020 2020 2020 2020 2f2f 2066              // f
+00000660: 6f72 206e 6f77 2e0d 0a20 2020 2020 2020  or now...       
+00000670: 2020 2020 2020 2020 2020 2020 206c 6574               let
+00000680: 2076 6572 7369 6f6e 203d 2076 2e76 6572   version = v.ver
+00000690: 7369 6f6e 2e74 6f5f 7374 7269 6e67 2829  sion.to_string()
+000006a0: 3b0d 0a20 2020 2020 2020 2020 2020 2020  ;..             
+000006b0: 2020 2020 2020 206c 6574 2063 6f6d 7061         let compa
+000006c0: 7261 746f 7220 3d20 762e 636f 6d70 6172  rator = v.compar
+000006d0: 6174 6f72 3b0d 0a20 2020 2020 2020 2020  ator;..         
+000006e0: 2020 2020 2020 2020 2020 2069 6d70 2e70             imp.p
+000006f0: 7573 6828 4465 7065 6e64 656e 6379 7b6e  ush(Dependency{n
+00000700: 616d 653a 2064 6e61 6d65 2c20 7665 7273  ame: dname, vers
+00000710: 696f 6e3a 2053 6f6d 6528 7665 7273 696f  ion: Some(versio
+00000720: 6e29 2c20 636f 6d70 6172 6174 6f72 3a20  n), comparator: 
+00000730: 536f 6d65 2863 6f6d 7061 7261 746f 7229  Some(comparator)
+00000740: 7d29 3b0d 0a20 2020 2020 2020 2020 2020  });..           
+00000750: 2020 2020 2020 2020 2062 7265 616b 3b0d           break;.
+00000760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000770: 207d 0d0a 2020 2020 2020 2020 2020 2020   }..            
+00000780: 7d0d 0a20 2020 2020 2020 207d 0d0a 2020  }..        }..  
+00000790: 2020 2020 2020 656c 7365 207b 0d0a 2020        else {..  
+000007a0: 2020 2020 2020 2020 2020 696d 702e 7075            imp.pu
+000007b0: 7368 2844 6570 656e 6465 6e63 797b 6e61  sh(Dependency{na
+000007c0: 6d65 3a20 646e 616d 652c 2076 6572 7369  me: dname, versi
+000007d0: 6f6e 3a20 4e6f 6e65 2c20 636f 6d70 6172  on: None, compar
+000007e0: 6174 6f72 3a20 4e6f 6e65 7d29 3b0d 0a20  ator: None});.. 
+000007f0: 2020 2020 2020 207d 0d0a 2020 2020 7d0d         }..    }.
+00000800: 0a0d 0a20 2020 200d 0a7d 0d0a 0d0a 7075  ...    ..}....pu
+00000810: 6220 666e 2065 7874 7261 6374 5f69 6d70  b fn extract_imp
+00000820: 6f72 7473 5f70 7970 726f 6a65 6374 2866  orts_pyproject(f
+00000830: 3a20 5374 7269 6e67 2c20 696d 703a 2026  : String, imp: &
+00000840: 6d75 7420 5665 633c 4465 7065 6e64 656e  mut Vec<Dependen
+00000850: 6379 3e29 207b 0d0a 2020 2020 6c65 7420  cy>) {..    let 
+00000860: 7061 7273 6564 203d 2066 2e70 6172 7365  parsed = f.parse
+00000870: 3a3a 3c54 6162 6c65 3e28 293b 0d0a 2020  ::<Table>();..  
+00000880: 2020 6966 206c 6574 204f 6b28 7061 7273    if let Ok(pars
+00000890: 6564 2920 3d20 7061 7273 6564 207b 0d0a  ed) = parsed {..
+000008a0: 2020 2020 2020 2020 6c65 7420 7072 6f6a          let proj
+000008b0: 6563 7420 3d20 2670 6172 7365 645b 2270  ect = &parsed["p
+000008c0: 726f 6a65 6374 225d 3b0d 0a20 2020 2020  roject"];..     
+000008d0: 2020 206c 6574 2064 6570 7320 3d20 2670     let deps = &p
+000008e0: 726f 6a65 6374 5b22 6465 7065 6e64 656e  roject["dependen
+000008f0: 6369 6573 225d 3b0d 0a20 2020 2020 2020  cies"];..       
+00000900: 206c 6574 2064 6570 7320 3d20 6465 7073   let deps = deps
+00000910: 2e61 735f 6172 7261 7928 290d 0a20 2020  .as_array()..   
+00000920: 2020 2020 202e 6578 7065 6374 2822 436f       .expect("Co
+00000930: 756c 6420 6e6f 7420 6669 6e64 2074 6865  uld not find the
+00000940: 2064 6570 656e 6465 6e63 6965 7320 7461   dependencies ta
+00000950: 626c 6520 696e 2079 6f75 7220 7079 7072  ble in your pypr
+00000960: 6f6a 6563 742e 746f 6d6c 2229 3b0d 0a20  oject.toml");.. 
+00000970: 2020 2020 2020 2066 6f72 2064 2069 6e20         for d in 
+00000980: 6465 7073 207b 0d0a 2020 2020 2020 2020  deps {..        
+00000990: 2020 2020 6c65 7420 6420 3d20 642e 6173      let d = d.as
+000009a0: 5f73 7472 2829 2e75 6e77 7261 7028 292e  _str().unwrap().
+000009b0: 746f 5f73 7472 696e 6728 293b 0d0a 2020  to_string();..  
+000009c0: 2020 2020 2020 2020 2020 696d 702e 7075            imp.pu
+000009d0: 7368 2844 6570 656e 6465 6e63 7920 7b20  sh(Dependency { 
+000009e0: 6e61 6d65 3a20 642c 2076 6572 7369 6f6e  name: d, version
+000009f0: 3a20 4e6f 6e65 2c20 636f 6d70 6172 6174  : None, comparat
+00000a00: 6f72 3a20 4e6f 6e65 207d 290d 0a0d 0a20  or: None }).... 
+00000a10: 2020 2020 2020 207d 0d0a 2020 2020 7d0d         }..    }.
+00000a20: 0a7d                                     .}
```

### Comparing `pyscan_rs-0.1.1/src/parser/mod.rs` & `pyscan_rs-0.1.2/src/parser/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 use std::io::{BufReader, BufRead};
 use std::{ffi::OsString, fs::File};
-/// ^\s*(?:from|import)\s+(\w+(?:\s*,\s*\w+)*)
-/// regex used to match imports from python filesr
 use std::fs;
 use std::path::Path;
 pub mod structs;
 mod extractor;
 use super::scanner;
 use structs::{FoundFile, FileTypes, FoundFileResult};
 
@@ -26,24 +24,24 @@
                         name: filename,
                         filetype: FileTypes::Python,
                         path: OsString::from(entry.path())
                     });
                     result.python();
                 }
                 // requirements.txt
-                else if OsString::from("requirements.txt") == filename.clone() {
+                else if *"requirements.txt" == filename.clone() {
                     result.add(FoundFile {
                         name: filename,
                         filetype: FileTypes::Requirements,
                         path: OsString::from(entry.path())
                     });
                     result.reqs();
                 }
                 // pyproject.toml
-                else if OsString::from("pyproject.toml") == filename.clone() {
+                else if *"pyproject.toml" == filename.clone() {
                     result.add(FoundFile {
                         name: filename,
                         filetype: FileTypes::Pyproject,
                         path: OsString::from(entry.path())
                     });
                     result.pyproject();
                 } 
@@ -70,22 +68,20 @@
         // if both reqs and pyproject is present, go for reqs first
         find_reqs_imports(&files)
     }
     else if res.pyproject_found != 0 {
         // use pyproject instead (if it exists)
         find_pyproject_imports(&files)
     }
+    else if res.py_found != 0 {
+        // make sure theres atleast one python file, then use that
+        find_python_imports(&files)
+    }
     else {
-        if res.py_found != 0 {
-            // make sure theres atleast one python file, then use that
-            find_python_imports(&files)
-        }
-        else {
-            eprintln!("Could not find any requirements.txt, pyproject.toml or python files in this directory");
-        }
+        eprintln!("Could not find any requirements.txt, pyproject.toml or python files in this directory");
     }
 }
 
 fn find_python_imports(f: &Vec<FoundFile>) {
     let cons = console::Term::stdout();
     cons.write_line("Using python file as source...").unwrap();
```

### Comparing `pyscan_rs-0.1.1/src/parser/structs.rs` & `pyscan_rs-0.1.2/src/parser/structs.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 use std::{ffi::OsString};
 use super::scanner::models::Vulnerability;
 
 // struct Python;
 // struct Requirements;
 // struct Pyproject;
 
-#[derive(Debug, PartialEq, Clone)]
+#[derive(Debug, PartialEq, Eq, Clone)]
 pub enum FileTypes {
     Python,
     Requirements,
     Pyproject
 }
 
 #[derive(Debug, Clone)]
```

### Comparing `pyscan_rs-0.1.1/src/scanner/api.rs` & `pyscan_rs-0.1.2/src/scanner/api.rs`

 * *Files 3% similar despite different names*

```diff
@@ -41,27 +41,21 @@
 
     }
 
     pub fn query(&self, d: Dependency) -> Option<Vulnerability> {
         // returns None if no vulns found
         // else Some(Vulnerability)
 
-        let version = if d.version != None {d.version} else {self.get_latest_package_version(d.name.clone())};
+        let version = if d.version.is_some() {d.version} else {self.get_latest_package_version(d.name.clone())};
         // println!("{:?}", self.get_latest_package_version(d.name.clone()));
 
         let res = self.get_json(d.name.as_str(), &version.unwrap());
         // println!("{:?}", res);
 
-        if let Some(v) = res {
-            // println!("{:?}", v);
-            Some(v)
-        }
-        else {
-            None
-        }
+        res
 
     }
 
     pub fn get_json(&self, name: &str, version: &str) -> Option<Vulnerability> {
         let url = r"https://api.osv.dev/v1/query";
 
         let body = format!("{{\"version\": \"{}\",\"package\": {{\"name\": \"{}\", \"ecosystem\":\"PyPI\"}}}}",version, name);
@@ -71,15 +65,15 @@
         let res = self.client.request(Method::POST, url).body(body).send();
 
         // println!("{:?}", res);
 
         if let Ok(response) = res {
             if response.status().is_client_error() {eprintln!("Failed connecting to OSV. [Client error]")} else if response.status().is_server_error() {eprintln!("Failed connecting to OSV. [Server error]")}
             let restext = response.text().unwrap();
-            if restext.clone().len() > 3 {}
+            if restext.len() > 3 {}
             // check if vulns exist by char len of json
             // api returns '{}' if none found so this is easy
 
             let parsed: Result<Vulnerability, serde_json::Error> = serde_json::from_str(&restext);
             // println!("{:?}", parsed);
             if let Ok(v) = parsed {
                 Some(v)
@@ -92,15 +86,15 @@
         else {
             eprintln!("Could not fetch a response from osv.dev"); None
         }
 
 
     }
     pub fn get_latest_package_version(&self, n: String) -> Option<String> {
-        let url = format!("https://api.deps.dev/v3alpha/systems/pypi/packages/{}", n.clone());
+        let url = format!("https://api.deps.dev/v3alpha/systems/pypi/packages/{}", n);
         // gets the latest released version of a package from pypi.
     
         let res = self.client.get(url).send();
 
         // println!("{:?}", res.unwrap().text());
         // Some("l".to_string())
 
@@ -111,24 +105,24 @@
                 // println!("{:?}", pypi);
                 // Some("()".to_string())
                 if let Some(v) = pypi.versions.iter().last().cloned() {
                     let s = v.iter().last().unwrap().to_owned().version_key.unwrap().version;
                     Some(s)
                 }
                 else {
-                    eprintln!("Could not identify the latest version of the package {}. Please add the version specification to your source and try again.", n.clone());
+                    eprintln!("Could not identify the latest version of the package {}. Please add the version specification to your source and try again.", n);
                     None
                 }
             }
             else {
-                eprintln!("There was a problem finding the latest version of {}. Either it does not exist or the API cannot identify the latest version. Please provide a version specification in your source instead.", n.clone());
+                eprintln!("There was a problem finding the latest version of {}. Either it does not exist or the API cannot identify the latest version. Please provide a version specification in your source instead.", n);
                 None
             }
         }
         else {
-            eprintln!("Could not reach the pypi API to fetch the latest version of {}. Please provide a version specification in your source.", n.clone());
+            eprintln!("Could not reach the pypi API to fetch the latest version of {}. Please provide a version specification in your source.", n);
             None
         }
 
     }
 }
```

### Comparing `pyscan_rs-0.1.1/src/scanner/mod.rs` & `pyscan_rs-0.1.2/src/utils.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,109 +1,141 @@
-pub mod api;
-pub mod models;
-use std::process::exit;
-
-use crate::parser::structs::ScannedDependency;
-
-use super::parser::structs::Dependency;
-use console::{Term, style};
-
-pub fn start(imports: Vec<Dependency>) -> Result<(), std::io::Error> {
-    let cons = Term::stdout();
-    let s = format!("Found {} dependencies...", style(format!("{}", imports.len()))
-    .bold()
-    .green());
-
-    cons.write_line(&s)?;
-
-    let osv = api::Osv::new().unwrap(); // err handling done inside, unwrapping is safe
-    let mut collected: Vec<ScannedDependency> = Vec::new();
-
-    for mut d in imports {
-        // check if version was provided
-        d.version = if let Some(provided) = d.version {
-            Some(provided)
-        }
-        else {
-            osv.get_latest_package_version(d.name.clone())
-        };
-        let mut depstr = format!("|-| {} [{}]", style(d.name.clone()).bold().bright().yellow(), style(d.version.clone().unwrap().to_string()).bold().dim());
-        cons.write_line(&depstr)?;
-
-        let res = osv.query(d.clone());
-        if let Some(v) = res {
-            depstr.push_str(
-                format!("{}", style(" -> Found vulnerabilities!").bold().bright().red()).as_str()
-            );
-            cons.clear_last_lines(1)?;
-            cons.write_line(&depstr)?;
-            collected.push(ScannedDependency { name:  d.name, version: d.version.unwrap(), vuln: v });
 
-        }
-        else {
-            depstr.push_str(
-                format!("{}", style(" -> No vulnerabilities found.").bold().bright().green()).as_str()
-            );
-            cons.clear_last_lines(1)?;
-            cons.write_line(&depstr)?;
-        }
+use chrono::{Timelike, Utc};
+use reqwest::{
+    self,
+    blocking::{Response},
+    Method,
+};
+use crate::scanner::models::Pypi;
+
+pub fn get_time() -> String {
+    // get the current time in a stting format i like.
+    let now = Utc::now();
+    let (is_pm, hour) = now.hour12();
+    {
+        let time = format!(
+            "{:02}:{:02}:{:02} {}",
+            hour,
+            now.minute(),
+            now.second(),
+            if is_pm { "PM" } else { "AM" }
+        );
 
+        time
     }
+}
 
-    // --- summary starts here ---
+pub fn get_version() -> String {
+    "0.1.1".to_string()
+}
 
-    if collected.len() != 0 {
-        cons.write_line(&format!("{}", style("SUMMARY").bold().yellow().underlined()).to_string())?;
-        for v in collected {
-    
-    
-                for vuln in v.vuln.vulns {
-    
-                    let name = format!("Dependency: {}", style(v.name.clone()).bold().bright().red());
-                    let id = format!("ID: {}",style(vuln.id).bold().bright().yellow());
-                    let details = format!("Details: {}", style(vuln.details).italic());
-                    // let summary = format!("summary: {}", vuln.summary);
-                    let vers: Vec<Vec<String>> = vuln.affected.iter().map(|affected| {vec![affected.versions.first().unwrap().to_string(), affected.versions.last().unwrap().to_string()]}).collect();
-                    let version = format!("Versions affected: {} to {}", style(vers.first().expect("No version found affected").first().unwrap()).dim().underlined(), style(vers.last().expect("No version found affected").last().unwrap()).dim().underlined());
-                    print!("\n");
-    
-    
-                    cons.write_line(name.as_str())?;
-                    cons.write_line(id.as_str())?;
-                    cons.write_line(details.as_str())?;
-                    cons.write_line(version.as_str())?;
-    
-                }
-    
+pub fn reqwest_send(method: &str, url: String) -> Option<Response> {
+    let client = reqwest::blocking::Client::builder()
+        .user_agent(format!("pyscan v{}", get_version()))
+        .build();
+
+    if let Ok(client) = client {
+        let method = match method {
+            "get" => Method::GET,
+            "post" => Method::POST,
+            "put" => Method::PUT,
+            "head" => Method::HEAD,
+            "connect" => Method::CONNECT,
+            "trace" => Method::TRACE,
+            &_ => {
+                println!("Didn't recognize that method so defaulting to GET");
+                Method::GET
             }
+        };
+        let res = client.request(method, url).send();
+
+        if let Ok(success) = res {
+            Some(success)
+        } else {
+            eprintln!(
+                "Could not establish an internet connection. Check your internet or try again."
+            );
+            None
+        }
+    } else {
+        eprintln!("Could not build the network client. Report this at https://github.com/aswinnnn/pyscan/issues");
+        None
     }
-    else { exit(0)}
-    
-    Ok(())
 }
 
+pub fn get_latest_package_version(name: String) -> Option<String> {
+    let url = format!(
+        "https://api.deps.dev/v3alpha/systems/pypi/packages/{}",
+        name
+    );
+    // gets the latest released version of a package from pypi.
+
+    let res = reqwest_send("get", url);
+
+    // println!("{:?}", res.unwrap().text());
+    // Some("l".to_string())
+
+    if let Some(response) = res {
+        let parsed: Result<Pypi, serde_json::Error> =
+            serde_json::from_str(response.text().unwrap().as_str());
+
+        if let Ok(pypi) = parsed {
+            // println!("{:?}", pypi);
+            // Some("()".to_string())
+            if let Some(v) = pypi.versions.iter().last().cloned() {
+                let s = v
+                    .iter()
+                    .last()
+                    .unwrap()
+                    .to_owned()
+                    .version_key
+                    .unwrap()
+                    .version;
+                Some(s)
+            } else {
+                eprintln!("Could not identify the latest version of the package {}. Please add the version specification to your source and try again.", name);
+                None
+            }
+        } else {
+            eprintln!("There was a problem finding the latest version of {}. Either it does not exist or the API cannot identify the latest version. Please provide a version specification in your source instead.", name);
+            None
+        }
+    } else {
+        eprintln!("Could not reach the pypi API to fetch the latest version of {}. Please provide a version specification in your source.", name);
+        None
+    }
+}
 
-// more rigourous version checking against the input might be needed in the future
-// function commented out due to being experimental
-// fn version_check(against: ScannedDependency) -> bool {
-//     // Check input version against the affected versions
-//     // from OSV. Would osv return a vuln that doesnt have our version? idk
-//     // but im not gonna fear-monger the user. Lets make sure. 
-//     let mut check = false;
-//     let vulns = against.vuln.vulns;
-//     let ver = against.version;
-
-//     for vuln in vulns {
-//         let multi_affected = vuln.affected.iter().map(|x| {x.clone().versions}); // multi-dimensional array of versions
-//         let pre_single_affected: Vec<Vec<String>> = multi_affected.map(|v| {v}).collect(); // processing it
-//         let single_affected: Vec<String> = pre_single_affected.iter().map(|x| {x.to_owned().drain(..x.len()).collect()}).collect(); // yay single array of versions
-
-//         for a in single_affected {
-//             if ver == a {
-//                 check = true
-//             }
-//             else {continue}
-//         }
-//     }
+use std::process::Command;
+// Define a custom error type that wraps a String message
+#[derive(Debug)]
+pub struct PipError(String);
+
+// Implement the std::error::Error trait for DockerError
+impl std::error::Error for PipError {}
+
+// Implement the std::fmt::Display trait for DockerError
+impl std::fmt::Display for PipError {
+    fn fmt(&self, f: &mut std::fmt::Formatter) -> std::fmt::Result {
+        write!(f, "Pip error: {}", self.0)
+    }
+}
 
-//     check
-// }
+pub fn get_python_package_version(package: &str) -> Result<String, PipError> {
+    
+    let output = Command::new("pip")
+        .arg("show")
+        .arg(package)
+        .output().map_err(|e| {PipError(e.to_string())})?;
+
+    let output = output.stdout;
+    let output = String::from_utf8(output)
+    .map_err(|e| {PipError(e.to_string())})?;
+
+    let version = output
+        .lines()
+        .find(|line| line.starts_with("Version: "))
+        .map(|line| line[9..].to_string());
+    
+    if let Some(v) = version { Ok(v)} 
+    else { Err(PipError("could not retrive package version from Pip".to_string())) }
+}
```

### Comparing `pyscan_rs-0.1.1/src/scanner/models.rs` & `pyscan_rs-0.1.2/src/scanner/models.rs`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.1/PKG-INFO` & `pyscan_rs-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscan-rs
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python dependency vulnerability scanner
 Keywords: cli,python,security,vulnerability,pyo3
 Home-Page: https://github.com/aswinnnn/pyscan
@@ -13,75 +13,86 @@
 License: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/aswinnnn/pyscan
 
 <h1 align="center"> 🐍 Pyscan </h1>
 
-![CI](https://github.com/aswinnnn/pyscan/actions/workflows/CI.yml/badge.svg) ![Liscense](https://img.shields.io/github/license/aswinnnn/pyscan?color=ff64b4) [![PyPI](https://img.shields.io/pypi/v/pyscan-rs?color=ff69b4)](https://pypi.org/project/pyscan-rs) [![](https://img.shields.io/crates/v/pyscan?color=ff64b4)](https://crates.io/pyscan) [![GitHub issues](https://img.shields.io/github/issues/aswinnnn/pyscan.svg?color=ff69b4)](https://GitHub.com/aswinnnn/pyscan/issues/) [![Top Language](https://img.shields.io/github/languages/top/aswinnnn/pyscan?color=ff69b4)](https://img.shields.io/github/languages/top/aswinnnn/pyscan)
+![CI](https://github.com/aswinnnn/pyscan/actions/workflows/CI.yml/badge.svg) ![Liscense](https://img.shields.io/github/license/aswinnnn/pyscan?color=ff64b4) [![PyPI](https://img.shields.io/pypi/v/pyscan-rs?color=ff69b4)](https://pypi.org/project/pyscan-rs) [![](https://img.shields.io/crates/v/pyscan?color=ff64b4)](https://crates.io/crates/pyscan) [![GitHub issues](https://img.shields.io/github/issues/aswinnnn/pyscan.svg?color=ff69b4)](https://GitHub.com/aswinnnn/pyscan/issues/) [![Top Language](https://img.shields.io/github/languages/top/aswinnnn/pyscan?color=ff69b4)](https://img.shields.io/github/languages/top/aswinnnn/pyscan)
 
 <h4 align="center"> 
 
 <img src="https://media.discordapp.net/attachments/1002212458502557718/1107648562004758538/pyscan.png?width=779&height=206">
 
 </h4>
 
 <h5 align="center"> <i>A dependency vulnerability scanner for your python projects, straight from the terminal.</i> </h5>
 
-+ 🚀 blazingly fast and efficient scanner that can be used to scan large projects fairly quickly.
-+ 🤖 automatically uses `requirements.txt`, `pyproject.toml` or straight from the source code (though not reccomended)
-+ 🧑‍💻 easy to use, and can be integrated into existing build processes.
-+ 💽 In its very early alpha stage, so some features may not work correctly. PRs and issue makers welcome.
++ 🚀 blazingly fast scanner that can be used within large projects quickly.
++ 🤖 automatically uses `requirements.txt`, `pyproject.toml` or, the source code (highly discouraged)
++ 🧑‍💻 can be integrated into existing build processes.
++ 💽 In its alpha stage, some features may not work correctly. PRs and issue makers welcome.
 
 ## 🕊️ Install
 
 ```bash
-pip install pyscan-rs
+> pip install pyscan-rs
 ```
 look out for the "-rs" part
 or
 
 ```bash
-cargo install pyscan
+> cargo install pyscan
 ```
 
-or check out the [releases](https://github.com/aswinnnn/pyscan/releases).
+check out the [releases](https://github.com/aswinnnn/pyscan/releases).
 
 ## 🐇 Usage
 
-Go to your python source directory (or wherever you keep your requirements.txt/pyproject.toml) and run:
+Go to your python source directory (or wherever you keep your `requirements.txt`/`pyproject.toml`) and run:
 
 ```bash
-pyscan
+> pyscan
 ```
 or
 ```bash
-pyscan -d path/to/src
+> pyscan -d path/to/src
 ```
 
-that should get the thing going.
+## Docker
+
+Pyscan can scan inside docker images given you provide the correct path inside. This is still in its early stage and may break easily.
+
+```bash
+> pyscan docker -n my-docker-image -p /path/inside/container/to/source
+```
+
+by <i>"source"</i> I mean `requirements.txt`, `pyproject.toml` or your python files.
+
+<br>
 Here's the order of precedence for a "source" file:
 
-+ requirements.txt
-+ pyproject.toml
-+ your python source code (.py) [highly not reccomended]
++ `requirements.txt`
++ `pyproject.toml`
++ your python source code (`.py`) [highly discouraged]
 
-Any dependencies without a specified version defaults to its latest stable version. **Make sure you version-ize your requirements** and use proper [pep-508 syntax](https://peps.python.org/pep-0508/).
+Pyscan will find dependency versions from `pip` if not provided within the source file. Even though, **Make sure you version-ize your requirements** and use proper [pep-508 syntax](https://peps.python.org/pep-0508/).
 
 ## 🦀 Note
 
 pyscan uses [OSV](https://osv.dev) as its database for now. There are plans to add a few more.
 
-pyscan doesn't make sure your code is safe from everything. Use all resources available to you like Dependabot and other github features.
+pyscan doesn't make sure your code is safe from everything. Use all resources available to you like Dependabot, `pip-audit` or trivy.
 
 ## 🐰 Todo
 
 - [x] get it working.
-- [ ] add  tests.
-- [ ] more advisory databases.
-- [ ] query individual dependencies.
+- [ ] add  tests. [coming soon]
+- [x] query individual python packages. [v0.1.1]
 - [ ] perfomance optimizations.
+- [x] scan docker images [v0.1.2]
+- [ ] scan code health. [coming soon]
 
 ## 🐹 Sponsor
 
 While not coding, I am a broke high school student with nothing else to do. I appreciate all the help I'm worthy of.
```

