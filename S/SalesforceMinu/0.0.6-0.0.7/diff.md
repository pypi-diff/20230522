# Comparing `tmp/SalesforceMinu-0.0.6.tar.gz` & `tmp/SalesforceMinu-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SalesforceMinu-0.0.6.tar", last modified: Wed May 10 18:50:57 2023, max compression
+gzip compressed data, was "SalesforceMinu-0.0.7.tar", last modified: Mon May 22 17:33:00 2023, max compression
```

## Comparing `SalesforceMinu-0.0.6.tar` & `SalesforceMinu-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 18:50:57.155804 SalesforceMinu-0.0.6/
--rw-rw-rw-   0        0        0      610 2023-05-10 18:50:57.153809 SalesforceMinu-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-05-05 20:12:58.000000 SalesforceMinu-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 18:50:57.125107 SalesforceMinu-0.0.6/SalesforceMinu/
--rw-rw-rw-   0        0        0     4357 2023-05-10 18:49:28.000000 SalesforceMinu-0.0.6/SalesforceMinu/Funciones.py
--rw-rw-rw-   0        0        0        0 2023-04-25 17:16:47.000000 SalesforceMinu-0.0.6/SalesforceMinu/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 18:50:57.152812 SalesforceMinu-0.0.6/SalesforceMinu.egg-info/
--rw-rw-rw-   0        0        0      610 2023-05-10 18:50:56.000000 SalesforceMinu-0.0.6/SalesforceMinu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-05-10 18:50:56.000000 SalesforceMinu-0.0.6/SalesforceMinu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 18:50:56.000000 SalesforceMinu-0.0.6/SalesforceMinu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-10 18:50:56.000000 SalesforceMinu-0.0.6/SalesforceMinu.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-10 18:50:56.000000 SalesforceMinu-0.0.6/SalesforceMinu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 18:50:57.155804 SalesforceMinu-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1080 2023-05-10 18:49:41.000000 SalesforceMinu-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:33:00.979843 SalesforceMinu-0.0.7/
+-rw-rw-rw-   0        0        0      610 2023-05-22 17:33:00.979843 SalesforceMinu-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-22 17:31:27.000000 SalesforceMinu-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 17:33:00.969870 SalesforceMinu-0.0.7/SalesforceMinu/
+-rw-rw-rw-   0        0        0     4759 2023-05-22 17:32:52.000000 SalesforceMinu-0.0.7/SalesforceMinu/Funciones.py
+-rw-rw-rw-   0        0        0        0 2023-04-25 17:16:47.000000 SalesforceMinu-0.0.7/SalesforceMinu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-22 17:33:00.978846 SalesforceMinu-0.0.7/SalesforceMinu.egg-info/
+-rw-rw-rw-   0        0        0      610 2023-05-22 17:33:00.000000 SalesforceMinu-0.0.7/SalesforceMinu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2023-05-22 17:33:00.000000 SalesforceMinu-0.0.7/SalesforceMinu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 17:33:00.000000 SalesforceMinu-0.0.7/SalesforceMinu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-22 17:33:00.000000 SalesforceMinu-0.0.7/SalesforceMinu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-22 17:33:00.000000 SalesforceMinu-0.0.7/SalesforceMinu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 17:33:00.980841 SalesforceMinu-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1080 2023-05-22 17:31:10.000000 SalesforceMinu-0.0.7/setup.py
```

### Comparing `SalesforceMinu-0.0.6/PKG-INFO` & `SalesforceMinu-0.0.7/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: SalesforceMinu
-Version: 0.0.6
+Version: 0.0.7
 Summary: Librería para extraer datos de minu en salesforce
 Home-page: https://github.com/BalamCor?tab=repositories
 Author: Corchado Ramos Itzae Balam
 Author-email: g7_corc18@ens.cnyn.unam.mx
 License: MIT
 Description-Content-Type: text/markdown
 
 Pasos obtenidos de: https://antonio-fernandez-troyano.medium.com/crear-una-libreria-python-4e841fbd154f
 
 Corremos en carpeta de libreria el comando:
 python setup.py sdist bdist_wheel
 
 Subimos a PyPi:
