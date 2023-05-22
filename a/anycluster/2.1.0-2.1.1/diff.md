# Comparing `tmp/anycluster-2.1.0.tar.gz` & `tmp/anycluster-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anycluster-2.1.0.tar", last modified: Mon Apr 24 13:43:29 2023, max compression
+gzip compressed data, was "anycluster-2.1.1.tar", last modified: Mon May 22 06:46:05 2023, max compression
```

## Comparing `anycluster-2.1.0.tar` & `anycluster-2.1.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.679516 anycluster-2.1.0/
--rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.1.0/LICENSE
--rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.1.0/MANIFEST.in
--rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-04-24 13:43:29.679516 anycluster-2.1.0/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.1.0/README.md
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.671516 anycluster-2.1.0/anycluster/
--rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.1.0/anycluster/ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2680 2023-04-20 07:53:43.000000 anycluster-2.1.0/anycluster/FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    31624 2023-04-19 10:53:31.000000 anycluster-2.1.0/anycluster/MapClusterer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.1.0/anycluster/MapTools.py
--rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.1.0/anycluster/__init__.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.675516 anycluster-2.1.0/anycluster/api/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.675516 anycluster-2.1.0/anycluster/api/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.1.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.1.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2618 2023-04-24 13:23:49.000000 anycluster-2.1.0/anycluster/api/__pycache__/serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)      947 2023-04-24 13:16:49.000000 anycluster-2.1.0/anycluster/api/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     6016 2023-04-24 12:45:45.000000 anycluster-2.1.0/anycluster/api/__pycache__/views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.1.0/anycluster/api/json_schemas.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2572 2023-04-24 13:22:43.000000 anycluster-2.1.0/anycluster/api/serializers.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.675516 anycluster-2.1.0/anycluster/api/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.675516 anycluster-2.1.0/anycluster/api/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.1.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     1120 2023-03-17 13:45:55.000000 anycluster-2.1.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     6965 2023-04-19 19:03:37.000000 anycluster-2.1.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)      826 2023-03-02 13:13:55.000000 anycluster-2.1.0/anycluster/api/tests/test_serializers.py
--rw-r--r--   0 tom       (1000) tom       (1000)     9420 2023-04-19 19:03:34.000000 anycluster-2.1.0/anycluster/api/tests/test_views.py
--rw-r--r--   0 tom       (1000) tom       (1000)      882 2023-04-24 12:47:36.000000 anycluster-2.1.0/anycluster/api/urls.py
--rw-r--r--   0 tom       (1000) tom       (1000)     7323 2023-04-24 12:21:50.000000 anycluster-2.1.0/anycluster/api/views.py
--rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.1.0/anycluster/apps.py
--rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/clusters.py
--rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.1.0/anycluster/definitions.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/globalmaptiles.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.671516 anycluster-2.1.0/anycluster/static/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.671516 anycluster-2.1.0/anycluster/static/anycluster/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.675516 anycluster-2.1.0/anycluster/static/anycluster/images/
--rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/10.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/100.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/1000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/10000.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/10000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/1000_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/100_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/10_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/5.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/50.png
--rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/50_empty.png
--rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/5_empty.png
--rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.1.0/anycluster/static/anycluster/images/pin_unknown.png
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.675516 anycluster-2.1.0/anycluster/tests/
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.679516 anycluster-2.1.0/anycluster/tests/__pycache__/
--rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.1.0/anycluster/tests/__pycache__/common.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2533 2023-04-19 10:53:00.000000 anycluster-2.1.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.1.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2790 2023-04-21 13:19:15.000000 anycluster-2.1.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.1.0/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)    10728 2023-04-19 10:54:13.000000 anycluster-2.1.0/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
--rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.1.0/anycluster/tests/common.py
--rw-r--r--   0 tom       (1000) tom       (1000)     2096 2023-04-19 10:47:07.000000 anycluster-2.1.0/anycluster/tests/mixins.py
--rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.1.0/anycluster/tests/test_ClusterCache.py
--rw-r--r--   0 tom       (1000) tom       (1000)     3995 2023-04-21 13:19:10.000000 anycluster-2.1.0/anycluster/tests/test_FilterComposer.py
--rw-r--r--   0 tom       (1000) tom       (1000)    16495 2023-04-19 10:54:09.000000 anycluster-2.1.0/anycluster/tests/test_MapClusterer.py
-drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-04-24 13:43:29.671516 anycluster-2.1.0/anycluster.egg-info/
--rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-04-24 13:43:29.000000 anycluster-2.1.0/anycluster.egg-info/PKG-INFO
--rw-r--r--   0 tom       (1000) tom       (1000)     2191 2023-04-24 13:43:29.000000 anycluster-2.1.0/anycluster.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-04-24 13:43:29.000000 anycluster-2.1.0/anycluster.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-04-24 13:43:29.000000 anycluster-2.1.0/anycluster.egg-info/requires.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-04-24 13:43:29.000000 anycluster-2.1.0/anycluster.egg-info/top_level.txt
--rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-04-24 13:43:29.679516 anycluster-2.1.0/setup.cfg
--rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-04-24 13:43:01.000000 anycluster-2.1.0/setup.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.081524 anycluster-2.1.1/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1078 2023-01-20 06:49:37.000000 anycluster-2.1.1/LICENSE
+-rw-r--r--   0 tom       (1000) tom       (1000)      219 2023-04-22 19:21:48.000000 anycluster-2.1.1/MANIFEST.in
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-05-22 06:46:05.081524 anycluster-2.1.1/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     1668 2023-04-22 19:37:42.000000 anycluster-2.1.1/README.md
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.073525 anycluster-2.1.1/anycluster/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1594 2023-04-19 10:28:26.000000 anycluster-2.1.1/anycluster/ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     3656 2023-05-19 12:35:24.000000 anycluster-2.1.1/anycluster/FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    31624 2023-04-19 10:53:31.000000 anycluster-2.1.1/anycluster/MapClusterer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    10605 2023-03-06 13:41:59.000000 anycluster-2.1.1/anycluster/MapTools.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      112 2023-04-19 10:38:36.000000 anycluster-2.1.1/anycluster/__init__.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.073525 anycluster-2.1.1/anycluster/api/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.077525 anycluster-2.1.1/anycluster/api/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1584 2023-03-21 14:03:34.000000 anycluster-2.1.1/anycluster/api/__pycache__/json_schemas.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1214 2023-03-02 08:31:15.000000 anycluster-2.1.1/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2650 2023-05-19 13:08:28.000000 anycluster-2.1.1/anycluster/api/__pycache__/serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)      947 2023-04-24 13:16:49.000000 anycluster-2.1.1/anycluster/api/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     6016 2023-04-24 12:45:45.000000 anycluster-2.1.1/anycluster/api/__pycache__/views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3180 2023-03-21 14:03:34.000000 anycluster-2.1.1/anycluster/api/json_schemas.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2739 2023-05-19 13:08:27.000000 anycluster-2.1.1/anycluster/api/serializers.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.077525 anycluster-2.1.1/anycluster/api/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.077525 anycluster-2.1.1/anycluster/api/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1066 2023-03-02 09:10:26.000000 anycluster-2.1.1/anycluster/api/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     1120 2023-03-17 13:45:55.000000 anycluster-2.1.1/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     6965 2023-04-19 19:03:37.000000 anycluster-2.1.1/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)      826 2023-03-02 13:13:55.000000 anycluster-2.1.1/anycluster/api/tests/test_serializers.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     9420 2023-04-19 19:03:34.000000 anycluster-2.1.1/anycluster/api/tests/test_views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      882 2023-04-24 12:47:36.000000 anycluster-2.1.1/anycluster/api/urls.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     7323 2023-04-24 12:21:50.000000 anycluster-2.1.1/anycluster/api/views.py
+-rw-r--r--   0 tom       (1000) tom       (1000)       95 2023-03-02 07:01:38.000000 anycluster-2.1.1/anycluster/apps.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     1142 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/clusters.py
+-rw-r--r--   0 tom       (1000) tom       (1000)      602 2023-03-21 14:48:59.000000 anycluster-2.1.1/anycluster/definitions.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16529 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/globalmaptiles.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.069524 anycluster-2.1.1/anycluster/static/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.069524 anycluster-2.1.1/anycluster/static/anycluster/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.077525 anycluster-2.1.1/anycluster/static/anycluster/images/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1445 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/10.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1912 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/100.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2093 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/1000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     2811 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/10000.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1409 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/10000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1262 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/1000_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1034 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/100_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      784 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/10_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1253 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/5.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1974 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/50.png
+-rw-r--r--   0 tom       (1000) tom       (1000)     1023 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/50_empty.png
+-rw-r--r--   0 tom       (1000) tom       (1000)      749 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/5_empty.png
+-rwxr-xr-x   0 tom       (1000) tom       (1000)     1158 2023-01-20 06:49:37.000000 anycluster-2.1.1/anycluster/static/anycluster/images/pin_unknown.png
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.081524 anycluster-2.1.1/anycluster/tests/
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.081524 anycluster-2.1.1/anycluster/tests/__pycache__/
+-rw-r--r--   0 tom       (1000) tom       (1000)     1432 2023-04-19 10:14:42.000000 anycluster-2.1.1/anycluster/tests/__pycache__/common.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2533 2023-04-19 10:53:00.000000 anycluster-2.1.1/anycluster/tests/__pycache__/mixins.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3837 2023-04-21 13:16:50.000000 anycluster-2.1.1/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     3799 2023-05-19 12:42:28.000000 anycluster-2.1.1/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2882 2023-04-19 08:43:21.000000 anycluster-2.1.1/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)    10728 2023-04-19 10:54:13.000000 anycluster-2.1.1/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc
+-rw-r--r--   0 tom       (1000) tom       (1000)     2547 2023-04-19 10:13:34.000000 anycluster-2.1.1/anycluster/tests/common.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     2096 2023-04-19 10:47:07.000000 anycluster-2.1.1/anycluster/tests/mixins.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6963 2023-04-19 10:47:33.000000 anycluster-2.1.1/anycluster/tests/test_ClusterCache.py
+-rw-r--r--   0 tom       (1000) tom       (1000)     6582 2023-05-19 12:42:25.000000 anycluster-2.1.1/anycluster/tests/test_FilterComposer.py
+-rw-r--r--   0 tom       (1000) tom       (1000)    16495 2023-04-19 10:54:09.000000 anycluster-2.1.1/anycluster/tests/test_MapClusterer.py
+drwxr-xr-x   0 tom       (1000) tom       (1000)        0 2023-05-22 06:46:05.073525 anycluster-2.1.1/anycluster.egg-info/
+-rw-r--r--   0 tom       (1000) tom       (1000)     2257 2023-05-22 06:46:05.000000 anycluster-2.1.1/anycluster.egg-info/PKG-INFO
+-rw-r--r--   0 tom       (1000) tom       (1000)     2191 2023-05-22 06:46:05.000000 anycluster-2.1.1/anycluster.egg-info/SOURCES.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)        1 2023-05-22 06:46:05.000000 anycluster-2.1.1/anycluster.egg-info/dependency_links.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       40 2023-05-22 06:46:05.000000 anycluster-2.1.1/anycluster.egg-info/requires.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       11 2023-05-22 06:46:05.000000 anycluster-2.1.1/anycluster.egg-info/top_level.txt
+-rw-r--r--   0 tom       (1000) tom       (1000)       38 2023-05-22 06:46:05.081524 anycluster-2.1.1/setup.cfg
+-rw-r--r--   0 tom       (1000) tom       (1000)      989 2023-05-22 06:41:31.000000 anycluster-2.1.1/setup.py
```

### Comparing `anycluster-2.1.0/LICENSE` & `anycluster-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/PKG-INFO` & `anycluster-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.1.0
+Version: 2.1.1
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.1.0/README.md` & `anycluster-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/ClusterCache.py` & `anycluster-2.1.1/anycluster/ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/FilterComposer.py` & `anycluster-2.1.1/anycluster/FilterComposer.py`

 * *Files 21% similar despite different names*

```diff
@@ -55,38 +55,81 @@
 
         elif isinstance(value, numbers.Number) or isinstance(value, decimal.Decimal):
             return value
 
         else:
             return value
 
