# Comparing `tmp/GrappyLfjv-0.0.18.tar.gz` & `tmp/GrappyLfjv-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GrappyLfjv-0.0.18.tar", last modified: Mon May 22 07:17:23 2023, max compression
+gzip compressed data, was "GrappyLfjv-0.0.19.tar", last modified: Mon May 22 07:23:57 2023, max compression
```

## Comparing `GrappyLfjv-0.0.18.tar` & `GrappyLfjv-0.0.19.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:17:23.174525 GrappyLfjv-0.0.18/
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     1060 2023-05-16 15:35:17.000000 GrappyLfjv-0.0.18/LICENSE
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     3207 2023-05-22 07:17:23.174063 GrappyLfjv-0.0.18/PKG-INFO
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     3030 2023-05-22 07:17:05.000000 GrappyLfjv-0.0.18/README.md
--rw-r--r--   0 benjamintrevian   (501) staff       (20)       38 2023-05-22 07:17:23.174775 GrappyLfjv-0.0.18/setup.cfg
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      606 2023-05-22 07:17:19.000000 GrappyLfjv-0.0.18/setup.py
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:17:23.170511 GrappyLfjv-0.0.18/src/
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:17:23.173375 GrappyLfjv-0.0.18/src/GrappyLfjv.egg-info/
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     3207 2023-05-22 07:17:23.000000 GrappyLfjv-0.0.18/src/GrappyLfjv.egg-info/PKG-INFO
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      229 2023-05-22 07:17:23.000000 GrappyLfjv-0.0.18/src/GrappyLfjv.egg-info/SOURCES.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)        1 2023-05-22 07:17:23.000000 GrappyLfjv-0.0.18/src/GrappyLfjv.egg-info/dependency_links.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)       15 2023-05-22 07:17:23.000000 GrappyLfjv-0.0.18/src/GrappyLfjv.egg-info/requires.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)        7 2023-05-22 07:17:23.000000 GrappyLfjv-0.0.18/src/GrappyLfjv.egg-info/top_level.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     4085 2023-05-22 06:03:40.000000 GrappyLfjv-0.0.18/src/grappy.py
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:23:57.307484 GrappyLfjv-0.0.19/
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     1060 2023-05-16 15:35:17.000000 GrappyLfjv-0.0.19/LICENSE
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     3213 2023-05-22 07:23:57.306961 GrappyLfjv-0.0.19/PKG-INFO
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     3036 2023-05-22 07:23:42.000000 GrappyLfjv-0.0.19/README.md
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)       38 2023-05-22 07:23:57.307658 GrappyLfjv-0.0.19/setup.cfg
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)      606 2023-05-22 07:23:54.000000 GrappyLfjv-0.0.19/setup.py
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:23:57.303272 GrappyLfjv-0.0.19/src/
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:23:57.306128 GrappyLfjv-0.0.19/src/GrappyLfjv.egg-info/
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     3213 2023-05-22 07:23:57.000000 GrappyLfjv-0.0.19/src/GrappyLfjv.egg-info/PKG-INFO
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)      229 2023-05-22 07:23:57.000000 GrappyLfjv-0.0.19/src/GrappyLfjv.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)        1 2023-05-22 07:23:57.000000 GrappyLfjv-0.0.19/src/GrappyLfjv.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)       15 2023-05-22 07:23:57.000000 GrappyLfjv-0.0.19/src/GrappyLfjv.egg-info/requires.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)        7 2023-05-22 07:23:57.000000 GrappyLfjv-0.0.19/src/GrappyLfjv.egg-info/top_level.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     4085 2023-05-22 06:03:40.000000 GrappyLfjv-0.0.19/src/grappy.py
```

### Comparing `GrappyLfjv-0.0.18/LICENSE` & `GrappyLfjv-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `GrappyLfjv-0.0.18/PKG-INFO` & `GrappyLfjv-0.0.19/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GrappyLfjv
-Version: 0.0.18
+Version: 0.0.19
 Summary: Simplification de la création de graphiques avec matplotlib
 Home-page: https://github.com/Benjamin-Trevian/Grappy
 Author: Benjamin Trévian
 Author-email: benjamin.trevian@hotmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -118,22 +118,22 @@
 
 Description: affiche le graphique construit à partier du fichier importé
 
 ```python
 graphe.fonction(fonction, xdebut, xfin, pas)
 ```
 
-fonction: string -> fonction à afficher sous écriture python
-xdebut: integer -> première valeur du x à afficher
-xfin: integer -> dernière valeur du x à afficher
-pas: int -> optionel, pas entre chaque x
+-fonction: string -> fonction à afficher sous écriture python
+-xdebut: integer -> première valeur du x à afficher
+-xfin: integer -> dernière valeur du x à afficher
+-pas: int -> optionel, pas entre chaque x
 
-renvoie: rien
+-renvoie: rien
 
-Description: créer un graphique à partir d'une fonction
+-Description: créer un graphique à partir d'une fonction
 
 ```python
 graphe.fonction().afficher()
 ```
 
 renvoie: rien
```

