# Comparing `tmp/bm_utilities-0.1.4.tar.gz` & `tmp/bm_utilities-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bm_utilities-0.1.4.tar", last modified: Thu May 18 12:17:57 2023, max compression
+gzip compressed data, was "bm_utilities-0.1.5.tar", last modified: Mon May 22 12:09:39 2023, max compression
```

## Comparing `bm_utilities-0.1.4.tar` & `bm_utilities-0.1.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 12:17:57.063238 bm_utilities-0.1.4/
--rw-rw-rw-   0        0        0      313 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/.editorconfig
-drwxrwxrwx   0        0        0        0 2023-05-18 12:17:56.858124 bm_utilities-0.1.4/.github/
-drwxrwxrwx   0        0        0        0 2023-05-18 12:17:56.917237 bm_utilities-0.1.4/.github/ISSUE_TEMPLATE/
--rw-rw-rw-   0        0        0      537 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-rw-   0        0        0      524 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/.github/ISSUE_TEMPLATE/config.yml
--rw-rw-rw-   0        0        0      459 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
-drwxrwxrwx   0        0        0        0 2023-05-18 12:17:56.937243 bm_utilities-0.1.4/.github/workflows/
--rw-rw-rw-   0        0        0     2125 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/.github/workflows/docs-build.yml
--rw-rw-rw-   0        0        0     1041 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/.github/workflows/docs.yml
--rw-rw-rw-   0        0        0     1076 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/.github/workflows/macos.yml
--rw-rw-rw-   0        0        0     1032 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/.github/workflows/pypi.yml
--rw-rw-rw-   0        0        0     1586 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/.github/workflows/ubuntu.yml
--rw-rw-rw-   0        0        0      962 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/.github/workflows/windows.yml
--rw-rw-rw-   0        0        0     1310 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/.gitignore
--rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1356 2023-05-18 12:17:57.064238 bm_utilities-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 12:17:56.961239 bm_utilities-0.1.4/bm_utilities/
--rw-rw-rw-   0        0        0     5068 2023-05-18 11:00:54.000000 bm_utilities-0.1.4/bm_utilities/Address_finder.py
--rw-rw-rw-   0        0        0      136 2023-05-18 12:16:29.000000 bm_utilities-0.1.4/bm_utilities/__init__.py
--rw-rw-rw-   0        0        0     1053 2023-05-18 11:18:41.000000 bm_utilities-0.1.4/bm_utilities/bm_utilities.py
--rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/bm_utilities/common.py
--rw-rw-rw-   0        0        0    11097 2023-05-18 08:07:28.000000 bm_utilities-0.1.4/bm_utilities/quality_gates.py
-drwxrwxrwx   0        0        0        0 2023-05-18 12:17:56.983240 bm_utilities-0.1.4/bm_utilities.egg-info/
--rw-rw-rw-   0        0        0     1356 2023-05-18 12:17:56.000000 bm_utilities-0.1.4/bm_utilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1015 2023-05-18 12:17:56.000000 bm_utilities-0.1.4/bm_utilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      146 2023-05-18 12:17:56.000000 bm_utilities-0.1.4/bm_utilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-18 12:17:56.000000 bm_utilities-0.1.4/bm_utilities.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      146 2023-05-18 12:17:56.000000 bm_utilities-0.1.4/bm_utilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-18 12:17:56.000000 bm_utilities-0.1.4/bm_utilities.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 12:17:57.037241 bm_utilities-0.1.4/docs/
--rw-rw-rw-   0        0        0       57 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/docs/bm_utilities.md
--rw-rw-rw-   0        0        0       96 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/docs/changelog.md
--rw-rw-rw-   0        0        0       42 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/docs/common.md
--rw-rw-rw-   0        0        0     3303 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/docs/contributing.md
-drwxrwxrwx   0        0        0        0 2023-05-18 12:17:57.042241 bm_utilities-0.1.4/docs/examples/
--rw-rw-rw-   0        0        0      309 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/docs/examples/intro.ipynb
--rw-rw-rw-   0        0        0        7 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/docs/faq.md
--rw-rw-rw-   0        0        0      502 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/docs/index.md
--rw-rw-rw-   0        0        0      612 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/docs/installation.md
-drwxrwxrwx   0        0        0        0 2023-05-18 12:17:57.046240 bm_utilities-0.1.4/docs/overrides/
--rw-rw-rw-   0        0        0      285 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/docs/overrides/main.html
--rw-rw-rw-   0        0        0       79 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/docs/usage.md
--rw-rw-rw-   0        0        0     2242 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/mkdocs.yml
--rw-rw-rw-   0        0        0      162 2023-05-18 12:05:18.000000 bm_utilities-0.1.4/requirements.txt
--rw-rw-rw-   0        0        0      162 2023-05-18 12:17:47.000000 bm_utilities-0.1.4/requirements_dev.txt
--rw-rw-rw-   0        0        0      371 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/requirements_docs.txt
--rw-rw-rw-   0        0        0      420 2023-05-18 12:17:57.067239 bm_utilities-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1771 2023-05-18 12:16:23.000000 bm_utilities-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 12:17:57.059239 bm_utilities-0.1.4/tests/
--rw-rw-rw-   0        0        0       43 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/tests/__init__.py
--rw-rw-rw-   0        0        0      433 2023-04-24 13:32:39.000000 bm_utilities-0.1.4/tests/test_bm_utilities.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:09:39.971608 bm_utilities-0.1.5/
+-rw-rw-rw-   0        0        0      313 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/.editorconfig
+drwxrwxrwx   0        0        0        0 2023-05-22 12:09:39.734610 bm_utilities-0.1.5/.github/
+drwxrwxrwx   0        0        0        0 2023-05-22 12:09:39.774611 bm_utilities-0.1.5/.github/ISSUE_TEMPLATE/
+-rw-rw-rw-   0        0        0      537 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-rw-   0        0        0      524 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-rw-rw-   0        0        0      459 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxrwxrwx   0        0        0        0 2023-05-22 12:09:39.822609 bm_utilities-0.1.5/.github/workflows/
+-rw-rw-rw-   0        0        0     2125 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/.github/workflows/docs-build.yml
+-rw-rw-rw-   0        0        0     1041 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/.github/workflows/docs.yml
+-rw-rw-rw-   0        0        0     1076 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/.github/workflows/macos.yml
+-rw-rw-rw-   0        0        0     1032 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/.github/workflows/pypi.yml
+-rw-rw-rw-   0        0        0     1586 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/.github/workflows/ubuntu.yml
+-rw-rw-rw-   0        0        0      962 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/.github/workflows/windows.yml
+-rw-rw-rw-   0        0        0     1310 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/.gitignore
+-rw-rw-rw-   0        0        0     1092 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      129 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1356 2023-05-22 12:09:39.971608 bm_utilities-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      610 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 12:09:39.885608 bm_utilities-0.1.5/bm_utilities/
+-rw-rw-rw-   0        0        0     5068 2023-05-18 11:00:54.000000 bm_utilities-0.1.5/bm_utilities/Address_finder.py
+-rw-rw-rw-   0        0        0      136 2023-05-22 12:08:32.000000 bm_utilities-0.1.5/bm_utilities/__init__.py
+-rw-rw-rw-   0        0        0     1053 2023-05-18 11:18:41.000000 bm_utilities-0.1.5/bm_utilities/bm_utilities.py
+-rw-rw-rw-   0        0        0      194 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/bm_utilities/common.py
+-rw-rw-rw-   0        0        0    11623 2023-05-22 12:04:21.000000 bm_utilities-0.1.5/bm_utilities/quality_gates.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:09:39.939609 bm_utilities-0.1.5/bm_utilities.egg-info/
+-rw-rw-rw-   0        0        0     1356 2023-05-22 12:09:39.000000 bm_utilities-0.1.5/bm_utilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1015 2023-05-22 12:09:39.000000 bm_utilities-0.1.5/bm_utilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      146 2023-05-22 12:09:39.000000 bm_utilities-0.1.5/bm_utilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-22 12:09:39.000000 bm_utilities-0.1.5/bm_utilities.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      146 2023-05-22 12:09:39.000000 bm_utilities-0.1.5/bm_utilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-22 12:09:39.000000 bm_utilities-0.1.5/bm_utilities.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 12:09:39.957615 bm_utilities-0.1.5/docs/
+-rw-rw-rw-   0        0        0       57 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/docs/bm_utilities.md
+-rw-rw-rw-   0        0        0       96 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/docs/changelog.md
+-rw-rw-rw-   0        0        0       42 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/docs/common.md
+-rw-rw-rw-   0        0        0     3303 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/docs/contributing.md
+drwxrwxrwx   0        0        0        0 2023-05-22 12:09:39.959610 bm_utilities-0.1.5/docs/examples/
+-rw-rw-rw-   0        0        0      309 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/docs/examples/intro.ipynb
+-rw-rw-rw-   0        0        0        7 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/docs/faq.md
+-rw-rw-rw-   0        0        0      502 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/docs/index.md
+-rw-rw-rw-   0        0        0      612 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/docs/installation.md
+drwxrwxrwx   0        0        0        0 2023-05-22 12:09:39.961614 bm_utilities-0.1.5/docs/overrides/
+-rw-rw-rw-   0        0        0      285 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/docs/overrides/main.html
+-rw-rw-rw-   0        0        0       79 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/docs/usage.md
+-rw-rw-rw-   0        0        0     2242 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/mkdocs.yml
+-rw-rw-rw-   0        0        0      162 2023-05-18 12:05:18.000000 bm_utilities-0.1.5/requirements.txt
+-rw-rw-rw-   0        0        0      162 2023-05-18 12:17:47.000000 bm_utilities-0.1.5/requirements_dev.txt
+-rw-rw-rw-   0        0        0      371 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/requirements_docs.txt
+-rw-rw-rw-   0        0        0      420 2023-05-22 12:09:39.973616 bm_utilities-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1771 2023-05-22 12:08:24.000000 bm_utilities-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 12:09:39.968609 bm_utilities-0.1.5/tests/
+-rw-rw-rw-   0        0        0       43 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/tests/__init__.py
+-rw-rw-rw-   0        0        0      433 2023-04-24 13:32:39.000000 bm_utilities-0.1.5/tests/test_bm_utilities.py
```

### Comparing `bm_utilities-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md` & `bm_utilities-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/.github/ISSUE_TEMPLATE/config.yml` & `bm_utilities-0.1.5/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/.github/workflows/docs-build.yml` & `bm_utilities-0.1.5/.github/workflows/docs-build.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/.github/workflows/docs.yml` & `bm_utilities-0.1.5/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/.github/workflows/macos.yml` & `bm_utilities-0.1.5/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/.github/workflows/pypi.yml` & `bm_utilities-0.1.5/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/.github/workflows/ubuntu.yml` & `bm_utilities-0.1.5/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/.github/workflows/windows.yml` & `bm_utilities-0.1.5/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/.gitignore` & `bm_utilities-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/LICENSE` & `bm_utilities-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/PKG-INFO` & `bm_utilities-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm_utilities
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.1.4/README.md` & `bm_utilities-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/bm_utilities/Address_finder.py` & `bm_utilities-0.1.5/bm_utilities/Address_finder.py`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/bm_utilities/bm_utilities.py` & `bm_utilities-0.1.5/bm_utilities/bm_utilities.py`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/bm_utilities/quality_gates.py` & `bm_utilities-0.1.5/bm_utilities/quality_gates.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,53 +18,63 @@
     def read_data(self,path):
         data=pd.read_csv(path)
         return data
 
     def run_Quality_Gates(self,df,config_path):
         config=self.read_config(config_path)
         