-    def as_sql(self):
+
+    def parse_filter(self, filter):
 
         filterstring = ''
 
-        for filter in self.filters:
+        column = filter['column']
+        comparison_operator = filter['operator']
+        value = filter['value']
 
-            column = filter['column']
-            operator = filter['operator']
-            value = filter['value']
+        filterstring += '('
 
-            filterstring += ' AND ('
+        if isinstance(value, list):
+            parsed_operator = self.list_operator_mapping[comparison_operator]
 
-            if isinstance(value, list):
-                parsed_operator = self.list_operator_mapping[operator]
+            sql_value = str(tuple(value))
 
-                sql_value = str(tuple(value))
+            filterstring += '{column} {operator} {sql_value}'.format(column=column, operator=parsed_operator,
+                                                                    sql_value=sql_value)
 
-                filterstring += '{column} {operator} {sql_value}'.format(column=column, operator=parsed_operator,
-                                                                         sql_value=sql_value)
+        else:
+            parsed_operator = self.operator_mapping[comparison_operator]
 
-            else:
-                parsed_operator = self.operator_mapping[operator]
+            sql_value = self.parse_filter_value(comparison_operator, value)
+
+            filterstring += '{column} {operator} {sql_value}'.format(column=column, operator=parsed_operator,
+                                                                    sql_value=sql_value)
+
+        filterstring += ')'
+
+        return filterstring
+
+
+    def parse_filters(self, filters):
+
+        filterstring = ''
+
+        if len(filters) > 1:
+                filterstring += '('
+
+        for counter, filter in enumerate(filters, 0):
 
-                sql_value = self.parse_filter_value(operator, value)
+            is_nested = 'filters' in filter
 
-                filterstring += '{column} {operator} {sql_value}'.format(column=column, operator=parsed_operator,
-                                                                         sql_value=sql_value)
+            logical_operator = filter.get('logicalOperator', 'AND')
 
+            if counter > 0:
+                filterstring += ' {logical_operator} '.format(logical_operator=logical_operator)
+
+            if is_nested == False:
+                filterstring += self.parse_filter(filter)
+
+            else:
+                nested_filter_composer = FilterComposer(filter['filters'])
+                filterstring += nested_filter_composer.parse_filters(filter['filters'])
+            
+
+        
+        if len(filters) > 1:
             filterstring += ')'
 
         return filterstring
+
+
+    def as_sql(self):
+
+        filterstring = ''
+
+        if self.filters:
+
+            filterstring = ' AND '
+
+            filterstring += self.parse_filters(self.filters)
+
+        return filterstring
```

### Comparing `anycluster-2.1.0/anycluster/MapClusterer.py` & `anycluster-2.1.1/anycluster/MapClusterer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/MapTools.py` & `anycluster-2.1.1/anycluster/MapTools.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/api/__pycache__/json_schemas.cpython-38.pyc` & `anycluster-2.1.1/anycluster/api/__pycache__/json_schemas.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc` & `anycluster-2.1.1/anycluster/api/__pycache__/serializer_fields.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/api/__pycache__/serializers.cpython-38.pyc` & `anycluster-2.1.1/anycluster/api/__pycache__/serializers.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Mon Apr 24 13:22:43 2023 UTC, .py size: 2572 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 a382 4664 0c0a 0000  U.........Fd....
+00000000: 550d 0d0a 0000 0000 cb74 6764 b30a 0000  U........tgd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 6c00 0000 6400  .....@...sl...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6404  m.Z...d.d.l.Z.d.
 00000050: 6405 6c05 6d06 5a06 0100 6400 6406 6c07  d.l.m.Z...d.d.l.
 00000060: 6d08 5a08 6d09 5a09 0100 6407 6408 8400  m.Z.m.Z...d.d...
 00000070: 5a0a 4700 6409 640a 8400 640a 6503 6a0b  Z.G.d.d...d.e.j.
@@ -12,153 +12,155 @@
 000000b0: 0b73 6572 6961 6c69 7a65 7273 4ee9 0100  .serializersN...
 000000c0: 0000 2901 da23 4645 4154 5552 455f 4f52  ..)..#FEATURE_OR
 000000d0: 5f46 4541 5455 5245 434f 4c4c 4543 5449  _FEATURECOLLECTI
 000000e0: 4f4e 5f53 4348 454d 4129 02da 0e47 454f  ON_SCHEMA)...GEO
 000000f0: 4d45 5452 595f 5459 5045 53da 1647 454f  METRY_TYPES..GEO
 00000100: 4d45 5452 595f 5459 5045 5f56 4945 5750  METRY_TYPE_VIEWP
 00000110: 4f52 5463 0100 0000 0000 0000 0000 0000  ORTc............
