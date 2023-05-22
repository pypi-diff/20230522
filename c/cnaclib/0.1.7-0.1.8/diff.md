# Comparing `tmp/cnaclib-0.1.7.tar.gz` & `tmp/cnaclib-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnaclib-0.1.7.tar", last modified: Mon May 22 10:34:41 2023, max compression
+gzip compressed data, was "cnaclib-0.1.8.tar", last modified: Mon May 22 10:39:41 2023, max compression
```

## Comparing `cnaclib-0.1.7.tar` & `cnaclib-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 10:34:41.246626 cnaclib-0.1.7/
--rw-rw-rw-   0        0        0     1073 2023-05-10 09:44:18.000000 cnaclib-0.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0     2849 2023-05-22 10:34:41.246626 cnaclib-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1863 2023-05-21 07:31:25.000000 cnaclib-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 10:34:41.239625 cnaclib-0.1.7/cnaclib/
--rw-rw-rw-   0        0        0       17 2023-05-18 14:22:52.000000 cnaclib-0.1.7/cnaclib/__init__.py
--rw-rw-rw-   0        0        0     7923 2023-05-21 09:08:48.000000 cnaclib-0.1.7/cnaclib/lSix.py
--rw-rw-rw-   0        0        0    21717 2023-05-18 09:49:05.000000 cnaclib-0.1.7/cnaclib/rac.py
--rw-rw-rw-   0        0        0    21757 2023-05-11 15:43:48.000000 cnaclib-0.1.7/cnaclib/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:34:41.244626 cnaclib-0.1.7/cnaclib.egg-info/
--rw-rw-rw-   0        0        0     2849 2023-05-22 10:34:41.000000 cnaclib-0.1.7/cnaclib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-22 10:34:41.000000 cnaclib-0.1.7/cnaclib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 10:34:41.000000 cnaclib-0.1.7/cnaclib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2023-05-22 10:34:41.000000 cnaclib-0.1.7/cnaclib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-22 10:34:41.000000 cnaclib-0.1.7/cnaclib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 10:34:41.246626 cnaclib-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1253 2023-05-22 10:34:31.000000 cnaclib-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:39:41.170616 cnaclib-0.1.8/
+-rw-rw-rw-   0        0        0     1073 2023-05-10 09:44:18.000000 cnaclib-0.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     2784 2023-05-22 10:39:41.161615 cnaclib-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1846 2023-05-22 10:39:12.000000 cnaclib-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 10:39:41.112610 cnaclib-0.1.8/cnaclib/
+-rw-rw-rw-   0        0        0       17 2023-05-18 14:22:52.000000 cnaclib-0.1.8/cnaclib/__init__.py
+-rw-rw-rw-   0        0        0     7923 2023-05-21 09:08:48.000000 cnaclib-0.1.8/cnaclib/lSix.py
+-rw-rw-rw-   0        0        0    21717 2023-05-18 09:49:05.000000 cnaclib-0.1.8/cnaclib/rac.py
+-rw-rw-rw-   0        0        0    21757 2023-05-11 15:43:48.000000 cnaclib-0.1.8/cnaclib/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-22 10:39:41.142613 cnaclib-0.1.8/cnaclib.egg-info/
+-rw-rw-rw-   0        0        0     2784 2023-05-22 10:39:40.000000 cnaclib-0.1.8/cnaclib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-05-22 10:39:41.000000 cnaclib-0.1.8/cnaclib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 10:39:40.000000 cnaclib-0.1.8/cnaclib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2023-05-22 10:39:40.000000 cnaclib-0.1.8/cnaclib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-22 10:39:40.000000 cnaclib-0.1.8/cnaclib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 10:39:41.172616 cnaclib-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1253 2023-05-22 10:39:31.000000 cnaclib-0.1.8/setup.py
```

### Comparing `cnaclib-0.1.7/LICENSE.txt` & `cnaclib-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.7/PKG-INFO` & `cnaclib-0.1.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: cnaclib
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simulateur RAC
 Home-page: UNKNOWN
 Author: BENHAMADA Nadir
 Author-email: aistatendz@gmail.com
 License: UNKNOWN
