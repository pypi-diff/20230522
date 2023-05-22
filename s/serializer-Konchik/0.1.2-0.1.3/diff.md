# Comparing `tmp/serializer_Konchik-0.1.2.tar.gz` & `tmp/serializer_Konchik-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializer_Konchik-0.1.2.tar", last modified: Mon May 22 16:54:53 2023, max compression
+gzip compressed data, was "serializer_Konchik-0.1.3.tar", last modified: Mon May 22 16:59:40 2023, max compression
```

## Comparing `serializer_Konchik-0.1.2.tar` & `serializer_Konchik-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:54:53.741932 serializer_Konchik-0.1.2/
--rw-rw-rw-   0        0        0      262 2023-05-22 16:54:53.741932 serializer_Konchik-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 16:54:53.695158 serializer_Konchik-0.1.2/serializer_Konchik.egg-info/
--rw-rw-rw-   0        0        0      262 2023-05-22 16:54:53.000000 serializer_Konchik-0.1.2/serializer_Konchik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-05-22 16:54:53.000000 serializer_Konchik-0.1.2/serializer_Konchik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:54:53.000000 serializer_Konchik-0.1.2/serializer_Konchik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-22 16:54:53.000000 serializer_Konchik-0.1.2/serializer_Konchik.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-22 16:54:53.000000 serializer_Konchik-0.1.2/serializer_Konchik.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 16:54:53.741932 serializer_Konchik-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      550 2023-05-22 16:54:33.000000 serializer_Konchik-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:54:53.695158 serializer_Konchik-0.1.2/src/
--rw-rw-rw-   0        0        0      131 2023-05-22 14:43:23.000000 serializer_Konchik-0.1.2/src/__init__.py
--rw-rw-rw-   0        0        0     2698 2023-05-20 13:25:33.000000 serializer_Konchik-0.1.2/src/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:54:53.726317 serializer_Konchik-0.1.2/src/packer/
--rw-rw-rw-   0        0        0       80 2023-05-15 16:52:51.000000 serializer_Konchik-0.1.2/src/packer/__init__.py
--rw-rw-rw-   0        0        0     5256 2023-05-20 20:31:34.000000 serializer_Konchik-0.1.2/src/packer/packer.py
--rw-rw-rw-   0        0        0     5364 2023-05-20 20:11:55.000000 serializer_Konchik-0.1.2/src/packer/unpacker.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:54:53.741932 serializer_Konchik-0.1.2/src/serializer/
--rw-rw-rw-   0        0        0      181 2023-05-21 18:46:42.000000 serializer_Konchik-0.1.2/src/serializer/__init__.py
--rw-rw-rw-   0        0        0     1366 2023-05-22 16:01:32.000000 serializer_Konchik-0.1.2/src/serializer/base_serializer.py
--rw-rw-rw-   0        0        0     3301 2023-05-22 16:06:02.000000 serializer_Konchik-0.1.2/src/serializer/json_serializer.py
--rw-rw-rw-   0        0        0      702 2023-05-22 16:06:59.000000 serializer_Konchik-0.1.2/src/serializer/serializer_factory.py
--rw-rw-rw-   0        0        0     3854 2023-05-22 16:05:46.000000 serializer_Konchik-0.1.2/src/serializer/xml_serializer.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:59:40.432658 serializer_Konchik-0.1.3/
+-rw-rw-rw-   0        0        0      262 2023-05-22 16:59:40.432658 serializer_Konchik-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 16:59:40.421095 serializer_Konchik-0.1.3/serializer_Konchik.egg-info/
+-rw-rw-rw-   0        0        0      262 2023-05-22 16:59:40.000000 serializer_Konchik-0.1.3/serializer_Konchik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-05-22 16:59:40.000000 serializer_Konchik-0.1.3/serializer_Konchik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:59:40.000000 serializer_Konchik-0.1.3/serializer_Konchik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-22 16:59:40.000000 serializer_Konchik-0.1.3/serializer_Konchik.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-22 16:59:40.000000 serializer_Konchik-0.1.3/serializer_Konchik.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 16:59:40.432658 serializer_Konchik-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      704 2023-05-22 16:58:58.000000 serializer_Konchik-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:59:40.423509 serializer_Konchik-0.1.3/src/
+-rw-rw-rw-   0        0        0      131 2023-05-22 14:43:23.000000 serializer_Konchik-0.1.3/src/__init__.py
+-rw-rw-rw-   0        0        0     2698 2023-05-20 13:25:33.000000 serializer_Konchik-0.1.3/src/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:59:40.424650 serializer_Konchik-0.1.3/src/packer/
+-rw-rw-rw-   0        0        0       80 2023-05-15 16:52:51.000000 serializer_Konchik-0.1.3/src/packer/__init__.py
+-rw-rw-rw-   0        0        0     5256 2023-05-20 20:31:34.000000 serializer_Konchik-0.1.3/src/packer/packer.py
+-rw-rw-rw-   0        0        0     5364 2023-05-20 20:11:55.000000 serializer_Konchik-0.1.3/src/packer/unpacker.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:59:40.432658 serializer_Konchik-0.1.3/src/serializer/
+-rw-rw-rw-   0        0        0      181 2023-05-21 18:46:42.000000 serializer_Konchik-0.1.3/src/serializer/__init__.py
+-rw-rw-rw-   0        0        0     1366 2023-05-22 16:01:32.000000 serializer_Konchik-0.1.3/src/serializer/base_serializer.py
+-rw-rw-rw-   0        0        0     3301 2023-05-22 16:06:02.000000 serializer_Konchik-0.1.3/src/serializer/json_serializer.py
+-rw-rw-rw-   0        0        0      702 2023-05-22 16:06:59.000000 serializer_Konchik-0.1.3/src/serializer/serializer_factory.py
+-rw-rw-rw-   0        0        0     3854 2023-05-22 16:05:46.000000 serializer_Konchik-0.1.3/src/serializer/xml_serializer.py
```

### Comparing `serializer_Konchik-0.1.2/src/constants.py` & `serializer_Konchik-0.1.3/src/constants.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.2/src/packer/packer.py` & `serializer_Konchik-0.1.3/src/packer/packer.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.2/src/packer/unpacker.py` & `serializer_Konchik-0.1.3/src/packer/unpacker.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.2/src/serializer/base_serializer.py` & `serializer_Konchik-0.1.3/src/serializer/base_serializer.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.2/src/serializer/json_serializer.py` & `serializer_Konchik-0.1.3/src/serializer/json_serializer.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.2/src/serializer/serializer_factory.py` & `serializer_Konchik-0.1.3/src/serializer/serializer_factory.py`

 * *Files identical despite different names*

### Comparing `serializer_Konchik-0.1.2/src/serializer/xml_serializer.py` & `serializer_Konchik-0.1.3/src/serializer/xml_serializer.py`

 * *Files identical despite different names*