-00000120: 0300 0000 0600 0000 4300 0000 7342 0000  ........C...sB..
-00000130: 007c 0044 005d 387d 017c 01a0 0064 0164  .|.D.]8}.|...d.d
-00000140: 00a1 027d 027c 0273 2274 01a0 0264 02a1  ...}.|.s"t...d..
-00000150: 0182 017c 0274 036a 046b 0772 0474 01a0  ...|.t.j.k.r.t..
-00000160: 0264 03a0 057c 02a1 01a1 0182 0171 0464  .d...|.......q.d
-00000170: 0053 0029 044e da06 636f 6c75 6d6e 7a17  .S.).N..columnz.
-00000180: 4669 6c74 6572 2072 6571 7569 7265 2061  Filter require a
-00000190: 2063 6f6c 756d 6e7a 2649 7420 6973 206e   columnz&It is n
-000001a0: 6f74 2061 6c6c 6f77 6564 2074 6f20 6669  ot allowed to fi
-000001b0: 6c74 6572 2043 6f6c 756d 6e20 7b30 7d29  lter Column {0})
-000001c0: 06da 0367 6574 7203 0000 00da 0f56 616c  ...getr......Val
-000001d0: 6964 6174 696f 6e45 7272 6f72 7202 0000  idationErrorr...
-000001e0: 005a 1241 4e59 434c 5553 5445 525f 4649  .Z.ANYCLUSTER_FI
-000001f0: 4c54 4552 53da 0666 6f72 6d61 7429 03da  LTERS..format)..
-00000200: 0766 696c 7465 7273 da06 6669 6c74 6572  .filters..filter
-00000210: 7208 0000 00a9 0072 0e00 0000 fa58 2f68  r......r.....X/h
-00000220: 6f6d 652f 746f 6d2f 6c6f 6361 6c63 6f73  ome/tom/localcos
-00000230: 6d6f 732d 776f 726b 7370 6163 652f 636f  mos-workspace/co
-00000240: 6465 2f6c 6f63 616c 636f 736d 6f73 2d69  de/localcosmos-i
-00000250: 6e73 7469 7475 7465 2f61 6e79 636c 7573  nstitute/anyclus
-00000260: 7465 722f 6170 692f 7365 7269 616c 697a  ter/api/serializ
-00000270: 6572 732e 7079 da13 6669 6c74 6572 735f  ers.py..filters_
-00000280: 6172 655f 616c 6c6f 7765 640b 0000 0073  are_allowed....s
-00000290: 0c00 0000 0002 0801 0c01 0401 0a02 0a01  ................
-000002a0: 7210 0000 0063 0000 0000 0000 0000 0000  r....c..........
-000002b0: 0000 0000 0000 0500 0000 4000 0000 736e  ..........@...sn
-000002c0: 0000 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
-000002d0: 0164 0264 0364 048d 035a 0565 036a 0665  .d.d.d...Z.e.j.e
-000002e0: 0764 0364 058d 025a 0865 036a 0964 0364  .d.d...Z.e.j.d.d
-000002f0: 068d 015a 0a65 036a 0b64 0267 0064 0364  ...Z.e.j.d.g.d.d
-00000300: 078d 035a 0c65 036a 0d64 0264 0264 0364  ...Z.e.j.d.d.d.d
-00000310: 048d 035a 0e64 0864 0984 005a 0f64 0a64  ...Z.d.d...Z.d.d
-00000320: 0b84 005a 1064 0c64 0d84 005a 1164 0e53  ...Z.d.d...Z.d.S
-00000330: 0029 0fda 1843 6c75 7374 6572 5265 7175  .)...ClusterRequ
-00000340: 6573 7453 6572 6961 6c69 7a65 72fa 0945  estSerializer..E
-00000350: 5053 473a 3433 3236 4654 a903 da07 6465  PSG:4326FT....de
-00000360: 6661 756c 74da 0872 6571 7569 7265 64da  fault..required.
-00000370: 0a77 7269 7465 5f6f 6e6c 79a9 02da 0763  .write_only....c
-00000380: 686f 6963 6573 7216 0000 00a9 0172 1600  hoicesr......r..
-00000390: 0000 a903 7215 0000 0072 1400 0000 7216  ....r....r....r.
-000003a0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000003b0: 0400 0000 0300 0000 4300 0000 733e 0000  ........C...s>..
-000003c0: 007c 0164 0119 0074 006b 0272 3a7c 0164  .|.d...t.k.r:|.d
-000003d0: 0219 007d 027c 0264 0319 0064 0419 0064  ...}.|.d...d...d
-000003e0: 0519 007d 0374 017c 0383 0164 066b 0273  ...}.t.|...d.k.s
-000003f0: 3a74 02a0 0364 07a1 0182 017c 0153 0029  :t...d.....|.S.)
-00000400: 084e da0d 6765 6f6d 6574 7279 5f74 7970  .N..geometry_typ
-00000410: 65da 0767 656f 6a73 6f6e da08 6765 6f6d  e..geojson..geom
-00000420: 6574 7279 da0b 636f 6f72 6469 6e61 7465  etry..coordinate
-00000430: 7372 0100 0000 e905 0000 007a 2156 6965  sr.........z!Vie
-00000440: 7770 6f72 7420 6d75 7374 2063 6f6e 7369  wport must consi
-00000450: 7374 206f 6620 3520 706f 696e 7473 2904  st of 5 points).
-00000460: 7207 0000 00da 036c 656e 7203 0000 0072  r......lenr....r
-00000470: 0a00 0000 2904 da04 7365 6c66 da04 6461  ....)...self..da
-00000480: 7461 721c 0000 0072 1e00 0000 720e 0000  tar....r....r...
-00000490: 0072 0e00 0000 720f 0000 00da 0876 616c  .r....r......val
-000004a0: 6964 6174 6522 0000 0073 0c00 0000 0001  idate"...s......
-000004b0: 0c02 0801 1001 0c01 0a02 7a21 436c 7573  ..........z!Clus
-000004c0: 7465 7252 6571 7565 7374 5365 7269 616c  terRequestSerial
-000004d0: 697a 6572 2e76 616c 6964 6174 6563 0200  izer.validatec..
-000004e0: 0000 0000 0000 0000 0000 0400 0000 0a00  ................
-000004f0: 0000 4300 0000 7348 0000 007a 1074 00a0  ..C...sH...z.t..
-00000500: 017c 0174 02a1 027d 0257 006e 3204 0074  .|.t...}.W.n2..t
-00000510: 006a 036a 046b 0a72 4201 007d 0301 007a  .j.j.k.rB..}...z
-00000520: 1074 05a0 047c 036a 06a1 0182 0157 0035  .t...|.j.....W.5
-00000530: 0064 007d 037e 0358 0059 006e 0258 007c  .d.}.~.X.Y.n.X.|
-00000540: 0153 00a9 014e 2907 da0a 6a73 6f6e 7363  .S...N)...jsonsc
-00000550: 6865 6d61 7223 0000 0072 0500 0000 da0a  hemar#...r......
-00000560: 6578 6365 7074 696f 6e73 720a 0000 0072  exceptionsr....r
-00000570: 0300 0000 da07 6d65 7373 6167 6529 0472  ......message).r
-00000580: 2100 0000 da05 7661 6c75 65da 0869 735f  !.....value..is_
-00000590: 7661 6c69 64da 0165 720e 0000 0072 0e00  valid..er....r..
-000005a0: 0000 720f 0000 00da 1076 616c 6964 6174  ..r......validat
-000005b0: 655f 6765 6f6a 736f 6e2d 0000 0073 0a00  e_geojson-...s..
-000005c0: 0000 0001 0201 1001 1401 1e01 7a29 436c  ............z)Cl
-000005d0: 7573 7465 7252 6571 7565 7374 5365 7269  usterRequestSeri
-000005e0: 616c 697a 6572 2e76 616c 6964 6174 655f  alizer.validate_
-000005f0: 6765 6f6a 736f 6e63 0200 0000 0000 0000  geojsonc........
-00000600: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
-00000610: 730c 0000 0074 007c 0183 0101 007c 0153  s....t.|.....|.S
-00000620: 0072 2400 0000 a901 7210 0000 00a9 0272  .r$.....r......r
-00000630: 2100 0000 7228 0000 0072 0e00 0000 720e  !...r(...r....r.
-00000640: 0000 0072 0f00 0000 da10 7661 6c69 6461  ...r......valida
-00000650: 7465 5f66 696c 7465 7273 3400 0000 7304  te_filters4...s.
-00000660: 0000 0000 0108 017a 2943 6c75 7374 6572  .......z)Cluster
-00000670: 5265 7175 6573 7453 6572 6961 6c69 7a65  RequestSerialize
-00000680: 722e 7661 6c69 6461 7465 5f66 696c 7465  r.validate_filte
-00000690: 7273 4e29 12da 085f 5f6e 616d 655f 5fda  rsN)...__name__.
-000006a0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-000006b0: 7561 6c6e 616d 655f 5f72 0300 0000 da09  ualname__r......
-000006c0: 4368 6172 4669 656c 64da 0b6f 7574 7075  CharField..outpu
-000006d0: 745f 7372 6964 da0b 4368 6f69 6365 4669  t_srid..ChoiceFi
-000006e0: 656c 6472 0600 0000 721b 0000 00da 094a  eldr....r......J
-000006f0: 534f 4e46 6965 6c64 721c 0000 00da 094c  SONFieldr......L
-00000700: 6973 7446 6965 6c64 720c 0000 00da 0c42  istFieldr......B
-00000710: 6f6f 6c65 616e 4669 656c 64da 0b63 6c65  ooleanField..cle
-00000720: 6172 5f63 6163 6865 7223 0000 0072 2b00  ar_cacher#...r+.
-00000730: 0000 722e 0000 0072 0e00 0000 720e 0000  ..r....r....r...
-00000740: 0072 0e00 0000 720f 0000 0072 1100 0000  .r....r....r....
-00000750: 1600 0000 7310 0000 0008 0210 020e 020c  ....s...........
-00000760: 0110 0210 0308 0b08 0772 1100 0000 6300  .........r....c.
-00000770: 0000 0000 0000 0000 0000 0000 0000 0005  ................
-00000780: 0000 0040 0000 0073 7c00 0000 6500 5a01  ...@...s|...e.Z.
-00000790: 6400 5a02 6503 6a04 6401 6402 6403 6404  d.Z.e.j.d.d.d.d.
-000007a0: 8d03 5a05 6503 6a04 6401 6402 6403 6404  ..Z.e.j.d.d.d.d.
-000007b0: 8d03 5a06 6503 6a07 6508 6403 6405 8d02  ..Z.e.j.e.d.d...
-000007c0: 5a09 6503 6a0a 6503 a00b a100 6403 6406  Z.e.j.e.....d.d.
-000007d0: 8d02 5a0c 6503 6a0d 6403 6407 8d01 5a0e  ..Z.e.j.d.d...Z.
-000007e0: 6503 6a0d 6403 6407 8d01 5a0f 6503 6a0a  e.j.d.d...Z.e.j.
-000007f0: 6402 6700 6403 6408 8d03 5a10 6409 640a  d.g.d.d...Z.d.d.
-00000800: 8400 5a11 640b 5300 290c da1f 436c 7573  ..Z.d.S.)...Clus
-00000810: 7465 7243 6f6e 7465 6e74 5265 7175 6573  terContentReques
-00000820: 7453 6572 6961 6c69 7a65 7272 1200 0000  tSerializerr....
-00000830: 4654 7213 0000 0072 1700 0000 2902 da05  FTr....r....)...
-00000840: 6368 696c 6472 1600 0000 7219 0000 0072  childr....r....r
-00000850: 1a00 0000 6302 0000 0000 0000 0000 0000  ....c...........
-00000860: 0002 0000 0002 0000 0043 0000 0073 0c00  .........C...s..
-00000870: 0000 7400 7c01 8301 0100 7c01 5300 7224  ..t.|.....|.S.r$
-00000880: 0000 0072 2c00 0000 722d 0000 0072 0e00  ...r,...r-...r..
-00000890: 0000 720e 0000 0072 0f00 0000 722e 0000  ..r....r....r...
-000008a0: 0045 0000 0073 0400 0000 0001 0801 7a30  .E...s........z0
-000008b0: 436c 7573 7465 7243 6f6e 7465 6e74 5265  ClusterContentRe
-000008c0: 7175 6573 7453 6572 6961 6c69 7a65 722e  questSerializer.
-000008d0: 7661 6c69 6461 7465 5f66 696c 7465 7273  validate_filters
-000008e0: 4e29 1272 2f00 0000 7230 0000 0072 3100  N).r/...r0...r1.
-000008f0: 0000 7203 0000 0072 3200 0000 7233 0000  ..r....r2...r3..
-00000900: 00da 0a69 6e70 7574 5f73 7269 6472 3400  ...input_sridr4.
-00000910: 0000 7206 0000 0072 1b00 0000 7236 0000  ..r....r....r6..
-00000920: 00da 0c49 6e74 6567 6572 4669 656c 64da  ...IntegerField.
-00000930: 0369 6473 da0a 466c 6f61 7446 6965 6c64  .ids..FloatField
-00000940: da01 78da 0179 720c 0000 0072 2e00 0000  ..x..yr....r....
-00000950: 720e 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
-00000960: 0f00 0000 7239 0000 0039 0000 0073 1000  ....r9...9...s..
-00000970: 0000 0802 1001 1002 0e02 1201 0c01 0c01  ................
-00000980: 1002 7239 0000 0029 0eda 0b64 6a61 6e67  ..r9...)...djang
-00000990: 6f2e 636f 6e66 7202 0000 00da 0e72 6573  o.confr......res
-000009a0: 745f 6672 616d 6577 6f72 6b72 0300 0000  t_frameworkr....
-000009b0: 7225 0000 00da 0c6a 736f 6e5f 7363 6865  r%.....json_sche
-000009c0: 6d61 7372 0500 0000 da16 616e 7963 6c75  masr......anyclu
-000009d0: 7374 6572 2e64 6566 696e 6974 696f 6e73  ster.definitions
-000009e0: 7206 0000 0072 0700 0000 7210 0000 00da  r....r....r.....
-000009f0: 0a53 6572 6961 6c69 7a65 7272 1100 0000  .Serializerr....
-00000a00: 7239 0000 0072 0e00 0000 720e 0000 0072  r9...r....r....r
-00000a10: 0e00 0000 720f 0000 00da 083c 6d6f 6475  ....r......<modu
-00000a20: 6c65 3e01 0000 0073 0e00 0000 0c01 0c02  le>....s........
-00000a30: 0802 0c02 1003 080b 1223                 .........#
+00000120: 0400 0000 0600 0000 4300 0000 7360 0000  ........C...s`..
+00000130: 007c 0044 005d 567d 0164 017c 016b 067d  .|.D.]V}.d.|.k.}
+00000140: 027c 0264 026b 0272 4e7c 01a0 0064 0364  .|.d.k.rN|...d.d
+00000150: 00a1 027d 037c 0373 3274 01a0 0264 04a1  ...}.|.s2t...d..
+00000160: 0182 017c 0374 036a 046b 0772 5a74 01a0  ...|.t.j.k.rZt..
+00000170: 0264 05a0 057c 03a1 01a1 0182 0171 0474  .d...|.......q.t
+00000180: 067c 0164 0119 0083 0101 0071 0464 0053  .|.d.......q.d.S
+00000190: 0029 064e da07 6669 6c74 6572 7346 da06  .).N..filtersF..
+000001a0: 636f 6c75 6d6e 7a17 4669 6c74 6572 2072  columnz.Filter r
+000001b0: 6571 7569 7265 2061 2063 6f6c 756d 6e7a  equire a columnz
+000001c0: 2649 7420 6973 206e 6f74 2061 6c6c 6f77  &It is not allow
+000001d0: 6564 2074 6f20 6669 6c74 6572 2043 6f6c  ed to filter Col
+000001e0: 756d 6e20 7b30 7d29 07da 0367 6574 7203  umn {0})...getr.
+000001f0: 0000 00da 0f56 616c 6964 6174 696f 6e45  .....ValidationE
+00000200: 7272 6f72 7202 0000 00da 1241 4e59 434c  rrorr......ANYCL
+00000210: 5553 5445 525f 4649 4c54 4552 53da 0666  USTER_FILTERS..f
+00000220: 6f72 6d61 74da 1366 696c 7465 7273 5f61  ormat..filters_a
+00000230: 7265 5f61 6c6c 6f77 6564 2904 7208 0000  re_allowed).r...
+00000240: 00da 0666 696c 7465 72da 0969 735f 6e65  ...filter..is_ne
+00000250: 7374 6564 7209 0000 00a9 0072 1100 0000  stedr......r....
+00000260: fa3e 2f68 6f6d 652f 746f 6d2f 616e 7963  .>/home/tom/anyc
+00000270: 6c75 7374 6572 2f64 656d 6f2f 646a 616e  luster/demo/djan
+00000280: 676f 2f61 6e79 636c 7573 7465 722f 6170  go/anycluster/ap
+00000290: 692f 7365 7269 616c 697a 6572 732e 7079  i/serializers.py
+000002a0: 720e 0000 000b 0000 0073 1200 0000 0002  r........s......
+000002b0: 0802 0802 0801 0c01 0401 0a02 0a01 1203  ................
+000002c0: 720e 0000 0063 0000 0000 0000 0000 0000  r....c..........
+000002d0: 0000 0000 0000 0500 0000 4000 0000 736e  ..........@...sn
+000002e0: 0000 0065 005a 0164 005a 0265 036a 0464  ...e.Z.d.Z.e.j.d
+000002f0: 0164 0264 0364 048d 035a 0565 036a 0665  .d.d.d...Z.e.j.e
+00000300: 0764 0364 058d 025a 0865 036a 0964 0364  .d.d...Z.e.j.d.d
+00000310: 068d 015a 0a65 036a 0b64 0267 0064 0364  ...Z.e.j.d.g.d.d
+00000320: 078d 035a 0c65 036a 0d64 0264 0264 0364  ...Z.e.j.d.d.d.d
+00000330: 048d 035a 0e64 0864 0984 005a 0f64 0a64  ...Z.d.d...Z.d.d
+00000340: 0b84 005a 1064 0c64 0d84 005a 1164 0e53  ...Z.d.d...Z.d.S
+00000350: 0029 0fda 1843 6c75 7374 6572 5265 7175  .)...ClusterRequ
+00000360: 6573 7453 6572 6961 6c69 7a65 72fa 0945  estSerializer..E
+00000370: 5053 473a 3433 3236 4654 a903 da07 6465  PSG:4326FT....de
+00000380: 6661 756c 74da 0872 6571 7569 7265 64da  fault..required.
+00000390: 0a77 7269 7465 5f6f 6e6c 79a9 02da 0763  .write_only....c
+000003a0: 686f 6963 6573 7218 0000 00a9 0172 1800  hoicesr......r..
+000003b0: 0000 a903 7217 0000 0072 1600 0000 7218  ....r....r....r.
+000003c0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
+000003d0: 0400 0000 0300 0000 4300 0000 733e 0000  ........C...s>..
+000003e0: 007c 0164 0119 0074 006b 0272 3a7c 0164  .|.d...t.k.r:|.d
+000003f0: 0219 007d 027c 0264 0319 0064 0419 0064  ...}.|.d...d...d
+00000400: 0519 007d 0374 017c 0383 0164 066b 0273  ...}.t.|...d.k.s
+00000410: 3a74 02a0 0364 07a1 0182 017c 0153 0029  :t...d.....|.S.)
+00000420: 084e da0d 6765 6f6d 6574 7279 5f74 7970  .N..geometry_typ
+00000430: 65da 0767 656f 6a73 6f6e da08 6765 6f6d  e..geojson..geom
+00000440: 6574 7279 da0b 636f 6f72 6469 6e61 7465  etry..coordinate
+00000450: 7372 0100 0000 e905 0000 007a 2156 6965  sr.........z!Vie
+00000460: 7770 6f72 7420 6d75 7374 2063 6f6e 7369  wport must consi
+00000470: 7374 206f 6620 3520 706f 696e 7473 2904  st of 5 points).
+00000480: 7207 0000 00da 036c 656e 7203 0000 0072  r......lenr....r
+00000490: 0b00 0000 2904 da04 7365 6c66 da04 6461  ....)...self..da
+000004a0: 7461 721e 0000 0072 2000 0000 7211 0000  tar....r ...r...
+000004b0: 0072 1100 0000 7212 0000 00da 0876 616c  .r....r......val
+000004c0: 6964 6174 6529 0000 0073 0c00 0000 0001  idate)...s......
+000004d0: 0c02 0801 1001 0c01 0a02 7a21 436c 7573  ..........z!Clus
+000004e0: 7465 7252 6571 7565 7374 5365 7269 616c  terRequestSerial
+000004f0: 697a 6572 2e76 616c 6964 6174 6563 0200  izer.validatec..
+00000500: 0000 0000 0000 0000 0000 0400 0000 0a00  ................
+00000510: 0000 4300 0000 7348 0000 007a 1074 00a0  ..C...sH...z.t..
+00000520: 017c 0174 02a1 027d 0257 006e 3204 0074  .|.t...}.W.n2..t
+00000530: 006a 036a 046b 0a72 4201 007d 0301 007a  .j.j.k.rB..}...z
+00000540: 1074 05a0 047c 036a 06a1 0182 0157 0035  .t...|.j.....W.5
+00000550: 0064 007d 037e 0358 0059 006e 0258 007c  .d.}.~.X.Y.n.X.|
+00000560: 0153 00a9 014e 2907 da0a 6a73 6f6e 7363  .S...N)...jsonsc
+00000570: 6865 6d61 7225 0000 0072 0500 0000 da0a  hemar%...r......
+00000580: 6578 6365 7074 696f 6e73 720b 0000 0072  exceptionsr....r
+00000590: 0300 0000 da07 6d65 7373 6167 6529 0472  ......message).r
+000005a0: 2300 0000 da05 7661 6c75 65da 0869 735f  #.....value..is_
+000005b0: 7661 6c69 64da 0165 7211 0000 0072 1100  valid..er....r..
+000005c0: 0000 7212 0000 00da 1076 616c 6964 6174  ..r......validat
+000005d0: 655f 6765 6f6a 736f 6e34 0000 0073 0a00  e_geojson4...s..
+000005e0: 0000 0001 0201 1001 1401 1e01 7a29 436c  ............z)Cl
+000005f0: 7573 7465 7252 6571 7565 7374 5365 7269  usterRequestSeri
+00000600: 616c 697a 6572 2e76 616c 6964 6174 655f  alizer.validate_
+00000610: 6765 6f6a 736f 6e63 0200 0000 0000 0000  geojsonc........
+00000620: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00000630: 730c 0000 0074 007c 0183 0101 007c 0153  s....t.|.....|.S
+00000640: 0072 2600 0000 a901 720e 0000 00a9 0272  .r&.....r......r
+00000650: 2300 0000 722a 0000 0072 1100 0000 7211  #...r*...r....r.
+00000660: 0000 0072 1200 0000 da10 7661 6c69 6461  ...r......valida
+00000670: 7465 5f66 696c 7465 7273 3b00 0000 7304  te_filters;...s.
+00000680: 0000 0000 0108 017a 2943 6c75 7374 6572  .......z)Cluster
+00000690: 5265 7175 6573 7453 6572 6961 6c69 7a65  RequestSerialize
+000006a0: 722e 7661 6c69 6461 7465 5f66 696c 7465  r.validate_filte
+000006b0: 7273 4e29 12da 085f 5f6e 616d 655f 5fda  rsN)...__name__.
+000006c0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+000006d0: 7561 6c6e 616d 655f 5f72 0300 0000 da09  ualname__r......
+000006e0: 4368 6172 4669 656c 64da 0b6f 7574 7075  CharField..outpu
+000006f0: 745f 7372 6964 da0b 4368 6f69 6365 4669  t_srid..ChoiceFi
+00000700: 656c 6472 0600 0000 721d 0000 00da 094a  eldr....r......J
+00000710: 534f 4e46 6965 6c64 721e 0000 00da 094c  SONFieldr......L
+00000720: 6973 7446 6965 6c64 7208 0000 00da 0c42  istFieldr......B
+00000730: 6f6f 6c65 616e 4669 656c 64da 0b63 6c65  ooleanField..cle
+00000740: 6172 5f63 6163 6865 7225 0000 0072 2d00  ar_cacher%...r-.
+00000750: 0000 7230 0000 0072 1100 0000 7211 0000  ..r0...r....r...
+00000760: 0072 1100 0000 7212 0000 0072 1300 0000  .r....r....r....
+00000770: 1d00 0000 7310 0000 0008 0210 020e 020c  ....s...........
+00000780: 0110 0210 0308 0b08 0772 1300 0000 6300  .........r....c.
+00000790: 0000 0000 0000 0000 0000 0000 0000 0005  ................
+000007a0: 0000 0040 0000 0073 7c00 0000 6500 5a01  ...@...s|...e.Z.
+000007b0: 6400 5a02 6503 6a04 6401 6402 6403 6404  d.Z.e.j.d.d.d.d.
+000007c0: 8d03 5a05 6503 6a04 6401 6402 6403 6404  ..Z.e.j.d.d.d.d.
+000007d0: 8d03 5a06 6503 6a07 6508 6403 6405 8d02  ..Z.e.j.e.d.d...
+000007e0: 5a09 6503 6a0a 6503 a00b a100 6403 6406  Z.e.j.e.....d.d.
+000007f0: 8d02 5a0c 6503 6a0d 6403 6407 8d01 5a0e  ..Z.e.j.d.d...Z.
+00000800: 6503 6a0d 6403 6407 8d01 5a0f 6503 6a0a  e.j.d.d...Z.e.j.
+00000810: 6402 6700 6403 6408 8d03 5a10 6409 640a  d.g.d.d...Z.d.d.
+00000820: 8400 5a11 640b 5300 290c da1f 436c 7573  ..Z.d.S.)...Clus
+00000830: 7465 7243 6f6e 7465 6e74 5265 7175 6573  terContentReques
+00000840: 7453 6572 6961 6c69 7a65 7272 1400 0000  tSerializerr....
+00000850: 4654 7215 0000 0072 1900 0000 2902 da05  FTr....r....)...
+00000860: 6368 696c 6472 1800 0000 721b 0000 0072  childr....r....r
+00000870: 1c00 0000 6302 0000 0000 0000 0000 0000  ....c...........
+00000880: 0002 0000 0002 0000 0043 0000 0073 0c00  .........C...s..
+00000890: 0000 7400 7c01 8301 0100 7c01 5300 7226  ..t.|.....|.S.r&
+000008a0: 0000 0072 2e00 0000 722f 0000 0072 1100  ...r....r/...r..
+000008b0: 0000 7211 0000 0072 1200 0000 7230 0000  ..r....r....r0..
+000008c0: 004c 0000 0073 0400 0000 0001 0801 7a30  .L...s........z0
+000008d0: 436c 7573 7465 7243 6f6e 7465 6e74 5265  ClusterContentRe
+000008e0: 7175 6573 7453 6572 6961 6c69 7a65 722e  questSerializer.
+000008f0: 7661 6c69 6461 7465 5f66 696c 7465 7273  validate_filters
+00000900: 4e29 1272 3100 0000 7232 0000 0072 3300  N).r1...r2...r3.
+00000910: 0000 7203 0000 0072 3400 0000 7235 0000  ..r....r4...r5..
+00000920: 00da 0a69 6e70 7574 5f73 7269 6472 3600  ...input_sridr6.
+00000930: 0000 7206 0000 0072 1d00 0000 7238 0000  ..r....r....r8..
+00000940: 00da 0c49 6e74 6567 6572 4669 656c 64da  ...IntegerField.
+00000950: 0369 6473 da0a 466c 6f61 7446 6965 6c64  .ids..FloatField
+00000960: da01 78da 0179 7208 0000 0072 3000 0000  ..x..yr....r0...
+00000970: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+00000980: 1200 0000 723b 0000 0040 0000 0073 1000  ....r;...@...s..
+00000990: 0000 0802 1001 1002 0e02 1201 0c01 0c01  ................
+000009a0: 1002 723b 0000 0029 0eda 0b64 6a61 6e67  ..r;...)...djang
+000009b0: 6f2e 636f 6e66 7202 0000 00da 0e72 6573  o.confr......res
+000009c0: 745f 6672 616d 6577 6f72 6b72 0300 0000  t_frameworkr....
+000009d0: 7227 0000 005a 0c6a 736f 6e5f 7363 6865  r'...Z.json_sche
+000009e0: 6d61 7372 0500 0000 da16 616e 7963 6c75  masr......anyclu
+000009f0: 7374 6572 2e64 6566 696e 6974 696f 6e73  ster.definitions
+00000a00: 7206 0000 0072 0700 0000 720e 0000 00da  r....r....r.....
+00000a10: 0a53 6572 6961 6c69 7a65 7272 1300 0000  .Serializerr....
+00000a20: 723b 0000 0072 1100 0000 7211 0000 0072  r;...r....r....r
+00000a30: 1100 0000 7212 0000 00da 083c 6d6f 6475  ....r......<modu
+00000a40: 6c65 3e01 0000 0073 0e00 0000 0c01 0c02  le>....s........
+00000a50: 0802 0c02 1003 0812 1223                 .........#
```

