# Comparing `tmp/finlogic-0.4.5.tar.gz` & `tmp/finlogic-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finlogic-0.4.5.tar", last modified: Sun May 21 14:28:01 2023, max compression
+gzip compressed data, was "finlogic-0.4.6.tar", last modified: Mon May 22 11:24:22 2023, max compression
```

## Comparing `finlogic-0.4.5.tar` & `finlogic-0.4.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.5/LICENSE
--rw-r--r--   0        0        0     9611 2023-05-15 08:41:19.853254 finlogic-0.4.5/README.md
--rw-r--r--   0        0        0      423 2023-05-19 08:15:00.845332 finlogic-0.4.5/finlogic/__init__.py
--rw-r--r--   0        0        0    24331 2023-05-21 14:25:13.096740 finlogic-0.4.5/finlogic/company.py
--rw-r--r--   0        0        0      316 2023-05-14 15:04:47.182513 finlogic-0.4.5/finlogic/config.py
--rw-r--r--   0        0        0    10641 2023-05-21 14:25:13.096740 finlogic-0.4.5/finlogic/cvm.py
--rw-r--r--   0        0        0     4460 2023-05-17 10:44:29.881677 finlogic-0.4.5/finlogic/database.py
--rw-r--r--   0        0        0     3140 2023-05-21 14:25:13.096740 finlogic-0.4.5/finlogic/fduckdb.py
--rw-r--r--   0        0        0      961 2023-05-12 00:21:10.028393 finlogic-0.4.5/finlogic/fprint.py
--rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.4.5/finlogic/language.py
--rw-r--r--   0        0        0     1014 2023-05-21 14:28:01.503322 finlogic-0.4.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.5/tests/__init__.py
--rw-r--r--   0        0        0     3345 2023-05-21 14:25:13.096740 finlogic-0.4.5/tests/test_company.py
--rw-r--r--   0        0        0      900 2023-05-21 14:25:13.096740 finlogic-0.4.5/tests/test_database.py
--rw-r--r--   0        0        0    11687 1970-01-01 00:00:00.000000 finlogic-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-03-19 09:29:48.277335 finlogic-0.4.6/LICENSE
+-rw-r--r--   0        0        0     9611 2023-05-15 08:41:19.853254 finlogic-0.4.6/README.md
+-rw-r--r--   0        0        0      423 2023-05-22 09:28:18.165139 finlogic-0.4.6/finlogic/__init__.py
+-rw-r--r--   0        0        0    23964 2023-05-22 09:26:43.340205 finlogic-0.4.6/finlogic/company.py
+-rw-r--r--   0        0        0      316 2023-05-14 15:04:47.182513 finlogic-0.4.6/finlogic/config.py
+-rw-r--r--   0        0        0    11456 2023-05-22 09:16:26.215128 finlogic-0.4.6/finlogic/cvm.py
+-rw-r--r--   0        0        0     4637 2023-05-22 07:18:09.637242 finlogic-0.4.6/finlogic/database.py
+-rw-r--r--   0        0        0     2987 2023-05-22 11:17:06.704713 finlogic-0.4.6/finlogic/fduckdb.py
+-rw-r--r--   0        0        0      961 2023-05-12 00:21:10.028393 finlogic-0.4.6/finlogic/fprint.py
+-rw-r--r--   0        0        0      688 2023-05-14 15:12:41.688062 finlogic-0.4.6/finlogic/language.py
+-rw-r--r--   0        0        0     1014 2023-05-22 11:24:22.961533 finlogic-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-19 09:29:48.278335 finlogic-0.4.6/tests/__init__.py
+-rw-r--r--   0        0        0     3345 2023-05-21 14:25:13.096740 finlogic-0.4.6/tests/test_company.py
+-rw-r--r--   0        0        0      900 2023-05-22 09:30:35.054487 finlogic-0.4.6/tests/test_database.py
+-rw-r--r--   0        0        0    11687 1970-01-01 00:00:00.000000 finlogic-0.4.6/PKG-INFO
```

### Comparing `finlogic-0.4.5/LICENSE` & `finlogic-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.5/README.md` & `finlogic-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.5/finlogic/company.py` & `finlogic-0.4.6/finlogic/company.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,21 +261,25 @@
             SELECT *
               FROM reports
              WHERE cvm_id = {self._cvm_id}
                AND acc_method = '{self._acc_method}'
              ORDER BY 
                 acc_code,
                 period_reference,
