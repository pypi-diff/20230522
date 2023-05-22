# Comparing `tmp/zypl_macro-1.0.4.tar.gz` & `tmp/zypl_macro-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zypl_macro-1.0.4.tar", last modified: Fri May 19 14:36:14 2023, max compression
+gzip compressed data, was "zypl_macro-1.0.5.tar", last modified: Mon May 22 06:55:24 2023, max compression
```

## Comparing `zypl_macro-1.0.4.tar` & `zypl_macro-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 14:36:14.284538 zypl_macro-1.0.4/
--rw-rw-rw-   0        0        0     1085 2023-05-16 15:19:29.000000 zypl_macro-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     4568 2023-05-19 14:36:14.284538 zypl_macro-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4205 2023-05-19 14:33:02.000000 zypl_macro-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-19 14:36:14.284538 zypl_macro-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      707 2023-05-19 14:35:04.000000 zypl_macro-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 14:36:14.278550 zypl_macro-1.0.4/zypl_macro/
--rw-rw-rw-   0        0        0        2 2023-05-14 06:12:43.000000 zypl_macro-1.0.4/zypl_macro/__init__.py
--rw-rw-rw-   0        0        0     4692 2023-05-19 14:33:24.000000 zypl_macro-1.0.4/zypl_macro/library.py
-drwxrwxrwx   0        0        0        0 2023-05-19 14:36:14.283543 zypl_macro-1.0.4/zypl_macro.egg-info/
--rw-rw-rw-   0        0        0     4568 2023-05-19 14:36:14.000000 zypl_macro-1.0.4/zypl_macro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-05-19 14:36:14.000000 zypl_macro-1.0.4/zypl_macro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 14:36:14.000000 zypl_macro-1.0.4/zypl_macro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-19 14:36:14.000000 zypl_macro-1.0.4/zypl_macro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-19 14:36:14.000000 zypl_macro-1.0.4/zypl_macro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 06:55:24.913644 zypl_macro-1.0.5/
+-rw-rw-rw-   0        0        0     1085 2023-05-16 15:19:29.000000 zypl_macro-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     4568 2023-05-22 06:55:24.913644 zypl_macro-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4205 2023-05-19 14:33:02.000000 zypl_macro-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 06:55:24.914642 zypl_macro-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      707 2023-05-22 06:54:43.000000 zypl_macro-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:55:24.908278 zypl_macro-1.0.5/zypl_macro/
+-rw-rw-rw-   0        0        0        2 2023-05-14 06:12:43.000000 zypl_macro-1.0.5/zypl_macro/__init__.py
+-rw-rw-rw-   0        0        0     4626 2023-05-22 06:54:14.000000 zypl_macro-1.0.5/zypl_macro/library.py
+drwxrwxrwx   0        0        0        0 2023-05-22 06:55:24.912648 zypl_macro-1.0.5/zypl_macro.egg-info/
+-rw-rw-rw-   0        0        0     4568 2023-05-22 06:55:24.000000 zypl_macro-1.0.5/zypl_macro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2023-05-22 06:55:24.000000 zypl_macro-1.0.5/zypl_macro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 06:55:24.000000 zypl_macro-1.0.5/zypl_macro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-05-22 06:55:24.000000 zypl_macro-1.0.5/zypl_macro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-22 06:55:24.000000 zypl_macro-1.0.5/zypl_macro.egg-info/top_level.txt
```

### Comparing `zypl_macro-1.0.4/LICENSE` & `zypl_macro-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `zypl_macro-1.0.4/PKG-INFO` & `zypl_macro-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zypl_macro
-Version: 1.0.4
+Version: 1.0.5
 Summary: zypl.ai alternative data API interface lib
 Author: Me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `zypl_macro-1.0.4/README.md` & `zypl_macro-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `zypl_macro-1.0.4/setup.py` & `zypl_macro-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="zypl_macro",
-    version="1.0.4",
+    version="1.0.5",
     author="Me",
     description="zypl.ai alternative data API interface lib",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `zypl_macro-1.0.4/zypl_macro/library.py` & `zypl_macro-1.0.5/zypl_macro/library.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         self._API_KEY = token
         response = self._api_call(frequency='Yearly', country='Tajikistan')
         if response.status_code == 403:
             print('Invalid authorization key')
             self._API_KEY = ''
 
 
-    def get_data(self, indicators=None, **kwargs) -> pd.DataFrame | str:
+    def get_data(self, indicators=None, **kwargs):
       
         if 'start' in kwargs.keys():
             try: datetime.date.fromisoformat(kwargs['start']) 
             except ValueError: 
                 return "Dates should be provided in YYYY-MM-DD format!"
         if 'end' in kwargs.keys():
             try: datetime.date.fromisoformat(kwargs['end']) 
@@ -80,26 +80,26 @@
             df.drop(columns=cols, inplace=True)
             df.dropna(subset=df.drop(columns=['Country', 'Date']).columns, inplace=True, how='all')
 
         # df.to_csv("%s/%s_macrodata.csv" % (os.getcwd(), kwargs['country']), header=df.columns, index=False,  sep=";")
         df.sort_values(by='Date', inplace=True)
         return df
     
-    def get_countries(self) -> pd.DataFrame | str:
+    def get_countries(self):
         try: data = self._api_call(frequency="Yearly").json()
         except NoAuthorization as e: 
             return e.message
         
         entirety = pd.DataFrame(data)
         countries = pd.DataFrame({'Country name': entirety['country'].unique()})
         # countries.to_csv('%s/supported_countries.csv' % os.getcwd(), index=False,  sep=";")
         
         return countries
 
-    def get_indicators(self, **kwargs) -> pd.DataFrame | str:
+    def get_indicators(self, **kwargs):
         try: data = self._api_call(country=kwargs.get('country') or '').json()
         except NoAuthorization as e: 
             return e.message
         
         if len(data) == 0: 
             return 'Invalid country name.'
```

### Comparing `zypl_macro-1.0.4/zypl_macro.egg-info/PKG-INFO` & `zypl_macro-1.0.5/zypl_macro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zypl-macro
-Version: 1.0.4
+Version: 1.0.5
 Summary: zypl.ai alternative data API interface lib
 Author: Me
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

