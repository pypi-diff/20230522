# Comparing `tmp/GrappyLfjv-0.0.19.tar.gz` & `tmp/GrappyLfjv-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GrappyLfjv-0.0.19.tar", last modified: Mon May 22 07:23:57 2023, max compression
+gzip compressed data, was "GrappyLfjv-0.0.20.tar", last modified: Mon May 22 07:30:45 2023, max compression
```

## Comparing `GrappyLfjv-0.0.19.tar` & `GrappyLfjv-0.0.20.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:23:57.307484 GrappyLfjv-0.0.19/
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     1060 2023-05-16 15:35:17.000000 GrappyLfjv-0.0.19/LICENSE
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     3213 2023-05-22 07:23:57.306961 GrappyLfjv-0.0.19/PKG-INFO
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     3036 2023-05-22 07:23:42.000000 GrappyLfjv-0.0.19/README.md
--rw-r--r--   0 benjamintrevian   (501) staff       (20)       38 2023-05-22 07:23:57.307658 GrappyLfjv-0.0.19/setup.cfg
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      606 2023-05-22 07:23:54.000000 GrappyLfjv-0.0.19/setup.py
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:23:57.303272 GrappyLfjv-0.0.19/src/
-drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:23:57.306128 GrappyLfjv-0.0.19/src/GrappyLfjv.egg-info/
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     3213 2023-05-22 07:23:57.000000 GrappyLfjv-0.0.19/src/GrappyLfjv.egg-info/PKG-INFO
--rw-r--r--   0 benjamintrevian   (501) staff       (20)      229 2023-05-22 07:23:57.000000 GrappyLfjv-0.0.19/src/GrappyLfjv.egg-info/SOURCES.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)        1 2023-05-22 07:23:57.000000 GrappyLfjv-0.0.19/src/GrappyLfjv.egg-info/dependency_links.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)       15 2023-05-22 07:23:57.000000 GrappyLfjv-0.0.19/src/GrappyLfjv.egg-info/requires.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)        7 2023-05-22 07:23:57.000000 GrappyLfjv-0.0.19/src/GrappyLfjv.egg-info/top_level.txt
--rw-r--r--   0 benjamintrevian   (501) staff       (20)     4085 2023-05-22 06:03:40.000000 GrappyLfjv-0.0.19/src/grappy.py
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:30:45.732955 GrappyLfjv-0.0.20/
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     1060 2023-05-16 15:35:17.000000 GrappyLfjv-0.0.20/LICENSE
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     3396 2023-05-22 07:30:45.732541 GrappyLfjv-0.0.20/PKG-INFO
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     3244 2023-05-22 07:30:28.000000 GrappyLfjv-0.0.20/README.md
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)       38 2023-05-22 07:30:45.733170 GrappyLfjv-0.0.20/setup.cfg
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)      606 2023-05-22 07:30:42.000000 GrappyLfjv-0.0.20/setup.py
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:30:45.729228 GrappyLfjv-0.0.20/src/
+drwxr-xr-x   0 benjamintrevian   (501) staff       (20)        0 2023-05-22 07:30:45.731920 GrappyLfjv-0.0.20/src/GrappyLfjv.egg-info/
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     3396 2023-05-22 07:30:45.000000 GrappyLfjv-0.0.20/src/GrappyLfjv.egg-info/PKG-INFO
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)      229 2023-05-22 07:30:45.000000 GrappyLfjv-0.0.20/src/GrappyLfjv.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)        1 2023-05-22 07:30:45.000000 GrappyLfjv-0.0.20/src/GrappyLfjv.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)       15 2023-05-22 07:30:45.000000 GrappyLfjv-0.0.20/src/GrappyLfjv.egg-info/requires.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)        7 2023-05-22 07:30:45.000000 GrappyLfjv-0.0.20/src/GrappyLfjv.egg-info/top_level.txt
+-rw-r--r--   0 benjamintrevian   (501) staff       (20)     4085 2023-05-22 06:03:40.000000 GrappyLfjv-0.0.20/src/grappy.py
```

### Comparing `GrappyLfjv-0.0.19/LICENSE` & `GrappyLfjv-0.0.20/LICENSE`

 * *Files identical despite different names*

### Comparing `GrappyLfjv-0.0.19/PKG-INFO` & `GrappyLfjv-0.0.20/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GrappyLfjv
-Version: 0.0.19
+Version: 0.0.20
 Summary: Simplification de la création de graphiques avec matplotlib
 Home-page: https://github.com/Benjamin-Trevian/Grappy
 Author: Benjamin Trévian
 Author-email: benjamin.trevian@hotmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -60,85 +60,110 @@
 
 ## Documentation
 
 ```python
 graphe(titre, labelx, labely)
 ```
 
+-Paramètres:
+
 titre: string -> titre du graphique
+
 labelx: string -> titre du label sur l'axe x
+
 labely: string -> titre du label sur l'axe y
 
 renvoie: rien
 
