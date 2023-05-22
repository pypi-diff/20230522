# Comparing `tmp/learntools_dados_ufv-1.0.8.tar.gz` & `tmp/learntools_dados_ufv-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "learntools_dados_ufv-1.0.8.tar", last modified: Wed Jul  6 21:57:39 2022, max compression
+gzip compressed data, was "learntools_dados_ufv-1.0.9.tar", last modified: Thu Jul 14 04:18:11 2022, max compression
```

## Comparing `learntools_dados_ufv-1.0.8.tar` & `learntools_dados_ufv-1.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 viegas     (501) staff       (20)        0 2022-07-06 21:57:39.161470 learntools_dados_ufv-1.0.8/
--rw-r--r--   0 viegas     (501) staff       (20)    11357 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.8/LICENSE
--rw-r--r--   0 viegas     (501) staff       (20)      341 2022-07-06 21:57:39.160321 learntools_dados_ufv-1.0.8/PKG-INFO
--rw-r--r--   0 viegas     (501) staff       (20)     1942 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.8/README.md
-drwxr-xr-x   0 viegas     (501) staff       (20)        0 2022-07-06 21:57:39.139412 learntools_dados_ufv-1.0.8/learntools_dados_ufv/
--rw-r--r--   0 viegas     (501) staff       (20)       50 2022-07-06 21:57:18.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/__init__.py
-drwxr-xr-x   0 viegas     (501) staff       (20)        0 2022-07-06 21:57:39.148756 learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/
--rw-r--r--   0 viegas     (501) staff       (20)        0 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/__init__.py
-drwxr-xr-x   0 viegas     (501) staff       (20)        0 2022-07-06 21:57:39.149483 learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/input/
--rw-r--r--   0 viegas     (501) staff       (20)        0 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/input/__init__.py
--rw-r--r--   0 viegas     (501) staff       (20)     8399 2022-04-25 00:10:36.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/pratica_1.py
--rw-r--r--   0 viegas     (501) staff       (20)    11618 2022-04-28 23:26:14.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/pratica_2.py
--rw-r--r--   0 viegas     (501) staff       (20)     5584 2022-05-17 00:32:50.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/pratica_3.py
--rw-r--r--   0 viegas     (501) staff       (20)     6773 2022-06-01 23:40:00.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/pratica_5.py
--rw-r--r--   0 viegas     (501) staff       (20)     8593 2022-06-28 05:08:43.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/pratica_7.py
--rw-r--r--   0 viegas     (501) staff       (20)     2105 2022-07-06 21:53:45.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/pratica_8.py
--rw-r--r--   0 viegas     (501) staff       (20)      474 2022-04-03 13:45:08.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/pratica_9.py
-drwxr-xr-x   0 viegas     (501) staff       (20)        0 2022-07-06 21:57:39.159456 learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/
--rw-r--r--   0 viegas     (501) staff       (20)     1743 2022-04-03 13:42:57.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/__init__.py
--rw-r--r--   0 viegas     (501) staff       (20)     6895 2022-04-03 14:00:47.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/asserts.py
--rw-r--r--   0 viegas     (501) staff       (20)      115 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/colors.py
--rw-r--r--   0 viegas     (501) staff       (20)      711 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/constants.py
--rw-r--r--   0 viegas     (501) staff       (20)      641 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/exceptions.py
--rw-r--r--   0 viegas     (501) staff       (20)     1320 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/globals_binder.py
--rw-r--r--   0 viegas     (501) staff       (20)      804 2022-04-04 23:06:46.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/multiproblem.py
--rw-r--r--   0 viegas     (501) staff       (20)    10729 2022-04-03 13:43:51.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/problem.py
--rw-r--r--   0 viegas     (501) staff       (20)     6891 2022-04-03 14:04:19.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/problem_view.py
--rw-r--r--   0 viegas     (501) staff       (20)     3473 2022-04-03 14:07:54.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/richtext.py
--rw-r--r--   0 viegas     (501) staff       (20)     2052 2022-04-03 13:46:16.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/tracking.py
--rw-r--r--   0 viegas     (501) staff       (20)     3813 2022-04-03 13:43:51.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/utils.py
-drwxr-xr-x   0 viegas     (501) staff       (20)        0 2022-07-06 21:57:39.142846 learntools_dados_ufv-1.0.8/learntools_dados_ufv.egg-info/
--rw-r--r--   0 viegas     (501) staff       (20)      341 2022-07-06 21:57:38.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv.egg-info/PKG-INFO
--rw-r--r--   0 viegas     (501) staff       (20)     1113 2022-07-06 21:57:38.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv.egg-info/SOURCES.txt
--rw-r--r--   0 viegas     (501) staff       (20)        1 2022-07-06 21:57:38.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv.egg-info/dependency_links.txt
--rw-r--r--   0 viegas     (501) staff       (20)       21 2022-07-06 21:57:38.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv.egg-info/top_level.txt
--rw-r--r--   0 viegas     (501) staff       (20)        1 2022-03-25 14:30:16.000000 learntools_dados_ufv-1.0.8/learntools_dados_ufv.egg-info/zip-safe
--rw-r--r--   0 viegas     (501) staff       (20)       38 2022-07-06 21:57:39.161615 learntools_dados_ufv-1.0.8/setup.cfg
--rw-r--r--   0 viegas     (501) staff       (20)      529 2022-04-24 23:05:41.000000 learntools_dados_ufv-1.0.8/setup.py
+drwxr-xr-x   0 viegas     (501) staff       (20)        0 2022-07-14 04:18:11.769054 learntools_dados_ufv-1.0.9/
+-rw-r--r--   0 viegas     (501) staff       (20)    11357 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.9/LICENSE
+-rw-r--r--   0 viegas     (501) staff       (20)      313 2022-07-14 04:18:11.760497 learntools_dados_ufv-1.0.9/PKG-INFO
+-rw-r--r--   0 viegas     (501) staff       (20)     1942 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.9/README.md
+drwxr-xr-x   0 viegas     (501) staff       (20)        0 2022-07-14 04:18:11.741783 learntools_dados_ufv-1.0.9/learntools_dados_ufv/
+-rw-r--r--   0 viegas     (501) staff       (20)       50 2022-07-14 04:09:27.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/__init__.py
+drwxr-xr-x   0 viegas     (501) staff       (20)        0 2022-07-14 04:18:11.749159 learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/
+-rw-r--r--   0 viegas     (501) staff       (20)        0 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/__init__.py
+drwxr-xr-x   0 viegas     (501) staff       (20)        0 2022-07-14 04:18:11.749627 learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/input/
+-rw-r--r--   0 viegas     (501) staff       (20)        0 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/input/__init__.py
+-rw-r--r--   0 viegas     (501) staff       (20)     8399 2022-04-25 00:10:36.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/pratica_1.py
+-rw-r--r--   0 viegas     (501) staff       (20)    11618 2022-04-28 23:26:14.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/pratica_2.py
+-rw-r--r--   0 viegas     (501) staff       (20)     5584 2022-05-17 00:32:50.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/pratica_3.py
+-rw-r--r--   0 viegas     (501) staff       (20)     6773 2022-06-01 23:40:00.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/pratica_5.py
+-rw-r--r--   0 viegas     (501) staff       (20)     8593 2022-06-28 05:08:43.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/pratica_7.py
+-rw-r--r--   0 viegas     (501) staff       (20)     2105 2022-07-06 21:53:45.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/pratica_8.py
+-rw-r--r--   0 viegas     (501) staff       (20)     3132 2022-07-14 04:09:15.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/pratica_9.py
+drwxr-xr-x   0 viegas     (501) staff       (20)        0 2022-07-14 04:18:11.759687 learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/
+-rw-r--r--   0 viegas     (501) staff       (20)     1743 2022-04-03 13:42:57.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/__init__.py
+-rw-r--r--   0 viegas     (501) staff       (20)     6895 2022-04-03 14:00:47.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/asserts.py
+-rw-r--r--   0 viegas     (501) staff       (20)      115 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/colors.py
+-rw-r--r--   0 viegas     (501) staff       (20)      711 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/constants.py
+-rw-r--r--   0 viegas     (501) staff       (20)      641 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/exceptions.py
+-rw-r--r--   0 viegas     (501) staff       (20)     1320 2022-03-25 13:56:53.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/globals_binder.py
+-rw-r--r--   0 viegas     (501) staff       (20)      804 2022-04-04 23:06:46.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/multiproblem.py
+-rw-r--r--   0 viegas     (501) staff       (20)    10729 2022-04-03 13:43:51.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/problem.py
+-rw-r--r--   0 viegas     (501) staff       (20)     6891 2022-04-03 14:04:19.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/problem_view.py
+-rw-r--r--   0 viegas     (501) staff       (20)     3473 2022-04-03 14:07:54.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/richtext.py
+-rw-r--r--   0 viegas     (501) staff       (20)     2052 2022-04-03 13:46:16.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/tracking.py
+-rw-r--r--   0 viegas     (501) staff       (20)     3813 2022-04-03 13:43:51.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/utils.py
+drwxr-xr-x   0 viegas     (501) staff       (20)        0 2022-07-14 04:18:11.744749 learntools_dados_ufv-1.0.9/learntools_dados_ufv.egg-info/
+-rw-r--r--   0 viegas     (501) staff       (20)      313 2022-07-14 04:18:10.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv.egg-info/PKG-INFO
+-rw-r--r--   0 viegas     (501) staff       (20)     1113 2022-07-14 04:18:11.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv.egg-info/SOURCES.txt
+-rw-r--r--   0 viegas     (501) staff       (20)        1 2022-07-14 04:18:10.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv.egg-info/dependency_links.txt
+-rw-r--r--   0 viegas     (501) staff       (20)       21 2022-07-14 04:18:11.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv.egg-info/top_level.txt
+-rw-r--r--   0 viegas     (501) staff       (20)        1 2022-03-25 14:30:16.000000 learntools_dados_ufv-1.0.9/learntools_dados_ufv.egg-info/zip-safe
+-rw-r--r--   0 viegas     (501) staff       (20)       38 2022-07-14 04:18:11.771177 learntools_dados_ufv-1.0.9/setup.cfg
+-rw-r--r--   0 viegas     (501) staff       (20)      529 2022-04-24 23:05:41.000000 learntools_dados_ufv-1.0.9/setup.py
```

### Comparing `learntools_dados_ufv-1.0.8/LICENSE` & `learntools_dados_ufv-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/README.md` & `learntools_dados_ufv-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/pratica_1.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/pratica_1.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/pratica_2.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/pratica_2.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/pratica_3.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/pratica_3.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/pratica_5.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/pratica_5.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/pratica_7.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/pratica_7.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/ccf425/pratica_8.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/ccf425/pratica_8.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/__init__.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/__init__.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/asserts.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/asserts.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/constants.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/constants.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/exceptions.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/globals_binder.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/globals_binder.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/multiproblem.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/multiproblem.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/problem.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/problem.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/problem_view.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/problem_view.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/richtext.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/richtext.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/tracking.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/tracking.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv/core/utils.py` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv/core/utils.py`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/learntools_dados_ufv.egg-info/SOURCES.txt` & `learntools_dados_ufv-1.0.9/learntools_dados_ufv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `learntools_dados_ufv-1.0.8/setup.py` & `learntools_dados_ufv-1.0.9/setup.py`

 * *Files identical despite different names*

