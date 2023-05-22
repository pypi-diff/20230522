# Comparing `tmp/finlogic-0.4.6.tar.gz` & `tmp/finlogic-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlogic-0.4.6.tar", last modified: Mon May 22 11:24:22 2023, max compression
+gzip compressed data, was "finlogic-0.4.7.tar", last modified: Mon May 22 11:46:10 2023, max compression
```

## Comparing `finlogic-0.4.6.tar` & `finlogic-0.4.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.6/LICENSE
--rw-r--r--   0        0        0     9611 2023-05-15 08:41:19.853254 finlogic-0.4.6/README.md
--rw-r--r--   0        0        0      423 2023-05-22 09:28:18.165139 finlogic-0.4.6/finlogic/__init__.py
--rw-r--r--   0        0        0    23964 2023-05-22 09:26:43.340205 finlogic-0.4.6/finlogic/company.py
--rw-r--r--   0        0        0      316 2023-05-14 15:04:47.182513 finlogic-0.4.6/finlogic/config.py
--rw-r--r--   0        0        0    11456 2023-05-22 09:16:26.215128 finlogic-0.4.6/finlogic/cvm.py
--rw-r--r--   0        0        0     4637 2023-05-22 07:18:09.637242 finlogic-0.4.6/finlogic/database.py
--rw-r--r--   0        0        0     2987 2023-05-22 11:17:06.704713 finlogic-0.4.6/finlogic/fduckdb.py
--rw-r--r--   0        0        0      961 2023-05-12 00:21:10.028393 finlogic-0.4.6/finlogic/fprint.py
--rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.4.6/finlogic/language.py
--rw-r--r--   0        0        0     1014 2023-05-22 11:24:22.961533 finlogic-0.4.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.6/tests/__init__.py
--rw-r--r--   0        0        0     3345 2023-05-21 14:25:13.096740 finlogic-0.4.6/tests/test_company.py
--rw-r--r--   0        0        0      900 2023-05-22 09:30:35.054487 finlogic-0.4.6/tests/test_database.py
--rw-r--r--   0        0        0    11687 1970-01-01 00:00:00.000000 finlogic-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.7/LICENSE
+-rw-r--r--   0        0        0     9216 2023-05-22 11:45:26.558019 finlogic-0.4.7/README.md
+-rw-r--r--   0        0        0      423 2023-05-22 11:32:57.010081 finlogic-0.4.7/finlogic/__init__.py
+-rw-r--r--   0        0        0    23964 2023-05-22 11:25:57.286389 finlogic-0.4.7/finlogic/company.py
+-rw-r--r--   0        0        0      316 2023-05-14 15:04:47.182513 finlogic-0.4.7/finlogic/config.py
+-rw-r--r--   0        0        0    11456 2023-05-22 11:25:57.286389 finlogic-0.4.7/finlogic/cvm.py
+-rw-r--r--   0        0        0     4637 2023-05-22 11:25:57.286389 finlogic-0.4.7/finlogic/database.py
+-rw-r--r--   0        0        0     2987 2023-05-22 11:25:57.286389 finlogic-0.4.7/finlogic/fduckdb.py
+-rw-r--r--   0        0        0      961 2023-05-12 00:21:10.028393 finlogic-0.4.7/finlogic/fprint.py
+-rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.4.7/finlogic/language.py
+-rw-r--r--   0        0        0     1039 2023-05-22 11:46:10.598431 finlogic-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.7/tests/__init__.py
+-rw-r--r--   0        0        0     3345 2023-05-21 14:25:13.096740 finlogic-0.4.7/tests/test_company.py
+-rw-r--r--   0        0        0      900 2023-05-22 11:25:57.287389 finlogic-0.4.7/tests/test_database.py
+-rw-r--r--   0        0        0    11325 1970-01-01 00:00:00.000000 finlogic-0.4.7/PKG-INFO
```

### Comparing `finlogic-0.4.6/LICENSE` & `finlogic-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.6/README.md` & `finlogic-0.4.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -24,18 +24,19 @@
 # PyPI:
 pip install finlogic
 ```
 
 ### Requirements
 
 - [Python](https://www.python.org) \>= 3.10
-- [DuckDB](https://github.com/pydata/pandas) \>= 0.7.0
-- [Pandas](https://github.com/pydata/pandas) \>= 1.4.0
-- [Requests](http://docs.python-requests.org/en/master/) \>= 2.27.0
+- [DuckDB](https://github.com/pydata/pandas) \>= 0.8.0
+- [Pandas](https://github.com/pydata/pandas) \>= 1.5.0
+- [Requests](http://docs.python-requests.org/en/master/) \>= 2.30.0
 - [Rich](https://github.com/Textualize/rich) \>= 13.0.0
+- [Zstandard](https://python-zstandard.readthedocs.io/en/latest/) \>= 0.21.0
 
 ---
 
 ## Quick Start
 
 ### Create FinLogic Database
 
@@ -51,58 +52,55 @@
 ...
 FinLogic database updated ✅
 
 # Show database info:
 >>> fl.database_info()
 ```
 