-Description: # cnaclib : Librairie Python dأ©veloppأ©e pour les usagers et les employأ©s de la CNAC. 
+Description: # cnaclib : Librairie Python developpee pour les usagers et les employes de la CNAC. 
         
         ## About cnaclib
         
-        **cnaclib** Câ€™est un package `Python` dأ©diأ© aux usagers et aux employأ©s de la CNAC.
+        **cnaclib** Câ€™est un package `Python` dedie aux usagers et aux employes de la CNAC.
         
         ## Pourquoi utiliser cnaclib?
         
         * Il dispose de plusieurs modules et fonctions `Python` pour : 
-            * Faire une simulation de calculs pour le bأ©nأ©fice du rأ©gime dâ€™assurance chأ´mage (RAC)
-            * Faire une simulation de calculs pour le bأ©nأ©fice des mesures dâ€™encouragement أ  lâ€™emploi (loi 06-21)
-            * Gأ©nأ©rer la liste des codes de wilaya de 01 أ  58
-            * Avoir le nom de la wilaya en arabe ou en franأ§ais en fonction de son code 
-            * Avoir le code de la wilaya en fonction de son nom en arabe ou en franأ§ais
-            * Gأ©nأ©rer des dossiers qui postent le nom des wilayas en arabe ou en franأ§ais
-            * Avoir le montant du SNMG en fonction de la date أ  compter du 01/01/1990
+            * Faire une simulation de calculs pour le benefice du rأ©gime dâ€™assurance chomage (RAC);
+            * Faire une simulation de calculs pour le benefice des mesures dâ€™encouragement أ  lâ€™emploi (loi 06-21);
+            * Generer la liste des codes de wilaya de 01 a 58;
+            * Avoir le nom de la wilaya en arabe ou en francais en fonction de son code ;
+            * Avoir le code de la wilaya en fonction de son nom en arabe ou en francais;
+            * Generer des dossiers qui postent le nom des wilayas en arabe ou en francais;
+            * Avoir le montant du SNMG en fonction de la date a compter du 01/01/1990;
         
-        * Il sera mis أ  jour rأ©guliأ¨rement par des modules qui peuvent automatiser certaines tأ¢ches.
+        * Il sera mis a jour regulierement par des modules qui peuvent automatiser certaines taches.
         
         
         ## Installation
         
         ### Dependencies
         
         cnaclib requires
```

### Comparing `cnaclib-0.1.7/README.md` & `cnaclib-0.1.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# cnaclib : Librairie Python développée pour les usagers et les employés de la CNAC. 
+# cnaclib : Librairie Python developpee pour les usagers et les employes de la CNAC. 
 
 ## About cnaclib
 
-**cnaclib** C’est un package `Python` dédié aux usagers et aux employés de la CNAC.
+**cnaclib** C’est un package `Python` dedie aux usagers et aux employes de la CNAC.
 
 ## Pourquoi utiliser cnaclib?
 
 * Il dispose de plusieurs modules et fonctions `Python` pour : 
-    * Faire une simulation de calculs pour le bénéfice du régime d’assurance chômage (RAC)
-    * Faire une simulation de calculs pour le bénéfice des mesures d’encouragement à l’emploi (loi 06-21)
-    * Générer la liste des codes de wilaya de 01 à 58
-    * Avoir le nom de la wilaya en arabe ou en français en fonction de son code 
-    * Avoir le code de la wilaya en fonction de son nom en arabe ou en français
-    * Générer des dossiers qui postent le nom des wilayas en arabe ou en français
-    * Avoir le montant du SNMG en fonction de la date à compter du 01/01/1990
+    * Faire une simulation de calculs pour le benefice du régime d’assurance chomage (RAC);
+    * Faire une simulation de calculs pour le benefice des mesures d’encouragement à l’emploi (loi 06-21);
+    * Generer la liste des codes de wilaya de 01 a 58;
+    * Avoir le nom de la wilaya en arabe ou en francais en fonction de son code ;
+    * Avoir le code de la wilaya en fonction de son nom en arabe ou en francais;
+    * Generer des dossiers qui postent le nom des wilayas en arabe ou en francais;
+    * Avoir le montant du SNMG en fonction de la date a compter du 01/01/1990;
 
