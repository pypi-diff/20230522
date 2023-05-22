# Comparing `tmp/kthutils-1.1.tar.gz` & `tmp/kthutils-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kthutils-1.1.tar", max compression
+gzip compressed data, was "kthutils-1.2.tar", max compression
```

## Comparing `kthutils-1.1.tar` & `kthutils-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-03-28 06:51:16.830958 kthutils-1.1/LICENSE
--rw-r--r--   0        0        0      921 2023-03-28 08:50:20.937172 kthutils-1.1/README.md
--rw-r--r--   0        0        0      721 2023-04-27 18:35:31.070513 kthutils-1.1/pyproject.toml
--rw-r--r--   0        0        0       56 2023-03-28 06:51:16.830958 kthutils-1.1/src/kthutils/.gitignore
--rw-r--r--   0        0        0      268 2023-03-28 06:51:16.830958 kthutils-1.1/src/kthutils/Makefile
--rw-r--r--   0        0        0        0 2022-11-07 09:18:59.264876 kthutils-1.1/src/kthutils/__init__.py
--rw-r--r--   0        0        0     3441 2023-03-28 06:51:16.834959 kthutils-1.1/src/kthutils/cli.nw
--rw-r--r--   0        0        0      281 2023-04-27 18:36:23.514363 kthutils-1.1/src/kthutils/cli.py
--rw-r--r--   0        0        0      770 2023-04-27 18:36:23.514363 kthutils-1.1/src/kthutils/credentials.py
--rw-r--r--   0        0        0    16503 2023-03-28 08:32:20.170796 kthutils-1.1/src/kthutils/ug.nw
--rw-r--r--   0        0        0     8343 2023-04-27 18:36:23.518363 kthutils-1.1/src/kthutils/ug.py
--rw-r--r--   0        0        0      745 2023-03-28 08:50:25.909228 kthutils-1.1/tests/test_ug.py
--rw-r--r--   0        0        0     1880 1970-01-01 00:00:00.000000 kthutils-1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-28 06:51:16.830958 kthutils-1.2/LICENSE
+-rw-r--r--   0        0        0      921 2023-03-28 08:50:20.937172 kthutils-1.2/README.md
+-rw-r--r--   0        0        0      721 2023-05-22 13:22:56.490253 kthutils-1.2/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-03-28 06:51:16.830958 kthutils-1.2/src/kthutils/.gitignore
+-rw-r--r--   0        0        0      268 2023-03-28 06:51:16.830958 kthutils-1.2/src/kthutils/Makefile
+-rw-r--r--   0        0        0        0 2022-11-07 09:18:59.264876 kthutils-1.2/src/kthutils/__init__.py
+-rw-r--r--   0        0        0     3441 2023-03-28 06:51:16.834959 kthutils-1.2/src/kthutils/cli.nw
+-rw-r--r--   0        0        0      281 2023-04-27 18:36:23.514363 kthutils-1.2/src/kthutils/cli.py
+-rw-r--r--   0        0        0      770 2023-04-27 18:36:23.514363 kthutils-1.2/src/kthutils/credentials.py
+-rw-r--r--   0        0        0    16807 2023-05-22 13:22:37.453672 kthutils-1.2/src/kthutils/ug.nw
+-rw-r--r--   0        0        0     8414 2023-05-22 13:23:19.007254 kthutils-1.2/src/kthutils/ug.py
+-rw-r--r--   0        0        0      745 2023-05-22 13:23:19.227229 kthutils-1.2/tests/test_ug.py
+-rw-r--r--   0        0        0     1880 1970-01-01 00:00:00.000000 kthutils-1.2/PKG-INFO
```

### Comparing `kthutils-1.1/LICENSE` & `kthutils-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kthutils-1.1/README.md` & `kthutils-1.2/README.md`

 * *Files identical despite different names*

### Comparing `kthutils-1.1/pyproject.toml` & `kthutils-1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kthutils"
-version = "1.1"
+version = "1.2"
 description = "Various tools for automation at KTH"
 authors = ["Daniel Bosk <dbosk@kth.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbosk/kthutils"
 include = ["*/**/*.py"]
```

### Comparing `kthutils-1.1/src/kthutils/cli.nw` & `kthutils-1.2/src/kthutils/cli.nw`

 * *Files identical despite different names*

### Comparing `kthutils-1.1/src/kthutils/credentials.py` & `kthutils-1.2/src/kthutils/credentials.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.1/src/kthutils/ug.nw` & `kthutils-1.2/src/kthutils/ug.nw`

 * *Files 2% similar despite different names*

```diff
@@ -425,21 +425,30 @@
 @
 
 When printing the members, we don't want to print each member's JSON 
 object.
 We want something more useful for the terminal.
 We print tab-separated fields of data, so that we can use grep(1), cut(1) and 
 join(1).
+
+We also note that we must treat the title attribute differently.
+The title attribute can sometimes contain empty lists.
+(Also interesting about the title attribute is that despite being a list, it 
+always seem to contain only one element.)
 <<clean and print members>>=
 for member in ug.list_group_members(group_kthid):
+  try:
+    title = member['title']['en'][0]
+  except IndexError:
+    title = None
   print(f"{member['username']}"
         f"\t{member['kthid']}"
         f"\t{member['givenName']}"
         f"\t{member['surname']}"
-        f"\t{member['title']['en'][0]}")
+        f"\t{title}")
 @
 
 
 \subsection{Set members of a group}
 
 The API doesn't allow us to add or remove individual users.
 It only allows us to set a new members list.
```

### Comparing `kthutils-1.1/src/kthutils/ug.py` & `kthutils-1.2/src/kthutils/ug.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,19 +208,23 @@
   """
   Returns a list of the members of a group.
   The list contains JSON objects.
   """
   ug = UGsession(*kthutils.credentials.get_credentials())
   group_kthid = ug.group_name_to_kthid(group_name)
   for member in ug.list_group_members(group_kthid):
+    try:
+      title = member['title']['en'][0]
+    except IndexError:
+      title = None
     print(f"{member['username']}"
           f"\t{member['kthid']}"
           f"\t{member['givenName']}"
           f"\t{member['surname']}"
-          f"\t{member['title']['en'][0]}")
+          f"\t{title}")
 @members.command(name="set")
 def cli_set_members(group_name: str = group_name_arg,
                     users: typing.List[str] = user_list_arg):
   """
   Sets the members of a group. Any existing members not in the list will be 
   removed.
   """
```

### Comparing `kthutils-1.1/tests/test_ug.py` & `kthutils-1.2/tests/test_ug.py`

 * *Files identical despite different names*

### Comparing `kthutils-1.1/PKG-INFO` & `kthutils-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kthutils
-Version: 1.1
+Version: 1.2
 Summary: Various tools for automation at KTH
 Home-page: https://github.com/dbosk/kthutils
 License: MIT
 Author: Daniel Bosk
 Author-email: dbosk@kth.se
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