-| FinLogic Database Info      |                       Value |
-| :-------------------------- | --------------------------: |
-| Data path                   | /.../FinLogic/finlogic/data |
-| File size (MB)              |                       301.0 |
-| Last update call            |         2022-04-20 07:29:08 |
-| Last modified               |         2022-04-20 07:31:48 |
-| Last updated data           |         2022-04-17 13:09:01 |
-| Accounting rows             |                   8,757,249 |
-| Unique accounting codes     |                       2,008 |
-| Number of companies         |                       1,037 |
-| Unique Financial Statements |                      13,172 |
-| First Financial Statement   |                  2009-01-31 |
-| Last Financial Statement    |                  2023-03-31 |
+| FinLogic Database Info |                         Value |
+| :--------------------- | ----------------------------: |
+| db_path                | .../finlogic/data/finlogic.db |
+| db_size                |                      301.0 MB |
+| db_last_modified       |           2023-04-20 07:29:08 |
+| number_of_companies    |                         1,139 |
+| number_of_rows         |                     4,379,496 |
+| number_of_reports      |                        13,770 |
+| first_report           |                    2009-01-31 |
+| last_report            |                    2023-03-31 |
 
 ```python
 # Search for a company in database:
 >>> fl.search_company('petro')
 ```
 
-|     | name                                   |    id | fiscal_id          |
-| --: | :------------------------------------- | ----: | :----------------- |
-|   0 | 3R PETROLEUM ÓLEO E GÁS S.A.           | 25291 | 12.091.809/0001-55 |
-|   1 | PETRO RIO S.A.                         | 22187 | 10.629.105/0001-68 |
-|   2 | PETROBRAS DISTRIBUIDORA S/A            | 24295 | 34.274.233/0001-02 |
-|   3 | PETROLEO BRASILEIRO S.A. PETROBRAS     |  9512 | 33.000.167/0001-01 |
-|   4 | PETROLEO LUB DO NORDESTE SA            |  9520 | 07.275.159/0001-68 |
-|   5 | PETRORECÔNCAVO S.A.                    | 25780 | 03.342.704/0001-30 |
-|   6 | PRONOR PETROQUIMICA SA                 |  9784 | 13.552.070/0001-02 |
-|   7 | REFINARIA DE PETROLEOS MANGUINHOS S.A. |  9989 | 33.412.081/0001-96 |
+|     | name_id                                | cvm_id | tax_id             |
+| --: | :------------------------------------- | -----: | :----------------- |
+|   0 | 3R PETROLEUM ÓLEO E GÁS S.A.           |  25291 | 12.091.809/0001-55 |
+|   1 | PETRO RIO S.A.                         |  22187 | 10.629.105/0001-68 |
+|   2 | PETROBRAS DISTRIBUIDORA S/A            |  24295 | 34.274.233/0001-02 |
+|   3 | PETROLEO BRASILEIRO S.A. PETROBRAS     |   9512 | 33.000.167/0001-01 |
+|   4 | PETROLEO LUB DO NORDESTE SA            |   9520 | 07.275.159/0001-68 |
+|   5 | PETRORECÔNCAVO S.A.                    |  25780 | 03.342.704/0001-30 |
+|   6 | PRONOR PETROQUIMICA SA                 |   9784 | 13.552.070/0001-02 |
+|   7 | REFINARIA DE PETROLEOS MANGUINHOS S.A. |   9989 | 33.412.081/0001-96 |
 
 ### The Company Class
 
 The Company Class allows you to easily access financial data from Brazilian companies. All values are in local currency (Real).
 
 ```python
 # Create a Company object to acces its financial data:
 # Both CVM (regulator) ID or Fiscal ID can be used as an identifier.
->>> petro = fl.Company(9512, acc_method='separate', acc_unit='million')
+>>> petro = fl.Company(9512, acc_method='sep', acc_unit='m')
 
 # Change company accounting method back to consolidated (default):
->>> petro.acc_method = 'consolidated'
+>>> petro.acc_method = 'con'
 
 # Change company accounting unit to billion (default is 1):
->>> petro.acc_unit = 'billion'
+>>> petro.acc_unit = 'b'
 
 # Show company info:
 >>> petro.info()
 ```
 
 | Company Info               |                             Values |
 | :------------------------- | ---------------------------------: |
