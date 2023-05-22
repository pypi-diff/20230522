# Comparing `tmp/kinepy-0.1.0.tar.gz` & `tmp/kinepy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kinepy-0.1.0.tar", last modified: Wed May 17 07:04:49 2023, max compression
+gzip compressed data, was "kinepy-0.1.1.tar", last modified: Mon May 22 13:07:04 2023, max compression
```

## Comparing `kinepy-0.1.0.tar` & `kinepy-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:04:49.732165 kinepy-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-17 07:04:34.000000 kinepy-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-17 07:04:49.732165 kinepy-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-17 07:04:34.000000 kinepy-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:04:49.732165 kinepy-0.1.0/kinepy/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 07:04:34.000000 kinepy-0.1.0/kinepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-05-17 07:04:34.000000 kinepy-0.1.0/kinepy/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-17 07:04:34.000000 kinepy-0.1.0/kinepy/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:04:49.732165 kinepy-0.1.0/kinepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-17 07:04:49.000000 kinepy-0.1.0/kinepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-17 07:04:49.000000 kinepy-0.1.0/kinepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:04:49.000000 kinepy-0.1.0/kinepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 07:04:49.000000 kinepy-0.1.0/kinepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-17 07:04:49.732165 kinepy-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-17 07:04:34.000000 kinepy-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:07:04.864031 kinepy-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-22 13:06:47.000000 kinepy-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-22 13:07:04.864031 kinepy-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-05-22 13:06:47.000000 kinepy-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:07:04.864031 kinepy-0.1.1/kinepy/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:07:04.864031 kinepy-0.1.1/kinepy/compilation/
+-rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/compilation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/compilation/graph_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/compilation/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/compilation/preparation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:07:04.864031 kinepy-0.1.1/kinepy/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/gui/Rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/gui/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4748 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/gui/drawing_tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/gui/getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/gui/grid_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/gui/gui_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7544 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/gui/system_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:07:04.864031 kinepy-0.1.1/kinepy/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/interface/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/interface/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/interface/joints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/interface/metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/interface/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/interface/solid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/interface/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:07:04.864031 kinepy-0.1.1/kinepy/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/math/calculus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/math/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/math/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/math/kinematic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:07:04.864031 kinepy-0.1.1/kinepy/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/objects/interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9827 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/objects/joints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/objects/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/objects/solid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/objects/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12520 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-22 13:06:47.000000 kinepy-0.1.1/kinepy/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:07:04.864031 kinepy-0.1.1/kinepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-22 13:07:04.000000 kinepy-0.1.1/kinepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-22 13:07:04.000000 kinepy-0.1.1/kinepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:07:04.000000 kinepy-0.1.1/kinepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 13:07:04.000000 kinepy-0.1.1/kinepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-22 13:07:04.868031 kinepy-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-22 13:06:47.000000 kinepy-0.1.1/setup.py
```

### Comparing `kinepy-0.1.0/LICENSE` & `kinepy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.0/README.md` & `kinepy-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,60 @@
 <p align="center" width="100%">
     <img width="70%" src="https://user-images.githubusercontent.com/93446869/234020322-1ef75f2b-1900-4b86-a83c-96becd308c8c.svg">
 </p>
 
 <p align="center" width="100%">
