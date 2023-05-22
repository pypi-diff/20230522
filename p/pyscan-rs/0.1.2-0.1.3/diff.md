# Comparing `tmp/pyscan_rs-0.1.2.tar.gz` & `tmp/pyscan_rs-0.1.3.tar.gz`

## Comparing `pyscan_rs-0.1.2.tar` & `pyscan_rs-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pyscan_rs-0.1.2/Cargo.toml
--rw-r--r--   0        0        0      834 2023-05-16 11:24:31.000000 pyscan_rs-0.1.2/.github/FUNDING.yml
--rw-r--r--   0        0        0      872 2023-05-16 11:24:31.000000 pyscan_rs-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      615 2023-05-16 11:24:31.000000 pyscan_rs-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     2662 2023-05-17 11:57:45.000000 pyscan_rs-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0        0        0      756 2023-05-15 14:06:10.000000 pyscan_rs-0.1.2/.gitignore
--rw-r--r--   0        0        0     1507 2023-05-22 12:59:21.000000 pyscan_rs-0.1.2/CHANGELOG.md
--rw-r--r--   0        0        0     5355 2023-05-16 11:24:31.000000 pyscan_rs-0.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1280 2023-05-16 11:24:31.000000 pyscan_rs-0.1.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    38864 2023-05-22 08:00:37.000000 pyscan_rs-0.1.2/Cargo.lock
--rw-r--r--   0        0        0     1086 2023-05-16 11:24:31.000000 pyscan_rs-0.1.2/LICENSE
--rw-r--r--   0        0        0     3046 2023-05-22 07:58:55.000000 pyscan_rs-0.1.2/README.md
--rw-r--r--   0        0        0      201 2023-05-16 11:24:31.000000 pyscan_rs-0.1.2/SECURITY.md
--rw-r--r--   0        0        0     8746 2023-04-22 10:47:51.000000 pyscan_rs-0.1.2/osv_schema.json
--rw-r--r--   0        0        0      367 2023-05-16 07:21:52.000000 pyscan_rs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-15 13:16:26.000000 pyscan_rs-0.1.2/python/pyscan/__init__.py
--rw-r--r--   0        0        0      913 2023-05-15 13:49:45.000000 pyscan_rs-0.1.2/python/pyscan/__main__.py
--rw-r--r--   0        0        0     4182 2023-05-21 04:54:34.000000 pyscan_rs-0.1.2/src/docker/mod.rs
--rw-r--r--   0        0        0     3749 2023-05-21 04:44:58.000000 pyscan_rs-0.1.2/src/main.rs
--rw-r--r--   0        0        0     2594 2023-05-21 05:27:06.000000 pyscan_rs-0.1.2/src/parser/extractor.rs
--rw-r--r--   0        0        0     5381 2023-05-21 05:26:22.000000 pyscan_rs-0.1.2/src/parser/mod.rs
--rw-r--r--   0        0        0     1795 2023-05-20 04:05:11.000000 pyscan_rs-0.1.2/src/parser/structs.rs
--rw-r--r--   0        0        0     4737 2023-05-20 04:05:14.000000 pyscan_rs-0.1.2/src/scanner/api.rs
--rw-r--r--   0        0        0     3354 2023-05-21 04:33:52.000000 pyscan_rs-0.1.2/src/scanner/mod.rs
--rw-r--r--   0        0        0     4505 2023-05-16 04:29:05.000000 pyscan_rs-0.1.2/src/scanner/models.rs
--rw-r--r--   0        0        0     4462 2023-05-20 04:06:07.000000 pyscan_rs-0.1.2/src/utils.rs
--rw-r--r--   0        0        0     3704 1970-01-01 00:00:00.000000 pyscan_rs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      717 1970-01-01 00:00:00.000000 pyscan_rs-0.1.3/Cargo.toml
+-rw-r--r--   0        0        0      834 2023-05-16 11:24:31.000000 pyscan_rs-0.1.3/.github/FUNDING.yml
+-rw-r--r--   0        0        0      872 2023-05-16 11:24:31.000000 pyscan_rs-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      615 2023-05-16 11:24:31.000000 pyscan_rs-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2662 2023-05-17 11:57:45.000000 pyscan_rs-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      756 2023-05-15 14:06:10.000000 pyscan_rs-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1818 2023-05-22 13:28:59.000000 pyscan_rs-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     5355 2023-05-16 11:24:31.000000 pyscan_rs-0.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1280 2023-05-16 11:24:31.000000 pyscan_rs-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0    38864 2023-05-22 13:29:17.000000 pyscan_rs-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0     1086 2023-05-16 11:24:31.000000 pyscan_rs-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3146 2023-05-22 13:07:35.000000 pyscan_rs-0.1.3/README.md
+-rw-r--r--   0        0        0      201 2023-05-16 11:24:31.000000 pyscan_rs-0.1.3/SECURITY.md
+-rw-r--r--   0        0        0     8746 2023-04-22 10:47:51.000000 pyscan_rs-0.1.3/osv_schema.json
+-rw-r--r--   0        0        0      367 2023-05-16 07:21:52.000000 pyscan_rs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-15 13:16:26.000000 pyscan_rs-0.1.3/python/pyscan/__init__.py
+-rw-r--r--   0        0        0      913 2023-05-15 13:49:45.000000 pyscan_rs-0.1.3/python/pyscan/__main__.py
+-rw-r--r--   0        0        0     4683 2023-05-22 13:24:12.000000 pyscan_rs-0.1.3/src/docker/mod.rs
+-rw-r--r--   0        0        0     3749 2023-05-21 04:44:58.000000 pyscan_rs-0.1.3/src/main.rs
+-rw-r--r--   0        0        0     2594 2023-05-21 05:27:06.000000 pyscan_rs-0.1.3/src/parser/extractor.rs
+-rw-r--r--   0        0        0     5381 2023-05-21 05:26:22.000000 pyscan_rs-0.1.3/src/parser/mod.rs
+-rw-r--r--   0        0        0     1795 2023-05-20 04:05:11.000000 pyscan_rs-0.1.3/src/parser/structs.rs
+-rw-r--r--   0        0        0     4737 2023-05-20 04:05:14.000000 pyscan_rs-0.1.3/src/scanner/api.rs
+-rw-r--r--   0        0        0     3354 2023-05-21 04:33:52.000000 pyscan_rs-0.1.3/src/scanner/mod.rs
+-rw-r--r--   0        0        0     4505 2023-05-16 04:29:05.000000 pyscan_rs-0.1.3/src/scanner/models.rs
+-rw-r--r--   0        0        0     4462 2023-05-22 13:29:37.000000 pyscan_rs-0.1.3/src/utils.rs
+-rw-r--r--   0        0        0     3804 1970-01-01 00:00:00.000000 pyscan_rs-0.1.3/PKG-INFO
```

### Comparing `pyscan_rs-0.1.2/Cargo.toml` & `pyscan_rs-0.1.3/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyscan"
-version = "0.1.2"
+version = "0.1.3"
 edition = "2021"
 authors = ["Aswin <aswinsnair@protonmail.com>"]
 license = "MIT"
 description = "Python dependency vulnerability scanner"
 readme = "README.md"
 homepage = "https://github.com/aswinnnn/pyscan"
 repository = "https://github.com/aswinnnn/pyscan"