@@ -121,41 +119,41 @@
 # Show company assets in Brazilian currency:
 >>> petro.report(report_type='assets')
 ...
 # Show company liabilities with custom arguments:
 >>> petro.report(report_type='debt', acc_level=4, num_years=3)
 ```
 
-| acc_code   | acc_name            | acc_fixed | 2020-12-31 | 2021-12-31 | 2022-12-31 |
-| :--------- | :------------------ | :-------- | ---------: | ---------: | ---------: |
-| 2.01.04    | Loans and Financing | True      |     51.364 |     50.631 |      47.65 |
-| 2.01.04.01 | Loans and Financing | True      |     21.751 |     20.316 |     18.656 |
-| 2.01.04.02 | Debentures          | True      |          0 |          0 |          0 |
-| 2.01.04.03 | Lease Financing     | True      |     29.613 |     30.315 |     28.994 |
-| 2.02.01    | Loans and Financing | True      |    341.184 |    277.187 |    233.053 |
-| 2.02.01.01 | Loans and Financing | True      |    258.287 |    178.908 |     137.63 |
-| 2.02.01.02 | Debentures          | True      |          0 |          0 |          0 |
-| 2.02.01.03 | Lease Financing     | True      |     82.897 |     98.279 |     95.423 |
+| acc_code   | acc_name            | 2020-12-31 | 2021-12-31 | 2022-12-31 |
+| :--------- | :------------------ | ---------: | ---------: | ---------: |
+| 2.01.04    | Loans and Financing |     51.364 |     50.631 |      47.65 |
+| 2.01.04.01 | Loans and Financing |     21.751 |     20.316 |     18.656 |
+| 2.01.04.02 | Debentures          |          0 |          0 |          0 |
+| 2.01.04.03 | Lease Financing     |     29.613 |     30.315 |     28.994 |
+| 2.02.01    | Loans and Financing |    341.184 |    277.187 |    233.053 |
+| 2.02.01.01 | Loans and Financing |    258.287 |    178.908 |     137.63 |
+| 2.02.01.02 | Debentures          |          0 |          0 |          0 |
+| 2.02.01.03 | Lease Financing     |     82.897 |     98.279 |     95.423 |
 
 ```python
 # Change account names to Portuguese:
 >>> petro.language = "portuguese"
 >>> petro.report(report_type='debt', acc_level=4, num_years=3)
 ```
 
-| acc_code   | acc_name                       | acc_fixed | 2020-12-31 | 2021-12-31 | 2022-12-31 |
-| ---------- | ------------------------------ | --------- | ---------: | ---------: | ---------: |
-| 2.01.04    | Empréstimos e Financiamentos   | True      |     51.364 |     50.631 |      47.65 |
-| 2.01.04.01 | Empréstimos e Financiamentos   | True      |     21.751 |     20.316 |     18.656 |
-| 2.01.04.02 | Debêntures                     | True      |          0 |          0 |          0 |
-| 2.01.04.03 | Financiamento por Arrendamento | True      |     29.613 |     30.315 |     28.994 |
-| 2.02.01    | Empréstimos e Financiamentos   | True      |    341.184 |    277.187 |    233.053 |
-| 2.02.01.01 | Empréstimos e Financiamentos   | True      |    258.287 |    178.908 |     137.63 |
-| 2.02.01.02 | Debêntures                     | True      |          0 |          0 |          0 |
-| 2.02.01.03 | Financiamento por Arrendamento | True      |     82.897 |     98.279 |     95.423 |
+| acc_code   | acc_name                       | 2020-12-31 | 2021-12-31 | 2022-12-31 |
+| ---------- | ------------------------------ | ---------: | ---------: | ---------: |
+| 2.01.04    | Empréstimos e Financiamentos   |     51.364 |     50.631 |      47.65 |
+| 2.01.04.01 | Empréstimos e Financiamentos   |     21.751 |     20.316 |     18.656 |
+| 2.01.04.02 | Debêntures                     |          0 |          0 |          0 |
+| 2.01.04.03 | Financiamento por Arrendamento |     29.613 |     30.315 |     28.994 |
+| 2.02.01    | Empréstimos e Financiamentos   |    341.184 |    277.187 |    233.053 |
+| 2.02.01.01 | Empréstimos e Financiamentos   |    258.287 |    178.908 |     137.63 |
+| 2.02.01.02 | Debêntures                     |          0 |          0 |          0 |
+| 2.02.01.03 | Financiamento por Arrendamento |     82.897 |     98.279 |     95.423 |
 
 ```python
 # Show company main indicators:
 >>> petro.indicators(num_years=3)
 ```
 
 | Company Financial Indicators | 2019-12-31 | 2020-12-31 | 2021-12-31 |
```