-                acc_fixed,
                 report_type,
                 period_begin,
                 period_end
         """
         df = execute(query, "df")
 
+        # Convert category columns back to string
+        columns = df.columns
+        cat_cols = [c for c in columns if df[c].dtype == "category"]
+        df[cat_cols] = df[cat_cols].astype("string")
+
         # Change acc_unit only for accounts different from 3.99
         df["acc_value"] = np.where(
             df["acc_code"].str.startswith("3.99"),
             df["acc_value"],
             df["acc_value"] / self._acc_unit,
         )
         annual_df = df.query('report_type == "ANNUAL"')
@@ -290,34 +294,15 @@
         df.query(
             'report_type == "ANNUAL" or \
              period_reference == @self._last_period',
             inplace=True,
         )
 
         # Drop columns that are already company attributes or will not be used
-        df.drop(
-            columns=[
-                "name_id",
-                "cvm_id",
-                "tax_id",
-                "acc_method",
-                "file_source",
-                "file_mtime",
-            ],
-            inplace=True,
-        )
-
-        # Keep only the last value for the same account code and period (begin and end)
-        # The dataframe was already sorted by the SQL query.
-        cols = [
-            "acc_code",
-            "period_begin",
-            "period_end",
-        ]
-        df.drop_duplicates(subset=cols, keep="last", inplace=True, ignore_index=True)
+        df.drop(columns=["name_id", "cvm_id", "tax_id", "acc_method"], inplace=True)
 
         # Set company data frame
         self._df = df
 
     def info(self) -> dict:
         """Print a concise summary of a company."""
         # Some companies have no quarterly reports (see cvm_id 9784)
@@ -340,16 +325,16 @@
         }
         print_dict(info_dict=company_info, table_name="Company Info")
 
     def _build_report_index(self, dfi: pd.DataFrame) -> pd.DataFrame:
         """Build the index for the report."""
         # "acc_code" works as a primary key. Other columns set the preference order
         df = (
-            dfi[["acc_code", "acc_fixed", "acc_name", "period_reference"]]
-            .sort_values(by=["acc_code", "acc_fixed", "period_reference"])
+            dfi[["acc_code", "acc_name", "period_reference"]]
+            .sort_values(by=["acc_code", "period_reference"])
             .drop_duplicates(subset=["acc_code"], keep="last", ignore_index=True)[
                 ["acc_code", "acc_name"]
             ]
         )
         return df
 
     def _build_report(self, dfi: pd.DataFrame) -> pd.DataFrame:
```

### Comparing `finlogic-0.4.5/finlogic/cvm.py` & `finlogic-0.4.6/finlogic/cvm.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Module to download and process CVM data."""
 import re
 from typing import List
 import zipfile as zf
 from pathlib import Path
-import duckdb
 import pandas as pd
 import requests
 from . import config as cfg
 
 URL_DFP = "https://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/DFP/DADOS/"
 URL_ITR = "https://dados.cvm.gov.br/dados/CIA_ABERTA/DOC/ITR/DADOS/"
 
@@ -138,40 +137,45 @@
 
     # Remove rows with acc_value == 0 and acc_fixed == False
     # df.query("acc_value != 0 or acc_fixed == True", inplace=True)
     df.query("acc_value != 0", inplace=True)
 
     # acc_fixed is being used used only non fixed accounts with acc_value == 0
     # So it can be dropped after the query above.
-    # df = df.drop(columns=["acc_fixed"])
+    df = df.drop(columns=["acc_fixed"])
 
     # cvm_id max. value is 600_000, so it can be uint32 (0 to 4_294_967_295)
     df["cvm_id"] = df["cvm_id"].astype("uint32")
 
     # There are two types of CVM files: DFP (ANNUAL) and ITR (QUARTERLY).
     # In database, "report_type" is positioned after "tax_id" -> position = 3
     if filepath.name.startswith("dfp"):
         df.insert(loc=3, column="report_type", value="ANNUAL")
     else:
         df.insert(loc=3, column="report_type", value="QUARTERLY")
 
     # For the moment, es_name will not be used since it adds to much complexity to
     # the database. It will be dropped.
     df = df.drop(columns=["es_name"])
+
     # Remove any extra spaces (line breaks, tabs, etc.) from columns below.
-    # columns = ["name_id", "acc_name", "es_name"]
-    # df[columns] = df[columns].apply(remove_empty_spaces)
+    columns = ["name_id", "acc_name"]
+    df[columns] = df[columns].apply(remove_empty_spaces)
 
     # Replace "BCO " with "BANCO " in "name_id" column.
     df["name_id"] = df["name_id"].str.replace("BCO ", "BANCO ")
 
     # Convert string columns to categorical before mapping.
     columns = df.select_dtypes(include="object").columns
     df[columns] = df[columns].astype("category")
 
