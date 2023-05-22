# Comparing `tmp/cicc_excel-0.1.0.tar.gz` & `tmp/cicc_excel-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cicc_excel-0.1.0.tar", last modified: Sun May 14 13:49:19 2023, max compression
+gzip compressed data, was "cicc_excel-0.2.0.tar", last modified: Mon May 22 08:08:50 2023, max compression
```

## Comparing `cicc_excel-0.1.0.tar` & `cicc_excel-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 13:49:18.970000 cicc_excel-0.1.0/
--rw-rw-rw-   0        0        0     1093 2023-05-14 05:35:00.000000 cicc_excel-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1705 2023-05-14 13:49:20.000000 cicc_excel-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1142 2023-05-14 13:39:04.000000 cicc_excel-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 13:49:19.000000 cicc_excel-0.1.0/cicc_excel/
--rw-rw-rw-   0        0        0        0 2023-05-14 05:35:00.000000 cicc_excel-0.1.0/cicc_excel/__init__.py
--rw-rw-rw-   0        0        0    13055 2023-05-14 13:44:14.000000 cicc_excel-0.1.0/cicc_excel/excelwriter.py
-drwxrwxrwx   0        0        0        0 2023-05-14 13:49:19.030000 cicc_excel-0.1.0/cicc_excel.egg-info/
--rw-rw-rw-   0        0        0     1705 2023-05-14 13:49:20.000000 cicc_excel-0.1.0/cicc_excel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-14 13:49:20.000000 cicc_excel-0.1.0/cicc_excel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 13:49:20.000000 cicc_excel-0.1.0/cicc_excel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-14 13:49:20.000000 cicc_excel-0.1.0/cicc_excel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-14 13:49:20.000000 cicc_excel-0.1.0/cicc_excel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 13:49:20.000000 cicc_excel-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      867 2023-05-14 13:43:54.000000 cicc_excel-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:08:50.280000 cicc_excel-0.2.0/
+-rw-rw-rw-   0        0        0     1093 2023-05-14 05:35:00.000000 cicc_excel-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1777 2023-05-22 08:08:52.000000 cicc_excel-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1214 2023-05-22 08:03:36.000000 cicc_excel-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 08:08:50.310000 cicc_excel-0.2.0/cicc_excel/
+-rw-rw-rw-   0        0        0        0 2023-05-14 05:35:00.000000 cicc_excel-0.2.0/cicc_excel/__init__.py
+-rw-rw-rw-   0        0        0    13899 2023-05-22 08:02:56.000000 cicc_excel-0.2.0/cicc_excel/excelwriter.py
+drwxrwxrwx   0        0        0        0 2023-05-22 08:08:50.340000 cicc_excel-0.2.0/cicc_excel.egg-info/
+-rw-rw-rw-   0        0        0     1777 2023-05-22 08:08:50.000000 cicc_excel-0.2.0/cicc_excel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-22 08:08:52.000000 cicc_excel-0.2.0/cicc_excel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 08:08:50.000000 cicc_excel-0.2.0/cicc_excel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-22 08:08:50.000000 cicc_excel-0.2.0/cicc_excel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-22 08:08:50.000000 cicc_excel-0.2.0/cicc_excel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 08:08:52.000000 cicc_excel-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      867 2023-05-22 08:08:38.000000 cicc_excel-0.2.0/setup.py
```

### Comparing `cicc_excel-0.1.0/LICENSE` & `cicc_excel-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cicc_excel-0.1.0/PKG-INFO` & `cicc_excel-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cicc_excel
-Version: 0.1.0
+Version: 0.2.0
 Summary: Library of export pandas into excel for CICCers
 Home-page: https://github.com/nyuspc/cicc_excel
 Author: Pengcheng Song
 Author-email: smth_spc@hotmail.com
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -36,14 +36,17 @@
 wb.set_hl_col_by_names('col_name2', 'sheet_name', 'background_color2', 'color2')
 #write dataframe to xlsx file
 wb.write_data('sheet_name')
 
 #hide cols
 wb.hide_col(5,12,'sheet_name')
 
+#collapse cols (have a + on top)
+wb.collapse_col(5,12,'sheet_name')
+
 #freeze cell
 wb.freeze(1,4, 'sheet_name')
 
 #set hightlight columns for another sheet
 #default background color is yellow
 wb.load_data(df2)
 wb.set_hl_col_by_names('col_name', 'another_sheet_name')
```

### Comparing `cicc_excel-0.1.0/README.md` & `cicc_excel-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 wb.set_hl_col_by_names('col_name2', 'sheet_name', 'background_color2', 'color2')
 #write dataframe to xlsx file
 wb.write_data('sheet_name')
 
 #hide cols
 wb.hide_col(5,12,'sheet_name')
 
