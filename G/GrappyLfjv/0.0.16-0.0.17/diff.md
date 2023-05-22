# Comparing `tmp/GrappyLfjv-0.0.16.tar.gz` & `tmp/GrappyLfjv-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GrappyLfjv-0.0.16.tar", last modified: Sun May 21 23:56:31 2023, max compression
+gzip compressed data, was "GrappyLfjv-0.0.17.tar", last modified: Mon May 22 00:37:41 2023, max compression
```

## Comparing `GrappyLfjv-0.0.16.tar` & `GrappyLfjv-0.0.17.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-21 23:56:31.703293 GrappyLfjv-0.0.16/
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     1060 2023-05-16 15:35:17.000000 GrappyLfjv-0.0.16/LICENSE
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      524 2023-05-21 23:56:31.702937 GrappyLfjv-0.0.16/PKG-INFO
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      267 2023-05-21 23:45:53.000000 GrappyLfjv-0.0.16/README.md
--rw-r--r--   0 benjamintrevian   (501) staff       (20)       38 2023-05-21 23:56:31.703455 GrappyLfjv-0.0.16/setup.cfg
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      555 2023-05-21 23:56:26.000000 GrappyLfjv-0.0.16/setup.py
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-21 23:56:31.699859 GrappyLfjv-0.0.16/src/
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-21 23:56:31.702344 GrappyLfjv-0.0.16/src/GrappyLfjv.egg-info/
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      524 2023-05-21 23:56:31.000000 GrappyLfjv-0.0.16/src/GrappyLfjv.egg-info/PKG-INFO
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      229 2023-05-21 23:56:31.000000 GrappyLfjv-0.0.16/src/GrappyLfjv.egg-info/SOURCES.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)        1 2023-05-21 23:56:31.000000 GrappyLfjv-0.0.16/src/GrappyLfjv.egg-info/dependency_links.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)       15 2023-05-21 23:56:31.000000 GrappyLfjv-0.0.16/src/GrappyLfjv.egg-info/requires.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)        7 2023-05-21 23:56:31.000000 GrappyLfjv-0.0.16/src/GrappyLfjv.egg-info/top_level.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     4086 2023-05-21 23:35:12.000000 GrappyLfjv-0.0.16/src/grappy.py
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 00:37:41.211758 GrappyLfjv-0.0.17/
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     1060 2023-05-16 15:35:17.000000 GrappyLfjv-0.0.17/LICENSE
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     1395 2023-05-22 00:37:41.211352 GrappyLfjv-0.0.17/PKG-INFO
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     1139 2023-05-22 00:26:49.000000 GrappyLfjv-0.0.17/README.md
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)       38 2023-05-22 00:37:41.211916 GrappyLfjv-0.0.17/setup.cfg
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)      606 2023-05-22 00:37:35.000000 GrappyLfjv-0.0.17/setup.py
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 00:37:41.207998 GrappyLfjv-0.0.17/src/
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 00:37:41.210615 GrappyLfjv-0.0.17/src/GrappyLfjv.egg-info/
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     1395 2023-05-22 00:37:41.000000 GrappyLfjv-0.0.17/src/GrappyLfjv.egg-info/PKG-INFO
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)      229 2023-05-22 00:37:41.000000 GrappyLfjv-0.0.17/src/GrappyLfjv.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)        1 2023-05-22 00:37:41.000000 GrappyLfjv-0.0.17/src/GrappyLfjv.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)       15 2023-05-22 00:37:41.000000 GrappyLfjv-0.0.17/src/GrappyLfjv.egg-info/requires.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)        7 2023-05-22 00:37:41.000000 GrappyLfjv-0.0.17/src/GrappyLfjv.egg-info/top_level.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     4085 2023-05-22 00:19:27.000000 GrappyLfjv-0.0.17/src/grappy.py
```

### Comparing `GrappyLfjv-0.0.16/LICENSE` & `GrappyLfjv-0.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `GrappyLfjv-0.0.16/src/grappy.py` & `GrappyLfjv-0.0.17/src/grappy.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,14 @@
                         plt.xlabel(label[0])
                         plt.ylabel(label[1])
                         break
 
                     for ligne in csv_reader:
                         self.x.append(ligne[0])
                         self.y.append(ligne[1])
-
                 else:
                     for ligne in csv_reader:
                         for x in range(len(ligne)):
                             self.x.append(ligne[x])
                         for y in range(len(ligne)):
                             self.y.append(ligne[y])
                         break
```