+    # Convert datetime columns
+    columns = ["period_reference", "period_begin", "period_end"]
+    df[columns] = df[columns].apply(pd.to_datetime)
+
     # currency_unit values are ['MIL', 'UNIDADE']
     map_dic = {"UNIDADE": 1, "MIL": 1000}
     df["currency_unit"] = df["currency_unit"].map(map_dic).astype(int)
 
     # Do not ajust acc_value for 3.99 codes.
     df["acc_value"] = df["acc_value"].where(
         df["acc_code"].str.startswith("3.99"),
@@ -227,42 +231,66 @@
     # In "itr_cia_aberta_2022.zip", as an example, 2742 rows are duplicated.
     # Few of them have different values in "acc_value". Only one them will be kept.
     # REMOVE ALL VALUES OR MARK THESE ROWS AS ERRORS?
     cols = df.columns.tolist()
     cols.remove("acc_value")
     df.drop_duplicates(subset=cols, keep="last", inplace=True, ignore_index=True)
 
-    # Add column for file source and file modification time.
-    df["file_source"] = filepath.name
-    df["file_mtime"] = filepath.stat().st_mtime
-
     return df
 
 
-def save_processed_df(df: pd.DataFrame, filepath: Path) -> None:
-    """Save a processed dataframe as a csv file."""
-    with duckdb.connect() as con:
-        sql = f"""
-            CREATE TEMP TABLE tbl AS SELECT * FROM df;
-            ALTER TABLE tbl ALTER period_reference TYPE DATE;
-            ALTER TABLE tbl ALTER period_begin TYPE DATE;
-            ALTER TABLE tbl ALTER period_end TYPE DATE;
-            COPY tbl TO '{filepath}' (FORMAT 'PARQUET', COMPRESSION 'zstd')
-        """
-        con.execute(sql)
-
-
 def process_file(raw_filepath: Path) -> Path:
     """Read, process and save a CVM file."""
     df = read_raw_file(raw_filepath)
     df = process_df(df, raw_filepath)
-    processed_filepath = cfg.CVM_PROCESSED_DIR / (raw_filepath.stem + ".parquet")
-    save_processed_df(df, processed_filepath)
+    processed_filepath = cfg.CVM_PROCESSED_DIR / (raw_filepath.stem + ".pickle")
+    # save_processed_df(df, processed_filepath)
+    df.to_pickle(processed_filepath, compression="zstd")
     print(f"    {CHECKMARK} {raw_filepath.name} processed.")
     return processed_filepath
 
 
 def get_raw_file_mtimes() -> pd.DataFrame:
     """Return a Pandas DataFrame with file_source and file_mtime columns."""
     filepaths = sorted(cfg.CVM_RAW_DIR.glob("*.zip"))
     d_mtimes = {filepath.name: filepath.stat().st_mtime for filepath in filepaths}
     return pd.DataFrame(d_mtimes.items(), columns=["file_source", "file_mtime"])
+
+
+def read_all_processed_files() -> pd.DataFrame:
+    """Read all processed CVM files."""
+    # list filepaths in processed folder
+    filepaths = sorted(cfg.CVM_PROCESSED_DIR.glob("*.pickle"))
+    df = pd.concat([pd.read_pickle(f, compression="zstd") for f in filepaths])
+    columns = df.columns
+    cat_cols = [c for c in columns if df[c].dtype in ["object", "datetime64[ns]"]]
+    df[cat_cols] = df[cat_cols].astype("category")
+    return df
+
+
+def drop_duplicates(df: pd.DataFrame) -> pd.DataFrame:
+    """Drop duplicates from a before building database
+    Because PREVIOUS value == LAST value for the year before, we can keep only
+    the most recent values by dropping duplicates. By doing this, we guarantee
+    that there is only one valid accounting value in database -> the last one
+    """
+    sort_cols = [
+        "cvm_id",
+        "acc_method",
+        "acc_code",
+        "period_reference",
+        "report_type",
+        "period_begin",
+        "period_end",
+    ]
+    df.sort_values(by=sort_cols, ascending=True, inplace=True, ignore_index=True)
+
+    subset_cols = [
+        "cvm_id",
+        "acc_method",
+        "acc_code",
+        "period_begin",
+        "period_end",
+    ]
+    df.drop_duplicates(subset=subset_cols, keep="last", inplace=True, ignore_index=True)
+
+    return df
```

### Comparing `finlogic-0.4.5/finlogic/database.py` & `finlogic-0.4.6/finlogic/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 """Finlogic Database module.
 
 This module provides functions to handle financial data from the CVM Portal. It
 allows updating, processing and consolidating financial statements, as well as
 searching for company names in the FinLogic Database and retrieving information
 about the database itself.
 """
+from pathlib import Path
 from typing import Literal
 import pandas as pd
 from . import cvm
 from . import config as cfg
 from . import language as lng
 from . import fprint as fpr
 from . import fduckdb as fdb
 
 CHECKMARK = "\033[32m\u2714\033[0m"
 
 
-def get_filepaths_to_process() -> list[str]:
+def get_filepaths_to_process(df1: pd.DataFrame, df2: pd.DataFrame) -> list[Path]:
     """Return a list of CVM files that has to be processed by comparing
-    the files mtimes from the raw folder with the database.
+    the files mtimes from the raw folder.
     """
-    df_raw = cvm.get_raw_file_mtimes()
-    df_fdb = fdb.get_file_mtimes()
-    df_new = pd.concat([df_raw, df_fdb]).drop_duplicates(keep=False)
-    file_sources = sorted(df_new["file_source"].drop_duplicates())
+    df = pd.concat([df1, df2]).drop_duplicates(keep=False)
+    file_sources = sorted(df["file_source"].drop_duplicates())
     return [cfg.CVM_RAW_DIR / file_source for file_source in file_sources]
 
 
 def update_database(rebuild: bool = False):
     """Verify changes in CVM files and update Finlogic Database if necessary.
 
     Args:
@@ -38,26 +37,30 @@
     """
     # Language files
     print('\nUpdating "language" database...')
     lng.process_language_df()
 
     # CVM raw files
     print("Updating CVM files...")
+    # Get files mtimes from the raw folder before updating
+    df_raw1 = cvm.get_raw_file_mtimes()
     urls = cvm.get_all_file_urls()
     updated_raw_filepaths = cvm.update_raw_files(urls)
     print(f"Number of CVM files updated = {len(updated_raw_filepaths)}")
+    # Get files mtimes from the raw folder after updating
+    df_raw2 = cvm.get_raw_file_mtimes()
 
     # CVM processed files
     print("\nProcessing CVM files...")
     if rebuild:
         # Process all files
         filepaths_to_process = sorted(cfg.CVM_RAW_DIR.glob("*.zip"))
     else:
         # Process only updated files
-        filepaths_to_process = get_filepaths_to_process()
+        filepaths_to_process = get_filepaths_to_process(df1=df_raw1, df2=df_raw2)
     print(f"Number of new files to process = {len(filepaths_to_process)}")
     if filepaths_to_process:
         [cvm.process_file(filepath) for filepath in filepaths_to_process]
 
     # FinLogic Database
     fdb.build()
     print(f"\n{CHECKMARK} FinLogic Database updated!")
```

### Comparing `finlogic-0.4.5/finlogic/fduckdb.py` & `finlogic-0.4.6/finlogic/fduckdb.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """FinLogic Database module."""
 from typing import Literal
 import duckdb
 import pandas as pd
 from datetime import datetime
 from . import config as cfg
+from . import cvm
 
 # Start FinLogic Database connection
 FINLOGIC_DB_PATH = cfg.DATA_PATH / "finlogic.db"
 # Create a new database file and connect to it
 con = duckdb.connect(database=f"{FINLOGIC_DB_PATH}")
 con.close()
 
@@ -36,59 +37,56 @@
 
 
 def build():
     """Build FinLogic Database from processed CVM files."""
     print("Building FinLogic Database...")
     # Reset database
     reset()
+    df = cvm.read_all_processed_files()
+    df = cvm.drop_duplicates(df)
     # Create a table with all processed CVM files
-    sql = f"""
-        CREATE TABLE reports AS SELECT * FROM '{cfg.CVM_PROCESSED_DIR}/*.parquet'
-    """
-    execute(sql)
+    execute("CREATE TABLE reports AS SELECT * FROM df")
 
 
 def is_empty() -> bool:
     """Return True if database is considered empty."""
     return FINLOGIC_DB_PATH.stat().st_size / 1024**2 < 10
 
 
 def get_info() -> dict:
     """Return a dictionary with information about the database."""
-    info_dict = {}
+    info = {}
     if is_empty():
-        return info_dict
+        return info
+
+    info["db_path"] = f"{FINLOGIC_DB_PATH}"
+    info["db_size"] = f"{FINLOGIC_DB_PATH.stat().st_size / 1024**2:.2f} MB"
+
+    db_last_modified = datetime.fromtimestamp(FINLOGIC_DB_PATH.stat().st_mtime)
+    info["db_last_modified"] = db_last_modified.strftime("%Y-%m-%d %H:%M:%S")
+
+    query = "SELECT COUNT(*) FROM reports"
+    info["number_of_rows"] = execute(query, "fetchone")[0]
 
     query = """--sql
         SELECT DISTINCT cvm_id, report_type, period_reference
           FROM reports;
     """
-    num_of_reports = execute(query, "df").shape[0]
-    db_last_modified = datetime.fromtimestamp(FINLOGIC_DB_PATH.stat().st_mtime)
-    query = "SELECT COUNT(*) FROM reports"
-    number_of_rows = execute(query, "fetchone")[0]
-    query = "SELECT MIN(period_end) FROM reports"
-    first_statement = execute(query, "fetchone")[0]
-    query = "SELECT MAX(period_end) FROM reports"
-    last_statement = execute(query, "fetchone")[0]
+    info["number_of_reports"] = execute(query, "df").shape[0]
+
     query = "SELECT COUNT(DISTINCT cvm_id) FROM reports"
-    number_of_companies = execute(query, "fetchone")[0]
+    info["number_of_companies"] = execute(query, "fetchone")[0]
 
-    info_dict = {
-        "db_path": f"{FINLOGIC_DB_PATH}",
-        "db_size": f"{FINLOGIC_DB_PATH.stat().st_size / 1024**2:.2f} MB",
-        "db_last_modified": db_last_modified.strftime("%Y-%m-%d %H:%M:%S"),
-        "number_of_rows": number_of_rows,
-        "number_of_reports": num_of_reports,
-        "number_of_companies": number_of_companies,
-        "first_report": f"{first_statement}",
-        "last_report": f"{last_statement}",
-    }
+    query = "SELECT MIN(period_end) FROM reports"
+    info["first_report"] = execute(query, "fetchone")[0].strftime("%Y-%m-%d")
+
+    query = "SELECT MAX(period_end) FROM reports"
+    info["last_report"] = execute(query, "fetchone")[0].strftime("%Y-%m-%d")
 
-    return info_dict
+    return info
 
 
 def get_file_mtimes() -> pd.DataFrame:
     """Return a Pandas DataFrame with unique file_source and file_mtime."""
     if is_empty():
         return pd.DataFrame()
```

### Comparing `finlogic-0.4.5/finlogic/fprint.py` & `finlogic-0.4.6/finlogic/fprint.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.5/finlogic/language.py` & `finlogic-0.4.6/finlogic/language.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.5/pyproject.toml` & `finlogic-0.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 ]
 dependencies = [
     "pandas>=1.4.0",
     "requests>=2.27.0",
     "duckdb>=0.7.0",
     "rich>=13.0.0",
 ]
