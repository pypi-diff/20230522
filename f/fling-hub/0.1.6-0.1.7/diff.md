# Comparing `tmp/fling_hub-0.1.6.tar.gz` & `tmp/fling_hub-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fling_hub-0.1.6.tar", max compression
+gzip compressed data, was "fling_hub-0.1.7.tar", max compression
```

## Comparing `fling_hub-0.1.6.tar` & `fling_hub-0.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       57 2023-05-14 06:13:51.220760 fling_hub-0.1.6/README.md
--rw-r--r--   0        0        0        5 2023-05-21 21:20:45.888014 fling_hub-0.1.6/VERSION
--rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 fling_hub-0.1.6/build.py
--rw-r--r--   0        0        0       22 2023-05-21 21:20:43.379682 fling_hub-0.1.6/fling_hub/__init__.py
--rw-r--r--   0        0        0     2158 2023-05-19 22:01:24.121786 fling_hub-0.1.6/fling_hub/flingroute.py
--rw-r--r--   0        0        0      903 2023-05-20 00:05:15.055873 fling_hub-0.1.6/fling_hub/hub.plist.template
--rwxr-xr-x   0        0        0  8301312 2023-05-20 20:12:28.547737 fling_hub-0.1.6/fling_hub/loophost
--rw-r--r--   0        0        0      814 2023-05-20 01:14:11.424956 fling_hub-0.1.6/fling_hub/loophost.plist.template
--rw-r--r--   0        0        0     3994 2023-05-21 21:11:27.044451 fling_hub-0.1.6/fling_hub/postinstall.py
--rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 fling_hub-0.1.6/fling_hub/static/fling-logo-dark.png
--rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 fling_hub-0.1.6/fling_hub/static/fling-logo-light.png
--rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 fling_hub-0.1.6/fling_hub/static/logo-hc.txt
--rw-r--r--   0        0        0     1211 2023-05-21 21:11:46.157275 fling_hub-0.1.6/fling_hub/templates/admin.html
--rw-r--r--   0        0        0     2178 2023-05-21 21:11:54.645785 fling_hub-0.1.6/fling_hub/templates/local.html
--rw-r--r--   0        0        0     1081 2023-05-18 00:14:10.759502 fling_hub-0.1.6/fling_hub/templates/partials/apptable.html
--rw-r--r--   0        0        0      289 2023-05-21 21:12:35.820099 fling_hub-0.1.6/fling_hub/templates/partials/upgrade.html
--rw-r--r--   0        0        0     1099 2023-05-21 21:20:53.660432 fling_hub-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 fling_hub-0.1.6/setup.py
--rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 fling_hub-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-05-14 06:13:51.220760 fling_hub-0.1.7/README.md
+-rw-r--r--   0        0        0        5 2023-05-21 22:30:01.968323 fling_hub-0.1.7/VERSION
+-rw-r--r--   0        0        0      666 2023-05-20 06:37:17.640351 fling_hub-0.1.7/build.py
+-rw-r--r--   0        0        0       22 2023-05-21 22:29:52.271836 fling_hub-0.1.7/fling_hub/__init__.py
+-rw-r--r--   0        0        0     2158 2023-05-19 22:01:24.121786 fling_hub-0.1.7/fling_hub/flingroute.py
+-rw-r--r--   0        0        0      903 2023-05-20 00:05:15.055873 fling_hub-0.1.7/fling_hub/hub.plist.template
+-rwxr-xr-x   0        0        0  8301312 2023-05-20 20:12:28.547737 fling_hub-0.1.7/fling_hub/loophost
+-rw-r--r--   0        0        0      814 2023-05-20 01:14:11.424956 fling_hub-0.1.7/fling_hub/loophost.plist.template
+-rw-r--r--   0        0        0     4196 2023-05-21 22:29:28.373164 fling_hub-0.1.7/fling_hub/postinstall.py
+-rw-r--r--   0        0        0    95159 2023-04-07 23:50:14.944549 fling_hub-0.1.7/fling_hub/static/fling-logo-dark.png
+-rw-r--r--   0        0        0   265670 2023-04-08 00:23:03.250215 fling_hub-0.1.7/fling_hub/static/fling-logo-light.png
+-rw-r--r--   0        0        0     3834 2023-05-12 22:43:40.802704 fling_hub-0.1.7/fling_hub/static/logo-hc.txt
+-rw-r--r--   0        0        0     1211 2023-05-21 21:11:46.157275 fling_hub-0.1.7/fling_hub/templates/admin.html
+-rw-r--r--   0        0        0     2178 2023-05-21 21:11:54.645785 fling_hub-0.1.7/fling_hub/templates/local.html
+-rw-r--r--   0        0        0     1081 2023-05-18 00:14:10.759502 fling_hub-0.1.7/fling_hub/templates/partials/apptable.html
+-rw-r--r--   0        0        0      289 2023-05-21 21:12:35.820099 fling_hub-0.1.7/fling_hub/templates/partials/upgrade.html
+-rw-r--r--   0        0        0     1099 2023-05-21 22:29:58.250511 fling_hub-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       39 2023-05-20 00:34:26.794307 fling_hub-0.1.7/setup.py
+-rw-r--r--   0        0        0      783 1970-01-01 00:00:00.000000 fling_hub-0.1.7/PKG-INFO
```

### Comparing `fling_hub-0.1.6/build.py` & `fling_hub-0.1.7/build.py`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.6/fling_hub/flingroute.py` & `fling_hub-0.1.7/fling_hub/flingroute.py`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.6/fling_hub/hub.plist.template` & `fling_hub-0.1.7/fling_hub/hub.plist.template`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.6/fling_hub/loophost` & `fling_hub-0.1.7/fling_hub/loophost`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.6/fling_hub/loophost.plist.template` & `fling_hub-0.1.7/fling_hub/loophost.plist.template`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.6/fling_hub/postinstall.py` & `fling_hub-0.1.7/fling_hub/postinstall.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,47 +59,53 @@
     with open(pathlib.Path(TARGET_DIR, "flinguser.txt"), "r") as userfile:
         USERNAME = userfile.read()
 
 
 def issue_certs():
     global USERNAME, TARGET_DIR
     print("Generating SSL certificates (this may take a minute)...")
-    run(
-        " ".join(
+    cmd = " ".join(
             [
                 "certbot",
                 "certonly",
                 "--config-dir ./",
                 "--work-dir ./",
                 "--logs-dir ./",
                 "--non-interactive",
                 "--expand",
                 "--agree-tos",
                 f"-m webmaster@{LOOPHOST_DOMAIN}",
                 "--authenticator=fling_authenticator",
                 f'-d "*.{USERNAME}.{LOOPHOST_DOMAIN}"',
                 f'-d "{USERNAME}.{LOOPHOST_DOMAIN}"',
+                "--force-renewal",
                 "--fling_authenticator-propagation-seconds=15",
             ]
-        ),
+        )
+    print(cmd)
+    run(
+        cmd,
         stdout=subprocess.PIPE,
         stderr=subprocess.PIPE,
         stdin=subprocess.PIPE,
         cwd=TARGET_DIR,
         shell=True,
         check=True,
     )
 
 
 def setup_launchd_scripts():
     global USERNAME, TARGET_DIR, HUBDIR, PYEX
-    if not os.path.exists(pathlib.Path(TARGET_DIR, "loophost.json")):
-        with open(pathlib.Path(TARGET_DIR, "loophost.json"), "w") as datafile:
-            data = {"apps": {}, "fqdn": f"{USERNAME}.{LOOPHOST_DOMAIN}"}
-            datafile.write(json.dumps(data))
+    apps = {}
+    if os.path.exists(pathlib.Path(TARGET_DIR, "loophost.json")):
+        with open(pathlib.Path(TARGET_DIR, "loophost.json"), "r") as datafile:
+            apps = json.loads(datafile.read()).get("apps")
+    with open(pathlib.Path(TARGET_DIR, "loophost.json"), "w") as datafile:
+        data = {"apps": apps, "fqdn": f"{USERNAME}.{LOOPHOST_DOMAIN}"}
+        datafile.write(json.dumps(data))
     shutil.copy2(pathlib.Path(HUBDIR, "loophost.plist.template"), TARGET_DIR)
     shutil.copy2(pathlib.Path(HUBDIR, "hub.plist.template"), TARGET_DIR)
 
     d = {"CWD": TARGET_DIR, "USERNAME": USERNAME, "PYEX": PYEX, "HUBDIR": HUBDIR}
 
     templates = [
         (
```

