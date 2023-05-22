# Comparing `tmp/fmpsdk-20230312.0.tar.gz` & `tmp/fmpsdk-20230522.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmpsdk-20230312.0.tar", last modified: Sun Mar 12 18:12:18 2023, max compression
+gzip compressed data, was "fmpsdk-20230522.0.tar", last modified: Mon May 22 14:13:32 2023, max compression
```

## Comparing `fmpsdk-20230312.0.tar` & `fmpsdk-20230522.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-03-12 18:12:18.606613 fmpsdk-20230312.0/
--rw-r--r--   0 dmickelson   (503) staff       (20)     1500 2022-12-05 15:16:07.000000 fmpsdk-20230312.0/LICENSE.md
--rw-r--r--   0 dmickelson   (503) staff       (20)      877 2023-03-12 18:12:18.606671 fmpsdk-20230312.0/PKG-INFO
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-03-12 18:12:18.606006 fmpsdk-20230312.0/fmpsdk/
--rw-r--r--   0 dmickelson   (503) staff       (20)     5730 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/__init__.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     2607 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/alternative_data.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     4117 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/calendar.py
--rw-r--r--   0 dmickelson   (503) staff       (20)      728 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/commodities.py
--rw-r--r--   0 dmickelson   (503) staff       (20)    29207 2023-03-12 18:10:00.000000 fmpsdk-20230312.0/fmpsdk/company_valuation.py
--rw-r--r--   0 dmickelson   (503) staff       (20)      749 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/cryptocurrencies.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1561 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/etf.py
--rw-r--r--   0 dmickelson   (503) staff       (20)      714 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/euronext.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1022 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/forex.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     3076 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/general.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     3053 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/insider_trading.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     5203 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/institutional_fund.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     4410 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/market_indexes.py
--rw-r--r--   0 dmickelson   (503) staff       (20)      735 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/mutual_funds.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1782 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/senate.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     8759 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/settings.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     1774 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/stock_market.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     2228 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/stock_time_series.py
--rw-r--r--   0 dmickelson   (503) staff       (20)      949 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/technical_indicators.py
--rw-r--r--   0 dmickelson   (503) staff       (20)      684 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/tsx.py
--rw-r--r--   0 dmickelson   (503) staff       (20)     6796 2022-12-05 15:16:05.000000 fmpsdk-20230312.0/fmpsdk/url_methods.py
-drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-03-12 18:12:18.606519 fmpsdk-20230312.0/fmpsdk.egg-info/
--rw-r--r--   0 dmickelson   (503) staff       (20)      877 2023-03-12 18:12:18.000000 fmpsdk-20230312.0/fmpsdk.egg-info/PKG-INFO
--rw-r--r--   0 dmickelson   (503) staff       (20)      659 2023-03-12 18:12:18.000000 fmpsdk-20230312.0/fmpsdk.egg-info/SOURCES.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)        1 2023-03-12 18:12:18.000000 fmpsdk-20230312.0/fmpsdk.egg-info/dependency_links.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)       23 2023-03-12 18:12:18.000000 fmpsdk-20230312.0/fmpsdk.egg-info/requires.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)        7 2023-03-12 18:12:18.000000 fmpsdk-20230312.0/fmpsdk.egg-info/top_level.txt
--rw-r--r--   0 dmickelson   (503) staff       (20)      222 2022-12-05 15:16:06.000000 fmpsdk-20230312.0/pyproject.toml
--rw-r--r--   0 dmickelson   (503) staff       (20)       91 2023-03-12 18:12:18.606855 fmpsdk-20230312.0/setup.cfg
--rw-r--r--   0 dmickelson   (503) staff       (20)     1208 2023-03-12 18:10:29.000000 fmpsdk-20230312.0/setup.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-05-22 14:13:32.449701 fmpsdk-20230522.0/
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1500 2022-12-05 15:16:07.000000 fmpsdk-20230522.0/LICENSE.md
+-rw-r--r--   0 dmickelson   (503) staff       (20)      877 2023-05-22 14:13:32.449768 fmpsdk-20230522.0/PKG-INFO
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-05-22 14:13:32.448870 fmpsdk-20230522.0/fmpsdk/
+-rw-r--r--   0 dmickelson   (503) staff       (20)     5730 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/__init__.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     2607 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/alternative_data.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     4117 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/calendar.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)      728 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/commodities.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)    28897 2023-05-22 14:07:52.000000 fmpsdk-20230522.0/fmpsdk/company_valuation.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)      749 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/cryptocurrencies.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1561 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/etf.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)      714 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/euronext.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1022 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/forex.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     3076 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/general.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     3053 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/insider_trading.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     5203 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/institutional_fund.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     4410 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/market_indexes.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)      735 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/mutual_funds.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1782 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/senate.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     8572 2023-05-22 14:07:52.000000 fmpsdk-20230522.0/fmpsdk/settings.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1774 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/stock_market.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     2186 2023-05-22 14:07:52.000000 fmpsdk-20230522.0/fmpsdk/stock_time_series.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)      949 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/technical_indicators.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)      684 2022-12-05 15:16:05.000000 fmpsdk-20230522.0/fmpsdk/tsx.py
+-rw-r--r--   0 dmickelson   (503) staff       (20)     6361 2023-05-22 14:07:52.000000 fmpsdk-20230522.0/fmpsdk/url_methods.py
+drwxr-xr-x   0 dmickelson   (503) staff       (20)        0 2023-05-22 14:13:32.449602 fmpsdk-20230522.0/fmpsdk.egg-info/
+-rw-r--r--   0 dmickelson   (503) staff       (20)      877 2023-05-22 14:13:32.000000 fmpsdk-20230522.0/fmpsdk.egg-info/PKG-INFO
+-rw-r--r--   0 dmickelson   (503) staff       (20)      659 2023-05-22 14:13:32.000000 fmpsdk-20230522.0/fmpsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)        1 2023-05-22 14:13:32.000000 fmpsdk-20230522.0/fmpsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)       23 2023-05-22 14:13:32.000000 fmpsdk-20230522.0/fmpsdk.egg-info/requires.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)        7 2023-05-22 14:13:32.000000 fmpsdk-20230522.0/fmpsdk.egg-info/top_level.txt
+-rw-r--r--   0 dmickelson   (503) staff       (20)      222 2022-12-05 15:16:06.000000 fmpsdk-20230522.0/pyproject.toml
+-rw-r--r--   0 dmickelson   (503) staff       (20)       91 2023-05-22 14:13:32.450072 fmpsdk-20230522.0/setup.cfg
+-rw-r--r--   0 dmickelson   (503) staff       (20)     1369 2023-05-22 14:11:30.000000 fmpsdk-20230522.0/setup.py
```

### Comparing `fmpsdk-20230312.0/LICENSE.md` & `fmpsdk-20230522.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/PKG-INFO` & `fmpsdk-20230522.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmpsdk
-Version: 20230312.0
+Version: 20230522.0
 Summary: SDK for interacting with FMP's APIs.
 Home-page: https://github.com/daxm/fmpsdk
 Author: Dax Mickelson
 Author-email: fmp@daxm.net
 License: BSD
 Keywords: fmpsdk financial stock valuation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fmpsdk-20230312.0/fmpsdk/__init__.py` & `fmpsdk-20230522.0/fmpsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/alternative_data.py` & `fmpsdk-20230522.0/fmpsdk/alternative_data.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/calendar.py` & `fmpsdk-20230522.0/fmpsdk/calendar.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/commodities.py` & `fmpsdk-20230522.0/fmpsdk/commodities.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/company_valuation.py` & `fmpsdk-20230522.0/fmpsdk/company_valuation.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     INCOME_STATEMENT_AS_REPORTED_FILENAME,
     INCOME_STATEMENT_FILENAME,
     BASE_URL_v3,
 )
 from .url_methods import (
     __return_json_v3,
     __return_json_v4,
-    __validate_exchange,
     __validate_industry,
     __validate_period,
     __validate_sector,
 )
 
 
 def company_profile(
@@ -70,15 +69,15 @@
     :return: A list of dictionaries.
     """
     path = f"search/"
     query_vars = {
         "apikey": apikey,
         "limit": limit,
         "query": query,
-        "exchange": __validate_exchange(value=exchange),
+        "exchange": exchange,
     }
     return __return_json_v3(path=path, query_vars=query_vars)
 
 
 def search_ticker(
     apikey: str, query: str = "", limit: int = DEFAULT_LIMIT, exchange: str = ""
 ) -> typing.Optional[typing.List[typing.Dict]]:
@@ -93,15 +92,15 @@
     :return: A list of dictionaries.
     """
     path = f"search-ticker/"
     query_vars = {
         "apikey": apikey,
         "limit": limit,
         "query": query,
-        "exchange": __validate_exchange(value=exchange),
+        "exchange": exchange,
     }
     return __return_json_v3(path=path, query_vars=query_vars)
 
 
 def financial_statement(
     apikey: str, symbol: str, filename: str = FINANCIAL_STATEMENT_FILENAME
 ) -> None:
@@ -767,34 +766,29 @@
         query_vars["dividendMoreThan"] = dividend_more_than
     if dividend_lower_than:
         query_vars["dividendLowerThan"] = dividend_lower_than
     if price_more_than:
         query_vars["priceMoreThan"] = price_more_than
     if price_lower_than:
         query_vars["priceLowerThan"] = price_lower_than
-    if is_etf:
+    if is_etf is not None:
         query_vars["isEtf"] = is_etf
-    if is_actively_trading:
+    if is_actively_trading is not None:
         query_vars["isActivelyTrading"] = is_actively_trading
     if sector:
         query_vars["sector"] = __validate_sector(sector)
     if industry:
         query_vars["industry"] = __validate_industry(industry)
     if country:
         query_vars["country"] = country
     if exchange:
         if type(exchange) is list:
-            for item in exchange:
-                if item != __validate_exchange(item):
-                    msg = f"Invalid Exchange value: {exchange}."
-                    logging.error(msg)
-                    raise ValueError(msg)
             query_vars["exchange"] = ",".join(exchange)
         else:
-            query_vars["exchange"] = __validate_exchange(exchange)
+            query_vars["exchange"] = exchange
     return __return_json_v3(path=path, query_vars=query_vars)
 
 
 def delisted_companies(
     apikey: str, limit: int = DEFAULT_LIMIT
 ) -> typing.Optional[typing.List[typing.Dict]]:
     """
```

### Comparing `fmpsdk-20230312.0/fmpsdk/cryptocurrencies.py` & `fmpsdk-20230522.0/fmpsdk/cryptocurrencies.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/etf.py` & `fmpsdk-20230522.0/fmpsdk/etf.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/euronext.py` & `fmpsdk-20230522.0/fmpsdk/euronext.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/forex.py` & `fmpsdk-20230522.0/fmpsdk/forex.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/general.py` & `fmpsdk-20230522.0/fmpsdk/general.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/insider_trading.py` & `fmpsdk-20230522.0/fmpsdk/insider_trading.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/institutional_fund.py` & `fmpsdk-20230522.0/fmpsdk/institutional_fund.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/market_indexes.py` & `fmpsdk-20230522.0/fmpsdk/market_indexes.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/mutual_funds.py` & `fmpsdk-20230522.0/fmpsdk/mutual_funds.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/senate.py` & `fmpsdk-20230522.0/fmpsdk/senate.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/settings.py` & `fmpsdk-20230522.0/fmpsdk/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -277,27 +277,14 @@
     "Marine",
     "Diversified Consumer Services",
 ]
 PERIOD_VALUES: typing.List = [
     "annual",
     "quarter",
 ]
-EXCHANGE_VALUES: typing.List = [
-    "ETF",
-    "MUTUAL_FUND",
-    "COMMODITY",
-    "INDEX",
-    "CRYPTO",
-    "FOREX",
-    "TSX",
-    "AMEX",
-    "NASDAQ",
-    "NYSE",
-    "EURONEXT",
-]
 TIME_DELTA_VALUES: typing.List = [
     "1min",
     "5min",
     "15min",
     "30min",
     "1hour",
     "4hour",
```

### Comparing `fmpsdk-20230312.0/fmpsdk/stock_market.py` & `fmpsdk-20230522.0/fmpsdk/stock_market.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/stock_time_series.py` & `fmpsdk-20230522.0/fmpsdk/stock_time_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing
 
 from .general import __quotes
-from .url_methods import __return_json_v3, __return_json_v4, __validate_exchange
+from .url_methods import __return_json_v3, __return_json_v4
 
 
 def quote_short(apikey: str, symbol: str) -> typing.Optional[typing.List[typing.Dict]]:
     """
     Query FMP /quote-short/ API.
 
     :param apikey: Your API key
@@ -25,15 +25,15 @@
     """
     Query FMP /quotes/ API.
 
     :param apikey: Your API key
     :param exchange: Exchange symbol.
     :return: A list of dictionaries.
     """
-    return __quotes(apikey=apikey, value=__validate_exchange(exchange))
+    return __quotes(apikey=apikey, value=exchange)
 
 
 def historical_stock_dividend(
     apikey: str, symbol: str
 ) -> typing.Optional[typing.List[typing.Dict]]:
     """
     Query FMP /historical-price-full/stock_divident/ API
```

### Comparing `fmpsdk-20230312.0/fmpsdk/technical_indicators.py` & `fmpsdk-20230522.0/fmpsdk/technical_indicators.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/tsx.py` & `fmpsdk-20230522.0/fmpsdk/tsx.py`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/fmpsdk/url_methods.py` & `fmpsdk-20230522.0/fmpsdk/url_methods.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 import typing
 
 import requests
 
 from .settings import (
-    EXCHANGE_VALUES,
     INDUSTRY_VALUES,
     PERIOD_VALUES,
     SECTOR_VALUES,
     SERIES_TYPE_VALUES,
     STATISTICS_TYPE_VALUES,
     TECHNICAL_INDICATORS_TIME_DELTA_VALUES,
     TIME_DELTA_VALUES,
@@ -109,29 +108,14 @@
         logging.error(
             f"A requests exception has occurred that we have not yet detailed an 'except' clause for.  "
             f"Error: {e}"
         )
     return return_var
 
 
-def __validate_exchange(value: str) -> str:
-    """
-    Check to see if passed string is in the list of possible Exchanges.
-    :param value: Exchange name.
-    :return: Passed value or No Return
-    """
-    valid_values = EXCHANGE_VALUES
-    if value in valid_values:
-        return value
-    else:
-        logging.error(
-            f"Invalid exchange value: {value}.  Valid options: {valid_values}"
-        )
-
-
 def __validate_period(value: str) -> str:
     """
     Check to see if passed string is in the list of possible time periods.
     :param value: Period name.
     :return: Passed value or No Return
     """
     valid_values = PERIOD_VALUES
```

### Comparing `fmpsdk-20230312.0/fmpsdk.egg-info/PKG-INFO` & `fmpsdk-20230522.0/fmpsdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fmpsdk
-Version: 20230312.0
+Version: 20230522.0
 Summary: SDK for interacting with FMP's APIs.
 Home-page: https://github.com/daxm/fmpsdk
 Author: Dax Mickelson
 Author-email: fmp@daxm.net
 License: BSD
 Keywords: fmpsdk financial stock valuation
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `fmpsdk-20230312.0/fmpsdk.egg-info/SOURCES.txt` & `fmpsdk-20230522.0/fmpsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmpsdk-20230312.0/setup.py` & `fmpsdk-20230522.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from setuptools import find_packages, setup
 
+__version__ = "20230522.0"
 __author__ = "Dax Mickelson"
-__author_email = "fmp@daxm.net"
+__author_email__ = "fmp@daxm.net"
 __license__ = "BSD"
+__package_name__ = "fmpsdk"
+__description__ = "SDK for interacting with FMP's APIs."
+__long_description__ = """Interact with Financial Modeling Prep's APIs."""
+__url__ = "https://github.com/daxm/fmpsdk"
 
 setup(
-    name="fmpsdk",
-    version="20230312.0",
-    description="SDK for interacting with FMP's APIs.",
-    long_description="""Interact with Financial Modeling Prep's APIs.""",
-    url="https://github.com/daxm/fmpsdk",
-    author="Dax Mickelson",
-    author_email="fmp@daxm.net",
-    license="BSD",
+    name=__package_name__,
+    version=__version__,
+    description=__description__,
+    long_description=__long_description__,
+    url=__url__,
+    author=__author__,
+    author_email=__author_email__,
+    license=__license__,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Plugins",
         "Intended Audience :: Developers",
         "Intended Audience :: Other Audience",
         "License :: OSI Approved :: BSD License",
         "Natural Language :: English",
@@ -28,9 +33,9 @@
         "Topic :: Utilities",
     ],
     keywords="fmpsdk financial stock valuation",
     packages=find_packages(exclude=["docs", "tests*"]),
     install_requires=["python-dotenv", "requests"],
     python_requires=">=3.6",
     package_data={},
-    data_files=None,
+    data_files=[],
 )
```