-version = "0.4.5"
+version = "0.4.6"
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 dev = [
     "pytest",
```

### Comparing `finlogic-0.4.5/tests/test_company.py` & `finlogic-0.4.6/tests/test_company.py`

 * *Files identical despite different names*

### Comparing `finlogic-0.4.5/tests/test_database.py` & `finlogic-0.4.6/tests/test_database.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class TestDatabase(unittest.TestCase):
     def test_info(self):
         """Test the info method of the Database module."""
         db_info = fdb.get_info()
         self.assertEqual(db_info["first_report"], "2009-01-31")
-        self.assertTrue(db_info["number_of_rows"] > 7_000_000)
+        self.assertTrue(db_info["number_of_rows"] > 4_000_000)
 
     def test_search_company(self):
         """Test the search_company method of the Database module."""
         search_result = fl.search_company("petrobras")
         """
             name_id                            cvm_id  tax_id
         0   PETROBRAS DISTRIBUIDORA S/A         24295  34.274.233/0001-02
```

### Comparing `finlogic-0.4.5/PKG-INFO` & `finlogic-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finlogic
-Version: 0.4.5
+Version: 0.4.6
 Summary: Finance toolkit for listed Brazilian companies
 Keywords: pandas, cvm, finance, investment, accounting
 Author-Email: Carlos Carvalho <cr.cj@outlook.com>
 License: MIT License
         
         Copyright (c) 2022 Carlos Carvalho
```