```

### Comparing `pyscan_rs-0.1.2/.github/FUNDING.yml` & `pyscan_rs-0.1.3/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md` & `pyscan_rs-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md` & `pyscan_rs-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/.github/workflows/CI.yml` & `pyscan_rs-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/.gitignore` & `pyscan_rs-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/CHANGELOG.md` & `pyscan_rs-0.1.3/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -30,8 +30,13 @@
 -  better error messages, though panics are the main way of displaying them.
   
 -  This release was pretty rushed to fix that issue and get the docker feature on. I will be taking my sweet time with the next release to get:
   
 - - github actions integration
 - - make it easier for other tools to interact with pyscan
 - - code complexity analyzer (not doing a linter cuz any respectable python dev already has one)
-- - finally get to do tests, and lots of more ideas in my head. Thanks for the awesome support so far!
+- - finally get to do tests, and lots of more ideas in my head. Thanks for the awesome support so far!
+
+## 0.1.3
+
+- Fixed a grave error where docker command left remnants and did not perform a complete cleanup.
+- This release was made right after the previous release to fix this feature, however, the release page will contain both this message and the previous one so no one will miss out on the new stuff.
```

### Comparing `pyscan_rs-0.1.2/CODE_OF_CONDUCT.md` & `pyscan_rs-0.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/CONTRIBUTING.md` & `pyscan_rs-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/Cargo.lock` & `pyscan_rs-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -766,15 +766,15 @@
 checksum = "5787f7cda34e3033a72192c018bc5883100330f362ef279a8cbccfce8bb4e874"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "pyscan"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "chrono",
  "clap",
  "console",
  "lazy_static",
  "pep-508",
  "regex",
```

### Comparing `pyscan_rs-0.1.2/LICENSE` & `pyscan_rs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/README.md` & `pyscan_rs-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 Pyscan can scan inside docker images given you provide the correct path inside. This is still in its early stage and may break easily.
 
 ```bash
 > pyscan docker -n my-docker-image -p /path/inside/container/to/source
 ```
 
 by <i>"source"</i> I mean `requirements.txt`, `pyproject.toml` or your python files.