-Description: Créer la base du graphe, titre, titre labelx, titre labely
+-Description: Créer la base du graphe, titre, titre labelx, titre labely
 
 ```python
 graphe.points(liste_points)
 ```
 
+-Paramètres:
+
 liste_points: liste -> liste de points sous forme de tuples pour construire le graphique
 
 renvoie: rien
 
-Description: ajoute les points dans liste_points dans le graphique
+-Description: ajoute les points dans liste_points dans le graphique
 
 ```python
 graphe.points().exporter(nom)
 ```
 
+-Paramètres:
+
 nom: string -> nom du nouveau fichier csv qui sera crée
 
 renvoie: rien
 
-Description: Créer un fichier csv avec comme contenu la liste de points entrées dans graphe.points()
+-Description: Créer un fichier csv avec comme contenu la liste de points entrées dans graphe.points()
 
 ```python
 graphe.points().afficher()
 ```
 
+-Paramètres:
+
 renvoie: rien
 
-Description: affiche le graphique à partir des points entrées dans graphe.points()
+-Description: affiche le graphique à partir des points entrées dans graphe.points()
 
 ```python
 graphe.importer(nom_fichier, configuration, logiciel)
 ```
 
+-Paramètres:
+
 nom_fichier: string -> Nom du fichier à importer
+
 configuration: string -> "v" si le tableau importé est verticale, "h" si le tableau importé est horizontale
+
 logiciel: string -> optionel, permet de définir le logiciel ayant exporté le csv (pour le delimiteur)
 
 renvoie: rien
 
+-Decription: importe un graphique depuis un fichier csv
+
 ```python
 graphe.importer().afficher()
 ```
 
+-Paramètres:
+
 renvoie: rien
 
-Description: affiche le graphique construit à partier du fichier importé
+-Description: affiche le graphique construit à partier du fichier importé
 
 ```python
 graphe.fonction(fonction, xdebut, xfin, pas)
 ```
 
--fonction: string -> fonction à afficher sous écriture python
--xdebut: integer -> première valeur du x à afficher
--xfin: integer -> dernière valeur du x à afficher
--pas: int -> optionel, pas entre chaque x
+-Paramètres:
+
+fonction: string -> fonction à afficher sous écriture python
+
+xdebut: integer -> première valeur du x à afficher
 
--renvoie: rien
+xfin: integer -> dernière valeur du x à afficher
 
--Description: créer un graphique à partir d'une fonction
+pas: int -> optionel, pas entre chaque x
+
+renvoie: rien
+
+-Description: Créer un graphique à partir d'une fonction
 
 ```python
 graphe.fonction().afficher()
 ```
 