-* Il sera mis à jour régulièrement par des modules qui peuvent automatiser certaines tâches.
+* Il sera mis a jour regulierement par des modules qui peuvent automatiser certaines taches.
 
 
 ## Installation
 
 ### Dependencies
 
 cnaclib requires
```

### Comparing `cnaclib-0.1.7/cnaclib/lSix.py` & `cnaclib-0.1.8/cnaclib/lSix.py`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.7/cnaclib/rac.py` & `cnaclib-0.1.8/cnaclib/rac.py`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.7/cnaclib/tools.py` & `cnaclib-0.1.8/cnaclib/tools.py`

 * *Files identical despite different names*

### Comparing `cnaclib-0.1.7/cnaclib.egg-info/PKG-INFO` & `cnaclib-0.1.8/cnaclib.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: cnaclib
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simulateur RAC
 Home-page: UNKNOWN
 Author: BENHAMADA Nadir
 Author-email: aistatendz@gmail.com
 License: UNKNOWN
-Description: # cnaclib : Librairie Python dأ©veloppأ©e pour les usagers et les employأ©s de la CNAC. 
+Description: # cnaclib : Librairie Python developpee pour les usagers et les employes de la CNAC. 
         
         ## About cnaclib
         
-        **cnaclib** Câ€™est un package `Python` dأ©diأ© aux usagers et aux employأ©s de la CNAC.
+        **cnaclib** Câ€™est un package `Python` dedie aux usagers et aux employes de la CNAC.
         
         ## Pourquoi utiliser cnaclib?
         
         * Il dispose de plusieurs modules et fonctions `Python` pour : 
-            * Faire une simulation de calculs pour le bأ©nأ©fice du rأ©gime dâ€™assurance chأ´mage (RAC)
-            * Faire une simulation de calculs pour le bأ©nأ©fice des mesures dâ€™encouragement أ  lâ€™emploi (loi 06-21)
-            * Gأ©nأ©rer la liste des codes de wilaya de 01 أ  58
-            * Avoir le nom de la wilaya en arabe ou en franأ§ais en fonction de son code 
-            * Avoir le code de la wilaya en fonction de son nom en arabe ou en franأ§ais
-            * Gأ©nأ©rer des dossiers qui postent le nom des wilayas en arabe ou en franأ§ais
-            * Avoir le montant du SNMG en fonction de la date أ  compter du 01/01/1990
+            * Faire une simulation de calculs pour le benefice du rأ©gime dâ€™assurance chomage (RAC);
+            * Faire une simulation de calculs pour le benefice des mesures dâ€™encouragement أ  lâ€™emploi (loi 06-21);
+            * Generer la liste des codes de wilaya de 01 a 58;
+            * Avoir le nom de la wilaya en arabe ou en francais en fonction de son code ;
+            * Avoir le code de la wilaya en fonction de son nom en arabe ou en francais;
+            * Generer des dossiers qui postent le nom des wilayas en arabe ou en francais;
+            * Avoir le montant du SNMG en fonction de la date a compter du 01/01/1990;
         
-        * Il sera mis أ  jour rأ©guliأ¨rement par des modules qui peuvent automatiser certaines tأ¢ches.
+        * Il sera mis a jour regulierement par des modules qui peuvent automatiser certaines taches.
         
         
         ## Installation
         
         ### Dependencies
         
         cnaclib requires
```

### Comparing `cnaclib-0.1.7/setup.py` & `cnaclib-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 chemin = Path(__file__).parent
 long_description = (chemin / "README.md").read_text()
 
 
 setuptools.setup(
     name = 'cnaclib',
-    version = '0.1.7',
+    version = '0.1.8',
     author= 'BENHAMADA Nadir',
     author_email='aistatendz@gmail.com',
     description='Simulateur RAC',
     packages=setuptools.find_packages(),
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=["certifi>=2023.5.7",
```

