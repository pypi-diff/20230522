# Comparing `tmp/finary_uapi-0.1.1.tar.gz` & `tmp/finary_uapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finary_uapi-0.1.1.tar", max compression
+gzip compressed data, was "finary_uapi-0.1.2.tar", max compression
```

## Comparing `finary_uapi-0.1.1.tar` & `finary_uapi-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1064 2022-06-23 13:41:14.000000 finary_uapi-0.1.1/LICENSE
--rw-r--r--   0        0        0     5184 2023-05-22 20:32:05.637450 finary_uapi-0.1.1/README.md
--rw-r--r--   0        0        0      692 2023-05-22 20:27:22.472253 finary_uapi-0.1.1/finary_uapi/__init__.py
--rw-r--r--   0        0        0    16618 2023-05-22 20:29:53.501992 finary_uapi-0.1.1/finary_uapi/__main__.py
--rw-r--r--   0        0        0      323 2022-07-05 06:50:29.000000 finary_uapi-0.1.1/finary_uapi/auth.py
--rw-r--r--   0        0        0      694 2022-07-05 08:25:32.000000 finary_uapi-0.1.1/finary_uapi/bank_account_types.py
--rw-r--r--   0        0        0      118 2022-06-10 11:58:16.000000 finary_uapi-0.1.1/finary_uapi/constants.py
--rw-r--r--   0        0        0      241 2022-07-12 18:54:50.000000 finary_uapi-0.1.1/finary_uapi/crypto_chains.py
--rw-r--r--   0        0        0      824 2022-07-05 08:05:25.000000 finary_uapi-0.1.1/finary_uapi/currencies.py
--rw-r--r--   0        0        0      308 2022-07-04 18:16:08.000000 finary_uapi-0.1.1/finary_uapi/generic_asset_categories.py
--rw-r--r--   0        0        0     1310 2022-07-05 06:40:07.000000 finary_uapi-0.1.1/finary_uapi/importers/crypto_generic_csv.py
--rw-r--r--   0        0        0     3244 2022-07-09 16:21:57.000000 finary_uapi-0.1.1/finary_uapi/importers/cryptocom.py
--rw-r--r--   0        0        0     1204 2022-07-05 08:27:58.000000 finary_uapi-0.1.1/finary_uapi/importers/stocks_generic_csv.py
--rw-r--r--   0        0        0      391 2022-07-05 08:06:29.000000 finary_uapi-0.1.1/finary_uapi/institutions.py
--rw-r--r--   0        0        0      511 2022-07-05 08:07:06.000000 finary_uapi-0.1.1/finary_uapi/precious_metals.py
--rw-r--r--   0        0        0      494 2022-07-12 18:15:05.000000 finary_uapi-0.1.1/finary_uapi/scpis.py
--rw-r--r--   0        0        0     3681 2023-05-19 19:32:14.600649 finary_uapi-0.1.1/finary_uapi/securities.py
--rw-r--r--   0        0        0     2308 2022-07-13 19:33:49.000000 finary_uapi-0.1.1/finary_uapi/signin.py
--rw-r--r--   0        0        0     4177 2022-10-05 12:54:35.628064 finary_uapi-0.1.1/finary_uapi/user_cryptos.py
--rw-r--r--   0        0        0      221 2023-04-30 02:01:09.614218 finary_uapi-0.1.1/finary_uapi/user_fonds_euro.py
--rw-r--r--   0        0        0     2024 2022-07-12 13:10:04.000000 finary_uapi-0.1.1/finary_uapi/user_generic_assets.py
--rw-r--r--   0        0        0     3653 2022-10-05 12:54:35.628338 finary_uapi-0.1.1/finary_uapi/user_holdings_accounts.py
--rw-r--r--   0        0        0      411 2022-07-12 18:47:51.000000 finary_uapi-0.1.1/finary_uapi/user_me.py
--rw-r--r--   0        0        0     1998 2023-05-19 19:32:14.591775 finary_uapi-0.1.1/finary_uapi/user_portfolio.py
--rw-r--r--   0        0        0     1865 2022-07-05 08:11:56.000000 finary_uapi-0.1.1/finary_uapi/user_precious_metals.py
--rw-r--r--   0        0        0      222 2022-07-12 13:28:04.000000 finary_uapi-0.1.1/finary_uapi/user_real_estates.py
--rw-r--r--   0        0        0      208 2022-07-12 13:28:04.000000 finary_uapi-0.1.1/finary_uapi/user_scpis.py
--rw-r--r--   0        0        0     7762 2023-05-19 19:37:06.303119 finary_uapi-0.1.1/finary_uapi/user_securities.py
--rw-r--r--   0        0        0      221 2022-07-12 13:28:04.000000 finary_uapi-0.1.1/finary_uapi/user_startups.py
--rw-r--r--   0        0        0      196 2022-07-12 13:02:13.000000 finary_uapi-0.1.1/finary_uapi/utils.py
--rw-r--r--   0        0        0     3387 2023-04-30 01:57:20.675756 finary_uapi-0.1.1/finary_uapi/views.py
--rw-r--r--   0        0        0      474 2023-04-30 01:57:25.478991 finary_uapi-0.1.1/finary_uapi/watches.py
--rw-r--r--   0        0        0      741 2023-05-22 20:47:44.635742 finary_uapi-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5745 1970-01-01 00:00:00.000000 finary_uapi-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-06-23 13:41:14.000000 finary_uapi-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5184 2023-05-22 20:32:05.637450 finary_uapi-0.1.2/README.md
+-rw-r--r--   0        0        0      692 2023-05-22 21:06:01.990540 finary_uapi-0.1.2/finary_uapi/__init__.py
+-rw-r--r--   0        0        0    16618 2023-05-22 20:29:53.501992 finary_uapi-0.1.2/finary_uapi/__main__.py
+-rw-r--r--   0        0        0      323 2022-07-05 06:50:29.000000 finary_uapi-0.1.2/finary_uapi/auth.py
+-rw-r--r--   0        0        0      694 2022-07-05 08:25:32.000000 finary_uapi-0.1.2/finary_uapi/bank_account_types.py
+-rw-r--r--   0        0        0      118 2022-06-10 11:58:16.000000 finary_uapi-0.1.2/finary_uapi/constants.py
+-rw-r--r--   0        0        0      241 2022-07-12 18:54:50.000000 finary_uapi-0.1.2/finary_uapi/crypto_chains.py
+-rw-r--r--   0        0        0      824 2022-07-05 08:05:25.000000 finary_uapi-0.1.2/finary_uapi/currencies.py
+-rw-r--r--   0        0        0      308 2022-07-04 18:16:08.000000 finary_uapi-0.1.2/finary_uapi/generic_asset_categories.py
+-rw-r--r--   0        0        0     1310 2022-07-05 06:40:07.000000 finary_uapi-0.1.2/finary_uapi/importers/crypto_generic_csv.py
+-rw-r--r--   0        0        0     3244 2022-07-09 16:21:57.000000 finary_uapi-0.1.2/finary_uapi/importers/cryptocom.py
+-rw-r--r--   0        0        0     1204 2022-07-05 08:27:58.000000 finary_uapi-0.1.2/finary_uapi/importers/stocks_generic_csv.py
+-rw-r--r--   0        0        0      391 2022-07-05 08:06:29.000000 finary_uapi-0.1.2/finary_uapi/institutions.py
+-rw-r--r--   0        0        0      511 2022-07-05 08:07:06.000000 finary_uapi-0.1.2/finary_uapi/precious_metals.py
+-rw-r--r--   0        0        0      494 2022-07-12 18:15:05.000000 finary_uapi-0.1.2/finary_uapi/scpis.py
+-rw-r--r--   0        0        0     3681 2023-05-19 19:32:14.600649 finary_uapi-0.1.2/finary_uapi/securities.py
+-rw-r--r--   0        0        0     2308 2022-07-13 19:33:49.000000 finary_uapi-0.1.2/finary_uapi/signin.py
+-rw-r--r--   0        0        0     4177 2022-10-05 12:54:35.628064 finary_uapi-0.1.2/finary_uapi/user_cryptos.py
+-rw-r--r--   0        0        0      221 2023-04-30 02:01:09.614218 finary_uapi-0.1.2/finary_uapi/user_fonds_euro.py
+-rw-r--r--   0        0        0     2024 2022-07-12 13:10:04.000000 finary_uapi-0.1.2/finary_uapi/user_generic_assets.py
+-rw-r--r--   0        0        0     3653 2022-10-05 12:54:35.628338 finary_uapi-0.1.2/finary_uapi/user_holdings_accounts.py
+-rw-r--r--   0        0        0      411 2022-07-12 18:47:51.000000 finary_uapi-0.1.2/finary_uapi/user_me.py
+-rw-r--r--   0        0        0     1998 2023-05-19 19:32:14.591775 finary_uapi-0.1.2/finary_uapi/user_portfolio.py
+-rw-r--r--   0        0        0     1865 2022-07-05 08:11:56.000000 finary_uapi-0.1.2/finary_uapi/user_precious_metals.py
+-rw-r--r--   0        0        0      222 2022-07-12 13:28:04.000000 finary_uapi-0.1.2/finary_uapi/user_real_estates.py
+-rw-r--r--   0        0        0      208 2022-07-12 13:28:04.000000 finary_uapi-0.1.2/finary_uapi/user_scpis.py
+-rw-r--r--   0        0        0     7762 2023-05-19 19:37:06.303119 finary_uapi-0.1.2/finary_uapi/user_securities.py
+-rw-r--r--   0        0        0      221 2022-07-12 13:28:04.000000 finary_uapi-0.1.2/finary_uapi/user_startups.py
+-rw-r--r--   0        0        0      196 2022-07-12 13:02:13.000000 finary_uapi-0.1.2/finary_uapi/utils.py
+-rw-r--r--   0        0        0     3387 2023-04-30 01:57:20.675756 finary_uapi-0.1.2/finary_uapi/views.py
+-rw-r--r--   0        0        0      474 2023-04-30 01:57:25.478991 finary_uapi-0.1.2/finary_uapi/watches.py
+-rw-r--r--   0        0        0      741 2023-05-22 21:05:55.851620 finary_uapi-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5796 1970-01-01 00:00:00.000000 finary_uapi-0.1.2/PKG-INFO
```

### Comparing `finary_uapi-0.1.1/LICENSE` & `finary_uapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/README.md` & `finary_uapi-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/__init__.py` & `finary_uapi-0.1.2/finary_uapi/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 account.
 
 This module is maintained by lasconic.
 You can always get the latest version of this module at:
     https://github.com/lasconic/finary-uapi
 """
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __author__ = "lasconic"
 __copyright__ = """
 Copyright (c) 2021-2022, lasconic
 Permission to use, copy, modify, and distribute this software and its
 documentation for any purpose and without fee or royalty is hereby
 granted, provided that the above copyright notice appear in all copies
 and that both that copyright notice and this permission notice appear
