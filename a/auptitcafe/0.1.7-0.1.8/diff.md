# Comparing `tmp/auptitcafe-0.1.7.tar.gz` & `tmp/auptitcafe-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auptitcafe-0.1.7.tar", max compression
+gzip compressed data, was "auptitcafe-0.1.8.tar", max compression
```

## Comparing `auptitcafe-0.1.7.tar` & `auptitcafe-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      703 2023-05-13 06:57:43.061927 auptitcafe-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-05-13 06:58:27.626995 auptitcafe-0.1.7/auptitcafe/__init__.py
--rw-r--r--   0        0        0     2288 2023-05-13 06:57:43.061927 auptitcafe-0.1.7/auptitcafe/menus.py
--rw-r--r--   0        0        0      503 2023-05-13 06:57:43.061927 auptitcafe-0.1.7/auptitcafe/plat.py
--rw-r--r--   0        0        0      443 2023-05-13 06:57:43.061927 auptitcafe-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1193 1970-01-01 00:00:00.000000 auptitcafe-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1617 2023-05-21 22:23:53.020362 auptitcafe-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 22:24:30.480749 auptitcafe-0.1.8/auptitcafe/__init__.py
+-rw-r--r--   0        0        0     2755 2023-05-21 22:23:53.020362 auptitcafe-0.1.8/auptitcafe/menus.py
+-rw-r--r--   0        0        0      503 2023-05-21 22:23:53.020362 auptitcafe-0.1.8/auptitcafe/plat.py
+-rw-r--r--   0        0        0      443 2023-05-21 22:23:53.020362 auptitcafe-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2107 1970-01-01 00:00:00.000000 auptitcafe-0.1.8/PKG-INFO
```

### Comparing `auptitcafe-0.1.7/auptitcafe/menus.py` & `auptitcafe-0.1.8/auptitcafe/menus.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,28 +7,41 @@
 
 
 class Menus:
     def __init__(self):
         self.menus_url = "http://auptitcafe.nc/menu/"
 
 
+    def get_title(self):
+        response = requests.get(self.menus_url )
+        soup = BeautifulSoup(response.text, 'html.parser')
+        title = soup.find('h2', class_='elementor-heading-title elementor-size-default')
+        out = title.text.strip()
+        return out
+
+
     def get_all(self):
         out = []
         response = requests.get(self.menus_url )
         soup = BeautifulSoup(response.text, 'html.parser')
         title = soup.find('h2', class_='elementor-heading-title elementor-size-default')
         #print('title : <' + title.text.strip() + '>')
         # Plats
 
         menus = soup.find_all('div', class_='col-sm-6 col-md-6 mb-4 selfer-contact-info')
 
         for menu in menus:
             name = menu.find('h5').text.strip()
-            image = menu.find('img')['src']
-            recette = menu.find('div').text.strip()
+            # get the menu photo
+            if menu.find('img'):
+                image = menu.find('img')['src']
+            else:
+                image = ""
+            # Get the details fo the receipe
+            recette = menu.find('div', class_='contact_descriptions').text.strip()
             #print('name : <' + name + '>')
             titre_plat = name.split("-")[0].strip()
             #print('Titre plat : <' + titre_plat + '>')
             #print('url image : <' + image + '>')
             #print('recette : <' + recette + '>')
             #image_url = menu.find('img')['src']
             #print(name + " : " + image_url)
```

### Comparing `auptitcafe-0.1.7/PKG-INFO` & `auptitcafe-0.1.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,52 @@
-Metadata-Version: 2.1
-Name: auptitcafe
-Version: 0.1.7
-Summary: SDK pour interagir avec http://auptitcafe.nc/menu/
-Author: Adrien SALES
-Author-email: Adrien.Sales@gmail.com
-Requires-Python: >=3.9,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
-Description-Content-Type: text/markdown
-
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/auptitcafe)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/auptitcafe)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/auptitcafe)
 ![PyPI - Format](https://img.shields.io/pypi/format/auptitcafe)
 ![PyPI](https://img.shields.io/pypi/v/auptitcafe)
 
-# Quickstart
+# ❔ About
+
+> Finally a Python package to make **getting Au p'it café's menus a piece of (cheese) cake.😅**
+
+# 🔖 Resources
+
+- [Official website](http://auptitcafe.nc/)
+- [TripAdvisor](https://www.tripadvisor.com/Restaurant_Review-g294130-d1952994-Reviews-Au_P_tit_Cafe-Noumea_Grand_Terre.html)
+- [`pypi`](https://pypi.org/project/auptitcafe/)
+- [Instagram](https://www.instagram.com/auptitcafe.nc/?hl=en) 
+- [Facebook](https://www.facebook.com/auptitcafe.nc/)
+- [Google Maps](https://goo.gl/maps/4UcxegSnxMsE8qKs8)
+
+[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/iRSInif_Zwc/0.jpg)](https://www.youtube.com/watch?v=iRSInif_Zwc)
+
+
+# 🚀 Quickstart
+
+For the impatients, here is a quick and ready to use code snippet:
 
 ```python
+# Install the package
 !pip install auptitcafe
 
+# Make some imports
 from auptitcafe.menus import Menus
+import pandas as pd
 
+# Create the main utility instance
 menu_instance = Menus()
-menus = []
-menus = menu_instance.get_all()
-len(menus)
+
+# Dump menus as a csv file
+menus = 'menus.csv'
+menu_instance.to_csv(menus)
+
+# Load menus in a panda dataframe
+df = pd.read_csv(menus)
+# Diplay dataframe
+df
 ```
 
 # For devs
 
 ## Build
 
 ```
@@ -54,8 +68,7 @@
 
 ## Publish
 
 ```
 poetry config pypi-token.pypi $PYPI_TOKEM
 poetry publish
 ```
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

