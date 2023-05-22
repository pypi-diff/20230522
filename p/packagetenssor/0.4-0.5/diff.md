# Comparing `tmp/packagetenssor-0.4.tar.gz` & `tmp/packagetenssor-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packagetenssor-0.4.tar", last modified: Mon May 22 05:28:18 2023, max compression
+gzip compressed data, was "packagetenssor-0.5.tar", last modified: Mon May 22 05:55:57 2023, max compression
```

## Comparing `packagetenssor-0.4.tar` & `packagetenssor-0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        0 2023-05-22 05:28:18.371664 packagetenssor-0.4/
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)      215 2023-05-22 05:28:18.371268 packagetenssor-0.4/PKG-INFO
-drwxr-xr-x   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        0 2023-05-22 05:28:18.365460 packagetenssor-0.4/packagetenssor.egg-info/
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)      215 2023-05-22 05:28:18.000000 packagetenssor-0.4/packagetenssor.egg-info/PKG-INFO
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)      180 2023-05-22 05:28:18.000000 packagetenssor-0.4/packagetenssor.egg-info/SOURCES.txt
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        1 2023-05-22 05:28:18.000000 packagetenssor-0.4/packagetenssor.egg-info/dependency_links.txt
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        8 2023-05-22 05:28:18.000000 packagetenssor-0.4/packagetenssor.egg-info/top_level.txt
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)       38 2023-05-22 05:28:18.371741 packagetenssor-0.4/setup.cfg
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)      258 2023-05-22 05:28:02.000000 packagetenssor-0.4/setup.py
-drwxr-xr-x   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        0 2023-05-22 05:28:18.369506 packagetenssor-0.4/tenssor/
--rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)    19440 2023-05-22 05:27:39.000000 packagetenssor-0.4/tenssor/__init__.py
+drwxr-xr-x   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        0 2023-05-22 05:55:57.188758 packagetenssor-0.5/
+-rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)      215 2023-05-22 05:55:57.188400 packagetenssor-0.5/PKG-INFO
+drwxr-xr-x   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        0 2023-05-22 05:55:57.186501 packagetenssor-0.5/packagetenssor.egg-info/
+-rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)      215 2023-05-22 05:55:57.000000 packagetenssor-0.5/packagetenssor.egg-info/PKG-INFO
+-rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)      180 2023-05-22 05:55:57.000000 packagetenssor-0.5/packagetenssor.egg-info/SOURCES.txt
+-rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        1 2023-05-22 05:55:57.000000 packagetenssor-0.5/packagetenssor.egg-info/dependency_links.txt
+-rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        8 2023-05-22 05:55:57.000000 packagetenssor-0.5/packagetenssor.egg-info/top_level.txt
+-rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)       38 2023-05-22 05:55:57.188820 packagetenssor-0.5/setup.cfg
+-rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)      258 2023-05-22 05:55:46.000000 packagetenssor-0.5/setup.py
+drwxr-xr-x   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)        0 2023-05-22 05:55:57.187457 packagetenssor-0.5/tenssor/
+-rw-r--r--   0 ankit.sharma10 (101996570) FKIPL\Domain Users (1493847943)    31114 2023-05-22 05:54:15.000000 packagetenssor-0.5/tenssor/__init__.py
```