### Comparing `anycluster-2.1.0/anycluster/api/__pycache__/urls.cpython-38.pyc` & `anycluster-2.1.1/anycluster/api/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/api/__pycache__/views.cpython-38.pyc` & `anycluster-2.1.1/anycluster/api/__pycache__/views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/api/json_schemas.py` & `anycluster-2.1.1/anycluster/api/json_schemas.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/api/serializers.py` & `anycluster-2.1.1/anycluster/api/serializers.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,20 +7,27 @@
 
 from anycluster.definitions import GEOMETRY_TYPES, GEOMETRY_TYPE_VIEWPORT
 
 
 def filters_are_allowed(filters):
 
     for filter in filters:
-        column = filter.get('column', None)
-        if not column:
-            raise serializers.ValidationError('Filter require a column')
+
+        is_nested = 'filters' in filter
+
+        if is_nested == False:
+            column = filter.get('column', None)
+            if not column:
+                raise serializers.ValidationError('Filter require a column')
+        
+            if column not in settings.ANYCLUSTER_FILTERS:
+                raise serializers.ValidationError('It is not allowed to filter Column {0}'.format(column))
         
-        if column not in settings.ANYCLUSTER_FILTERS:
-            raise serializers.ValidationError('It is not allowed to filter Column {0}'.format(column))
+        else:
+            filters_are_allowed(filter['filters'])
 
 # needs to supprt FeatureCollection and Multipolygon
 class ClusterRequestSerializer(serializers.Serializer):
 
     output_srid = serializers.CharField(default='EPSG:4326', required=False, write_only=True)
 
     geometry_type = serializers.ChoiceField(choices=GEOMETRY_TYPES, write_only=True)
