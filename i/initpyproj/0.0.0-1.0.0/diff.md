# Comparing `tmp/initpyproj-0.0.0-py3-none-any.whl.zip` & `tmp/initpyproj-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
 Zip file size: 4260 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     7936 b- defN 23-May-18 17:46 initpyproj.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-May-18 17:48 initpyproj-0.0.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      930 b- defN 23-May-18 17:48 initpyproj-0.0.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-18 17:48 initpyproj-0.0.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       21 b- defN 23-May-18 17:48 initpyproj-0.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      470 b- defN 23-May-18 17:48 initpyproj-0.0.0.dist-info/RECORD
-6 files, 10526 bytes uncompressed, 3408 bytes compressed:  67.6%
+-rw-rw-rw-  2.0 fat     7946 b- defN 23-May-22 20:19 initpyproj.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-May-22 20:21 initpyproj-1.0.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      930 b- defN 23-May-22 20:21 initpyproj-1.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-22 20:21 initpyproj-1.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       21 b- defN 23-May-22 20:21 initpyproj-1.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      470 b- defN 23-May-22 20:21 initpyproj-1.0.0.dist-info/RECORD
+6 files, 10536 bytes uncompressed, 3408 bytes compressed:  67.7%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: initpyproj.py
 Comment: 
 
-Filename: initpyproj-0.0.0.dist-info/LICENSE
+Filename: initpyproj-1.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: initpyproj-0.0.0.dist-info/METADATA
+Filename: initpyproj-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: initpyproj-0.0.0.dist-info/WHEEL
+Filename: initpyproj-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: initpyproj-0.0.0.dist-info/top_level.txt
+Filename: initpyproj-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: initpyproj-0.0.0.dist-info/RECORD
+Filename: initpyproj-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## initpyproj.py

```diff
@@ -113,15 +113,15 @@
                    "--keywords",
                    help="some keywords for the python project",
                    nargs="*")
     p.add_argument("-dir",
                    "--parent-dir",
                    help="the parent dir of the python project, if omitted the current working directory is used",
                    dest="dir")
-    git_group = p.add_argument_group()
+    git_group = p.add_mutually_exclusive_group()
     git_group.add_argument("--no-git",
                            help="will not create a local git repo (and no GitHub repo)",
                            action="store_false",
                            dest="git")
     git_group.add_argument("--no-GitHub",
                            help="will create a local git repo but no GitHub repo",
                            action="store_false",
```

## Comparing `initpyproj-0.0.0.dist-info/LICENSE` & `initpyproj-1.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `initpyproj-0.0.0.dist-info/METADATA` & `initpyproj-1.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: initpyproj
-Version: 0.0.0
+Version: 1.0.0
 Summary: Initialize an empty python project; make it a git repo; and sync it with a new GitHub repo
 Home-page: https://github.com/Schnilsibus/initpyproj
 Author: Nils Urbach
 Author-email: ndu01u@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

