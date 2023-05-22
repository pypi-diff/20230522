# Comparing `tmp/cdk-redisdb-0.0.23.tar.gz` & `tmp/cdk-redisdb-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-redisdb-0.0.23.tar", last modified: Sat May 20 09:07:20 2023, max compression
+gzip compressed data, was "cdk-redisdb-0.0.24.tar", last modified: Mon May 22 02:21:18 2023, max compression
```

## Comparing `cdk-redisdb-0.0.23.tar` & `cdk-redisdb-0.0.24.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:07:20.837144 cdk-redisdb-0.0.23/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-20 09:07:20.837144 cdk-redisdb-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 09:07:20.837144 cdk-redisdb-0.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:07:20.833144 cdk-redisdb-0.0.23/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:07:20.837144 cdk-redisdb-0.0.23/src/cdk_redisdb/
--rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/src/cdk_redisdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:07:20.837144 cdk-redisdb-0.0.23/src/cdk_redisdb/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/src/cdk_redisdb/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25935 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.23.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 09:07:04.000000 cdk-redisdb-0.0.23/src/cdk_redisdb/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 09:07:20.837144 cdk-redisdb-0.0.23/src/cdk_redisdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-20 09:07:20.000000 cdk-redisdb-0.0.23/src/cdk_redisdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-20 09:07:20.000000 cdk-redisdb-0.0.23/src/cdk_redisdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 09:07:20.000000 cdk-redisdb-0.0.23/src/cdk_redisdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-20 09:07:20.000000 cdk-redisdb-0.0.23/src/cdk_redisdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-20 09:07:20.000000 cdk-redisdb-0.0.23/src/cdk_redisdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:21:18.228522 cdk-redisdb-0.0.24/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-22 02:21:18.228522 cdk-redisdb-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 02:21:18.228522 cdk-redisdb-0.0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:21:18.224521 cdk-redisdb-0.0.24/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:21:18.228522 cdk-redisdb-0.0.24/src/cdk_redisdb/
+-rw-r--r--   0 runner    (1001) docker     (123)    48408 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/src/cdk_redisdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:21:18.228522 cdk-redisdb-0.0.24/src/cdk_redisdb/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/src/cdk_redisdb/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25940 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.24.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 02:21:04.000000 cdk-redisdb-0.0.24/src/cdk_redisdb/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 02:21:18.228522 cdk-redisdb-0.0.24/src/cdk_redisdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-22 02:21:18.000000 cdk-redisdb-0.0.24/src/cdk_redisdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-22 02:21:18.000000 cdk-redisdb-0.0.24/src/cdk_redisdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 02:21:18.000000 cdk-redisdb-0.0.24/src/cdk_redisdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-22 02:21:18.000000 cdk-redisdb-0.0.24/src/cdk_redisdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-22 02:21:18.000000 cdk-redisdb-0.0.24/src/cdk_redisdb.egg-info/top_level.txt
```

### Comparing `cdk-redisdb-0.0.23/LICENSE` & `cdk-redisdb-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.23/PKG-INFO` & `cdk-redisdb-0.0.24/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.23
+Version: 0.0.24
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-redisdb-0.0.23/README.md` & `cdk-redisdb-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.23/setup.py` & `cdk-redisdb-0.0.24/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-redisdb",
-    "version": "0.0.23",
+    "version": "0.0.24",
     "description": "Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API",
     "license": "Apache-2.0",
     "url": "https://github.com/forkfork/cdk-redisdb.git",
     "long_description_content_type": "text/markdown",
     "author": "Timothy Downs<timothydowns@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_redisdb",
         "cdk_redisdb._jsii"
     ],
     "package_data": {
         "cdk_redisdb._jsii": [
-            "cdk-redisdb@0.0.23.jsii.tgz"
+            "cdk-redisdb@0.0.24.jsii.tgz"
         ],
         "cdk_redisdb": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-redisdb-0.0.23/src/cdk_redisdb/__init__.py` & `cdk-redisdb-0.0.24/src/cdk_redisdb/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-redisdb-0.0.23/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.23.jsii.tgz` & `cdk-redisdb-0.0.24/src/cdk_redisdb/_jsii/cdk-redisdb@0.0.24.jsii.tgz`

 * *Files 20% similar despite different names*

#### Comparing `cdk-redisdb@0.0.23.jsii.tgz-content` & `cdk-redisdb@0.0.24.jsii.tgz-content`

##### package/.jsii

###### Pretty-printed

 * *Similarity: 0.9444444444444444%*

 * *Differences: {"'fingerprint'": "'uz1hGChDhDWslkMBU7ZM9dYs2eqd2KV3NRS+hVWXB0s='", "'version'": "'0.0.24'"}*

```diff
@@ -3408,15 +3408,15 @@
             }
         }
     },
     "description": "Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API",
     "docs": {
         "stability": "stable"
     },