```

### Comparing `anycluster-2.1.0/anycluster/api/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.1.1/anycluster/api/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc` & `anycluster-2.1.1/anycluster/api/tests/__pycache__/test_serializers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc` & `anycluster-2.1.1/anycluster/api/tests/__pycache__/test_views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/api/tests/test_serializers.py` & `anycluster-2.1.1/anycluster/api/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/api/tests/test_views.py` & `anycluster-2.1.1/anycluster/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/api/urls.py` & `anycluster-2.1.1/anycluster/api/urls.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/api/views.py` & `anycluster-2.1.1/anycluster/api/views.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/clusters.py` & `anycluster-2.1.1/anycluster/clusters.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/definitions.py` & `anycluster-2.1.1/anycluster/definitions.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/globalmaptiles.py` & `anycluster-2.1.1/anycluster/globalmaptiles.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/static/anycluster/images/10.png` & `anycluster-2.1.1/anycluster/static/anycluster/images/10.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/static/anycluster/images/100.png` & `anycluster-2.1.1/anycluster/static/anycluster/images/100.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/static/anycluster/images/1000.png` & `anycluster-2.1.1/anycluster/static/anycluster/images/1000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/static/anycluster/images/10000.png` & `anycluster-2.1.1/anycluster/static/anycluster/images/10000.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/static/anycluster/images/10000_empty.png` & `anycluster-2.1.1/anycluster/static/anycluster/images/10000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/static/anycluster/images/1000_empty.png` & `anycluster-2.1.1/anycluster/static/anycluster/images/1000_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/static/anycluster/images/100_empty.png` & `anycluster-2.1.1/anycluster/static/anycluster/images/100_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/static/anycluster/images/10_empty.png` & `anycluster-2.1.1/anycluster/static/anycluster/images/10_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/static/anycluster/images/5.png` & `anycluster-2.1.1/anycluster/static/anycluster/images/5.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/static/anycluster/images/50.png` & `anycluster-2.1.1/anycluster/static/anycluster/images/50.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/static/anycluster/images/50_empty.png` & `anycluster-2.1.1/anycluster/static/anycluster/images/50_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/static/anycluster/images/5_empty.png` & `anycluster-2.1.1/anycluster/static/anycluster/images/5_empty.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/static/anycluster/images/pin_unknown.png` & `anycluster-2.1.1/anycluster/static/anycluster/images/pin_unknown.png`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/tests/__pycache__/common.cpython-38.pyc` & `anycluster-2.1.1/anycluster/tests/__pycache__/common.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/tests/__pycache__/mixins.cpython-38.pyc` & `anycluster-2.1.1/anycluster/tests/__pycache__/mixins.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc` & `anycluster-2.1.1/anycluster/tests/__pycache__/test_ClusterCache.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/tests/__pycache__/test_FilterComposer.cpython-38.pyc` & `anycluster-2.1.1/anycluster/tests/__pycache__/test_Filters.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Fri Apr 21 13:19:10 2023 UTC, .py size: 3995 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,175 +1,181 @@
-00000000: 550d 0d0a 0000 0000 4e8d 4264 9b0f 0000  U.......N.Bd....
+00000000: 550d 0d0a 0000 0000 a7a9 3f64 d20f 0000  U.........?d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3c00 0000 6400  .....@...s<...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c05 5a05 4700 6404 6405 8400 6405  d.l.Z.G.d.d...d.
 00000060: 6501 8303 5a06 6403 5300 2906 e900 0000  e...Z.d.S.).....
 00000070: 0029 01da 0854 6573 7443 6173 6529 01da  .)...TestCase)..
-00000080: 0e46 696c 7465 7243 6f6d 706f 7365 724e  .FilterComposerN
-00000090: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000000a0: 0002 0000 0040 0000 0073 3400 0000 6500  .....@...s4...e.
-000000b0: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
-000000c0: 6404 8400 5a04 6405 6406 8400 5a05 6407  d...Z.d.d...Z.d.
-000000d0: 6408 8400 5a06 6409 640a 8400 5a07 640b  d...Z.d.d...Z.d.
-000000e0: 5300 290c da0b 5465 7374 6669 6c74 6572  S.)...Testfilter
-000000f0: 7363 0200 0000 0000 0000 0000 0000 0200  sc..............
-00000100: 0000 0400 0000 4300 0000 7366 0000 0074  ......C...sf...t
-00000110: 007c 0183 0174 016b 0272 1864 0164 0264  .|...t.k.r.d.d.d
-00000120: 0364 0467 0453 0074 007c 0183 0174 026b  .d.g.S.t.|...t.k
-00000130: 0272 2c64 0164 0267 0253 0074 037c 0174  .r,d.d.g.S.t.|.t
-00000140: 046a 0583 0273 4474 037c 0174 066a 0783  .j...sDt.|.t.j..
-00000150: 0272 5064 0164 0264 0564 0667 0453 0074  .rPd.d.d.d.g.S.t
-00000160: 037c 0174 0883 0272 6264 0764 0867 0253  .|.t...rbd.d.g.S
-00000170: 0064 0053 0029 094e fa01 3dfa 0221 3dda  .d.S.).N..=..!=.
-00000180: 0a73 7461 7274 7377 6974 68da 0863 6f6e  .startswith..con
-00000190: 7461 696e 737a 023e 3d7a 023c 3dda 0269  tainsz.>=z.<=..i
-000001a0: 6efa 066e 6f74 2069 6e29 09da 0474 7970  n..not in)...typ
-000001b0: 65da 0373 7472 da04 626f 6f6c da0a 6973  e..str..bool..is
-000001c0: 696e 7374 616e 6365 da07 6e75 6d62 6572  instance..number
-000001d0: 73da 064e 756d 6265 72da 0764 6563 696d  s..Number..decim
-000001e0: 616c da07 4465 6369 6d61 6cda 046c 6973  al..Decimal..lis
-000001f0: 7429 02da 0473 656c 66da 0576 616c 7565  t)...self..value
-00000200: a900 7216 0000 00fa 482f 686f 6d65 2f74  ..r.....H/home/t
-00000210: 6f6d 2f61 6e79 636c 7573 7465 722f 6465  om/anycluster/de
-00000220: 6d6f 2f64 6a61 6e67 6f2f 616e 7963 6c75  mo/django/anyclu
-00000230: 7374 6572 2f74 6573 7473 2f74 6573 745f  ster/tests/test_
-00000240: 4669 6c74 6572 436f 6d70 6f73 6572 2e70  FilterComposer.p
-00000250: 79da 1667 6574 5f70 6f73 7369 626c 655f  y..get_possible_
-00000260: 6f70 6572 6174 6f72 730a 0000 0073 1000  operators....s..
-00000270: 0000 0002 0c01 0c02 0c01 0802 1801 0c02  ................
-00000280: 0a01 7a22 5465 7374 6669 6c74 6572 732e  ..z"Testfilters.
-00000290: 6765 745f 706f 7373 6962 6c65 5f6f 7065  get_possible_ope
-000002a0: 7261 746f 7273 6301 0000 0000 0000 0000  ratorsc.........
-000002b0: 0000 0006 0000 0005 0000 0043 0000 0073  ...........C...s
-000002c0: 3600 0000 6700 7d01 6401 7d02 7c00 a000  6...g.}.d.}.|...
-000002d0: 7c02 a101 7d03 7c03 4400 5d1a 7d04 6402  |...}.|.D.].}.d.
-000002e0: 7c02 7c04 6403 9c03 7d05 7c01 a001 7c05  |.|.d...}.|...|.
-000002f0: a101 0100 7116 7c01 5300 2904 4eda 0666  ....q.|.S.).N..f
-00000300: 6c6f 7765 72da 0573 7479 6c65 a903 da06  lower..style....
-00000310: 636f 6c75 6d6e 7215 0000 00da 086f 7065  columnr......ope
-00000320: 7261 746f 7229 0272 1800 0000 da06 6170  rator).r......ap
-00000330: 7065 6e64 2906 7214 0000 00da 0766 696c  pend).r......fil
-00000340: 7465 7273 da0c 7374 7269 6e67 5f76 616c  ters..string_val
-00000350: 7565 5a10 7374 7269 6e67 5f6f 7065 7261  ueZ.string_opera
-00000360: 746f 7273 721d 0000 00da 0666 696c 7465  torsr......filte
-00000370: 7272 1600 0000 7216 0000 0072 1700 0000  rr....r....r....
-00000380: da0b 6765 745f 6669 6c74 6572 7319 0000  ..get_filters...
-00000390: 0073 1400 0000 0001 0402 0401 0a02 0802  .s..............
-000003a0: 0201 0201 02fd 0606 0c02 7a17 5465 7374  ..........z.Test
-000003b0: 6669 6c74 6572 732e 6765 745f 6669 6c74  filters.get_filt
-000003c0: 6572 7363 0100 0000 0000 0000 0000 0000  ersc............
-000003d0: 0300 0000 0400 0000 4300 0000 7322 0000  ........C...s"..
-000003e0: 007c 00a0 00a1 007d 0174 017c 0183 017d  .|.....}.t.|...}
-000003f0: 027c 00a0 027c 026a 037c 01a1 0201 0064  .|...|.j.|.....d
-00000400: 0053 0029 014e 2904 7222 0000 0072 0300  .S.).N).r"...r..
-00000410: 0000 da0b 6173 7365 7274 4571 7561 6c72  ....assertEqualr
-00000420: 1f00 0000 2903 7214 0000 00da 0b66 696c  ....).r......fil
-00000430: 7465 725f 6c69 7374 da0f 6669 6c74 6572  ter_list..filter
-00000440: 5f63 6f6d 706f 7365 7272 1600 0000 7216  _composerr....r.
-00000450: 0000 0072 1700 0000 da0c 7465 7374 5f5f  ...r......test__
-00000460: 696e 6974 5f5f 2a00 0000 7306 0000 0000  init__*...s.....
-00000470: 0208 0208 017a 1854 6573 7466 696c 7465  .....z.Testfilte
-00000480: 7273 2e74 6573 745f 5f69 6e69 745f 5f63  rs.test__init__c
-00000490: 0100 0000 0000 0000 0000 0000 0e00 0000  ................
-000004a0: 0500 0000 4300 0000 73f6 0000 007c 00a0  ....C...s....|..
-000004b0: 00a1 007d 0174 017c 0183 017d 0264 017d  ...}.t.|...}.d.}
-000004c0: 037c 02a0 0264 027c 03a1 027d 047c 00a0  .|...d.|...}.|..
-000004d0: 037c 0464 03a1 0201 007c 02a0 0264 047c  .|.d.....|...d.|
-000004e0: 03a1 027d 057c 00a0 037c 0564 03a1 0201  ...}.|...|.d....
-000004f0: 007c 02a0 0264 057c 03a1 027d 067c 00a0  .|...d.|...}.|..
-00000500: 037c 0664 06a1 0201 007c 02a0 0264 077c  .|.d.....|...d.|
-00000510: 03a1 027d 067c 00a0 037c 0664 08a1 0201  ...}.|...|.d....
-00000520: 007c 026a 04a0 05a1 0044 005d 725c 027d  .|.j.....D.]r\.}
-00000530: 077d 087c 02a0 027c 0764 09a1 027d 097c  .}.|...|.d...}.|
-00000540: 00a0 037c 0964 0aa1 0201 007c 02a0 027c  ...|.d.....|...|
-00000550: 0764 0ba1 027d 0a7c 00a0 037c 0a64 0ca1  .d...}.|...|.d..
-00000560: 0201 007c 02a0 027c 0764 0da1 027d 0b7c  ...|...|.d...}.|
-00000570: 00a0 037c 0b64 0da1 0201 0074 06a0 0764  ...|.d.....t...d
-00000580: 0ea1 017d 0c7c 02a0 027c 077c 0ca1 027d  ...}.|...|.|...}
-00000590: 0d7c 00a0 037c 0c7c 0da1 0201 0071 7e64  .|...|.|.....q~d
-000005a0: 0053 0029 0f4e 7219 0000 0072 0500 0000  .S.).Nr....r....
-000005b0: 7a08 2766 6c6f 7765 7227 7206 0000 0072  z.'flower'r....r
-000005c0: 0700 0000 7a0b 275e 666c 6f77 6572 2e2a  ....z.'^flower.*
-000005d0: 2772 0800 0000 7a0a 2766 6c6f 7765 722e  'r....z.'flower.
-000005e0: 2a27 54da 0454 5255 4546 da05 4641 4c53  *'T..TRUEF..FALS
-000005f0: 4567 9a99 9999 9999 0b40 67cd cccc cccc  Eg.......@g.....
-00000600: ccf4 3f29 0872 2200 0000 7203 0000 00da  ..?).r"...r.....
-00000610: 1270 6172 7365 5f66 696c 7465 725f 7661  .parse_filter_va
-00000620: 6c75 6572 2300 0000 da10 6f70 6572 6174  luer#.....operat
-00000630: 6f72 5f6d 6170 7069 6e67 da05 6974 656d  or_mapping..item
-00000640: 7372 1100 0000 7212 0000 0029 0e72 1400  sr....r....).r..
-00000650: 0000 7224 0000 0072 2500 0000 7220 0000  ..r$...r%...r ..
-00000660: 005a 0d73 7472 696e 675f 6571 7561 6c73  .Z.string_equals
-00000670: 5a0f 7374 7269 6e67 5f75 6e65 7175 616c  Z.string_unequal
-00000680: 735a 1173 7472 696e 675f 7374 6172 7473  sZ.string_starts
-00000690: 7769 7468 721d 0000 00da 096f 7065 7261  withr......opera
-000006a0: 746f 725f 5a0a 7472 7565 5f76 616c 7565  tor_Z.true_value
-000006b0: 5a0b 6661 6c73 655f 7661 6c75 65da 0c6e  Z.false_value..n
-000006c0: 756d 6265 725f 7661 6c75 65da 0364 6563  umber_value..dec
-000006d0: 5a09 6465 635f 7661 6c75 6572 1600 0000  Z.dec_valuer....
-000006e0: 7216 0000 0072 1700 0000 da17 7465 7374  r....r......test
-000006f0: 5f70 6172 7365 5f66 696c 7465 725f 7661  _parse_filter_va
-00000700: 6c75 6531 0000 0073 2a00 0000 0002 0802  lue1...s*.......
-00000710: 0803 0402 0c01 0c02 0c01 0c02 0c01 0c02  ................
-00000720: 0c01 0c02 1202 0c01 0c02 0c01 0c02 0c01  ................
-00000730: 0c02 0a01 0c01 7a23 5465 7374 6669 6c74  ......z#Testfilt
-00000740: 6572 732e 7465 7374 5f70 6172 7365 5f66  ers.test_parse_f
-00000750: 696c 7465 725f 7661 6c75 6563 0100 0000  ilter_valuec....
-00000760: 0000 0000 0000 0000 0c00 0000 0400 0000  ................
-00000770: 4300 0000 73b8 0000 0064 017d 0164 027c  C...s....d.}.d.|
-00000780: 0164 0364 049c 037d 0274 007c 0267 0183  .d.d...}.t.|.g..
-00000790: 017d 037c 03a0 01a1 007d 047c 00a0 027c  .}.|.....}.|...|
-000007a0: 0464 05a1 0201 0064 027c 0164 0664 049c  .d.....d.|.d.d..
-000007b0: 037d 0574 007c 0567 0183 017d 037c 03a0  .}.t.|.g...}.|..
-000007c0: 01a1 007d 067c 00a0 027c 0664 07a1 0201  ...}.|...|.d....
-000007d0: 0064 0164 0867 027d 0764 027c 0764 0964  .d.d.g.}.d.|.d.d
-000007e0: 049c 037d 0874 007c 0867 0183 017d 037c  ...}.t.|.g...}.|
-000007f0: 03a0 01a1 007d 097c 00a0 027c 0964 0aa1  .....}.|...|.d..
-00000800: 0201 0064 027c 0764 0b64 049c 037d 0a74  ...d.|.d.d...}.t
-00000810: 007c 0a67 0183 017d 037c 03a0 01a1 007d  .|.g...}.|.....}
-00000820: 0b7c 00a0 027c 0b64 0ca1 0201 0064 0053  .|...|.d.....d.S
-00000830: 0029 0d4e 7219 0000 0072 1a00 0000 7205  .).Nr....r....r.
-00000840: 0000 0072 1b00 0000 7a17 2041 4e44 2028  ...r....z. AND (
-00000850: 7374 796c 6520 3d20 2766 6c6f 7765 7227  style = 'flower'
-00000860: 2972 0600 0000 7a18 2041 4e44 2028 7374  )r....z. AND (st
-00000870: 796c 6520 213d 2027 666c 6f77 6572 2729  yle != 'flower')
-00000880: da05 7374 6f6e 6572 0900 0000 7a23 2041  ..stoner....z# A
-00000890: 4e44 2028 7374 796c 6520 494e 2028 2766  ND (style IN ('f
-000008a0: 6c6f 7765 7227 2c20 2773 746f 6e65 2729  lower', 'stone')
-000008b0: 2972 0a00 0000 7a27 2041 4e44 2028 7374  )r....z' AND (st
-000008c0: 796c 6520 4e4f 5420 494e 2028 2766 6c6f  yle NOT IN ('flo
-000008d0: 7765 7227 2c20 2773 746f 6e65 2729 2929  wer', 'stone')))
-000008e0: 0372 0300 0000 da06 6173 5f73 716c 7223  .r......as_sqlr#
-000008f0: 0000 0029 0c72 1400 0000 7220 0000 005a  ...).r....r ...Z
-00000900: 0d65 7175 616c 735f 6669 6c74 6572 7225  .equals_filterr%
-00000910: 0000 005a 0a65 7175 616c 735f 7371 6c5a  ...Z.equals_sqlZ
-00000920: 0f75 6e65 7175 616c 735f 6669 6c74 6572  .unequals_filter
-00000930: 5a0c 756e 6571 7561 6c73 5f73 716c 5a0a  Z.unequals_sqlZ.
-00000940: 6c69 7374 5f76 616c 7565 5a0e 696e 5f6c  list_valueZ.in_l
-00000950: 6973 745f 6669 6c74 6572 5a0b 696e 5f6c  ist_filterZ.in_l
-00000960: 6973 745f 7371 6c5a 126e 6f74 5f69 6e5f  ist_sqlZ.not_in_
-00000970: 6c69 7374 5f66 696c 7465 725a 0f6e 6f74  list_filterZ.not
-00000980: 5f69 6e5f 6c69 7374 5f73 716c 7216 0000  _in_list_sqlr...
-00000990: 0072 1600 0000 7217 0000 00da 1274 6573  .r....r......tes
-000009a0: 745f 7374 7269 6e67 5f61 735f 7371 6c56  t_string_as_sqlV
-000009b0: 0000 0073 3c00 0000 0002 0403 0201 0201  ...s<...........
-000009c0: 02fd 0606 0a02 0802 0c03 0201 0201 02fd  ................
-000009d0: 0606 0a02 0802 0c03 0802 0201 0201 02fd  ................
-000009e0: 0606 0a02 0802 0c03 0201 0201 02fd 0606  ................
-000009f0: 0a02 0802 7a1e 5465 7374 6669 6c74 6572  ....z.Testfilter
-00000a00: 732e 7465 7374 5f73 7472 696e 675f 6173  s.test_string_as
-00000a10: 5f73 716c 4e29 08da 085f 5f6e 616d 655f  _sqlN)...__name_
-00000a20: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000a30: 5f71 7561 6c6e 616d 655f 5f72 1800 0000  _qualname__r....
-00000a40: 7222 0000 0072 2600 0000 722f 0000 0072  r"...r&...r/...r
-00000a50: 3200 0000 7216 0000 0072 1600 0000 7216  2...r....r....r.
-00000a60: 0000 0072 1700 0000 7204 0000 0007 0000  ...r....r.......
-00000a70: 0073 0a00 0000 0803 080f 0811 0807 0825  .s.............%
-00000a80: 7204 0000 0029 07da 0b64 6a61 6e67 6f2e  r....)...django.
-00000a90: 7465 7374 7202 0000 00da 0a61 6e79 636c  testr......anycl
-00000aa0: 7573 7465 7272 0300 0000 720f 0000 0072  usterr....r....r
-00000ab0: 1100 0000 7204 0000 0072 1600 0000 7216  ....r....r....r.
-00000ac0: 0000 0072 1600 0000 7217 0000 00da 083c  ...r....r......<
-00000ad0: 6d6f 6475 6c65 3e01 0000 0073 0600 0000  module>....s....
-00000ae0: 0c02 0c02 1002                           ......
+00000080: 0746 696c 7465 7273 4e63 0000 0000 0000  .FiltersNc......
+00000090: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+000000a0: 0000 7334 0000 0065 005a 0164 005a 0264  ..s4...e.Z.d.Z.d
+000000b0: 0164 0284 005a 0364 0364 0484 005a 0464  .d...Z.d.d...Z.d
+000000c0: 0564 0684 005a 0564 0764 0884 005a 0664  .d...Z.d.d...Z.d
+000000d0: 0964 0a84 005a 0764 0b53 0029 0cda 0b54  .d...Z.d.S.)...T
+000000e0: 6573 7466 696c 7465 7273 6302 0000 0000  estfiltersc.....
+000000f0: 0000 0000 0000 0002 0000 0004 0000 0043  ...............C
+00000100: 0000 0073 5400 0000 7400 7c01 8301 7401  ...sT...t.|...t.
+00000110: 6b02 7218 6401 6402 6403 6404 6704 5300  k.r.d.d.d.d.g.S.
+00000120: 7400 7c01 8301 7402 6b02 722c 6401 6402  t.|...t.k.r,d.d.
+00000130: 6702 5300 7403 7c01 7404 6a05 8302 7344  g.S.t.|.t.j...sD
+00000140: 7403 7c01 7406 6a07 8302 7250 6401 6402  t.|.t.j...rPd.d.
+00000150: 6405 6406 6704 5300 6400 5300 2907 4efa  d.d.g.S.d.S.).N.
+00000160: 013d fa02 213d da0a 7374 6172 7473 7769  .=..!=..startswi
+00000170: 7468 da08 636f 6e74 6169 6e73 7a02 3e3d  th..containsz.>=
+00000180: 7a02 3c3d 2908 da04 7479 7065 da03 7374  z.<=)...type..st
+00000190: 72da 0462 6f6f 6cda 0a69 7369 6e73 7461  r..bool..isinsta
+000001a0: 6e63 65da 076e 756d 6265 7273 da06 4e75  nce..numbers..Nu
+000001b0: 6d62 6572 da07 6465 6369 6d61 6cda 0744  mber..decimal..D
+000001c0: 6563 696d 616c 2902 da04 7365 6c66 da05  ecimal)...self..
+000001d0: 7661 6c75 65a9 0072 1300 0000 fa41 2f68  value..r.....A/h
+000001e0: 6f6d 652f 746f 6d2f 616e 7963 6c75 7374  ome/tom/anyclust
+000001f0: 6572 2f64 656d 6f2f 646a 616e 676f 2f61  er/demo/django/a
+00000200: 6e79 636c 7573 7465 722f 7465 7374 732f  nycluster/tests/
+00000210: 7465 7374 5f46 696c 7465 7273 2e70 79da  test_Filters.py.
+00000220: 1667 6574 5f70 6f73 7369 626c 655f 6f70  .get_possible_op
+00000230: 6572 6174 6f72 730a 0000 0073 0c00 0000  erators....s....
+00000240: 0002 0c01 0c02 0c01 0802 1801 7a22 5465  ............z"Te
+00000250: 7374 6669 6c74 6572 732e 6765 745f 706f  stfilters.get_po
+00000260: 7373 6962 6c65 5f6f 7065 7261 746f 7273  ssible_operators
+00000270: 6301 0000 0000 0000 0000 0000 0006 0000  c...............
+00000280: 0005 0000 0043 0000 0073 3600 0000 6700  .....C...s6...g.
+00000290: 7d01 6401 7d02 7c00 a000 7c02 a101 7d03  }.d.}.|...|...}.
+000002a0: 7c03 4400 5d1a 7d04 6402 7c02 7c04 6403  |.D.].}.d.|.|.d.
+000002b0: 9c03 7d05 7c01 a001 7c05 a101 0100 7116  ..}.|...|.....q.
+000002c0: 7c01 5300 2904 4eda 0666 6c6f 7765 72da  |.S.).N..flower.
+000002d0: 0573 7479 6c65 a903 da06 636f 6c75 6d6e  .style....column
+000002e0: 7212 0000 00da 086f 7065 7261 746f 7229  r......operator)
+000002f0: 0272 1500 0000 da06 6170 7065 6e64 2906  .r......append).
+00000300: 7211 0000 00da 0766 696c 7465 7273 da0c  r......filters..
+00000310: 7374 7269 6e67 5f76 616c 7565 5a10 7374  string_valueZ.st
+00000320: 7269 6e67 5f6f 7065 7261 746f 7273 721a  ring_operatorsr.
+00000330: 0000 00da 0666 696c 7465 7272 1300 0000  .....filterr....
+00000340: 7213 0000 0072 1400 0000 da0b 6765 745f  r....r......get_
+00000350: 6669 6c74 6572 7316 0000 0073 1400 0000  filters....s....
+00000360: 0001 0402 0401 0a02 0802 0201 0201 02fd  ................
+00000370: 0606 0c02 7a17 5465 7374 6669 6c74 6572  ....z.Testfilter
+00000380: 732e 6765 745f 6669 6c74 6572 7363 0100  s.get_filtersc..
+00000390: 0000 0000 0000 0000 0000 0300 0000 0400  ................
+000003a0: 0000 4300 0000 7322 0000 007c 00a0 00a1  ..C...s"...|....
+000003b0: 007d 0174 017c 0183 017d 027c 00a0 027c  .}.t.|...}.|...|
+000003c0: 026a 037c 01a1 0201 0064 0053 0029 014e  .j.|.....d.S.).N
+000003d0: 2904 721f 0000 0072 0300 0000 da0b 6173  ).r....r......as
+000003e0: 7365 7274 4571 7561 6c72 1c00 0000 2903  sertEqualr....).
+000003f0: 7211 0000 00da 0b66 696c 7465 725f 6c69  r......filter_li
+00000400: 7374 721c 0000 0072 1300 0000 7213 0000  str....r....r...
+00000410: 0072 1400 0000 da0c 7465 7374 5f5f 696e  .r......test__in
+00000420: 6974 5f5f 2700 0000 7306 0000 0000 0208  it__'...s.......
+00000430: 0208 017a 1854 6573 7466 696c 7465 7273  ...z.Testfilters
+00000440: 2e74 6573 745f 5f69 6e69 745f 5f63 0100  .test__init__c..
+00000450: 0000 0000 0000 0000 0000 0e00 0000 0500  ................
+00000460: 0000 4300 0000 73f6 0000 007c 00a0 00a1  ..C...s....|....
+00000470: 007d 0174 017c 0183 017d 0264 017d 037c  .}.t.|...}.d.}.|
+00000480: 02a0 0264 027c 03a1 027d 047c 00a0 037c  ...d.|...}.|...|
+00000490: 0464 03a1 0201 007c 02a0 0264 047c 03a1  .d.....|...d.|..
+000004a0: 027d 057c 00a0 037c 0564 03a1 0201 007c  .}.|...|.d.....|
+000004b0: 02a0 0264 057c 03a1 027d 067c 00a0 037c  ...d.|...}.|...|
+000004c0: 0664 06a1 0201 007c 02a0 0264 077c 03a1  .d.....|...d.|..
+000004d0: 027d 067c 00a0 037c 0664 08a1 0201 007c  .}.|...|.d.....|
+000004e0: 026a 04a0 05a1 0044 005d 725c 027d 077d  .j.....D.]r\.}.}
+000004f0: 087c 02a0 027c 0764 09a1 027d 097c 00a0  .|...|.d...}.|..
+00000500: 037c 0964 0aa1 0201 007c 02a0 027c 0764  .|.d.....|...|.d
+00000510: 0ba1 027d 0a7c 00a0 037c 0a64 0ca1 0201  ...}.|...|.d....
+00000520: 007c 02a0 027c 0764 0da1 027d 0b7c 00a0  .|...|.d...}.|..
+00000530: 037c 0b64 0da1 0201 0074 06a0 0764 0ea1  .|.d.....t...d..
+00000540: 017d 0c7c 02a0 027c 077c 0ca1 027d 0d7c  .}.|...|.|...}.|
+00000550: 00a0 037c 0c7c 0da1 0201 0071 7e64 0053  ...|.|.....q~d.S
+00000560: 0029 0f4e 7216 0000 0072 0500 0000 7a08  .).Nr....r....z.
+00000570: 2766 6c6f 7765 7227 7206 0000 0072 0700  'flower'r....r..
+00000580: 0000 7a0b 275e 666c 6f77 6572 2e2a 2772  ..z.'^flower.*'r
+00000590: 0800 0000 7a0a 2766 6c6f 7765 722e 2a27  ....z.'flower.*'
+000005a0: 54da 0454 5255 4546 da05 4641 4c53 4567  T..TRUEF..FALSEg
+000005b0: 9a99 9999 9999 0b40 67cd cccc cccc ccf4  .......@g.......
+000005c0: 3f29 0872 1f00 0000 7203 0000 00da 1270  ?).r....r......p
+000005d0: 6172 7365 5f66 696c 7465 725f 7661 6c75  arse_filter_valu
+000005e0: 6572 2000 0000 da10 6f70 6572 6174 6f72  er .....operator
+000005f0: 5f6d 6170 7069 6e67 da05 6974 656d 7372  _mapping..itemsr
+00000600: 0f00 0000 7210 0000 0029 0e72 1100 0000  ....r....).r....
+00000610: 7221 0000 0072 1c00 0000 721d 0000 005a  r!...r....r....Z
+00000620: 0d73 7472 696e 675f 6571 7561 6c73 5a0f  .string_equalsZ.
+00000630: 7374 7269 6e67 5f75 6e65 7175 616c 735a  string_unequalsZ
+00000640: 1173 7472 696e 675f 7374 6172 7473 7769  .string_startswi
+00000650: 7468 721a 0000 00da 096f 7065 7261 746f  thr......operato
+00000660: 725f 5a0a 7472 7565 5f76 616c 7565 5a0b  r_Z.true_valueZ.
+00000670: 6661 6c73 655f 7661 6c75 65da 0c6e 756d  false_value..num
+00000680: 6265 725f 7661 6c75 65da 0364 6563 5a09  ber_value..decZ.
+00000690: 6465 635f 7661 6c75 6572 1300 0000 7213  dec_valuer....r.
+000006a0: 0000 0072 1400 0000 da17 7465 7374 5f70  ...r......test_p
+000006b0: 6172 7365 5f66 696c 7465 725f 7661 6c75  arse_filter_valu
+000006c0: 652e 0000 0073 2a00 0000 0002 0802 0803  e....s*.........
+000006d0: 0402 0c01 0c02 0c01 0c02 0c01 0c02 0c01  ................
+000006e0: 0c02 1202 0c01 0c02 0c01 0c02 0c01 0c02  ................
+000006f0: 0a01 0c01 7a23 5465 7374 6669 6c74 6572  ....z#Testfilter
+00000700: 732e 7465 7374 5f70 6172 7365 5f66 696c  s.test_parse_fil
+00000710: 7465 725f 7661 6c75 6563 0100 0000 0000  ter_valuec......
+00000720: 0000 0000 0000 0e00 0000 0500 0000 4300  ..............C.
+00000730: 0000 73e4 0000 0064 017d 0164 027c 0164  ..s....d.}.d.|.d
+00000740: 0364 049c 037d 0274 007c 0267 0183 017d  .d...}.t.|.g...}
+00000750: 037c 03a0 01a1 007d 047c 00a0 027c 0464  .|.....}.|...|.d
+00000760: 05a1 0201 0064 027c 0164 0664 049c 037d  .....d.|.d.d...}
+00000770: 0574 007c 0567 0183 017d 037c 03a0 01a1  .t.|.g...}.|....
+00000780: 007d 067c 00a0 027c 0664 07a1 0201 0064  .}.|...|.d.....d
+00000790: 0164 0867 027d 0764 027c 0764 0364 049c  .d.g.}.d.|.d.d..
+000007a0: 037d 0874 007c 0867 0183 017d 037c 03a0  .}.t.|.g...}.|..
+000007b0: 01a1 007d 097c 00a0 027c 0964 09a1 0201  ...}.|...|.d....
+000007c0: 0064 027c 0764 0664 049c 037d 0a74 007c  .d.|.d.d...}.t.|
+000007d0: 0a67 0183 017d 037c 03a0 01a1 007d 0b7c  .g...}.|.....}.|
+000007e0: 00a0 027c 0b64 0aa1 0201 0064 027c 0764  ...|.d.....d.|.d
+000007f0: 0364 0b64 0c9c 047d 0c74 007c 0c67 0183  .d.d...}.t.|.g..
+00000800: 017d 037c 03a0 01a1 007d 0d7c 00a0 027c  .}.|.....}.|...|
+00000810: 0d64 0da1 0201 0064 0053 0029 0e4e 7216  .d.....d.S.).Nr.
+00000820: 0000 0072 1700 0000 7205 0000 0072 1800  ...r....r....r..
+00000830: 0000 7a17 2041 4e44 2028 7374 796c 6520  ..z. AND (style 
+00000840: 3d20 2766 6c6f 7765 7227 2972 0600 0000  = 'flower')r....
+00000850: 7a18 2041 4e44 2028 7374 796c 6520 213d  z. AND (style !=
+00000860: 2027 666c 6f77 6572 2729 da05 7374 6f6e   'flower')..ston
+00000870: 657a 2320 414e 4420 2873 7479 6c65 2049  ez# AND (style I
+00000880: 4e20 2827 666c 6f77 6572 272c 2027 7374  N ('flower', 'st
+00000890: 6f6e 6527 2929 7a27 2041 4e44 2028 7374  one'))z' AND (st
+000008a0: 796c 6520 4e4f 5420 494e 2028 2766 6c6f  yle NOT IN ('flo
+000008b0: 7765 7227 2c20 2773 746f 6e65 2729 29da  wer', 'stone')).
+000008c0: 026f 7229 0472 1900 0000 7212 0000 0072  .or).r....r....r
+000008d0: 1a00 0000 da0c 6c69 7374 4f70 6572 6174  ......listOperat
+000008e0: 6f72 7a2a 2041 4e44 2028 7374 796c 6520  orz* AND (style 
+000008f0: 3d20 2766 6c6f 7765 7227 204f 5220 7374  = 'flower' OR st
+00000900: 796c 6520 3d20 2773 746f 6e65 2729 2903  yle = 'stone')).
+00000910: 7203 0000 00da 0661 735f 7371 6c72 2000  r......as_sqlr .
+00000920: 0000 290e 7211 0000 0072 1d00 0000 5a0d  ..).r....r....Z.
+00000930: 6571 7561 6c73 5f66 696c 7465 7272 1c00  equals_filterr..
+00000940: 0000 5a0a 6571 7561 6c73 5f73 716c 5a0f  ..Z.equals_sqlZ.
+00000950: 756e 6571 7561 6c73 5f66 696c 7465 725a  unequals_filterZ
+00000960: 0c75 6e65 7175 616c 735f 7371 6c5a 0a6c  .unequals_sqlZ.l
+00000970: 6973 745f 7661 6c75 655a 0e69 6e5f 6c69  ist_valueZ.in_li
+00000980: 7374 5f66 696c 7465 725a 0b69 6e5f 6c69  st_filterZ.in_li
+00000990: 7374 5f73 716c 5a12 6e6f 745f 696e 5f6c  st_sqlZ.not_in_l
+000009a0: 6973 745f 6669 6c74 6572 5a0f 6e6f 745f  ist_filterZ.not_
+000009b0: 696e 5f6c 6973 745f 7371 6c5a 0e6f 725f  in_list_sqlZ.or_
+000009c0: 6c69 7374 5f66 696c 7465 725a 0b6f 725f  list_filterZ.or_
+000009d0: 6c69 7374 5f73 716c 7213 0000 0072 1300  list_sqlr....r..
+000009e0: 0000 7214 0000 00da 1274 6573 745f 7374  ..r......test_st
+000009f0: 7269 6e67 5f61 735f 7371 6c53 0000 0073  ring_as_sqlS...s
+00000a00: 4c00 0000 0002 0403 0201 0201 02fd 0606  L...............
+00000a10: 0a02 0802 0c03 0201 0201 02fd 0606 0a02  ................
+00000a20: 0802 0c03 0802 0201 0201 02fd 0606 0a02  ................
+00000a30: 0802 0c03 0201 0201 02fd 0606 0a02 0802  ................
+00000a40: 0c04 0201 0201 0201 02fc 0607 0a02 0802  ................
+00000a50: 7a1e 5465 7374 6669 6c74 6572 732e 7465  z.Testfilters.te
+00000a60: 7374 5f73 7472 696e 675f 6173 5f73 716c  st_string_as_sql
+00000a70: 4e29 08da 085f 5f6e 616d 655f 5fda 0a5f  N)...__name__.._
+00000a80: 5f6d 6f64 756c 655f 5fda 0c5f 5f71 7561  _module__..__qua
+00000a90: 6c6e 616d 655f 5f72 1500 0000 721f 0000  lname__r....r...
+00000aa0: 0072 2200 0000 722b 0000 0072 3000 0000  .r"...r+...r0...
+00000ab0: 7213 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
+00000ac0: 1400 0000 7204 0000 0007 0000 0073 0a00  ....r........s..
+00000ad0: 0000 0803 080c 0811 0807 0825 7204 0000  ...........%r...
+00000ae0: 0029 07da 0b64 6a61 6e67 6f2e 7465 7374  .)...django.test
+00000af0: 7202 0000 00da 0a61 6e79 636c 7573 7465  r......anycluste
+00000b00: 7272 0300 0000 720d 0000 0072 0f00 0000  rr....r....r....
+00000b10: 7204 0000 0072 1300 0000 7213 0000 0072  r....r....r....r
+00000b20: 1300 0000 7214 0000 00da 083c 6d6f 6475  ....r......<modu
+00000b30: 6c65 3e01 0000 0073 0600 0000 0c02 0c02  le>....s........
+00000b40: 1002                                     ..
```