-        columns_names=config['columns_names']
-        num_of_records=config['num_of_records']
-        if(not self.check_structure(df,columns_names,num_of_records)):
+        
+        if(not self.check_structure(df,config)):
             return
         df["reason_of_rejection"]=""
         df["explanation_of_rejection"]=""
 
-        if("column_checklist" in config.keys()):
-            self.run_columns_checklist(df,config['column_checklist'])
-        if("row_checklist" in config.keys()):
-            self.run_rows_checklist(df,config['row_checklist'])
+        if("columns_checklist" in config.keys()):
+            self.run_columns_checklist(df,config['columns_checklist'])
+        if("rows_checklist" in config.keys()):
+            self.run_rows_checklist(df,config['rows_checklist'])
         self.clean_rejection_columns(df)
         return df
 
 
 
     def clean_rejection_columns(self,df):
         columns=["reason_of_rejection","explanation_of_rejection"]
         for column_name in columns:
             df[column_name] = df[column_name].apply(lambda x: ','.join(set(filter(None, x.split(',')))).strip(','))
 
 
     ###########################################################################################################################################
     #high level checks
-    def check_structure(self,df,columns_names,num_of_records):
+    def check_structure(self,df,config):
         ans=True
-        if df.shape[0]!=num_of_records:
-            print("number of records is not matched")
-            ans=False
-        df_columns = df.columns.tolist()
-        list_set = set(columns_names)
-        df_set = set(df_columns)
-
-        missing_in_list = df_set - list_set
-        missing_in_df = list_set - df_set
-
-        if missing_in_df or missing_in_list:
-            print("Columns names are not matched")
-            ans=False
+        
+        if("check_number_of_columns" in config):
+            if(config["check_number_of_columns"]==True and df.shape[1]!=config["num_columns"]):
+                print("number of columns is not matched")
+                ans=False
+        if ("check_number_of_records" in config):
+            num_of_records=config["num_of_records"]
+            if (config["check_number_of_records"]==True and df.shape[0]!=num_of_records):
+                print("number of records is not matched")
+                ans=False
+        if("check_number_of_columns" in config):
+            if(config["check_number_of_columns"]==True):
+                columns_names=config["columns_names"]
+                
+                df_columns = df.columns.tolist()
+                list_set = set(columns_names)
+                df_set = set(df_columns)
+
+                missing_in_list = df_set - list_set
+                missing_in_df = list_set - df_set
+
+                if missing_in_df or missing_in_list:
+                    print("Columns names are not matched")
+                    ans=False
 
         return ans
 
     def run_rows_checklist(self,df,row_checklist_config):
         print("run_rows_checklist")
         if "completness_check" in row_checklist_config:
             self.completness_check(df,row_checklist_config["completness_check"])
