# Comparing `tmp/voliboli_pdf_scraper-1.5.tar.gz` & `tmp/voliboli_pdf_scraper-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voliboli_pdf_scraper-1.5.tar", last modified: Mon Apr 10 06:28:52 2023, max compression
+gzip compressed data, was "voliboli_pdf_scraper-1.6.tar", last modified: Mon May 22 09:34:49 2023, max compression
```

## Comparing `voliboli_pdf_scraper-1.5.tar` & `voliboli_pdf_scraper-1.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 06:28:52.010695 voliboli_pdf_scraper-1.5/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     1065 2023-03-07 14:17:09.000000 voliboli_pdf_scraper-1.5/LICENSE.md
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      929 2023-04-10 06:28:52.010695 voliboli_pdf_scraper-1.5/PKG-INFO
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      541 2023-03-11 12:17:05.000000 voliboli_pdf_scraper-1.5/README.md
--rw-rw-r--   0 dorka     (1000) dorka     (1000)       84 2023-03-05 11:20:22.000000 voliboli_pdf_scraper-1.5/pyproject.toml
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      496 2023-04-10 06:28:52.010695 voliboli_pdf_scraper-1.5/setup.cfg
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      340 2023-04-10 06:28:29.000000 voliboli_pdf_scraper-1.5/setup.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 06:28:52.006695 voliboli_pdf_scraper-1.5/src/
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 06:28:52.010695 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        0 2023-03-05 10:11:19.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper/__init__.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     9847 2023-03-11 11:19:59.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper/constants.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     4465 2023-04-09 12:53:21.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper/main.py
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 06:28:52.010695 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper.egg-info/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      929 2023-04-10 06:28:51.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      447 2023-04-10 06:28:52.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)        1 2023-04-10 06:28:51.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)       16 2023-04-10 06:28:51.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper.egg-info/requires.txt
--rw-rw-r--   0 dorka     (1000) dorka     (1000)       21 2023-04-10 06:28:52.000000 voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper.egg-info/top_level.txt
-drwxrwxr-x   0 dorka     (1000) dorka     (1000)        0 2023-04-10 06:28:52.010695 voliboli_pdf_scraper-1.5/tests/
--rw-rw-r--   0 dorka     (1000) dorka     (1000)      517 2023-04-09 12:52:55.000000 voliboli_pdf_scraper-1.5/tests/test_main.py
--rw-rw-r--   0 dorka     (1000) dorka     (1000)     5653 2023-04-10 06:26:08.000000 voliboli_pdf_scraper-1.5/tests/test_with_db_main.py
+drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-22 09:34:49.898289 voliboli_pdf_scraper-1.6/
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     1065 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.6/LICENSE.md
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     1219 2023-05-22 09:34:49.898289 voliboli_pdf_scraper-1.6/PKG-INFO
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      831 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.6/README.md
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)       84 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.6/pyproject.toml
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      496 2023-05-22 09:34:49.898289 voliboli_pdf_scraper-1.6/setup.cfg
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      340 2023-05-22 09:34:12.000000 voliboli_pdf_scraper-1.6/setup.py
+drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-22 09:34:49.898289 voliboli_pdf_scraper-1.6/src/
+drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-22 09:34:49.898289 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper/
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper/__init__.py
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     9885 2023-05-22 09:33:36.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper/constants.py
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     4496 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper/main.py
+drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-22 09:34:49.898289 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper.egg-info/
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     1219 2023-05-22 09:34:49.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      447 2023-05-22 09:34:49.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        1 2023-05-22 09:34:49.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)       16 2023-05-22 09:34:49.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper.egg-info/requires.txt
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)       21 2023-05-22 09:34:49.000000 voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 teodorpodobnik  (1000) teodorpodobnik  (1000)        0 2023-05-22 09:34:49.898289 voliboli_pdf_scraper-1.6/tests/
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)      517 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.6/tests/test_main.py
+-rw-rw-r--   0 teodorpodobnik  (1000) teodorpodobnik  (1000)     2877 2023-05-21 15:15:55.000000 voliboli_pdf_scraper-1.6/tests/test_with_db_main.py
```

### Comparing `voliboli_pdf_scraper-1.5/LICENSE.md` & `voliboli_pdf_scraper-1.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `voliboli_pdf_scraper-1.5/PKG-INFO` & `voliboli_pdf_scraper-1.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: voliboli_pdf_scraper
-Version: 1.5
+Version: 1.6
 Summary: Voliboli PDF Scraper
 Author: Teodor Janez Podobnik
 Author-email: teo.podobnik1234@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Voliboli PDF Scraper
 
+Main repository for scraping data of off installed statistics that are in PDF format. Data is stored in a Postgres database with the help of Flask server and GraphQL protocol.
+
+![image](https://user-images.githubusercontent.com/48418580/233640399-525d336e-ad3f-449a-b311-060489326123.png)
+
 ## Tests
 
 You can run test from the root of this repository using:
 
     pipenv run python tests/test_main.py
 
 ## Distribute
```

