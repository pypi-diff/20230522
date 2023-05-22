# Comparing `tmp/win_defender-0.1.0.tar.gz` & `tmp/win_defender-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "win_defender-0.1.0.tar", max compression
+gzip compressed data, was "win_defender-0.1.1.tar", max compression
```

## Comparing `win_defender-0.1.0.tar` & `win_defender-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2023-05-22 08:25:36.210303 win_defender-0.1.0/LICENSE
--rw-r--r--   0        0        0      507 2023-05-22 10:39:58.877514 win_defender-0.1.0/README.md
--rw-r--r--   0        0        0      425 2023-05-22 10:39:58.878249 win_defender-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-22 10:03:18.011429 win_defender-0.1.0/win_defender/__init__.py
--rw-r--r--   0        0        0     1610 2023-05-22 10:43:39.447159 win_defender-0.1.0/win_defender/tools.py
--rw-r--r--   0        0        0      987 2023-05-22 10:03:18.012403 win_defender-0.1.0/win_defender/utils.py
--rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 win_defender-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-22 08:25:36.210303 win_defender-0.1.1/LICENSE
+-rw-r--r--   0        0        0      507 2023-05-22 10:39:58.877514 win_defender-0.1.1/README.md
+-rw-r--r--   0        0        0      425 2023-05-22 11:02:43.147420 win_defender-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-22 10:03:18.011429 win_defender-0.1.1/win_defender/__init__.py
+-rw-r--r--   0        0        0     1724 2023-05-22 11:02:41.126435 win_defender-0.1.1/win_defender/tools.py
+-rw-r--r--   0        0        0      987 2023-05-22 10:03:18.012403 win_defender-0.1.1/win_defender/utils.py
+-rw-r--r--   0        0        0     1154 1970-01-01 00:00:00.000000 win_defender-0.1.1/PKG-INFO
```

### Comparing `win_defender-0.1.0/LICENSE` & `win_defender-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `win_defender-0.1.0/win_defender/tools.py` & `win_defender-0.1.1/win_defender/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,28 +12,35 @@
     
     Args:
         hostname (str): NTP hostname/IP. default: samay1.nic.1
 
     Returns:
         None
     '''
-    _, rcode = run_cmd(
+
+    run_cmd(
+        cmd='net stop w32time',
+        succ_msg='w32time service stopped',
+        err_msg='Failed to stop w32time service',
+        succ_rcode=2,
+    )
+
+    run_cmd(
         cmd='net start w32time',
         succ_msg='w32time service started',
         err_msg='Failed to start w32time service',
-        succ_rcode=0,
+        succ_rcode=2,
     )
 
-    if rcode == 0:
-         run_cmd(
-            cmd=f'w32tm /config /update /manualpeerlist:{hostname}',
-            succ_msg=f'Time Synced with {hostname} successfully',
-            err_msg=f'Failed to sync time with {hostname}',
-            succ_rcode=0,
-        )
+    run_cmd(
+        cmd=f'w32tm /config /update /manualpeerlist:{hostname}',
+        succ_msg=f'Time Synced with {hostname} successfully',
+        err_msg=f'Failed to sync time with {hostname}',
+        succ_rcode=0,
+    )
        
 
 def block_root_hubs():
     '''Blocks USB root hubs on windows machine
     
     Args:
         None
```

### Comparing `win_defender-0.1.0/win_defender/utils.py` & `win_defender-0.1.1/win_defender/utils.py`

 * *Files identical despite different names*

### Comparing `win_defender-0.1.0/PKG-INFO` & `win_defender-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win-defender
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools to defend windows and get compliant with common regulations
 License: MIT
 Author: Dhrumil Mistry
 Author-email: 56185972+dmdhrumilmistry@users.noreply.github.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