@@ -185,18 +195,19 @@
         
         explanation = "this row is repeated {} times".format(duplicate_rows.groupby(columns_to_check).size().get(0))
         df.loc[duplicate_indices, explanation_column] += explanation
         
         return df
 
 
-    def format_consistency_check(self,df,format_consistency_check_config):
+    def format_consistency_check(self,df, format_config):
         print("format_check")
-        for col_name in format_consistency_check_config.keys():
-            format_regex=format_consistency_check_config[col_name]["format"]
+        columns_to_check=list(format_config.keys())
+        for col_name in columns_to_check:
+            format_regex=format_config[col_name]["format_regex"]
             reason_column = 'reason_of_rejection'
             explanation_column = 'explanation_of_rejection'
             
             invalid_format_rows = df[~df[col_name].astype(str).str.match(format_regex, na=False)]
             
             df.loc[invalid_format_rows.index, reason_column] += self.invalid_format
             df.loc[invalid_format_rows.index, explanation_column] += "Column '{}' has invalid format".format(col_name) +" "
```

### Comparing `bm_utilities-0.1.4/bm_utilities.egg-info/PKG-INFO` & `bm_utilities-0.1.5/bm_utilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bm-utilities
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python package for bm utilities
 Home-page: https://github.com/Youssefamroo/bm_utilities
 Author: youssef amr
 Author-email: usef.amr11@gmail.com
 License: MIT license
 Keywords: bm_utilities
 Classifier: Intended Audience :: Developers
```

### Comparing `bm_utilities-0.1.4/bm_utilities.egg-info/SOURCES.txt` & `bm_utilities-0.1.5/bm_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/docs/contributing.md` & `bm_utilities-0.1.5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/docs/installation.md` & `bm_utilities-0.1.5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/mkdocs.yml` & `bm_utilities-0.1.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `bm_utilities-0.1.4/setup.py` & `bm_utilities-0.1.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='bm_utilities',
     name='bm_utilities',
     packages=find_packages(include=['bm_utilities', 'bm_utilities.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/Youssefamroo/bm_utilities',
-    version='0.1.4',
+    version='0.1.5',
     zip_safe=False,
 )
```