+Note: Your docker engine/daemon should be running as pyscan utilizes the `docker create` command. 
 
 <br>
 Here's the order of precedence for a "source" file:
 
 + `requirements.txt`
 + `pyproject.toml`
 + your python source code (`.py`) [highly discouraged]
```

### Comparing `pyscan_rs-0.1.2/osv_schema.json` & `pyscan_rs-0.1.3/osv_schema.json`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/python/pyscan/__main__.py` & `pyscan_rs-0.1.3/python/pyscan/__main__.py`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/src/docker/mod.rs` & `pyscan_rs-0.1.3/src/docker/mod.rs`

 * *Files 10% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     .expect("Could not create a temporary folder for the docker files. Try creating it yourself:\n./tmp/docker-files\n");
 
     // Use the "cp" subcommand to copy all files from the container
     // to a temporary directory on the host
     cmd.arg("cp")
         .arg(format!(
             "{}:/{}",
-            container_id,
+            container_id.clone(),
             path.to_str().expect("Path contains non-unicode characters")
         ))
         .arg("./tmp/docker-files");
 
     // Execute the command and get the output
     let output = cmd.output().map_err(|e| DockerError(e.to_string()))?;
 
@@ -71,15 +71,32 @@
         return Err(DockerError(
             String::from_utf8_lossy(&output.stderr).to_string(),
         ));
     }
 
     scan_dir(Path::new("./tmp/docker-files"));
     cleanup().map_err(|e| DockerError(e.to_string()) )?;
+
+    // docker stop
+    let mut cmd = Command::new("docker");
+    cmd.arg("stop")
+        .arg(container_id.clone());
+
+    // Execute the command and get the output
+    let _output = cmd.output().map_err(|e| DockerError(e.to_string()))?;
+
+    // docker remove
+    let mut cmd = Command::new("docker");
+    cmd.arg("rm")
+        .arg(container_id);
+
+    // Execute the command and get the output
+    let _output = cmd.output().map_err(|e| DockerError(e.to_string()))?;
     Ok(())
+   
 
     // // Create another Command object to run shell commands
     // let mut cmd = Command::new("sh");
 
     // // Use the "-c" argument to run a shell command that lists all files
     // // in the temporary directory and removes the directory prefix
     // cmd.arg("-c")
@@ -110,9 +127,9 @@
 fn create_tmp_folder(path: &str) -> std::io::Result<()> {
     let tmp_path = format!("{}/tmp/docker-files", path);
     std::fs::create_dir_all(&tmp_path)?;
     Ok(())
 }
 
 fn cleanup() -> Result<(), std::io::Error> {
-    std::fs::remove_dir("./tmp/docker-files")
+    std::fs::remove_dir_all("./tmp/docker-files")
 }
```

### Comparing `pyscan_rs-0.1.2/src/main.rs` & `pyscan_rs-0.1.3/src/main.rs`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/src/parser/extractor.rs` & `pyscan_rs-0.1.3/src/parser/extractor.rs`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/src/parser/mod.rs` & `pyscan_rs-0.1.3/src/parser/mod.rs`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/src/parser/structs.rs` & `pyscan_rs-0.1.3/src/parser/structs.rs`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/src/scanner/api.rs` & `pyscan_rs-0.1.3/src/scanner/api.rs`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/src/scanner/mod.rs` & `pyscan_rs-0.1.3/src/scanner/mod.rs`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/src/scanner/models.rs` & `pyscan_rs-0.1.3/src/scanner/models.rs`

 * *Files identical despite different names*

### Comparing `pyscan_rs-0.1.2/src/utils.rs` & `pyscan_rs-0.1.3/src/utils.rs`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         );
 
         time
     }
 }
 
 pub fn get_version() -> String {
-    "0.1.1".to_string()
+    "0.1.3".to_string()
 }
 
 pub fn reqwest_send(method: &str, url: String) -> Option<Response> {
     let client = reqwest::blocking::Client::builder()
         .user_agent(format!("pyscan v{}", get_version()))
         .build();
```

### Comparing `pyscan_rs-0.1.2/PKG-INFO` & `pyscan_rs-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscan-rs
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Python dependency vulnerability scanner
 Keywords: cli,python,security,vulnerability,pyo3
 Home-Page: https://github.com/aswinnnn/pyscan
@@ -63,14 +63,15 @@
 Pyscan can scan inside docker images given you provide the correct path inside. This is still in its early stage and may break easily.
 
 ```bash
 > pyscan docker -n my-docker-image -p /path/inside/container/to/source
 ```
 
 by <i>"source"</i> I mean `requirements.txt`, `pyproject.toml` or your python files.
+Note: Your docker engine/daemon should be running as pyscan utilizes the `docker create` command. 
 
 <br>
 Here's the order of precedence for a "source" file:
 
 + `requirements.txt`
 + `pyproject.toml`
 + your python source code (`.py`) [highly discouraged]
```