+#collapse cols (have a + on top)
+wb.collapse_col(5,12,'sheet_name')
+
 #freeze cell
 wb.freeze(1,4, 'sheet_name')
 
 #set hightlight columns for another sheet
 #default background color is yellow
 wb.load_data(df2)
 wb.set_hl_col_by_names('col_name', 'another_sheet_name')
```

### Comparing `cicc_excel-0.1.0/cicc_excel/excelwriter.py` & `cicc_excel-0.2.0/cicc_excel/excelwriter.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,33 @@
         }
         self.en_font = en_font
         self.ch_font = ch_font
         self.num_font = num_font
         self.hl_cols = {}
         #Setting Styles
         self.first_row_height = first_row_height
-        self.styles['normal']['header'] = self.workbook.add_format({
-            'border':None,
-            'bold': True,
-            'font_size': 10,
-            'font_name': ch_font,
-            'bg_color': first_row_color,
-            'align': 'center',
-            'valign': 'vcenter'
-        })
+        if first_row_color is None:
+            self.styles['normal']['header'] = self.workbook.add_format({
+                'border':None,
+                'bold': True,
+                'font_size': 10,
+                'font_name': ch_font,
+                'align': 'center',
+                'valign': 'vcenter'
+            })
+        else:
+            self.styles['normal']['header'] = self.workbook.add_format({
+                'border':None,
+                'bold': True,
+                'font_size': 10,
+                'font_name': ch_font,
+                'bg_color': first_row_color,
+                'align': 'center',
+                'valign': 'vcenter'
+            })
         self.styles['normal']['number_format'] = self.workbook.add_format({
             'font_size': 10,
             'align': 'right',
             'valign': 'vcenter',
             'font_name': num_font,
             'num_format': '#,##0'
         })
@@ -237,22 +247,33 @@
         if ws is not None:
             ws.autofit()
         else:
             print("Error: worksheets", sheet_name, "not found")
 
     def hide_col(self, start_col=0, end_col=0, sheet_name='Sheet1'):
         """
-        Hide acolumns.
+        Hide columns.
         """
         ws = self.workbook.get_worksheet_by_name(sheet_name)
         if ws is not None:
             ws.set_column(start_col-1, end_col-1, None, None, {'hidden': True})
         else:
             print("Error: worksheets", sheet_name, "not found")
     
+    def collapse_col(self, start_col=0, end_col=0, sheet_name='Sheet1'):
+        """
+        collapse columns.
+        """
+        ws = self.workbook.get_worksheet_by_name(sheet_name)
+        if ws is not None:
+        #collapsed note does not work, use hidden + level instead.
+            ws.set_column(start_col-1, end_col-1, None, None, {'hidden': True, 'level': 1})
+        else:
+            print("Error: worksheets", sheet_name, "not found")
+    
     def set_hl_col_by_names(self, col_name, sheet_name, hl_bg_color='#EEECE1', hl_color='#000000'):
         """
         Set col by col name
         """
         if self.hl_cols.get(sheet_name) is None:
             self.hl_cols[sheet_name] = [col_name]
         else:
@@ -337,10 +358,7 @@
         self.styles[sheet_name][col_name]['default_format'] = self.workbook.add_format({
             'font_size':10,
             'bg_color': hl_bg_color,
             'font_color': hl_color,
             'align': 'left',
             'valign': 'vcenter'
         })
-
-
-
```

### Comparing `cicc_excel-0.1.0/cicc_excel.egg-info/PKG-INFO` & `cicc_excel-0.2.0/cicc_excel.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cicc-excel
-Version: 0.1.0
+Version: 0.2.0
 Summary: Library of export pandas into excel for CICCers
 Home-page: https://github.com/nyuspc/cicc_excel
 Author: Pengcheng Song
 Author-email: smth_spc@hotmail.com
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Scientific/Engineering :: Mathematics
@@ -36,14 +36,17 @@
 wb.set_hl_col_by_names('col_name2', 'sheet_name', 'background_color2', 'color2')
 #write dataframe to xlsx file
 wb.write_data('sheet_name')
 
 #hide cols
 wb.hide_col(5,12,'sheet_name')
 
+#collapse cols (have a + on top)
+wb.collapse_col(5,12,'sheet_name')
+
 #freeze cell
 wb.freeze(1,4, 'sheet_name')
 
 #set hightlight columns for another sheet
 #default background color is yellow
 wb.load_data(df2)
 wb.set_hl_col_by_names('col_name', 'another_sheet_name')
```

### Comparing `cicc_excel-0.1.0/setup.py` & `cicc_excel-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cicc_excel",
-    version="0.1.0",
+    version="0.2.0",
     author="Pengcheng Song",
     author_email="smth_spc@hotmail.com",
     description="Library of export pandas into excel for CICCers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nyuspc/cicc_excel",
     install_requires=[
```