### Comparing `GrappyLfjv-0.0.18/README.md` & `GrappyLfjv-0.0.19/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -108,22 +108,22 @@
 
 Description: affiche le graphique construit à partier du fichier importé
 
 ```python
 graphe.fonction(fonction, xdebut, xfin, pas)
 ```
 
-fonction: string -> fonction à afficher sous écriture python
-xdebut: integer -> première valeur du x à afficher
-xfin: integer -> dernière valeur du x à afficher
-pas: int -> optionel, pas entre chaque x
+-fonction: string -> fonction à afficher sous écriture python
+-xdebut: integer -> première valeur du x à afficher
+-xfin: integer -> dernière valeur du x à afficher
+-pas: int -> optionel, pas entre chaque x
 
-renvoie: rien
+-renvoie: rien
 
-Description: créer un graphique à partir d'une fonction
+-Description: créer un graphique à partir d'une fonction
 
 ```python
 graphe.fonction().afficher()
 ```
 
 renvoie: rien
```

### Comparing `GrappyLfjv-0.0.18/setup.py` & `GrappyLfjv-0.0.19/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name= "GrappyLfjv",
-    version= "0.0.18",
+    version= "0.0.19",
     description= "Simplification de la création de graphiques avec matplotlib",
     long_description=read("README.md"),
     long_description_content_type='text/markdown',
     py_modules=["grappy"],
     package_dir={"": "src"},
     install_requires = [
         "matplotlib > 3.0"
```

### Comparing `GrappyLfjv-0.0.18/src/GrappyLfjv.egg-info/PKG-INFO` & `GrappyLfjv-0.0.19/src/GrappyLfjv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GrappyLfjv
-Version: 0.0.18
+Version: 0.0.19
 Summary: Simplification de la création de graphiques avec matplotlib
 Home-page: https://github.com/Benjamin-Trevian/Grappy
 Author: Benjamin Trévian
 Author-email: benjamin.trevian@hotmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -118,22 +118,22 @@
 
 Description: affiche le graphique construit à partier du fichier importé
 
 ```python
 graphe.fonction(fonction, xdebut, xfin, pas)
 ```
 
-fonction: string -> fonction à afficher sous écriture python
-xdebut: integer -> première valeur du x à afficher
-xfin: integer -> dernière valeur du x à afficher
-pas: int -> optionel, pas entre chaque x
+-fonction: string -> fonction à afficher sous écriture python
+-xdebut: integer -> première valeur du x à afficher
+-xfin: integer -> dernière valeur du x à afficher
+-pas: int -> optionel, pas entre chaque x
 
-renvoie: rien
+-renvoie: rien
 
-Description: créer un graphique à partir d'une fonction
+-Description: créer un graphique à partir d'une fonction
 
 ```python
 graphe.fonction().afficher()
 ```
 
 renvoie: rien
```

### Comparing `GrappyLfjv-0.0.18/src/grappy.py` & `GrappyLfjv-0.0.19/src/grappy.py`

 * *Files identical despite different names*