-twine upload dist/SalesforceMinu-0.0.5.tar.gz dist/SalesforceMinu-0.0.5-py3-none-any.whl
+twine upload dist/SalesforceMinu-0.0.7.tar.gz dist/SalesforceMinu-0.0.7-py3-none-any.whl
```

### Comparing `SalesforceMinu-0.0.6/SalesforceMinu/Funciones.py` & `SalesforceMinu-0.0.7/SalesforceMinu/Funciones.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,30 +5,38 @@
         data = df[df['name'].str.lower() == nam_or[i].lower()][title]
         ids_df.append(data[data.index[0]])
     return ids_df
 
 # OBTENER NOMBRES DE UN DATAFRAME
 def get_names_list(df, title = 'name'):
     if len(df[title]) == 1:
-        names = df[title].get(0)
+        names = df[title].reset_index(drop=True).get(0)
     else:
         names = ",".join(df[title])
     # Convertimos a lista
     names = names.split(',')
     return names
 
 # OBTENER LOS IDS DE ACCOUNT Y EL ORDEN DE SUS NOMBRE
 # Si no encuentra el nombre que mande mensaje de error o algo
 def get_account_id_names(names,sf):
+    from unicodedata import normalize
+
     # Puede ser un nombre o varios
     case = 0
     if type(names) == str:
-        where = f"Name = '{str(names)[1:-1]}'"
+        name = str(names)[1:-1]
+        trans_tab = dict.fromkeys(map(ord, u'\u0301\u0308'), None)
+        name = normalize('NFKC', normalize('NFKD', name).translate(trans_tab))
+        where = f"Name = '{name}'"
     else:
-        where = f"Name IN ({str(names)[1:-1]})"
+        name = str(names)[1:-1]
+        trans_tab = dict.fromkeys(map(ord, u'\u0301\u0308'), None)
+        name = normalize('NFKC', normalize('NFKD', name).translate(trans_tab))
+        where = f"Name IN ({name})"
         case = 1
     
     query = f"""SELECT Id, Name, NumberOfEmployees
     FROM Account
     WHERE {where}"""
     
     records = sf.query_all(query)
```

### Comparing `SalesforceMinu-0.0.6/SalesforceMinu.egg-info/PKG-INFO` & `SalesforceMinu-0.0.7/SalesforceMinu.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: SalesforceMinu
-Version: 0.0.6
+Version: 0.0.7
 Summary: Librería para extraer datos de minu en salesforce
 Home-page: https://github.com/BalamCor?tab=repositories
 Author: Corchado Ramos Itzae Balam
 Author-email: g7_corc18@ens.cnyn.unam.mx
 License: MIT
 Description-Content-Type: text/markdown
 
 Pasos obtenidos de: https://antonio-fernandez-troyano.medium.com/crear-una-libreria-python-4e841fbd154f
 
 Corremos en carpeta de libreria el comando:
 python setup.py sdist bdist_wheel
 
 Subimos a PyPi:
-twine upload dist/SalesforceMinu-0.0.5.tar.gz dist/SalesforceMinu-0.0.5-py3-none-any.whl
+twine upload dist/SalesforceMinu-0.0.7.tar.gz dist/SalesforceMinu-0.0.7-py3-none-any.whl
```

### Comparing `SalesforceMinu-0.0.6/setup.py` & `SalesforceMinu-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 PACKAGE_NAME = 'SalesforceMinu' 
 AUTHOR = 'Corchado Ramos Itzae Balam' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'g7_corc18@ens.cnyn.unam.mx' 
 URL = 'https://github.com/BalamCor?tab=repositories' 
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Librería para extraer datos de minu en salesforce'
```