### Comparing `anycluster-2.1.0/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc` & `anycluster-2.1.1/anycluster/tests/__pycache__/test_MapClusterer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/tests/common.py` & `anycluster-2.1.1/anycluster/tests/common.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/tests/mixins.py` & `anycluster-2.1.1/anycluster/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/tests/test_ClusterCache.py` & `anycluster-2.1.1/anycluster/tests/test_ClusterCache.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster/tests/test_FilterComposer.py` & `anycluster-2.1.1/anycluster/tests/test_FilterComposer.py`

 * *Files 26% similar despite different names*

```diff
@@ -82,14 +82,15 @@
             dec_value = filter_composer.parse_filter_value(operator, dec)
             self.assertEqual(dec, dec_value)
 
 
     def test_string_as_sql(self):
 
         string_value = 'flower'
+        string_value_2 = 'stone'
         
         equals_filter = {
             'column': 'style',
             'value': string_value,
             'operator': '=',
         }
 
@@ -97,23 +98,23 @@
 
         equals_sql = filter_composer.as_sql()
         
         self.assertEqual(equals_sql, " AND (style = 'flower')")
         
         unequals_filter = {
             'column': 'style',
-            'value': string_value,
+            'value': string_value_2,
             'operator': '!=',
         }
 
         filter_composer = FilterComposer([unequals_filter])
 
         unequals_sql = filter_composer.as_sql()
         
-        self.assertEqual(unequals_sql, " AND (style != 'flower')")
+        self.assertEqual(unequals_sql, " AND (style != 'stone')")
 
         # list
         list_value = ['flower', 'stone']
         in_list_filter = {
             'column': 'style',
             'value': list_value,
             'operator': 'in',
@@ -131,8 +132,93 @@
             'operator': 'not in',
         }
 
         filter_composer = FilterComposer([not_in_list_filter])
 
         not_in_list_sql = filter_composer.as_sql()
         
-        self.assertEqual(not_in_list_sql, " AND (style NOT IN ('flower', 'stone'))")
+        self.assertEqual(not_in_list_sql, " AND (style NOT IN ('flower', 'stone'))")
+
+        # test multiple filters
+        filter_composer = FilterComposer([equals_filter, unequals_filter])
+
+        equals_sql = filter_composer.as_sql()
+        
+        self.assertEqual(equals_sql, " AND ((style = 'flower') AND (style != 'stone'))")
+
+
+    def test_nested_filter(self):
+        
+        nested_filter = {
+            'filters' : [
+                {
+                    'column': 'style',
+                    'value': 'flower',
+                    'operator': '=',
+                },
+                {
+                    'column': 'style',
+                    'value': 'stone',
+                    'operator': '=',
+                    'logicalOperator': 'OR'
+                }
+            ],
+        }
+
+        filter_composer = FilterComposer([nested_filter])
+
+        nested_sql = filter_composer.as_sql()
+        
+        self.assertEqual(nested_sql, " AND ((style = 'flower') OR (style = 'stone'))")
+
+        equals_filter = {
+            'column': 'free_entrance',
+            'value': True,
+            'operator': '=',
+        }
+
+        nested_filter_2 = {
+            'filters' : [
+                {
+                    'column': 'style',
+                    'value': 'flower',
+                    'operator': '=',
+                },
+                {
+                    'column': 'free_entrance',
+                    'value': True,
+                    'operator': '=',
+                    'logicalOperator': 'AND'
+                }
+            ],
+        }
+
+        nested_filter_3 = {
+            'logicalOperator': 'OR',
+            'filters' : [
+                {
+                    'column': 'style',
+                    'value': 'stone',
+                    'operator': '=',
+                },
+                {
+                    'column': 'free_entrance',
+                    'value': False,
+                    'operator': '=',
+                    'logicalOperator': 'AND'
+                }
+            ],
+        }
+
+
+        filter_composer = FilterComposer([nested_filter_2, nested_filter_3])
+
+        nested_sql = filter_composer.as_sql()
+        
+        self.assertEqual(nested_sql, " AND (((style = 'flower') AND (free_entrance = TRUE)) OR ((style = 'stone') AND (free_entrance = FALSE)))")
+
+
+        filter_composer = FilterComposer([nested_filter_2, nested_filter_3, equals_filter])
+
+        nested_sql = filter_composer.as_sql()
+
+        self.assertEqual(nested_sql, " AND (((style = 'flower') AND (free_entrance = TRUE)) OR ((style = 'stone') AND (free_entrance = FALSE)) AND (free_entrance = TRUE))")
```

### Comparing `anycluster-2.1.0/anycluster/tests/test_MapClusterer.py` & `anycluster-2.1.1/anycluster/tests/test_MapClusterer.py`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/anycluster.egg-info/PKG-INFO` & `anycluster-2.1.1/anycluster.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anycluster
-Version: 2.1.0
+Version: 2.1.1
 Summary: anycluster provides Server-Side clustering of map markers for Geodjango
 Home-page: https://github.com/biodiv/anycluster
 Author: Thomas Uher
 Author-email: thomas.uher@sisol-systems.com
 License: The MIT License
 Keywords: django,cluster,kmeans,grid,server-side clustering
 Platform: OS Independent
```

### Comparing `anycluster-2.1.0/anycluster.egg-info/SOURCES.txt` & `anycluster-2.1.1/anycluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anycluster-2.1.0/setup.py` & `anycluster-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     'psycopg2',
     'djangorestframework',
     'jsonschema',
 ]
 
 setup(
     name="anycluster",
-    version='2.1.0',
+    version='2.1.1',
     description='anycluster provides Server-Side clustering of map markers for Geodjango',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='The MIT License',
     platforms=['OS Independent'],
     keywords='django, cluster, kmeans, grid, server-side clustering',
     author='Thomas Uher',
```