### Comparing `voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper/constants.py` & `voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,14 +85,15 @@
                              "17": "Videčnik Matic",
                              "18": "Kök Matej",
                              "19": "Šen Klemen"},
     "Črnuče": {"1": "Kržič Jošt",
                "2": "Mihelčič Gregor",
                "5": "Prevorčnik Jaka",
                "6": "Karadža Pevc Matevž",
+               "7": "Gornik Aljaž",
                "8": "Verdinek Jožef",
                "9": "Rojnik Matic",
                "10": "Oman Jurij",
                "11": "Sešek Jaka",
                "13": "Marovt Luka",
                "15": "Jančič Jan Karl",
                "16": "Valenčič Martin",
@@ -221,8 +222,8 @@
                "10": "Uršič Urša",
                "12": "Grubišič Čabo Julija",
                "13": "Milošič Nika",
                "14": "Divjak Naja",
                "16": "Klavžar Ema",
                "18": "Halužan Sagadin Žana",
                "21": "Bračič Neja"}
-}
+}
```

### Comparing `voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper/main.py` & `voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,31 +32,31 @@
 
 def scrape_pdf(file, upper_bound, left_bound, lower_bound, right_bound, debug):
     res = tb.read_pdf(file, area = (upper_bound, left_bound, lower_bound, right_bound), pages = '1')[0]
     if debug: logging.debug(res)
 
     return unpack_df(res)
 
-def resolve_names(numbers, teams, team, gender):
+def resolve_names(numbers, teams, team, gender, debug):
     names = []
     for num in numbers:
         try:
             names.append(teams[team][str(num)])
         except:
-            logging.warning(f"Failed to match shirt number #{num} to a {gender} in team {team}!")
+            if debug: logging.warning(f"Failed to match shirt number #{num} to a {gender} in team {team}!")
             return None
     return names
 
 def extract_players(upper_bound, lower_bound, ateam, file, debug):
     team_numbers = scrape_pdf(file, upper_bound, 20, lower_bound, 40, debug)
 
     # Unpack names based on player number - men's (in case of failure try women's)
-    names = resolve_names(team_numbers, teams_men, ateam, 'men')
+    names = resolve_names(team_numbers, teams_men, ateam, 'men', debug)
     if names is None:
-        names = resolve_names(team_numbers, teams_women, ateam, 'women')
+        names = resolve_names(team_numbers, teams_women, ateam, 'women', debug)
     if not names:
         raise Exception("Failed to resolve numbers to names while processing")
 
     if debug: logging.info(f"Players names from {ateam}: {names}")
 
     # call the function for each item in parallel
     pool = multiprocessing.Pool()
```

### Comparing `voliboli_pdf_scraper-1.5/src/voliboli_pdf_scraper.egg-info/PKG-INFO` & `voliboli_pdf_scraper-1.6/src/voliboli_pdf_scraper.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 Metadata-Version: 2.1
 Name: voliboli-pdf-scraper
-Version: 1.5
+Version: 1.6
 Summary: Voliboli PDF Scraper
 Author: Teodor Janez Podobnik
 Author-email: teo.podobnik1234@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # Voliboli PDF Scraper
 
+Main repository for scraping data of off installed statistics that are in PDF format. Data is stored in a Postgres database with the help of Flask server and GraphQL protocol.
+
+![image](https://user-images.githubusercontent.com/48418580/233640399-525d336e-ad3f-449a-b311-060489326123.png)
+
 ## Tests
 
 You can run test from the root of this repository using:
 
     pipenv run python tests/test_main.py
 
 ## Distribute
```

### Comparing `voliboli_pdf_scraper-1.5/tests/test_main.py` & `voliboli_pdf_scraper-1.6/tests/test_main.py`

 * *Files identical despite different names*