-    <img width="70%" src="https://github.com/valentin-burillier/kinepy/assets/93446869/a7faddd1-3816-4345-8965-eea9d503379c">
+    <img width="80%" src="https://github.com/valentin-burillier/kinepy/assets/93446869/a7faddd1-3816-4345-8965-eea9d503379c">
 </p>
 
 [![PyPI Downloads](https://img.shields.io/pypi/dm/kinepy.svg?label=PyPI%20downloads)](https://pypi.org/project/kinepy/)
 
-KinePy est une librairie python dédiée à la simulation de mécanisme plan.
+**KinePy est une librairie python dédiée à la simulation cinématique, dynamique et statique de mécanisme plan.** Elle est utilisée pour :
 
-- KinePy permet de simuler rapidement et précisément un mécanisme complexe constituer de plusieurs boucles cinématiques. Il est facile d'évaluer les performances d'un mécanisme que ce soit du point de vue de la position, de la vitesse des différents solides ou encore des efforts que subissent les pièces au niveau des liaisons. Cet outil est donc destiné pour réaliser le premier dimensionnement d'un mécanisme.
+- `Evaluation de performences` : KinePy permet de simuler rapidement et précisément un mécanisme complexe constituer de plusieurs boucles cinématiques. Il est facile d'évaluer les performances d'un mécanisme que ce soit du point de vue de la position, de la vitesse des différents solides ou encore des efforts que subissent les pièces au niveau des liaisons.
+- `Dimensionnement de composants` : En récupérant les informations de vitesse ou d'effort de certaines liaisons, il est possible de connaître les composants adéquates à utiliser. Par exemple, c'est utile dans le choix d'un moteur, d'un ressort, de roulements à bille, de paliers lisses...
+- `Optimisation de mécanisme` : KinePy offre la possibilité de modifier les dimensions d'un solide sans recréer un nouveau système. Ainsi, un tel modèle peut être couplé à des algorithme d'optimisation afin de définir un mécanisme répondant à vos attentes. Il existe de nombreux algorithmes d'otimisation fournient par d'autres bibliothèques : [scikit-learn](https://scikit-learn.org/stable/), [scipy](https://scipy.org/)...
+- `Cinématique inverse` : KinePy permet de réaliser la cinématique inverse d'un mécanisme. En ajoutant des liaisons pilotés ne faisant pas partie du mécanisme, on peut trouver le pilotage d'actionneurs. 
 
-- KinePy a été conçu pour pouvoir être utilisé avec des algorithme d'optimisation. En effet, après la création d'un mécanisme, l'utilisateur à la possibilité de modifier les dimensions d'un solide sans recréer un nouveau système. Cela fournit un modèle paramètrable où il est possible de créer une fonction coût. Cette dernière pourra être minimiser avec des algorithme d'optimisation fournit par d'autres bibliothèques : [scikit-learn](https://scikit-learn.org/stable/), [scipy](https://scipy.org/)...
+# Documentation et pré-requis
 
-- De plus, KinePy permet de réaliser la cinématique inverse d'un mécanisme. En ajoutant des liaisons pilotés ne faisant pas partie du mécanisme, on peut trouver le pilotage d'actionneurs.  
+Nous vous invitons à aller voir le fichier [tutoriel](https://github.com/valentin-burillier/kinepy/blob/main/docs/utiliser_kinepy.md) montrant dans le détail comment simuler un mécanisme. Ce fichier renvoit sur la documentation des éléments utiliser.
 
-# Pré-requis
+La documentation compléte est accessible [ici](https://github.com/valentin-burillier/kinepy/blob/main/docs).
 
-Des connaissances en science de l'ingénieur sont nécessaire pour utiliser KinePy notament dans les domaines de la modélisation, la cinématique et la dynamique. La documentation de KinePy seul ne permet pas de comprendre ces domaines.
+*N.B. Des connaissances en science de l'ingénieur sont nécessaire pour utiliser KinePy notament dans les domaines de la modélisation, la cinématique et la dynamique. La documentation de KinePy seul ne permet pas de comprendre ces domaines.*
 
-# Documentation
+# Exemples
 
-Nous vous invitons à aller voir ce [fichier](https://github.com/valentin-burillier/kinepy/blob/main/docs/utiliser_kinepy.md) montrant comment simuler un mécanisme. Il renvoit sur la documentation des éléments utiliser.
+Vous pourrez trouver [ici](https://github.com/valentin-burillier/kinepy/tree/main/examples) des exemples d'application de KinePy sur des systèmes réels :
 
-La documentation des éléments permettant de créer un mécanisme est [ici](https://github.com/valentin-burillier/kinepy/blob/main/docs/System.md).
+- Cinématique du bras d'une [pelleteuse](https://github.com/valentin-burillier/kinepy/blob/main/examples/pelleteuse.py) :
+<p align="center" width="100%">
+    <img width="70%" src="https://github.com/valentin-burillier/kinepy/assets/93446869/86fb79ad-6ebd-40fd-b010-c2c279667e6f">
+</p>
 
-# Exemples
+- Cinématique inverse d'une [machine à tracer](https://github.com/valentin-burillier/kinepy/blob/main/examples/plotter_machine.py) :
+<p align="center" width="100%">
+    <img width="70%" src="https://github.com/valentin-burillier/kinepy/assets/93446869/9ba76909-b850-41ba-b97f-ce6decb20e2b">
+</p>
 
-Vous pourrez trouver [ici](https://github.com/valentin-burillier/kinepy/tree/main/examples) des exemples d'application de KinePy sur des systèmes réels.
+- Dynamique d'un [moteur](https://github.com/valentin-burillier/kinepy/blob/main/examples/engine.py) :
+<p align="center" width="100%">
+    <img width="70%" src="https://github.com/valentin-burillier/kinepy/assets/93446869/0959f164-5b58-4f4d-b8b0-86433319ea70">
+</p>
 
-- Simulation cinématique du bras d'une pelleteuse :
+- Quasi-statique d'un [camion benne](https://github.com/valentin-burillier/kinepy/blob/main/examples/Camion%20benne.py) :
 <p align="center" width="100%">
-    <img width="70%" src="https://github.com/valentin-burillier/kinepy/assets/93446869/86fb79ad-6ebd-40fd-b010-c2c279667e6f">
+    <img width="70%" src="https://github.com/valentin-burillier/kinepy/assets/93446869/4506a1f9-8d50-4b30-a14c-5c1d1b6a2323">
 </p>
 
 # Hypothèses
 
-La bibliothèque suit un certain nombre d'hypothèses. Il est nécessaire que le mécanisme que vous voulez simuler les respecte :
+La bibliothèque suit un certains nombre d'hypothèses. Il est nécessaire que le mécanisme que vous voulez simuler les respecte :
+
 - Le mécanisme est plan
 - Le système est isostatique, le schéma cinématique doit être minimal
 - Les solides sont indéformables
 - Les liaisons sont parfaites
 - La masse des solides est constante
 - Le référentiel global associé au bâti est galiléen
 - Le système est soumis un champ de forces uniformes
@@ -55,17 +68,17 @@
 pip install kinepy
 ```
 
 *Notez que la version télécharger avec pip peut être bien antérieur au dépot le plus récent. Des fonctionnalités peuvent manquer.*
 
 # Disclaimer
 
-La bibliothèque est en développement. Il peut donc y avoir des bugs. Merci de les faire remonter aux développeurs afin de les corriger. Actuellement, l'interface graphique est en train d'être codé. La représentation de schéma cinématique animé n'étant pas une tâche triviale, veuillez signaler si vous rencontrez des problèmes.
+La bibliothèque est en développement. Il peut donc y avoir des bugs. Merci de les faire remonter aux développeurs afin de les corriger. Actuellement, l'interface graphique permettant de réaliser les schémas cinématiques animés est en train d'être codé. Veuillez signaler si vous rencontrez des problèmes.
 
 De plus, les dévelopeurs seront très attentifs aux demandes d'intégration de nouvelles fonctionnalités.
 
-Nous vous encourageons également à partager aux développeurs les applications que vous faites de KinePy.
+Nous vous encourageons également à partager les applications que vous faites de KinePy.
 
 # Liens
 
 - https://cdfg.mit.edu/assets/files/CDMC_0.pdf, https://n.ethz.ch/~bthomasz/assets/PDF/Megaro17Compliant.pdf - Ce qui a inspiré ce répertoire
 - http://faculty.tamucc.edu/psimionescu/PDFs/ASME%20DETC%202016%20-%2059086.pdf, https://blog.rectorsquid.com/linkage-mechanism-designer-and-simulator/ - Simulateurs cinématiques existants
```

### Comparing `kinepy-0.1.0/kinepy/tools.py` & `kinepy-0.1.1/kinepy/tools.py`

 * *Files identical despite different names*

### Comparing `kinepy-0.1.0/kinepy/units.py` & `kinepy-0.1.1/kinepy/units.py`

 * *Files identical despite different names*