### Comparing `finlogic-0.4.6/finlogic/company.py` & `finlogic-0.4.7/finlogic/company.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.6/finlogic/cvm.py` & `finlogic-0.4.7/finlogic/cvm.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.6/finlogic/database.py` & `finlogic-0.4.7/finlogic/database.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.6/finlogic/fduckdb.py` & `finlogic-0.4.7/finlogic/fduckdb.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.6/finlogic/fprint.py` & `finlogic-0.4.7/finlogic/fprint.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.6/finlogic/language.py` & `finlogic-0.4.7/finlogic/language.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.6/pyproject.toml` & `finlogic-0.4.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -20,20 +20,21 @@
     "Topic :: Office/Business :: Financial :: Accounting",
     "Topic :: Office/Business :: Financial :: Investment",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
-    "pandas>=1.4.0",
-    "requests>=2.27.0",
-    "duckdb>=0.7.0",
+    "pandas>=1.5.0",
+    "requests>=2.30.0",
+    "duckdb>=0.8.0",
     "rich>=13.0.0",
+    "zstandard>=0.21.0",
 ]
-version = "0.4.6"
+version = "0.4.7"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
```

### Comparing `finlogic-0.4.6/tests/test_company.py` & `finlogic-0.4.7/tests/test_company.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.6/tests/test_database.py` & `finlogic-0.4.7/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.6/PKG-INFO` & `finlogic-0.4.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finlogic
-Version: 0.4.6
+Version: 0.4.7
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Carlos Carvalho
         
@@ -28,18 +28,19 @@
 Classifier: Topic :: Office/Business :: Financial :: Accounting
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Project-URL: Repository, https://github.com/crdcj/FinLogic
 Requires-Python: >=3.10
-Requires-Dist: pandas>=1.4.0
-Requires-Dist: requests>=2.27.0
-Requires-Dist: duckdb>=0.7.0
+Requires-Dist: pandas>=1.5.0
+Requires-Dist: requests>=2.30.0
+Requires-Dist: duckdb>=0.8.0
 Requires-Dist: rich>=13.0.0
