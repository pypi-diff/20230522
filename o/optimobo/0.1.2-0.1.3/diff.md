# Comparing `tmp/optimobo-0.1.2.tar.gz` & `tmp/optimobo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimobo-0.1.2.tar", last modified: Mon May 22 12:04:03 2023, max compression
+gzip compressed data, was "optimobo-0.1.3.tar", last modified: Mon May 22 12:09:36 2023, max compression
```

## Comparing `optimobo-0.1.2.tar` & `optimobo-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:04:03.970973 optimobo-0.1.2/
--rw-rw-r--   0 lecky     (1000) lecky     (1000)     1063 2023-05-20 14:55:19.000000 optimobo-0.1.2/LICENSE
--rw-rw-r--   0 lecky     (1000) lecky     (1000)      205 2023-05-22 12:04:03.970973 optimobo-0.1.2/PKG-INFO
--rw-rw-r--   0 lecky     (1000) lecky     (1000)     3443 2023-05-20 19:14:19.000000 optimobo-0.1.2/README.md
-drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:04:03.970973 optimobo-0.1.2/optimobo/
--rw-rw-r--   0 lecky     (1000) lecky     (1000)        0 2023-05-22 11:49:17.000000 optimobo-0.1.2/optimobo/__init__.py
--rw-rw-r--   0 lecky     (1000) lecky     (1000)    16114 2023-05-20 15:16:09.000000 optimobo-0.1.2/optimobo/optimisers.py
--rw-rw-r--   0 lecky     (1000) lecky     (1000)     7822 2023-05-20 14:58:32.000000 optimobo-0.1.2/optimobo/scalarisations.py
--rw-rw-r--   0 lecky     (1000) lecky     (1000)    11483 2023-05-18 23:42:13.000000 optimobo-0.1.2/optimobo/util_functions.py
-drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:04:03.970973 optimobo-0.1.2/optimobo.egg-info/
--rw-rw-r--   0 lecky     (1000) lecky     (1000)      205 2023-05-22 12:04:03.000000 optimobo-0.1.2/optimobo.egg-info/PKG-INFO
--rw-rw-r--   0 lecky     (1000) lecky     (1000)      300 2023-05-22 12:04:03.000000 optimobo-0.1.2/optimobo.egg-info/SOURCES.txt
--rw-rw-r--   0 lecky     (1000) lecky     (1000)        1 2023-05-22 12:04:03.000000 optimobo-0.1.2/optimobo.egg-info/dependency_links.txt
--rw-rw-r--   0 lecky     (1000) lecky     (1000)       73 2023-05-22 12:04:03.000000 optimobo-0.1.2/optimobo.egg-info/requires.txt
--rw-rw-r--   0 lecky     (1000) lecky     (1000)        9 2023-05-22 12:04:03.000000 optimobo-0.1.2/optimobo.egg-info/top_level.txt
--rw-rw-r--   0 lecky     (1000) lecky     (1000)       38 2023-05-22 12:04:03.970973 optimobo-0.1.2/setup.cfg
--rw-rw-r--   0 lecky     (1000) lecky     (1000)      419 2023-05-22 12:00:35.000000 optimobo-0.1.2/setup.py
-drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:04:03.970973 optimobo-0.1.2/tests/
--rw-rw-r--   0 lecky     (1000) lecky     (1000)     6837 2023-05-20 18:55:15.000000 optimobo-0.1.2/tests/testing.py
+drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:09:36.771198 optimobo-0.1.3/
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)     1063 2023-05-20 14:55:19.000000 optimobo-0.1.3/LICENSE
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)     3689 2023-05-22 12:09:36.767198 optimobo-0.1.3/PKG-INFO
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)     3443 2023-05-20 19:14:19.000000 optimobo-0.1.3/README.md
+drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:09:36.767198 optimobo-0.1.3/optimobo/
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)        0 2023-05-22 11:49:17.000000 optimobo-0.1.3/optimobo/__init__.py
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)    16114 2023-05-20 15:16:09.000000 optimobo-0.1.3/optimobo/optimisers.py
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)     7822 2023-05-20 14:58:32.000000 optimobo-0.1.3/optimobo/scalarisations.py
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)    11483 2023-05-18 23:42:13.000000 optimobo-0.1.3/optimobo/util_functions.py
+drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:09:36.767198 optimobo-0.1.3/optimobo.egg-info/
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)     3689 2023-05-22 12:09:36.000000 optimobo-0.1.3/optimobo.egg-info/PKG-INFO
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)      300 2023-05-22 12:09:36.000000 optimobo-0.1.3/optimobo.egg-info/SOURCES.txt
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)        1 2023-05-22 12:09:36.000000 optimobo-0.1.3/optimobo.egg-info/dependency_links.txt
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)       73 2023-05-22 12:09:36.000000 optimobo-0.1.3/optimobo.egg-info/requires.txt
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)        9 2023-05-22 12:09:36.000000 optimobo-0.1.3/optimobo.egg-info/top_level.txt
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)       38 2023-05-22 12:09:36.771198 optimobo-0.1.3/setup.cfg
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)      634 2023-05-22 12:09:33.000000 optimobo-0.1.3/setup.py
+drwxrwxr-x   0 lecky     (1000) lecky     (1000)        0 2023-05-22 12:09:36.767198 optimobo-0.1.3/tests/
+-rw-rw-r--   0 lecky     (1000) lecky     (1000)     6837 2023-05-20 18:55:15.000000 optimobo-0.1.3/tests/testing.py
```

### Comparing `optimobo-0.1.2/LICENSE` & `optimobo-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `optimobo-0.1.2/README.md` & `optimobo-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `optimobo-0.1.2/optimobo/optimisers.py` & `optimobo-0.1.3/optimobo/optimisers.py`

 * *Files identical despite different names*

### Comparing `optimobo-0.1.2/optimobo/scalarisations.py` & `optimobo-0.1.3/optimobo/scalarisations.py`

 * *Files identical despite different names*

### Comparing `optimobo-0.1.2/optimobo/util_functions.py` & `optimobo-0.1.3/optimobo/util_functions.py`

 * *Files identical despite different names*

### Comparing `optimobo-0.1.2/tests/testing.py` & `optimobo-0.1.3/tests/testing.py`

 * *Files identical despite different names*