+Paramètres:
+
 renvoie: rien
 
 Description: affiche le graphique à partir de la fonction entrée précédemment
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `GrappyLfjv-0.0.19/README.md` & `GrappyLfjv-0.0.20/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -50,85 +50,110 @@
 
 ## Documentation
 
 ```python
 graphe(titre, labelx, labely)
 ```
 
+-Paramètres:
+
 titre: string -> titre du graphique
+
 labelx: string -> titre du label sur l'axe x
+
 labely: string -> titre du label sur l'axe y
 
 renvoie: rien
 
-Description: Créer la base du graphe, titre, titre labelx, titre labely
+-Description: Créer la base du graphe, titre, titre labelx, titre labely
 
 ```python
 graphe.points(liste_points)
 ```
 
+-Paramètres:
+
 liste_points: liste -> liste de points sous forme de tuples pour construire le graphique
 
 renvoie: rien
 
-Description: ajoute les points dans liste_points dans le graphique
+-Description: ajoute les points dans liste_points dans le graphique
 
 ```python
 graphe.points().exporter(nom)
 ```
 
+-Paramètres:
+
 nom: string -> nom du nouveau fichier csv qui sera crée
 
 renvoie: rien
 
-Description: Créer un fichier csv avec comme contenu la liste de points entrées dans graphe.points()
+-Description: Créer un fichier csv avec comme contenu la liste de points entrées dans graphe.points()
 
 ```python
 graphe.points().afficher()
 ```
 
+-Paramètres:
+
 renvoie: rien
 
-Description: affiche le graphique à partir des points entrées dans graphe.points()
+-Description: affiche le graphique à partir des points entrées dans graphe.points()
 
 ```python
 graphe.importer(nom_fichier, configuration, logiciel)
 ```
 
+-Paramètres:
+
 nom_fichier: string -> Nom du fichier à importer
+
 configuration: string -> "v" si le tableau importé est verticale, "h" si le tableau importé est horizontale
+
 logiciel: string -> optionel, permet de définir le logiciel ayant exporté le csv (pour le delimiteur)
 
 renvoie: rien
 
+-Decription: importe un graphique depuis un fichier csv
+
 ```python
 graphe.importer().afficher()
 ```
 
+-Paramètres:
+
 renvoie: rien
 
-Description: affiche le graphique construit à partier du fichier importé
+-Description: affiche le graphique construit à partier du fichier importé
 
 ```python
 graphe.fonction(fonction, xdebut, xfin, pas)
 ```
 
--fonction: string -> fonction à afficher sous écriture python
--xdebut: integer -> première valeur du x à afficher
--xfin: integer -> dernière valeur du x à afficher
--pas: int -> optionel, pas entre chaque x
+-Paramètres:
+
+fonction: string -> fonction à afficher sous écriture python
+
+xdebut: integer -> première valeur du x à afficher
 
--renvoie: rien
+xfin: integer -> dernière valeur du x à afficher
 
--Description: créer un graphique à partir d'une fonction
+pas: int -> optionel, pas entre chaque x
+
+renvoie: rien
+
+-Description: Créer un graphique à partir d'une fonction
 
 ```python
 graphe.fonction().afficher()
 ```
 
+Paramètres:
+
 renvoie: rien
 
 Description: affiche le graphique à partir de la fonction entrée précédemment
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `GrappyLfjv-0.0.19/setup.py` & `GrappyLfjv-0.0.20/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name= "GrappyLfjv",
-    version= "0.0.19",
+    version= "0.0.20",
     description= "Simplification de la création de graphiques avec matplotlib",
     long_description=read("README.md"),
     long_description_content_type='text/markdown',
     py_modules=["grappy"],
     package_dir={"": "src"},
     install_requires = [
         "matplotlib > 3.0"
```

### Comparing `GrappyLfjv-0.0.19/src/GrappyLfjv.egg-info/PKG-INFO` & `GrappyLfjv-0.0.20/src/GrappyLfjv.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GrappyLfjv
-Version: 0.0.19
+Version: 0.0.20
 Summary: Simplification de la création de graphiques avec matplotlib
 Home-page: https://github.com/Benjamin-Trevian/Grappy
 Author: Benjamin Trévian
 Author-email: benjamin.trevian@hotmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -60,85 +60,110 @@
 
 ## Documentation
 
 ```python
 graphe(titre, labelx, labely)
 ```
 
+-Paramètres:
+
 titre: string -> titre du graphique
+
 labelx: string -> titre du label sur l'axe x
+
 labely: string -> titre du label sur l'axe y
 
 renvoie: rien
 
-Description: Créer la base du graphe, titre, titre labelx, titre labely
+-Description: Créer la base du graphe, titre, titre labelx, titre labely
 
 ```python
 graphe.points(liste_points)
 ```
 
+-Paramètres:
+
 liste_points: liste -> liste de points sous forme de tuples pour construire le graphique
 
 renvoie: rien
 
-Description: ajoute les points dans liste_points dans le graphique
+-Description: ajoute les points dans liste_points dans le graphique
 
 ```python
 graphe.points().exporter(nom)
 ```
 
+-Paramètres:
+
 nom: string -> nom du nouveau fichier csv qui sera crée
 
 renvoie: rien
 
-Description: Créer un fichier csv avec comme contenu la liste de points entrées dans graphe.points()
+-Description: Créer un fichier csv avec comme contenu la liste de points entrées dans graphe.points()
 
 ```python
 graphe.points().afficher()
 ```
 
+-Paramètres:
+
 renvoie: rien
 
-Description: affiche le graphique à partir des points entrées dans graphe.points()
+-Description: affiche le graphique à partir des points entrées dans graphe.points()
 
 ```python
 graphe.importer(nom_fichier, configuration, logiciel)
 ```
 
+-Paramètres:
+
 nom_fichier: string -> Nom du fichier à importer
+
 configuration: string -> "v" si le tableau importé est verticale, "h" si le tableau importé est horizontale
+
 logiciel: string -> optionel, permet de définir le logiciel ayant exporté le csv (pour le delimiteur)
 
 renvoie: rien
 
+-Decription: importe un graphique depuis un fichier csv
+
 ```python
 graphe.importer().afficher()
 ```
 
+-Paramètres:
+
 renvoie: rien
 
-Description: affiche le graphique construit à partier du fichier importé
+-Description: affiche le graphique construit à partier du fichier importé
 
 ```python
 graphe.fonction(fonction, xdebut, xfin, pas)
 ```
 
--fonction: string -> fonction à afficher sous écriture python
--xdebut: integer -> première valeur du x à afficher
--xfin: integer -> dernière valeur du x à afficher
--pas: int -> optionel, pas entre chaque x
+-Paramètres:
+
+fonction: string -> fonction à afficher sous écriture python
+
+xdebut: integer -> première valeur du x à afficher
 
--renvoie: rien
+xfin: integer -> dernière valeur du x à afficher
 
--Description: créer un graphique à partir d'une fonction
+pas: int -> optionel, pas entre chaque x
+
+renvoie: rien
+
+-Description: Créer un graphique à partir d'une fonction
 
 ```python
 graphe.fonction().afficher()
 ```
 
+Paramètres:
+
 renvoie: rien
 
 Description: affiche le graphique à partir de la fonction entrée précédemment
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `GrappyLfjv-0.0.19/src/grappy.py` & `GrappyLfjv-0.0.20/src/grappy.py`

 * *Files identical despite different names*

