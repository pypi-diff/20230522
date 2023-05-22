# Comparing `tmp/stringtokenizer-1.1.2.tar.gz` & `tmp/stringtokenizer-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringtokenizer-1.1.2.tar", last modified: Sun May 21 05:54:25 2023, max compression
+gzip compressed data, was "stringtokenizer-1.1.3.tar", last modified: Mon May 22 08:49:04 2023, max compression
```

## Comparing `stringtokenizer-1.1.2.tar` & `stringtokenizer-1.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-21 05:54:25.678735 stringtokenizer-1.1.2/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1464 2023-05-21 05:54:25.678442 stringtokenizer-1.1.2/PKG-INFO
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      953 2023-05-21 05:54:17.000000 stringtokenizer-1.1.2/README.md
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       38 2023-05-21 05:54:25.678821 stringtokenizer-1.1.2/setup.cfg
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      448 2023-05-21 05:50:46.000000 stringtokenizer-1.1.2/setup.py
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-21 05:54:25.675643 stringtokenizer-1.1.2/stringtokenizer/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       46 2023-05-17 18:44:19.000000 stringtokenizer-1.1.2/stringtokenizer/__init__.py
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1595 2023-05-21 05:49:54.000000 stringtokenizer-1.1.2/stringtokenizer/stringtokenizer.py
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-21 05:54:25.677532 stringtokenizer-1.1.2/stringtokenizer.egg-info/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1464 2023-05-21 05:54:25.000000 stringtokenizer-1.1.2/stringtokenizer.egg-info/PKG-INFO
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      237 2023-05-21 05:54:25.000000 stringtokenizer-1.1.2/stringtokenizer.egg-info/SOURCES.txt
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        1 2023-05-21 05:54:25.000000 stringtokenizer-1.1.2/stringtokenizer.egg-info/dependency_links.txt
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       16 2023-05-21 05:54:25.000000 stringtokenizer-1.1.2/stringtokenizer.egg-info/top_level.txt
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-22 08:49:04.304425 stringtokenizer-1.1.3/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1500 2023-05-22 08:49:04.303981 stringtokenizer-1.1.3/PKG-INFO
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      953 2023-05-21 05:54:17.000000 stringtokenizer-1.1.3/README.md
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       38 2023-05-22 08:49:04.304525 stringtokenizer-1.1.3/setup.cfg
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      513 2023-05-22 08:48:40.000000 stringtokenizer-1.1.3/setup.py
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-22 08:49:04.301788 stringtokenizer-1.1.3/stringtokenizer/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       46 2023-05-17 18:44:19.000000 stringtokenizer-1.1.3/stringtokenizer/__init__.py
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1595 2023-05-21 05:49:54.000000 stringtokenizer-1.1.3/stringtokenizer/stringtokenizer.py
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-22 08:49:04.303464 stringtokenizer-1.1.3/stringtokenizer.egg-info/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1500 2023-05-22 08:49:04.000000 stringtokenizer-1.1.3/stringtokenizer.egg-info/PKG-INFO
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      237 2023-05-22 08:49:04.000000 stringtokenizer-1.1.3/stringtokenizer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        1 2023-05-22 08:49:04.000000 stringtokenizer-1.1.3/stringtokenizer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       16 2023-05-22 08:49:04.000000 stringtokenizer-1.1.3/stringtokenizer.egg-info/top_level.txt
```

### Comparing `stringtokenizer-1.1.2/PKG-INFO` & `stringtokenizer-1.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: stringtokenizer
-Version: 1.1.2
+Version: 1.1.3
 Summary: A string tokenizer implementation
 Home-page: UNKNOWN
 Author: Tanmay Mandal
-License: UNKNOWN
+Author-email: tanmay.mandal@zohomail.in
+License: MIT
 Description: **This project is a python implementation of the StringTokenizer class present in java**
         
         
         __How to import ?__
         
         from stringtokenizer import StringTokenizer
```

### Comparing `stringtokenizer-1.1.2/README.md` & `stringtokenizer-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `stringtokenizer-1.1.2/stringtokenizer/stringtokenizer.py` & `stringtokenizer-1.1.3/stringtokenizer/stringtokenizer.py`

 * *Files identical despite different names*

### Comparing `stringtokenizer-1.1.2/stringtokenizer.egg-info/PKG-INFO` & `stringtokenizer-1.1.3/stringtokenizer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: stringtokenizer
-Version: 1.1.2
+Version: 1.1.3
 Summary: A string tokenizer implementation
 Home-page: UNKNOWN
 Author: Tanmay Mandal
-License: UNKNOWN
+Author-email: tanmay.mandal@zohomail.in
+License: MIT
 Description: **This project is a python implementation of the StringTokenizer class present in java**
         
         
         __How to import ?__
         
         from stringtokenizer import StringTokenizer
```