### Comparing `fling_hub-0.1.6/fling_hub/static/fling-logo-dark.png` & `fling_hub-0.1.7/fling_hub/static/fling-logo-dark.png`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.6/fling_hub/static/fling-logo-light.png` & `fling_hub-0.1.7/fling_hub/static/fling-logo-light.png`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.6/fling_hub/static/logo-hc.txt` & `fling_hub-0.1.7/fling_hub/static/logo-hc.txt`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.6/fling_hub/templates/admin.html` & `fling_hub-0.1.7/fling_hub/templates/admin.html`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.6/fling_hub/templates/local.html` & `fling_hub-0.1.7/fling_hub/templates/local.html`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.6/fling_hub/templates/partials/apptable.html` & `fling_hub-0.1.7/fling_hub/templates/partials/apptable.html`

 * *Files identical despite different names*

### Comparing `fling_hub-0.1.6/pyproject.toml` & `fling_hub-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "poetry>=0.12", "setuptools", "wheel", "setuptools-cpp", "setuptools-golang"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "fling-hub"
-version = "0.1.6"
+version = "0.1.7"
 description = "Loophost: for a better local dev"
 authors = [
     "Joshua McKenty <jmckenty@gmail.com>",
     "Anouk Ruhaak <anoukruhaak@gmail.com>",
 ]
 readme = "README.md"
 include = [{ path = "VERSION" },
```

### Comparing `fling_hub-0.1.6/PKG-INFO` & `fling_hub-0.1.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fling-hub
-Version: 0.1.6
+Version: 0.1.7
 Summary: Loophost: for a better local dev
 Author: Joshua McKenty
 Author-email: jmckenty@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