+Requires-Dist: zstandard>=0.21.0
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ipykernel; extra == "dev"
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://img.shields.io/pypi/v/finlogic.svg)](https://pypi.python.org/pypi/finlogic)
 [![Made with Python](https://img.shields.io/badge/Python->=3.10-blue?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
@@ -67,18 +68,19 @@
 # PyPI:
 pip install finlogic
 ```
 
 ### Requirements
 
 - [Python](https://www.python.org) \>= 3.10
-- [DuckDB](https://github.com/pydata/pandas) \>= 0.7.0
-- [Pandas](https://github.com/pydata/pandas) \>= 1.4.0
-- [Requests](http://docs.python-requests.org/en/master/) \>= 2.27.0
+- [DuckDB](https://github.com/pydata/pandas) \>= 0.8.0
+- [Pandas](https://github.com/pydata/pandas) \>= 1.5.0
+- [Requests](http://docs.python-requests.org/en/master/) \>= 2.30.0
 - [Rich](https://github.com/Textualize/rich) \>= 13.0.0
+- [Zstandard](https://python-zstandard.readthedocs.io/en/latest/) \>= 0.21.0
 
 ---
 
 ## Quick Start
 
 ### Create FinLogic Database
 
@@ -94,58 +96,55 @@
 ...
 FinLogic database updated ✅
 
 # Show database info:
 >>> fl.database_info()
 ```
 
-| FinLogic Database Info      |                       Value |
-| :-------------------------- | --------------------------: |
-| Data path                   | /.../FinLogic/finlogic/data |
-| File size (MB)              |                       301.0 |
-| Last update call            |         2022-04-20 07:29:08 |
-| Last modified               |         2022-04-20 07:31:48 |
-| Last updated data           |         2022-04-17 13:09:01 |
-| Accounting rows             |                   8,757,249 |
-| Unique accounting codes     |                       2,008 |
-| Number of companies         |                       1,037 |
-| Unique Financial Statements |                      13,172 |
-| First Financial Statement   |                  2009-01-31 |
-| Last Financial Statement    |                  2023-03-31 |
+| FinLogic Database Info |                         Value |
+| :--------------------- | ----------------------------: |
+| db_path                | .../finlogic/data/finlogic.db |
+| db_size                |                      301.0 MB |
+| db_last_modified       |           2023-04-20 07:29:08 |
+| number_of_companies    |                         1,139 |
+| number_of_rows         |                     4,379,496 |
+| number_of_reports      |                        13,770 |
+| first_report           |                    2009-01-31 |
+| last_report            |                    2023-03-31 |
 
 ```python
 # Search for a company in database:
 >>> fl.search_company('petro')
 ```
 
-|     | name                                   |    id | fiscal_id          |
-| --: | :------------------------------------- | ----: | :----------------- |
-|   0 | 3R PETROLEUM ÓLEO E GÁS S.A.           | 25291 | 12.091.809/0001-55 |
-|   1 | PETRO RIO S.A.                         | 22187 | 10.629.105/0001-68 |
-|   2 | PETROBRAS DISTRIBUIDORA S/A            | 24295 | 34.274.233/0001-02 |
-|   3 | PETROLEO BRASILEIRO S.A. PETROBRAS     |  9512 | 33.000.167/0001-01 |
-|   4 | PETROLEO LUB DO NORDESTE SA            |  9520 | 07.275.159/0001-68 |
-|   5 | PETRORECÔNCAVO S.A.                    | 25780 | 03.342.704/0001-30 |
-|   6 | PRONOR PETROQUIMICA SA                 |  9784 | 13.552.070/0001-02 |
-|   7 | REFINARIA DE PETROLEOS MANGUINHOS S.A. |  9989 | 33.412.081/0001-96 |
+|     | name_id                                | cvm_id | tax_id             |
+| --: | :------------------------------------- | -----: | :----------------- |
+|   0 | 3R PETROLEUM ÓLEO E GÁS S.A.           |  25291 | 12.091.809/0001-55 |
+|   1 | PETRO RIO S.A.                         |  22187 | 10.629.105/0001-68 |
+|   2 | PETROBRAS DISTRIBUIDORA S/A            |  24295 | 34.274.233/0001-02 |
+|   3 | PETROLEO BRASILEIRO S.A. PETROBRAS     |   9512 | 33.000.167/0001-01 |
+|   4 | PETROLEO LUB DO NORDESTE SA            |   9520 | 07.275.159/0001-68 |
+|   5 | PETRORECÔNCAVO S.A.                    |  25780 | 03.342.704/0001-30 |
+|   6 | PRONOR PETROQUIMICA SA                 |   9784 | 13.552.070/0001-02 |
+|   7 | REFINARIA DE PETROLEOS MANGUINHOS S.A. |   9989 | 33.412.081/0001-96 |
 
 ### The Company Class
 
 The Company Class allows you to easily access financial data from Brazilian companies. All values are in local currency (Real).
 
 ```python
 # Create a Company object to acces its financial data:
 # Both CVM (regulator) ID or Fiscal ID can be used as an identifier.
->>> petro = fl.Company(9512, acc_method='separate', acc_unit='million')
+>>> petro = fl.Company(9512, acc_method='sep', acc_unit='m')
 
 # Change company accounting method back to consolidated (default):
->>> petro.acc_method = 'consolidated'
+>>> petro.acc_method = 'con'
 
 # Change company accounting unit to billion (default is 1):
->>> petro.acc_unit = 'billion'
+>>> petro.acc_unit = 'b'
 
 # Show company info:
 >>> petro.info()
 ```
 
 | Company Info               |                             Values |
 | :------------------------- | ---------------------------------: |
@@ -164,41 +163,41 @@
 # Show company assets in Brazilian currency:
 >>> petro.report(report_type='assets')
 ...
 # Show company liabilities with custom arguments:
 >>> petro.report(report_type='debt', acc_level=4, num_years=3)
 ```
 
-| acc_code   | acc_name            | acc_fixed | 2020-12-31 | 2021-12-31 | 2022-12-31 |
-| :--------- | :------------------ | :-------- | ---------: | ---------: | ---------: |
-| 2.01.04    | Loans and Financing | True      |     51.364 |     50.631 |      47.65 |
-| 2.01.04.01 | Loans and Financing | True      |     21.751 |     20.316 |     18.656 |
-| 2.01.04.02 | Debentures          | True      |          0 |          0 |          0 |
-| 2.01.04.03 | Lease Financing     | True      |     29.613 |     30.315 |     28.994 |
-| 2.02.01    | Loans and Financing | True      |    341.184 |    277.187 |    233.053 |
-| 2.02.01.01 | Loans and Financing | True      |    258.287 |    178.908 |     137.63 |
-| 2.02.01.02 | Debentures          | True      |          0 |          0 |          0 |
-| 2.02.01.03 | Lease Financing     | True      |     82.897 |     98.279 |     95.423 |
+| acc_code   | acc_name            | 2020-12-31 | 2021-12-31 | 2022-12-31 |
+| :--------- | :------------------ | ---------: | ---------: | ---------: |
+| 2.01.04    | Loans and Financing |     51.364 |     50.631 |      47.65 |
+| 2.01.04.01 | Loans and Financing |     21.751 |     20.316 |     18.656 |
+| 2.01.04.02 | Debentures          |          0 |          0 |          0 |
+| 2.01.04.03 | Lease Financing     |     29.613 |     30.315 |     28.994 |
+| 2.02.01    | Loans and Financing |    341.184 |    277.187 |    233.053 |
+| 2.02.01.01 | Loans and Financing |    258.287 |    178.908 |     137.63 |
+| 2.02.01.02 | Debentures          |          0 |          0 |          0 |
+| 2.02.01.03 | Lease Financing     |     82.897 |     98.279 |     95.423 |
 
 ```python
 # Change account names to Portuguese:
 >>> petro.language = "portuguese"
 >>> petro.report(report_type='debt', acc_level=4, num_years=3)
 ```
 
-| acc_code   | acc_name                       | acc_fixed | 2020-12-31 | 2021-12-31 | 2022-12-31 |
-| ---------- | ------------------------------ | --------- | ---------: | ---------: | ---------: |
-| 2.01.04    | Empréstimos e Financiamentos   | True      |     51.364 |     50.631 |      47.65 |
-| 2.01.04.01 | Empréstimos e Financiamentos   | True      |     21.751 |     20.316 |     18.656 |
-| 2.01.04.02 | Debêntures                     | True      |          0 |          0 |          0 |
-| 2.01.04.03 | Financiamento por Arrendamento | True      |     29.613 |     30.315 |     28.994 |
-| 2.02.01    | Empréstimos e Financiamentos   | True      |    341.184 |    277.187 |    233.053 |
-| 2.02.01.01 | Empréstimos e Financiamentos   | True      |    258.287 |    178.908 |     137.63 |
-| 2.02.01.02 | Debêntures                     | True      |          0 |          0 |          0 |
-| 2.02.01.03 | Financiamento por Arrendamento | True      |     82.897 |     98.279 |     95.423 |
+| acc_code   | acc_name                       | 2020-12-31 | 2021-12-31 | 2022-12-31 |
+| ---------- | ------------------------------ | ---------: | ---------: | ---------: |
+| 2.01.04    | Empréstimos e Financiamentos   |     51.364 |     50.631 |      47.65 |
+| 2.01.04.01 | Empréstimos e Financiamentos   |     21.751 |     20.316 |     18.656 |
+| 2.01.04.02 | Debêntures                     |          0 |          0 |          0 |
+| 2.01.04.03 | Financiamento por Arrendamento |     29.613 |     30.315 |     28.994 |
+| 2.02.01    | Empréstimos e Financiamentos   |    341.184 |    277.187 |    233.053 |
+| 2.02.01.01 | Empréstimos e Financiamentos   |    258.287 |    178.908 |     137.63 |
+| 2.02.01.02 | Debêntures                     |          0 |          0 |          0 |
+| 2.02.01.03 | Financiamento por Arrendamento |     82.897 |     98.279 |     95.423 |
 
 ```python
 # Show company main indicators:
 >>> petro.indicators(num_years=3)
 ```
 
 | Company Financial Indicators | 2019-12-31 | 2020-12-31 | 2021-12-31 |
```