```

### Comparing `finary_uapi-0.1.1/finary_uapi/__main__.py` & `finary_uapi-0.1.2/finary_uapi/__main__.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/bank_account_types.py` & `finary_uapi-0.1.2/finary_uapi/bank_account_types.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/currencies.py` & `finary_uapi-0.1.2/finary_uapi/currencies.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/importers/crypto_generic_csv.py` & `finary_uapi-0.1.2/finary_uapi/importers/crypto_generic_csv.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/importers/cryptocom.py` & `finary_uapi-0.1.2/finary_uapi/importers/cryptocom.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/importers/stocks_generic_csv.py` & `finary_uapi-0.1.2/finary_uapi/importers/stocks_generic_csv.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/securities.py` & `finary_uapi-0.1.2/finary_uapi/securities.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/signin.py` & `finary_uapi-0.1.2/finary_uapi/signin.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/user_cryptos.py` & `finary_uapi-0.1.2/finary_uapi/user_cryptos.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/user_generic_assets.py` & `finary_uapi-0.1.2/finary_uapi/user_generic_assets.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/user_holdings_accounts.py` & `finary_uapi-0.1.2/finary_uapi/user_holdings_accounts.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/user_portfolio.py` & `finary_uapi-0.1.2/finary_uapi/user_portfolio.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/user_precious_metals.py` & `finary_uapi-0.1.2/finary_uapi/user_precious_metals.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/user_securities.py` & `finary_uapi-0.1.2/finary_uapi/user_securities.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/finary_uapi/views.py` & `finary_uapi-0.1.2/finary_uapi/views.py`

 * *Files identical despite different names*

### Comparing `finary_uapi-0.1.1/pyproject.toml` & `finary_uapi-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "finary-uapi"
-version = "0.1.1"
+version = "0.1.2"
 description = "Finary API client and command line tool to interact with your Finary account."
 authors = ["lasconic <lasconic@gmail.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "finary_uapi"}]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.10"
 docopt = "^0.6.2"
 fuzzywuzzy = {version = "^0.18.0", extras = ["speedup"]}
 requests = "^2.30.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "23.3.0"
 flake8 = "6.0.0"
```

### Comparing `finary_uapi-0.1.1/PKG-INFO` & `finary_uapi-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: finary-uapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: Finary API client and command line tool to interact with your Finary account.
 License: MIT
 Author: lasconic
 Author-email: lasconic@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Requires-Dist: fuzzywuzzy[speedup] (>=0.18.0,<0.19.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 Finary Unofficial API wrapper
```