-    "fingerprint": "h1nf4oVCeeGmUP5jDsPUa/dt1FrS3Bq4KruleSSaHgQ=",
+    "fingerprint": "uz1hGChDhDWslkMBU7ZM9dYs2eqd2KV3NRS+hVWXB0s=",
     "homepage": "https://github.com/forkfork/cdk-redisdb.git",
     "jsiiVersion": "1.81.0 (build 80988b0)",
     "keywords": [
         "cdk"
     ],
     "license": "Apache-2.0",
     "metadata": {
@@ -3871,9 +3871,9 @@
                         }
                     }
                 }
             ],
             "symbolId": "src/index:RedisDBProps"
         }
     },
-    "version": "0.0.23"
+    "version": "0.0.24"
 }
```

##### package/lib/index.js

###### js-beautify {}

```diff
@@ -112,15 +112,15 @@
         }
     }
 }
 exports.RedisDB = RedisDB;
 _a = JSII_RTTI_SYMBOL_1;
 RedisDB[_a] = {
     fqn: "cdk-redisdb.RedisDB",
-    version: "0.0.23"
+    version: "0.0.24"
 };
 class MemoryDB extends constructs_1.Construct {
     constructor(scope, id, props = {}) {
         super(scope, id);
         let isolatedSubnets = [];
         let redisVpc = setupVpc(this, props);
         this.vpc = redisVpc;
@@ -176,10 +176,10 @@
         //cfnACL.node.addDependency(cfnUser);
     }
 }
 exports.MemoryDB = MemoryDB;
 _b = JSII_RTTI_SYMBOL_1;
 MemoryDB[_b] = {
     fqn: "cdk-redisdb.MemoryDB",
-    version: "0.0.23"
+    version: "0.0.24"
 };
 //# sourceMappingURL=data:application/json;base64,eyJ2ZXJzaW9uIjozLCJmaWxlIjoiaW5kZXguanMiLCJzb3VyY2VSb290IjoiIiwic291cmNlcyI6WyIuLi9zcmMvaW5kZXgudHMiXSwibmFtZXMiOltdLCJtYXBwaW5ncyI6Ijs7Ozs7QUFBQSw2Q0FPcUI7QUFDckIsMkNBQXVDO0FBb0J2QyxTQUFTLFFBQVEsQ0FBQyxNQUFXLEVBQUUsS0FBbUI7SUFDaEQsT0FBTyxLQUFLLENBQUMsV0FBVyxJQUFJLElBQUkscUJBQUcsQ0FBQyxHQUFHLENBQUMsTUFBTSxFQUFFLEtBQUssRUFBRTtRQUNyRCxtQkFBbUIsRUFBRTtZQUNuQjtnQkFDRSxRQUFRLEVBQUUsRUFBRTtnQkFDWixJQUFJLEVBQUUsZUFBZTtnQkFDckIsVUFBVSxFQUFFLHFCQUFHLENBQUMsVUFBVSxDQUFDLE1BQU07YUFDbEM7WUFDRDtnQkFDRSxRQUFRLEVBQUUsRUFBRTtnQkFDWixJQUFJLEVBQUUsaUJBQWlCO2dCQUN2QixVQUFVLEVBQUUscUJBQUcsQ0FBQyxVQUFVLENBQUMsZ0JBQWdCO2FBQzVDO1NBQ0Y7S0FDRixDQUFDLENBQUM7QUFDTCxDQUFDO0FBRUQsTUFBYSxPQUFRLFNBQVEsc0JBQVM7SUFHcEMsWUFBWSxLQUFnQixFQUFFLEVBQVUsRUFBRSxRQUFzQixFQUFFO1FBQ2hFLEtBQUssQ0FBQyxLQUFLLEVBQUUsRUFBRSxDQUFDLENBQUM7UUFFakIsSUFBSSxlQUFlLEdBQWEsRUFBRSxDQUFDO1FBQ25DLElBQUksUUFBUSxHQUFHLFFBQVEsQ0FBQyxJQUFJLEVBQUUsS0FBSyxDQUFDLENBQUM7UUFDckMsSUFBSSxDQUFDLEdBQUcsR0FBRyxRQUFRLENBQUM7UUFDcEIsUUFBUSxDQUFDLGVBQWUsQ0FBQyxPQUFPLENBQUMsVUFBUyxLQUFLO1lBQzdDLGVBQWUsQ0FBQyxJQUFJLENBQUMsS0FBSyxDQUFDLFFBQVEsQ0FBQyxDQUFDO1FBQ3ZDLENBQUMsQ0FBQyxDQUFDO1FBQ0gsSUFBSSxlQUFlLENBQUMsTUFBTSxJQUFJLENBQUMsRUFBRTtZQUMvQixRQUFRLENBQUMsY0FB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O2dCQUMxQixlQUFlLEVBQUUsS0FBSyxDQUFDLGVBQWUsSUFBSSxxQkFBcUI7YUFDaEUsQ0FBQyxDQUFDO1lBQ0gsU0FBUyxHQUFHLGFBQWEsQ0FBQyxlQUFnQixDQUFDO1NBQzVDO2FBQU07WUFDTCxTQUFTLEdBQUcsS0FBSyxDQUFDLHVCQUF3QixDQUFDO1NBQzVDO1FBRUQ7Ozs7Ozs7Ozs7VUFVRTtRQUNGLE1BQU0sZ0JBQWdCLEdBQUcsSUFBSSwwQkFBUSxDQUFDLFVBQVUsQ0FBQyxJQUFJLEVBQUUsVUFBVSxFQUFFO1lBQ2pFLE9BQU8sRUFBRSxhQUFhO1lBQ3RCLFdBQVcsRUFBRSxhQUFhO1lBQzFCLFFBQVEsRUFBRSxLQUFLLENBQUMsUUFBUSxJQUFJLGNBQWM7WUFFMUMsdUJBQXVCLEVBQUUsS0FBSztZQUM5QixXQUFXLEVBQUUsYUFBYTtZQUMxQixhQUFhLEVBQUUsS0FBSyxDQUFDLGFBQWEsSUFBSSxLQUFLO1lBQzNDLFNBQVMsRUFBRSxLQUFLLENBQUMsS0FBSyxJQUFFLENBQUM7WUFDekIsbUJBQW1CLEVBQUUsS0FBSyxDQUFDLFFBQVEsSUFBRSxDQUFDO1lBQ3RDLGdCQUFnQixFQUFFLENBQUMsZUFBZSxDQUFDLGVBQWUsQ0FBQztZQUNuRCxlQUFlLEVBQUUsU0FBUztZQUMxQixVQUFVLEVBQUUsSUFBSTtTQUNqQixDQUFDLENBQUM7UUFDSCxJQUFJLENBQUMsS0FBSyxDQUFDLHVCQUF1QixFQUFFO1lBQ2xDLGdCQUFnQixDQUFDLElBQUksQ0FBQyxhQUFhLENBQUMsYUFBYyxDQUFDLENBQUM7U0FDckQ7UUFDRCxJQUFJLENBQUMsT0FBTyxHQUFHLGdCQUFnQixDQUFDO1FBQ2hDLDhDQUE4QztRQUM5QyxxQ0FBcUM7SUFDdkMsQ0FBQzs7QUE1REgsNEJBNkRDIiwic291cmNlc0NvbnRlbnQiOlsiaW1wb3J0IHtcbiAgYXdzX2VsYXN0aWNhY2hlIGFzIGVsYXN0aWNhY2hlLFxuICBhd3NfbWVtb3J5ZGIgYXMgbWVtb3J5ZGIsXG4gIGF3c19lYzIgYXMgZWMyLFxuICBhd3NfYXBwbGljYXRpb25hdXRvc2NhbGluZyBhcyBhcHBzY2FsaW5nLFxuICBTdGFja1Byb3BzLFxuICBJUmVzb2x2YWJsZSxcbn0gZnJvbSAnYXdzLWNkay1saWInO1xuaW1wb3J0IHsgQ29uc3RydWN0IH0gZnJvbSAnY29uc3RydWN0cyc7XG5cbmV4cG9ydCBpbnRlcmZhY2UgUmVkaXNEQlByb3BzIGV4dGVuZHMgU3RhY2tQcm9wcyB7XG4gIHJlYWRvbmx5IGV4aXN0aW5nVnBjPzogZWMyLklWcGM7XG4gIHJlYWRvbmx5IGV4aXN0aW5nU2VjdXJpdHlHcm91cD86IGVjMi5JU2VjdXJpdHlHcm91cDtcbiAgcmVhZG9ubHkgZXhpc3RpbmdTdWJuZXRHcm91cE5hbWU/OiBzdHJpbmc7XG4gIHJlYWRvbmx5IGF0UmVzdEVuY3J5cHRpb25FbmFibGVkPzogYm9vbGVhbiB8IElSZXNvbHZhYmxlO1xuICByZWFkb25seSB0cmFuc2l0RW5jcnlwdGlvbkVuYWJsZWQ/OiBib29sZWFuIHwgSVJlc29sdmFibGU7XG4gIHJlYWRvbmx5IGVuZ2luZVZlcnNpb24/OiBzdHJpbmc7XG4gIHJlYWRvbmx5IHBhcmFtZXRlckdyb3VwTmFtZT86IHN0cmluZztcbiAgcmVhZG9ubHkgbWVtb3J5QXV0b3NjYWxpbmdUYXJnZXQ/OiBudW1iZXI7XG4gIHJlYWRvbmx5IHJlcGxpY2FzQ3B1QXV0b3NjYWxpbmdUYXJnZXQ/OiBudW1iZXI7XG4gIHJlYWRvbmx5IG5vZGVzQ3B1QXV0b3NjYWxpbmdUYXJnZXQ/OiBudW1iZXI7XG4gIHJlYWRvbmx5IG5vZGVzPzogbnVtYmVyO1xuICByZWFkb25seSBub2RlVHlwZT86IHN0cmluZztcbiAgcmVhZG9ubHkgcmVwbGljYXM/OiBudW1iZXI7XG4gIHJlYWRvbmx5IGF1dGhUb2tlbj86IHN0cmluZztcbiAgcmVhZG9ubHkgc3VibmV0R3JvdXBOYW1lPzogc3RyaW5nO1xufVxuXG5mdW5jdGlvbiBzZXR1cFZwYyhwYXJlbnQ6IGFueSwgcHJvcHM6IFJlZGlzREJQcm9wcykgOiBlYzIuSVZwYyB7XG4gIHJldHVybiBwcm9wcy5leGlzdGluZ1ZwYyA/PyBuZXcgZWMyLlZwYyhwYXJlbnQsICdWcGMnLCB7XG4gICAgc3VibmV0Q29uZmlndXJhdGlvbjogW1xuICAgICAge1xuICAgICAgICBjaWRyTWFzazogMjQsXG4gICAgICAgIG5hbWU6ICdQdWJsaWMgU3VibmV0JyxcbiAgICAgICAgc3VibmV0VHlwZTogZWMyLlN1Ym5ldFR5cGUuUFVCTElDLFxuICAgICAgfSxcbiAgICAgIHtcbiAgICAgICAgY2lkck1hc2s6IDI0LFxuICAgICAgICBuYW1lOiAnSXNvbGF0ZWQgU3VibmV0JyxcbiAgICAgICAgc3VibmV0VHlwZTogZWMyLlN1Ym5ldFR5cGUuUFJJVkFURV9JU09MQVRFRCxcbiAgICAgIH0sXG4gICAgXSxcbiAgfSk7XG59XG5cbmV4cG9ydCBjbGFzcyBSZWRpc0RCIGV4dGVuZHMgQ29uc3RydWN0IHtcbiAgcHVibGljIHJlYWRvbmx5IHJlcGxpY2F0aW9uR3JvdXAgOiBlbGFzdGljYWNoZS5DZm5SZXBsaWNhdGlvbkdyb3VwO1xuICBwdWJsaWMgcmVhZG9ubHkgdnBjIDogZWMyLklWcGM7XG4gIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHByb3BzOiBSZWRpc0RCUHJvcHMgPSB7fSkge1xuICAgIHN1cGVyKHNjb3BlLCBpZCk7XG5cbiAgICBsZXQgaXNvbGF0ZWRTdWJuZXRzOiBzdHJpbmdbXSA9IFtdO1xuICAgIGxldCByZWRpc1ZwYyA9IHNldHVwVnBjKHRoaXMsIHByb3BzKTtcbiAgICB0aGlzLnZwYyA9IHJlZGlzVnBjO1xuICAgIHJlZGlzVnBjLmlzb2xhdGVkU3VibmV0cy5mb3JFYWNoKGZ1bmN0aW9uKHZhbHVlKSB7XG4gICAgICBpc29sYXRlZFN1Ym5ldHMucHVzaCh2YWx1ZS5zdWJuZXRJZCk7XG4gICAgfSk7XG4gICAgaWYgKGlzb2xhdGVkU3VibmV0cy5sZW5ndGggPT0gMCkge1xuICAgICAgcmVkaXNWcGMucHJpdmF0ZVN1Ym5ldHMuZm9yRWFjaChmdW5jdGlvbih2YWx1ZSkge1xuICAgICAgICBpc29sYXRlZFN1Ym5ldHMucHVzaCh2YWx1ZS5zdWJuZXRJZCk7XG4gICAgICB9KTtcbiAgICB9XG4gICAgY29uc3QgZWNTZWN1cml0eUdyb3VwID0gcHJvcHMuZXhpc3RpbmdTZWN1cml0eUdyb3VwID8/IG5ldyBlYzIuU2VjdXJpdHlHcm91cCh0aGlzLCBpZCArICctUmVkaXNEQi1TRycsIHtcbiAgICAgIHZwYzogcmVkaXNWcGMsXG4gICAgICBkZXNjcmlwdGlvbjogJ1NlY3VyaXR5R3JvdXAgYXNzb2NpYXRlZCB3aXRoIFJlZGlzREIgQ2x1c3RlciAnICsgaWQsXG4gICAgICBhbGxvd0FsbE91dGJvdW5kOiBmYWxzZSxcbiAgICB9KTtcbiAgICBsZXQgZ3JvdXBOYW1lOiBzdHJpbmc7XG4gICAgbGV0IGVjU3VibmV0R3JvdXA6IGVsYXN0aWNhY2hlLkNmblN1Ym5ldEdyb3VwO1xuICAgIGlmICghcHJvcHMuZXhpc3RpbmdTdWJuZXRHcm91cE5hbWUpIHtcbiAgICAgIGVjU3VibmV0R3JvdXAgPSBuZXcgZWxhc3RpY2FjaGUuQ2ZuU3VibmV0R3JvdXAodGhpcywgaWQgKyAnLVJlZGlzREItU3VibmV0R3JvdXAnLCB7XG4gICAgICAgIGRlc2NyaXB0aW9uOiAnUmVkaXNEQiBTdWJuZXQgR3JvdXAnLFxuICAgICAgICBzdWJuZXRJZHM6IGlzb2xhdGVkU3VibmV0cyxcbiAgICAgICAgY2FjaGVTdWJuZXRHcm91cE5hbWU6IHByb3BzLnN1Ym5ldEdyb3VwTmFtZSB8fCAnUmVkaXNEQlN1Ym5ldEdyb3VwJyxcbiAgICAgIH0pO1xuICAgICAgZ3JvdXBOYW1lID0gZWNTdWJuZXRHcm91cC5jYWNoZVN1Ym5ldEdyb3VwTmFtZSE7XG4gICAgfSBlbHNlIHtcbiAgICAgIGdyb3VwTmFtZSA9IHByb3BzLmV4aXN0aW5nU3VibmV0R3JvdXBOYW1lITtcbiAgICB9XG5cbiAgICBsZXQgZWxhc3RpY2FjaGVSZXBsaWNhdGlvbkdyb3VwTmFtZSA9IGlkICsgJy1SZWRpc0RCJztcbiAgICBsZXQgcmVkaXNfY2x1c3RlciA9IG5ldyBlbGFzdGljYWNoZS5DZm5SZXBsaWNhdGlvbkdyb3VwKHRoaXMsIGVsYXN0aWNhY2hlUmVwbGljYXRpb25Hcm91cE5hbWUsIHtcbiAgICAgIG51bU5vZGVHcm91cHM6IHByb3BzLm5vZGVzIHx8IDEsXG4gICAgICBjYWNoZU5vZGVUeXBlOiBwcm9wcy5ub2RlVHlwZSB8fCAnY2FjaGUubTZnLmxhcmdlJyxcbiAgICAgIGVuZ2luZTogJ1JlZGlzJyxcbiAgICAgIG11bHRpQXpFbmFibGVkOiBmYWxzZSxcbiAgICAgIGF1dG9NaW5vclZlcnNpb25VcGdyYWRlOiBmYWxzZSxcbiAgICAgIGNhY2hlUGFyYW1ldGVyR3JvdXBOYW1lOiBwcm9wcy5wYXJhbWV0ZXJHcm91cE5hbWUgPz8gJ2RlZmF1bHQucmVkaXM3LmNsdXN0ZXIub24nLFxuICAgICAgZW5naW5lVmVyc2lvbjogcHJvcHMuZW5naW5lVmVyc2lvbiA/PyAnNy4wJyxcbiAgICAgIGNhY2hlU3VibmV0R3JvdXBOYW1lOiBncm91cE5hbWUsXG4gICAgICBzZWN1cml0eUdyb3VwSWRzOiBbZWNTZWN1cml0eUdyb3VwLnNlY3VyaXR5R3JvdXBJZF0sXG4gICAgICByZXBsaWNhdGlvbkdyb3VwRGVzY3JpcHRpb246ICdSZWRpc0RCIHNldHVwIGJ5IENESycsXG4gICAgICBhdFJlc3RFbmNyeXB0aW9uRW5hYmxlZDogcHJvcHMuYXRSZXN0RW5jcnlwdGlvbkVuYWJsZWQsXG4gICAgICB0cmFuc2l0RW5jcnlwdGlvbkVuYWJsZWQ6IHByb3BzLnRyYW5zaXRFbmNyeXB0aW9uRW5hYmxlZCxcbiAgICAgIHJlcGxpY2FzUGVyTm9kZUdyb3VwOiBwcm9wcy5yZXBsaWNhcyB8fCAwLFxuICAgICAgYXV0aFRva2VuOiBwcm9wcy5hdXRoVG9rZW4sXG4gICAgfSk7XG4gICAgdGhpcy5yZXBsaWNhdGlvbkdyb3VwID0gcmVkaXNfY2x1c3RlcjtcbiAgICBpZiAoIXByb3BzLmV4aXN0aW5nU3VibmV0R3JvdXBOYW1lKSB7XG4gICAgICByZWRpc19jbHVzdGVyLm5vZGUuYWRkRGVwZW5kZW5jeShlY1N1Ym5ldEdyb3VwISk7XG4gICAgfVxuICAgIGlmICh0eXBlb2YgcHJvcHMubWVtb3J5QXV0b3NjYWxpbmdUYXJnZXQgPT0gJ251bWJlcicpIHtcbiAgICAgIGNvbnN0IHRhcmdldCA9IG5ldyBhcHBzY2FsaW5nLlNjYWxhYmxlVGFyZ2V0KHRoaXMsICdTY2FsYWJsZVRhcmdldCcsIHtcbiAgICAgICAgc2VydmljZU5hbWVzcGFjZTogYXBwc2NhbGluZy5TZXJ2aWNlTmFtZXNwYWNlLkVMQVNUSUNBQ0hFLFxuICAgICAgICByZXNvdXJjZUlkOiAncmVwbGljYXRpb24tZ3JvdXAvJyArIHJlZGlzX2NsdXN0ZXIucmVmLFxuICAgICAgICBzY2FsYWJsZURpbWVuc2lvbjogJ2VsYXN0aWNhY2hlOnJlcGxpY2F0aW9uLWdyb3VwOk5vZGVHcm91cHMnLFxuICAgICAgICBtYXhDYXBhY2l0eTogcHJvcHMubm9kZXN8fDEgKjMsXG4gICAgICAgIG1pbkNhcGFjaXR5OiBwcm9wcy5ub2Rlc3x8MSxcbiAgICAgIH0pO1xuICAgICAgdGFyZ2V0LnNjYWxlVG9UcmFja01ldHJpYygnTWVtVHJhY2tpbmcnLCB7XG4gICAgICAgIHRhcmdldFZhbHVlOiBwcm9wcy5tZW1vcnlBdXRvc2NhbGluZ1RhcmdldCxcbiAgICAgICAgcHJlZGVmaW5lZE1ldHJpYzogYXBwc2NhbGluZy5QcmVkZWZpbmVkTWV0cmljLkVMQVNUSUNBQ0hFX0RBVEFCQVNFX01FTU9SWV9VU0FHRV9DT1VOVEVEX0ZPUl9FVklDVF9QRVJDRU5UQUdFLFxuICAgICAgfSk7XG4gICAgfSBlbHNlIGlmICh0eXBlb2YgcHJvcHMucmVwbGljYXNDcHVBdXRvc2NhbGluZ1RhcmdldCA9PSAnbnVtYmVyJykge1xuICAgICAgY29uc3QgdGFyZ2V0ID0gbmV3IGFwcHNjYWxpbmcuU2NhbGFibGVUYXJnZXQodGhpcywgJ1NjYWxhYmxlVGFyZ2V0Jywge1xuICAgICAgICBzZXJ2aWNlTmFtZXNwYWNlOiBhcHBzY2FsaW5nLlNlcnZpY2VOYW1lc3BhY2UuRUxBU1RJQ0FDSEUsXG4gICAgICAgIHJlc291cmNlSWQ6ICdyZXBsaWNhdGlvbi1ncm91cC8nICsgcmVkaXNfY2x1c3Rlci5yZWYsXG4gICAgICAgIHNjYWxhYmxlRGltZW5zaW9uOiAnZWxhc3RpY2FjaGU6cmVwbGljYXRpb24tZ3JvdXA6Z3JvdXA6UmVwbGljYXMnLFxuICAgICAgICBtYXhDYXBhY2l0eTogcHJvcHMubm9kZXN8fDEgKjMsXG4gICAgICAgIG1pbkNhcGFjaXR5OiBwcm9wcy5ub2Rlc3x8MSxcbiAgICAgIH0pO1xuICAgICAgdGFyZ2V0LnNjYWxlVG9UcmFja01ldHJpYygnQ3B1VHJhY2tpbmcnLCB7XG4gICAgICAgIHRhcmdldFZhbHVlOiBwcm9wcy5yZXBsaWNhc0NwdUF1dG9zY2FsaW5nVGFyZ2V0LFxuICAgICAgICBwcmVkZWZpbmVkTWV0cmljOiBhcHBzY2FsaW5nLlByZWRlZmluZWRNZXRyaWMuRUxBU1RJQ0FDSEVfUFJJTUFSWV9FTkdJTkVfQ1BVX1VUSUxJWkFUSU9OLFxuICAgICAgfSk7XG4gICAgfSBlbHNlIGlmICh0eXBlb2YgcHJvcHMubm9kZXNDcHVBdXRvc2NhbGluZ1RhcmdldCA9PSAnbnVtYmVyJykge1xuICAgICAgY29uc3QgdGFyZ2V0ID0gbmV3IGFwcHNjYWxpbmcuU2NhbGFibGVUYXJnZXQodGhpcywgJ1NjYWxhYmxlVGFyZ2V0Jywge1xuICAgICAgICBzZXJ2aWNlTmFtZXNwYWNlOiBhcHBzY2FsaW5nLlNlcnZpY2VOYW1lc3BhY2UuRUxBU1RJQ0FDSEUsXG4gICAgICAgIHJlc291cmNlSWQ6ICdyZXBsaWNhdGlvbi1ncm91cC8nICsgcmVkaXNfY2x1c3Rlci5yZWYsXG4gICAgICAgIHNjYWxhYmxlRGltZW5zaW9uOiAnZWxhc3RpY2FjaGU6cmVwbGljYXRpb24tZ3JvdXA6Tm9kZUdyb3VwcycsXG4gICAgICAgIG1heENhcGFjaXR5OiBwcm9wcy5ub2Rlc3x8MSAqMyxcbiAgICAgICAgbWluQ2FwYWNpdHk6IHByb3BzLm5vZGVzfHwxLFxuICAgICAgfSk7XG4gICAgICB0YXJnZXQuc2NhbGVUb1RyYWNrTWV0cmljKCdDcHVUcmFja2luZycsIHtcbiAgICAgICAgdGFyZ2V0VmFsdWU6IHByb3BzLm5vZGVzQ3B1QXV0b3NjYWxpbmdUYXJnZXQsXG4gICAgICAgIHByZWRlZmluZWRNZXRyaWM6IGFwcHNjYWxpbmcuUHJlZGVmaW5lZE1ldHJpYy5FTEFTVElDQUNIRV9QUklNQVJZX0VOR0lORV9DUFVfVVRJTElaQVRJT04sXG4gICAgICB9KTtcbiAgICB9XG4gIH1cbn1cblxuZXhwb3J0IGNsYXNzIE1lbW9yeURCIGV4dGVuZHMgQ29uc3RydWN0IHtcbiAgcHVibGljIHJlYWRvbmx5IGNsdXN0ZXIgOiBtZW1vcnlkYi5DZm5DbHVzdGVyO1xuICBwdWJsaWMgcmVhZG9ubHkgdnBjIDogZWMyLklWcGM7XG4gIGNvbnN0cnVjdG9yKHNjb3BlOiBDb25zdHJ1Y3QsIGlkOiBzdHJpbmcsIHByb3BzOiBSZWRpc0RCUHJvcHMgPSB7fSkge1xuICAgIHN1cGVyKHNjb3BlLCBpZCk7XG4gICAgbGV0IGlzb2xhdGVkU3VibmV0czogc3RyaW5nW10gPSBbXTtcbiAgICBsZXQgcmVkaXNWcGMgPSBzZXR1cFZwYyh0aGlzLCBwcm9wcyk7XG4gICAgdGhpcy52cGMgPSByZWRpc1ZwYztcbiAgICByZWRpc1ZwYy5pc29sYXRlZFN1Ym5ldHMuZm9yRWFjaChmdW5jdGlvbih2YWx1ZSkge1xuICAgICAgaXNvbGF0ZWRTdWJuZXRzLnB1c2godmFsdWUuc3VibmV0SWQpO1xuICAgIH0pO1xuICAgIGNvbnN0IGVjU2VjdXJpdHlHcm91cCA9IHByb3BzLmV4aXN0aW5nU2VjdXJpdHlHcm91cCA/PyBuZXcgZWMyLlNlY3VyaXR5R3JvdXAodGhpcywgaWQgKyAnLVJlZGlzREItU0cnLCB7XG4gICAgICB2cGM6IHJlZGlzVnBjLFxuICAgICAgZGVzY3JpcHRpb246ICdTZWN1cml0eUdyb3VwIGFzc29jaWF0ZWQgd2l0aCBSZWRpc0RCIENsdXN0ZXIgJyArIGlkLFxuICAgICAgYWxsb3dBbGxPdXRib3VuZDogZmFsc2UsXG4gICAgfSk7XG4gICAgbGV0IGdyb3VwTmFtZTogc3RyaW5nO1xuICAgIGxldCBlY1N1Ym5ldEdyb3VwOiBtZW1vcnlkYi5DZm5TdWJuZXRHcm91cDtcbiAgICBpZiAoIXByb3BzLmV4aXN0aW5nU3VibmV0R3JvdXBOYW1lKSB7XG4gICAgICBlY1N1Ym5ldEdyb3VwID0gbmV3IG1lbW9yeWRiLkNmblN1Ym5ldEdyb3VwKHRoaXMsIGlkICsgJy1SZWRpc0RCLVN1Ym5ldEdyb3VwJywge1xuICAgICAgICBkZXNjcmlwdGlvbjogJ1JlZGlzREIgU3VibmV0IEdyb3VwJyxcbiAgICAgICAgc3VibmV0SWRzOiBpc29sYXRlZFN1Ym5ldHMsXG4gICAgICAgIHN1Ym5ldEdyb3VwTmFtZTogcHJvcHMuc3VibmV0R3JvdXBOYW1lIHx8ICdtZW1vcnlkYnN1Ym5ldGdyb3VwJyxcbiAgICAgIH0pO1xuICAgICAgZ3JvdXBOYW1lID0gZWNTdWJuZXRHcm91cC5zdWJuZXRHcm91cE5hbWUhO1xuICAgIH0gZWxzZSB7XG4gICAgICBncm91cE5hbWUgPSBwcm9wcy5leGlzdGluZ1N1Ym5ldEdyb3VwTmFtZSE7XG4gICAgfVxuXG4gICAgLypcbiAgICBjb25zdCBjZm5Vc2VyID0gbmV3IG1lbW9yeWRiLkNmblVzZXIodGhpcywgJ21lbW9yeWRiLXVzZXInLCB7XG4gICAgICBhY2Nlc3NTdHJpbmc6ICdvbiB+KiArQGFsbCcsXG4gICAgICBhdXRoZW50aWNhdGlvbk1vZGU6IHtcIlBhc3N3b3Jkc1wiOltcIioqKioqaHVudGVyMioqKioqXCJdLFwiVHlwZVwiOlwicGFzc3dvcmRcIn0sXG4gICAgICB1c2VyTmFtZTogJ2FkbWluJyxcbiAgICB9KTtcbiAgICBjb25zdCBjZm5BQ0wgPSBuZXcgbWVtb3J5ZGIuQ2ZuQUNMKHRoaXMsICdtZW1vcnlkYi1hY2wnLCB7XG4gICAgICBhY2xOYW1lOiAnbXlhY2wnLFxuICAgICAgdXNlck5hbWVzOiBbJ2FkbWluJ10sXG4gICAgfSk7XG4gICAgKi9cbiAgICBjb25zdCBtZW1vcnlkYl9jbHVzdGVyID0gbmV3IG1lbW9yeWRiLkNmbkNsdXN0ZXIodGhpcywgJ21lbW9yeWRiJywge1xuICAgICAgYWNsTmFtZTogJ29wZW4tYWNjZXNzJyxcbiAgICAgIGNsdXN0ZXJOYW1lOiAnY2x1c3Rlcm5hbWUnLFxuICAgICAgbm9kZVR5cGU6IHByb3BzLm5vZGVUeXBlIHx8ICdkYi50NGcuc21hbGwnLFxuXG4gICAgICBhdXRvTWlub3JWZXJzaW9uVXBncmFkZTogZmFsc2UsXG4gICAgICBkZXNjcmlwdGlvbjogJ2Rlc2NyaXB0aW9uJyxcbiAgICAgIGVuZ2luZVZlcnNpb246IHByb3BzLmVuZ2luZVZlcnNpb24gPz8gJzcuMCcsXG4gICAgICBudW1TaGFyZHM6IHByb3BzLm5vZGVzfHwxLFxuICAgICAgbnVtUmVwbGljYXNQZXJTaGFyZDogcHJvcHMucmVwbGljYXN8fDAsXG4gICAgICBzZWN1cml0eUdyb3VwSWRzOiBbZWNTZWN1cml0eUdyb3VwLnNlY3VyaXR5R3JvdXBJZF0sXG4gICAgICBzdWJuZXRHcm91cE5hbWU6IGdyb3VwTmFtZSxcbiAgICAgIHRsc0VuYWJsZWQ6IHRydWUsXG4gICAgfSk7XG4gICAgaWYgKCFwcm9wcy5leGlzdGluZ1N1Ym5ldEdyb3VwTmFtZSkge1xuICAgICAgbWVtb3J5ZGJfY2x1c3Rlci5ub2RlLmFkZERlcGVuZGVuY3koZWNTdWJuZXRHcm91cCEpO1xuICAgIH1cbiAgICB0aGlzLmNsdXN0ZXIgPSBtZW1vcnlkYl9jbHVzdGVyO1xuICAgIC8vbWVtb3J5ZGJfY2x1c3Rlci5ub2RlLmFkZERlcGVuZGVuY3koY2ZuQUNMKTtcbiAgICAvL2NmbkFDTC5ub2RlLmFkZERlcGVuZGVuY3koY2ZuVXNlcik7XG4gIH1cbn1cbiJdfQ==
