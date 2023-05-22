# Comparing `tmp/sidra_helpers-1.0.6.tar.gz` & `tmp/sidra_helpers-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sidra_helpers-1.0.6.tar", last modified: Sat Jan 28 19:15:14 2023, max compression
+gzip compressed data, was "sidra_helpers-1.0.7.tar", last modified: Mon May 22 14:57:38 2023, max compression
```

## Comparing `sidra_helpers-1.0.6.tar` & `sidra_helpers-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-28 19:15:14.464568 sidra_helpers-1.0.6/
--rw-rw-rw-   0        0        0     1102 2023-01-09 13:29:55.000000 sidra_helpers-1.0.6/LICENSE
--rw-rw-rw-   0        0        0     1224 2023-01-28 19:15:14.464568 sidra_helpers-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      748 2023-01-09 13:31:15.000000 sidra_helpers-1.0.6/README.md
--rw-rw-rw-   0        0        0      106 2023-01-09 13:31:29.000000 sidra_helpers-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0      491 2023-01-28 19:15:14.465567 sidra_helpers-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      376 2023-01-28 19:13:24.000000 sidra_helpers-1.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-28 19:15:14.453565 sidra_helpers-1.0.6/sidra_helpers/
--rw-rw-rw-   0        0        0       28 2023-01-09 13:43:50.000000 sidra_helpers-1.0.6/sidra_helpers/__init__.py
--rw-rw-rw-   0        0        0     5462 2023-01-28 19:12:44.000000 sidra_helpers-1.0.6/sidra_helpers/sidra_helpers.py
-drwxrwxrwx   0        0        0        0 2023-01-28 19:15:14.462566 sidra_helpers-1.0.6/sidra_helpers.egg-info/
--rw-rw-rw-   0        0        0     1224 2023-01-28 19:15:14.000000 sidra_helpers-1.0.6/sidra_helpers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-01-28 19:15:14.000000 sidra_helpers-1.0.6/sidra_helpers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-28 19:15:14.000000 sidra_helpers-1.0.6/sidra_helpers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-01-28 19:15:14.000000 sidra_helpers-1.0.6/sidra_helpers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-01-28 19:15:14.000000 sidra_helpers-1.0.6/sidra_helpers.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:38.608756 sidra_helpers-1.0.7/
+-rw-rw-rw-   0        0        0     1102 2023-01-09 13:29:55.000000 sidra_helpers-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0     1224 2023-05-22 14:57:38.608756 sidra_helpers-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      748 2023-01-09 13:31:15.000000 sidra_helpers-1.0.7/README.md
+-rw-rw-rw-   0        0        0      106 2023-01-09 13:31:29.000000 sidra_helpers-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      491 2023-05-22 14:57:38.610759 sidra_helpers-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      376 2023-05-22 14:55:47.000000 sidra_helpers-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:38.596756 sidra_helpers-1.0.7/sidra_helpers/
+-rw-rw-rw-   0        0        0       28 2023-01-09 13:43:50.000000 sidra_helpers-1.0.7/sidra_helpers/__init__.py
+-rw-rw-rw-   0        0        0     6698 2023-05-22 14:53:24.000000 sidra_helpers-1.0.7/sidra_helpers/sidra_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-22 14:57:38.607757 sidra_helpers-1.0.7/sidra_helpers.egg-info/
+-rw-rw-rw-   0        0        0     1224 2023-05-22 14:57:38.000000 sidra_helpers-1.0.7/sidra_helpers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-05-22 14:57:38.000000 sidra_helpers-1.0.7/sidra_helpers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 14:57:38.000000 sidra_helpers-1.0.7/sidra_helpers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 14:57:38.000000 sidra_helpers-1.0.7/sidra_helpers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 14:57:38.000000 sidra_helpers-1.0.7/sidra_helpers.egg-info/top_level.txt
```

### Comparing `sidra_helpers-1.0.6/LICENSE` & `sidra_helpers-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sidra_helpers-1.0.6/PKG-INFO` & `sidra_helpers-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidra_helpers
-Version: 1.0.6
+Version: 1.0.7
 Summary: Helper functions made for personal use to work with the SIDRA API
 Home-page: https://github.com/GuilhermeFrainer/sidra_helpers
 Author: Guilherme da Silva Frainer
 Author-email: guilherme.sfrainer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sidra_helpers-1.0.6/README.md` & `sidra_helpers-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `sidra_helpers-1.0.6/sidra_helpers/sidra_helpers.py` & `sidra_helpers-1.0.7/sidra_helpers/sidra_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -139,7 +139,42 @@
     try:
         with open(path, 'r') as file:
             config = json.load(file)
     except FileNotFoundError:
         sys.exit("Config file not found")
     return config
 
+
+# Adds a sheet with the data to the workbook
+# Sets default date and number formats if they haven't been set
+def make_sheet(sheet_name: str, series_list: list[list], workbook: xlsxwriter.Workbook, headers: list[str], index_chart=False) -> xlsxwriter.Workbook.worksheet_class:
+    global date_format, number_format
+
+    skipped_lines = 0
+    if index_chart:
+        skipped_lines = 4
+
+    worksheet = workbook.add_worksheet(sheet_name)
+    
+    # Sets date and number formats if there are none
+    if date_format == None:
+        date_format = workbook.add_format({'num_format': 'mmm/yy'})
+    
+    if number_format == None:
+        number_format = workbook.add_format({'num_format': '##0.0'})
+
+    # Writes headers
+    for (i, header) in enumerate(headers):
+        worksheet.write(0 + skipped_lines, i, header)
+
+    # Writes data
+    for (j, series) in enumerate(series_list):
+        for (i, entry) in enumerate(series):
+            # Writes dates
+            if j == 0:
+                worksheet.write_datetime(skipped_lines + 1 + i, j, entry, date_format)
+            # Writes numeric data
+            else:
+                worksheet.write(skipped_lines + 1 + i, j, entry)
+
+    return worksheet
+
```

### Comparing `sidra_helpers-1.0.6/sidra_helpers.egg-info/PKG-INFO` & `sidra_helpers-1.0.7/sidra_helpers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sidra-helpers
-Version: 1.0.6
+Version: 1.0.7
 Summary: Helper functions made for personal use to work with the SIDRA API
 Home-page: https://github.com/GuilhermeFrainer/sidra_helpers
 Author: Guilherme da Silva Frainer
 Author-email: guilherme.sfrainer@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