```

##### package/package.json

###### Pretty-printed

 * *Similarity: 0.9699197860962566%*

 * *Differences: {"'devDependencies'": "{'projen': '^0.71.66'}", "'version'": "'0.0.24'"}*

```diff
@@ -21,15 +21,15 @@
         "jest": "^27",
         "jest-junit": "^15",
         "jsii": "1.x",
         "jsii-diff": "^1.81.0",
         "jsii-docgen": "^7.2.9",
         "jsii-pacmak": "^1.81.0",
         "npm-check-updates": "^16",
-        "projen": "^0.71.64",
+        "projen": "^0.71.66",
         "standard-version": "^9",
         "ts-jest": "^27",
         "typescript": "^5.0.4"
     },
     "jest": {
         "clearMocks": true,
         "collectCoverage": true,
@@ -124,9 +124,9 @@
         "test:watch": "npx projen test:watch",
         "unbump": "npx projen unbump",
         "upgrade": "npx projen upgrade",
         "watch": "npx projen watch"
     },
     "stability": "stable",
     "types": "lib/index.d.ts",
-    "version": "0.0.23"
+    "version": "0.0.24"
 }
```

### Comparing `cdk-redisdb-0.0.23/src/cdk_redisdb.egg-info/PKG-INFO` & `cdk-redisdb-0.0.24/src/cdk_redisdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-redisdb
-Version: 0.0.23
+Version: 0.0.24
 Summary: Simple & featureful Redis on AWS - Elasticache Replication Group & MemoryDB with a unified API
 Home-page: https://github.com/forkfork/cdk-redisdb.git
 Author: Timothy Downs<timothydowns@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/forkfork/cdk-redisdb.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

