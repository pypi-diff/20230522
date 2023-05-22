# Comparing `tmp/robin_stocks-2.1.0.tar.gz` & `tmp/robin_stocks-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robin_stocks-2.1.0.tar", last modified: Wed Oct 20 03:45:11 2021, max compression
+gzip compressed data, was "dist/robin_stocks-3.0.0.tar", last modified: Mon May 22 01:15:38 2023, max compression
```

## Comparing `robin_stocks-2.1.0.tar` & `robin_stocks-3.0.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-10-20 03:45:11.163815 robin_stocks-2.1.0/
--rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-2.1.0/LICENSE.txt
--rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-2.1.0/MANIFEST.in
--rw-r--r--   0 josh       (501) staff       (20)     5801 2021-10-20 03:45:11.163413 robin_stocks-2.1.0/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/README.rst
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-10-20 03:45:11.145118 robin_stocks-2.1.0/robin_stocks/
--rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/__init__.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-10-20 03:45:11.150657 robin_stocks-2.1.0/robin_stocks/gemini/
--rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/gemini/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/gemini/account.py
--rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/gemini/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/gemini/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/gemini/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/gemini/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/gemini/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/gemini/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-10-20 03:45:11.156525 robin_stocks-2.1.0/robin_stocks/robinhood/
--rw-r--r--   0 josh       (501) staff       (20)     5012 2021-02-23 04:31:10.000000 robin_stocks-2.1.0/robin_stocks/robinhood/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    30505 2021-10-20 03:38:49.000000 robin_stocks-2.1.0/robin_stocks/robinhood/account.py
--rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-2.1.0/robin_stocks/robinhood/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-2.1.0/robin_stocks/robinhood/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)     6036 2021-02-23 04:46:14.000000 robin_stocks-2.1.0/robin_stocks/robinhood/export.py
--rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/robinhood/globals.py
--rw-r--r--   0 josh       (501) staff       (20)    13217 2021-02-23 04:29:35.000000 robin_stocks-2.1.0/robin_stocks/robinhood/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-2.1.0/robin_stocks/robinhood/markets.py
--rw-r--r--   0 josh       (501) staff       (20)    20166 2021-02-27 17:24:31.000000 robin_stocks-2.1.0/robin_stocks/robinhood/options.py
--rw-r--r--   0 josh       (501) staff       (20)    61794 2021-05-12 02:21:53.000000 robin_stocks-2.1.0/robin_stocks/robinhood/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     9406 2021-02-27 17:12:00.000000 robin_stocks-2.1.0/robin_stocks/robinhood/profiles.py
--rw-r--r--   0 josh       (501) staff       (20)    25212 2021-02-27 17:42:35.000000 robin_stocks-2.1.0/robin_stocks/robinhood/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     7154 2021-02-27 17:42:35.000000 robin_stocks-2.1.0/robin_stocks/robinhood/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-10-20 03:45:11.160738 robin_stocks-2.1.0/robin_stocks/tda/
--rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/tda/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/tda/accounts.py
--rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/tda/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/tda/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/tda/helper.py
--rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/tda/markets.py
--rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/tda/orders.py
--rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-2.1.0/robin_stocks/tda/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/robin_stocks/tda/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-10-20 03:45:11.147181 robin_stocks-2.1.0/robin_stocks.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)     5801 2021-10-20 03:45:11.000000 robin_stocks-2.1.0/robin_stocks.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     1330 2021-10-20 03:45:11.000000 robin_stocks-2.1.0/robin_stocks.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2021-10-20 03:45:11.000000 robin_stocks-2.1.0/robin_stocks.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-2.1.0/robin_stocks.egg-info/not-zip-safe
--rw-r--r--   0 josh       (501) staff       (20)       42 2021-10-20 03:45:11.000000 robin_stocks-2.1.0/robin_stocks.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)       19 2021-10-20 03:45:11.000000 robin_stocks-2.1.0/robin_stocks.egg-info/top_level.txt
--rw-r--r--   0 josh       (501) staff       (20)       38 2021-10-20 03:45:11.163940 robin_stocks-2.1.0/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)      929 2021-10-20 03:43:55.000000 robin_stocks-2.1.0/setup.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2021-10-20 03:45:11.162748 robin_stocks-2.1.0/tests/
--rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-2.1.0/tests/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     9780 2021-02-23 04:18:12.000000 robin_stocks-2.1.0/tests/app_tests.py
--rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/tests/test_gemini.py
--rw-r--r--   0 josh       (501) staff       (20)    32257 2021-05-12 02:09:55.000000 robin_stocks-2.1.0/tests/test_robinhood.py
--rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-2.1.0/tests/test_tda.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 01:15:38.451269 robin_stocks-3.0.0/
+-rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.0.0/LICENSE.txt
+-rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.0.0/MANIFEST.in
+-rw-r--r--   0 josh       (501) staff       (20)     5803 2023-05-22 01:15:38.450786 robin_stocks-3.0.0/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/README.rst
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 01:15:38.430340 robin_stocks-3.0.0/robin_stocks/
+-rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 01:15:38.435842 robin_stocks-3.0.0/robin_stocks/gemini/
+-rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 01:15:38.442599 robin_stocks-3.0.0/robin_stocks/robinhood/
+-rw-r--r--   0 josh       (501) staff       (20)     5012 2021-02-23 04:31:10.000000 robin_stocks-3.0.0/robin_stocks/robinhood/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    30654 2023-05-22 00:46:39.000000 robin_stocks-3.0.0/robin_stocks/robinhood/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.0.0/robin_stocks/robinhood/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.0.0/robin_stocks/robinhood/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.0.0/robin_stocks/robinhood/export.py
+-rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/robinhood/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)    13217 2021-02-23 04:29:35.000000 robin_stocks-3.0.0/robin_stocks/robinhood/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.0.0/robin_stocks/robinhood/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)    20319 2023-05-22 00:46:39.000000 robin_stocks-3.0.0/robin_stocks/robinhood/options.py
+-rw-r--r--   0 josh       (501) staff       (20)    63387 2023-05-22 01:12:04.000000 robin_stocks-3.0.0/robin_stocks/robinhood/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     9622 2023-05-22 00:46:39.000000 robin_stocks-3.0.0/robin_stocks/robinhood/profiles.py
+-rw-r--r--   0 josh       (501) staff       (20)    25261 2023-05-22 01:12:04.000000 robin_stocks-3.0.0/robin_stocks/robinhood/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     7284 2023-05-22 00:46:39.000000 robin_stocks-3.0.0/robin_stocks/robinhood/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 01:15:38.446627 robin_stocks-3.0.0/robin_stocks/tda/
+-rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/accounts.py
+-rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.0.0/robin_stocks/tda/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 01:15:38.432279 robin_stocks-3.0.0/robin_stocks.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)     5803 2023-05-22 01:15:38.000000 robin_stocks-3.0.0/robin_stocks.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     1330 2023-05-22 01:15:38.000000 robin_stocks-3.0.0/robin_stocks.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2023-05-22 01:15:38.000000 robin_stocks-3.0.0/robin_stocks.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.0.0/robin_stocks.egg-info/not-zip-safe
+-rw-r--r--   0 josh       (501) staff       (20)       42 2023-05-22 01:15:38.000000 robin_stocks-3.0.0/robin_stocks.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       19 2023-05-22 01:15:38.000000 robin_stocks-3.0.0/robin_stocks.egg-info/top_level.txt
+-rw-r--r--   0 josh       (501) staff       (20)       38 2023-05-22 01:15:38.451448 robin_stocks-3.0.0/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)      931 2023-05-22 01:12:25.000000 robin_stocks-3.0.0/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 01:15:38.449585 robin_stocks-3.0.0/tests/
+-rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.0.0/tests/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     9780 2021-10-20 03:47:23.000000 robin_stocks-3.0.0/tests/app_tests.py
+-rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/tests/test_gemini.py
+-rw-r--r--   0 josh       (501) staff       (20)    33003 2023-05-22 01:12:04.000000 robin_stocks-3.0.0/tests/test_robinhood.py
+-rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/tests/test_tda.py
```

### Comparing `robin_stocks-2.1.0/LICENSE.txt` & `robin_stocks-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/PKG-INFO` & `robin_stocks-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin_stocks
-Version: 2.1.0
+Version: 3.0.0
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
 Description: .. image:: docs/source/_static/pics/title.PNG
         
@@ -97,9 +97,9 @@
         .. _Gemini Documentation: gemini.rst
         .. _TDA Documentation: tda.rst
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
 Platform: UNKNOWN
 Requires: requests
 Requires: pyotp
 Requires: cryptography
-Requires-Python: >=3
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
```

### Comparing `robin_stocks-2.1.0/README.rst` & `robin_stocks-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/gemini/__init__.py` & `robin_stocks-3.0.0/robin_stocks/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/gemini/account.py` & `robin_stocks-3.0.0/robin_stocks/gemini/account.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/gemini/authentication.py` & `robin_stocks-3.0.0/robin_stocks/gemini/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/gemini/crypto.py` & `robin_stocks-3.0.0/robin_stocks/gemini/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/gemini/globals.py` & `robin_stocks-3.0.0/robin_stocks/gemini/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/gemini/helper.py` & `robin_stocks-3.0.0/robin_stocks/gemini/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/gemini/orders.py` & `robin_stocks-3.0.0/robin_stocks/gemini/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/gemini/urls.py` & `robin_stocks-3.0.0/robin_stocks/gemini/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/robinhood/__init__.py` & `robin_stocks-3.0.0/robin_stocks/robinhood/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/robinhood/account.py` & `robin_stocks-3.0.0/robin_stocks/robinhood/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,19 @@
     url = positions_url()
     data = request_get(url, 'pagination')
 
     return(filter_data(data, info))
 
 
 @login_required
-def get_open_stock_positions(info=None):
+def get_open_stock_positions(account_number=None, info=None):
     """Returns a list of stocks that are currently held.
 
+    :param acccount_number: the robinhood account number.
+    :type acccount_number: Optional[str]
     :param info: Will filter the results to get a specific value.
     :type info: Optional[str]
     :returns: [list] Returns a list of dictionaries of key/value pairs for each ticker. If info parameter is provided, \
     a list of strings is returned where the strings are the value of the key that matches info.
     :Dictionary Keys: * url
                       * instrument
                       * account
@@ -139,15 +141,15 @@
                       * shares_held_for_options_collateral
                       * shares_held_for_options_events
                       * shares_pending_from_options_events
                       * updated_at
                       * created_at
 
     """
-    url = positions_url()
+    url = positions_url(account_number=account_number)
     payload = {'nonzero': 'true'}
     data = request_get(url, 'pagination', payload)
 
     return(filter_data(data, info))
 
 
 @login_required
```

### Comparing `robin_stocks-2.1.0/robin_stocks/robinhood/authentication.py` & `robin_stocks-3.0.0/robin_stocks/robinhood/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/robinhood/crypto.py` & `robin_stocks-3.0.0/robin_stocks/robinhood/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/robinhood/export.py` & `robin_stocks-3.0.0/robin_stocks/robinhood/export.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,14 +60,27 @@
             'order_type',
             'side',
             'fees',
             'quantity',
             'average_price'
         ])
         for order in all_orders:
+            # include candled order if partial executed
+            if order['state'] == 'cancelled' and len(order['executions']) > 0:
+                for partial in order['executions']:
+                    csv_writer.writerow([
+                        get_symbol_by_url(order['instrument']),
+                        partial['timestamp'],
+                        order['type'],
+                        order['side'],
+                        order['fees'],
+                        partial['quantity'],
+                        partial['price']
+                    ])
+
             if order['state'] == 'filled' and order['cancel'] is None:
                 csv_writer.writerow([
                     get_symbol_by_url(order['instrument']),
                     order['last_transaction_at'],
                     order['type'],
                     order['side'],
                     order['fees'],
```

### Comparing `robin_stocks-2.1.0/robin_stocks/robinhood/globals.py` & `robin_stocks-3.0.0/robin_stocks/robinhood/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/robinhood/helper.py` & `robin_stocks-3.0.0/robin_stocks/robinhood/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/robinhood/markets.py` & `robin_stocks-3.0.0/robin_stocks/robinhood/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/robinhood/options.py` & `robin_stocks-3.0.0/robin_stocks/robinhood/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,24 +63,26 @@
     """
     url = option_positions_url()
     data = request_get(url, 'pagination')
     return(filter_data(data, info))
 
 
 @login_required
-def get_open_option_positions(info=None):
+def get_open_option_positions(account_number=None, info=None):
     """Returns all open option positions for the account.
-
+    
+    :param acccount_number: the robinhood account number.
+    :type acccount_number: Optional[str]
     :param info: Will filter the results to get a specific value.
     :type info: Optional[str]
     :returns: Returns a list of dictionaries of key/value pairs for each option. If info parameter is provided, \
     a list of strings is returned where the strings are the value of the key that matches info.
 
     """
-    url = option_positions_url()
+    url = option_positions_url(account_number=account_number)
     payload = {'nonzero': 'True'}
     data = request_get(url, 'pagination', payload)
 
     return(filter_data(data, info))
 
 
 def get_chains(symbol, info=None):
```

### Comparing `robin_stocks-2.1.0/robin_stocks/robinhood/orders.py` & `robin_stocks-3.0.0/robin_stocks/robinhood/orders.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,15 +160,16 @@
     url = orders_url()
     data = request_get(url, 'pagination')
 
     if (len(arguments) == 0):
         return(data)
 
     for item in data:
-        item['quantity'] = str(int(float(item['quantity'])))
+        item['quantity'] = str(float(item['quantity']))
+        item['cumulative_quantity'] = str(float(item['cumulative_quantity']))
 
     if 'symbol' in arguments.keys():
         arguments['instrument'] = get_instruments_by_symbols(
             arguments['symbol'], info='url')[0]
         del arguments['symbol']
 
     if 'quantity' in arguments.keys():
@@ -317,47 +318,51 @@
     the price, and the quantity.
 
     """ 
     return order(symbol, quantity, "buy", None, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
-def order_buy_fractional_by_quantity(symbol, quantity, timeInForce='gfd', extendedHours=False, jsonify=True):
+def order_buy_fractional_by_quantity(symbol, quantity, account_number=None, timeInForce='gfd', extendedHours=False, jsonify=True):
     """Submits a market order to be executed immediately for fractional shares by specifying the amount that you want to trade.
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
 
     :param symbol: The stock ticker of the stock to purchase.
     :type symbol: str
     :param quantity: The amount of the fractional shares you want to buy.
     :type quantity: float
+    :param acccount_number: the robinhood account number.
+    :type acccount_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "buy", None, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "buy", account_number, None, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
-def order_buy_fractional_by_price(symbol, amountInDollars, timeInForce='gfd', extendedHours=False, jsonify=True):
+def order_buy_fractional_by_price(symbol, amountInDollars, account_number=None, timeInForce='gfd', extendedHours=False, jsonify=True):
     """Submits a market order to be executed immediately for fractional shares by specifying the amount in dollars that you want to trade.
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
 
     :param symbol: The stock ticker of the stock to purchase.
     :type symbol: str
     :param amountInDollars: The amount in dollars of the fractional shares you want to buy.
     :type amountInDollars: float
+    :param acccount_number: the robinhood account number.
+    :type acccount_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
@@ -369,15 +374,15 @@
         print("ERROR: Fractional share price should meet minimum 1.00.", file=get_output())
         return None
 
     # turn the money amount into decimal number of shares
     price = next(iter(get_latest_price(symbol, 'ask_price', extendedHours)), 0.00)
     fractional_shares = 0 if (price == 0.00) else round_price(amountInDollars/float(price))
 
-    return order(symbol, fractional_shares, "buy", None, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, fractional_shares, "buy", account_number, None, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_buy_limit(symbol, quantity, limitPrice, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a limit order to be executed once a certain price is reached.
 
     :param symbol: The stock ticker of the stock to purchase.
@@ -503,39 +508,41 @@
     the price, and the quantity.
 
     """ 
     return order(symbol, quantity, "sell", None, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
-def order_sell_fractional_by_quantity(symbol, quantity, timeInForce='gfd', priceType='bid_price', extendedHours=False, jsonify=True):
+def order_sell_fractional_by_quantity(symbol, quantity, account_number=None, timeInForce='gfd', priceType='bid_price', extendedHours=False, jsonify=True):
     """Submits a market order to be executed immediately for fractional shares by specifying the amount that you want to trade.
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
 
     :param symbol: The stock ticker of the stock to purchase.
     :type symbol: str
     :param quantity: The amount of the fractional shares you want to buy.
     :type quantity: float
+    :param acccount_number: the robinhood account number.
+    :type acccount_number: Optional[str]
     :param timeInForce: Changes how long the order will be in effect for. 'gfd' = good for the day.
     :type timeInForce: Optional[str]
     :param extendedHours: Premium users only. Allows trading during extended hours. Should be true or false.
     :type extendedHours: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the purchase of stocks, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
-    return order(symbol, quantity, "sell", None, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, quantity, "sell", account_number, None, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
-def order_sell_fractional_by_price(symbol, amountInDollars, timeInForce='gfd', extendedHours=False, jsonify=True):
+def order_sell_fractional_by_price(symbol, amountInDollars, account_number=None, timeInForce='gfd', extendedHours=False, jsonify=True):
     """Submits a market order to be executed immediately for fractional shares by specifying the amount in dollars that you want to trade.
     Good for share fractions up to 6 decimal places. Robinhood does not currently support placing limit, stop, or stop loss orders
     for fractional trades.
 
     :param symbol: The stock ticker of the stock to purchase.
     :type symbol: str
     :param amountInDollars: The amount in dollars of the fractional shares you want to buy.
@@ -554,15 +561,15 @@
     if amountInDollars < 1:
         print("ERROR: Fractional share price should meet minimum 1.00.", file=get_output())
         return None
     # turn the money amount into decimal number of shares
     price = next(iter(get_latest_price(symbol, 'bid_price', extendedHours)), 0.00)
     fractional_shares = 0 if (price == 0.00) else round_price(amountInDollars/float(price))
 
-    return order(symbol, fractional_shares, "sell", None, None, timeInForce, extendedHours, jsonify)
+    return order(symbol, fractional_shares, "sell", account_number, None, None, timeInForce, extendedHours, jsonify)
 
 
 @login_required
 def order_sell_limit(symbol, quantity, limitPrice, timeInForce='gtc', extendedHours=False, jsonify=True):
     """Submits a limit order to be executed once a certain price is reached.
 
     :param symbol: The stock ticker of the stock to sell.
@@ -744,23 +751,25 @@
     url = orders_url()
     data = request_post(url, payload, json=True, jsonify_data=jsonify)
 
     return (data)
 
 
 @login_required
-def order(symbol, quantity, side, limitPrice=None, stopPrice=None, timeInForce='gtc', extendedHours=False, jsonify=True):
+def order(symbol, quantity, side, account_number=None, limitPrice=None, stopPrice=None, timeInForce='gtc', extendedHours=False, jsonify=True):
     """A generic order function.
 
     :param symbol: The stock ticker of the stock to sell.
     :type symbol: str
     :param quantity: The number of stocks to sell.
     :type quantity: int
     :param side: Either 'buy' or 'sell'
     :type side: str
+    :param acccount_number: the robinhood account number.
+    :type acccount_number: Optional[str]
     :param limitPrice: The price to trigger the market order.
     :type limitPrice: float
     :param stopPrice: The price to trigger the limit or market order.
     :type stopPrice: float
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day.
     :type timeInForce: str
@@ -800,38 +809,39 @@
         if side == "buy":
             price = stopPrice
         else:
             price = None
         trigger = "stop"
     else:
         price = round_price(next(iter(get_latest_price(symbol, priceType, extendedHours)), 0.00))
-
     payload = {
-        'account': load_account_profile(info='url'),
+        'account': load_account_profile(account_number=account_number, info='url'),
         'instrument': get_instruments_by_symbols(symbol, info='url')[0],
         'symbol': symbol,
         'price': price,
         'quantity': quantity,
         'ref_id': str(uuid4()),
         'type': orderType,
         'stop_price': stopPrice,
         'time_in_force': timeInForce,
         'trigger': trigger,
         'side': side,
         'extended_hours': extendedHours
     }
 
     url = orders_url()
+
+
     data = request_post(url, payload, jsonify_data=jsonify)
 
     return(data)
 
 
 @login_required
-def order_option_credit_spread(price, symbol, quantity, spread, timeInForce='gtc', jsonify=True):
+def order_option_credit_spread(price, symbol, quantity, spread, timeInForce='gtc', account_number=None, jsonify=True):
     """Submits a limit order for an option credit spread.
 
     :param price: The limit price to trigger a sell of the option.
     :type price: float
     :param symbol: The stock ticker of the stock to trade.
     :type symbol: str
     :param quantity: The number of options to sell.
@@ -843,25 +853,27 @@
         - effect: This should be 'open' or 'close'.\n
         - action: This should be 'buy' or 'sell'.
     :type spread: dict
     :param timeInForce: Changes how long the order will be in effect for. \
      'gtc' = good until cancelled. \
      'gfd' = good for the day. 'ioc' = immediate or cancel. 'opg' = execute at opening.
     :type timeInForce: Optional[str]
+    :param acccount_number: the robinhood account number.
+    :type acccount_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the trading of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
     """
-    return(order_option_spread("credit", price, symbol, quantity, spread, timeInForce, jsonify))
+    return(order_option_spread("credit", price, symbol, quantity, spread, timeInForce, account_number, jsonify))
 
 
 @login_required
-def order_option_debit_spread(price, symbol, quantity, spread, timeInForce='gtc', jsonify=True):
+def order_option_debit_spread(price, symbol, quantity, spread, timeInForce='gtc', account_number=None, jsonify=True):
     """Submits a limit order for an option debit spread.
 
     :param price: The limit price to trigger a sell of the option.
     :type price: float
     :param symbol: The stock ticker of the stock to trade.
     :type symbol: str
     :param quantity: The number of options to sell.
@@ -873,25 +885,27 @@
         - effect: This should be 'open' or 'close'.\n
         - action: This should be 'buy' or 'sell'.
     :type spread: dict
     :param timeInForce: Changes how long the order will be in effect for.
      'gtc' = good until cancelled. \
      'gfd' = good for the day. 'ioc' = immediate or cancel. 'opg' execute at opening.
     :type timeInForce: Optional[str]
+    :param acccount_number: the robinhood account number.
+    :type acccount_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the trading of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
     """
-    return(order_option_spread("debit", price, symbol, quantity, spread, timeInForce, jsonify))
+    return(order_option_spread("debit", price, symbol, quantity, spread, timeInForce, account_number, jsonify))
 
 
 @login_required
-def order_option_spread(direction, price, symbol, quantity, spread, timeInForce='gtc', jsonify=True):
+def order_option_spread(direction, price, symbol, quantity, spread, timeInForce='gtc', account_number=None, jsonify=True):
     """Submits a limit order for an option spread. i.e. place a debit / credit spread
 
     :param direction: Can be "credit" or "debit".
     :type direction: str
     :param price: The limit price to trigger a trade of the option.
     :type price: float
     :param symbol: The stock ticker of the stock to trade.
@@ -907,14 +921,16 @@
     :type spread: dict
     :param timeInForce: Changes how long the order will be in effect for.
      'gtc' = good until cancelled. \
      'gfd' = good for the day. 'ioc' = immediate or cancel. 'opg' execute at opening.
     :type timeInForce: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
+    :param acccount_number: the robinhood account number.
+    :type acccount_number: Optional[str]
     :returns: Dictionary that contains information regarding the trading of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
     """ 
     try:
         symbol = symbol.upper().strip()
     except AttributeError as message:
@@ -928,15 +944,15 @@
                                         each['optionType'])
         legs.append({'position_effect': each['effect'],
                      'side': each['action'],
                      'ratio_quantity': 1,
                      'option': option_instruments_url(optionID)})
 
     payload = {
-        'account': load_account_profile(info='url'),
+        'account': load_account_profile(account_number=account_number, info='url'),
         'direction': direction,
         'time_in_force': timeInForce,
         'legs': legs,
         'type': 'limit',
         'trigger': 'immediate',
         'price': price,
         'quantity': quantity,
@@ -948,15 +964,15 @@
     url = option_orders_url()
     data = request_post(url, payload, json=True, jsonify_data=jsonify)
 
     return(data)
 
 
 @login_required
-def order_buy_option_limit(positionEffect, creditOrDebit, price, symbol, quantity, expirationDate, strike, optionType='both', timeInForce='gtc', jsonify=True):
+def order_buy_option_limit(positionEffect, creditOrDebit, price, symbol, quantity, expirationDate, strike, optionType='both', timeInForce='gtc', account_number=None, jsonify=True):
     """Submits a limit order for an option. i.e. place a long call or a long put.
 
     :param positionEffect: Either 'open' for a buy to open effect or 'close' for a buy to close effect.
     :type positionEffect: str
     :param creditOrDebit: Either 'debit' or 'credit'.
     :type creditOrDebit: str
     :param price: The limit price to trigger a buy of the option.
@@ -970,14 +986,16 @@
     :param strike: The strike price of the option.
     :type strike: float
     :param optionType: This should be 'call' or 'put'
     :type optionType: str
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day. 'ioc' = immediate or cancel. 'opg' execute at opening.
     :type timeInForce: Optional[str]
+    :param acccount_number: the robinhood account number.
+    :type acccount_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the buying of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
@@ -986,15 +1004,15 @@
     except AttributeError as message:
         print(message, file=get_output())
         return None
 
     optionID = id_for_option(symbol, expirationDate, strike, optionType)
 
     payload = {
-        'account': load_account_profile(info='url'),
+        'account': load_account_profile(account_number=account_number, info='url'),
         'direction': creditOrDebit,
         'time_in_force': timeInForce,
         'legs': [
             {'position_effect': positionEffect, 'side': 'buy',
                 'ratio_quantity': 1, 'option': option_instruments_url(optionID)},
         ],
         'type': 'limit',
@@ -1033,14 +1051,16 @@
     :param strike: The strike price of the option.
     :type strike: float
     :param optionType: This should be 'call' or 'put'
     :type optionType: str
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day. 'ioc' = immediate or cancel. 'opg' execute at opening.
     :type timeInForce: Optional[str]
+    :param acccount_number: the robinhood account number.
+    :type acccount_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the buying of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
@@ -1096,14 +1116,16 @@
     :param strike: The strike price of the option.
     :type strike: float
     :param optionType: This should be 'call' or 'put'
     :type optionType: str
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day. 'ioc' = immediate or cancel. 'opg' execute at opening.
     :type timeInForce: Optional[str]
+    :param acccount_number: the robinhood account number.
+    :type acccount_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the buying of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """ 
@@ -1136,15 +1158,15 @@
     url = option_orders_url()
     data = request_post(url, payload, json=True, jsonify_data=jsonify)
 
     return(data)
 
 
 @login_required
-def order_sell_option_limit(positionEffect, creditOrDebit, price, symbol, quantity, expirationDate, strike, optionType='both', timeInForce='gtc', jsonify=True):
+def order_sell_option_limit(positionEffect, creditOrDebit, price, symbol, quantity, expirationDate, strike, optionType='both', timeInForce='gtc', account_number=None, jsonify=True):
     """Submits a limit order for an option. i.e. place a short call or a short put.
 
     :param positionEffect: Either 'open' for a sell to open effect or 'close' for a sell to close effect.
     :type positionEffect: str
     :param creditOrDebit: Either 'debit' or 'credit'.
     :type creditOrDebit: str
     :param price: The limit price to trigger a sell of the option.
@@ -1158,14 +1180,16 @@
     :param strike: The strike price of the option.
     :type strike: float
     :param optionType: This should be 'call' or 'put'
     :type optionType: str
     :param timeInForce: Changes how long the order will be in effect for. 'gtc' = good until cancelled. \
     'gfd' = good for the day. 'ioc' = immediate or cancel. 'opg' execute at opening.
     :type timeInForce: Optional[str]
+    :param acccount_number: the robinhood account number.
+    :type acccount_number: Optional[str]
     :param jsonify: If set to False, function will return the request object which contains status code and headers.
     :type jsonify: Optional[str]
     :returns: Dictionary that contains information regarding the selling of options, \
     such as the order id, the state of order (queued, confired, filled, failed, canceled, etc.), \
     the price, and the quantity.
 
     """
@@ -1174,15 +1198,15 @@
     except AttributeError as message:
         print(message, file=get_output())
         return None
 
     optionID = id_for_option(symbol, expirationDate, strike, optionType)
 
     payload = {
-        'account': load_account_profile(info='url'),
+        'account': load_account_profile(account_number=account_number, info='url'),
         'direction': creditOrDebit,
         'time_in_force': timeInForce,
         'legs': [
             {'position_effect': positionEffect, 'side': 'sell',
                 'ratio_quantity': 1, 'option': option_instruments_url(optionID)},
         ],
         'type': 'limit',
```

### Comparing `robin_stocks-2.1.0/robin_stocks/robinhood/profiles.py` & `robin_stocks-3.0.0/robin_stocks/robinhood/profiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """Contains functions for getting all the information tied to a user account."""
 from robin_stocks.robinhood.helper import *
 from robin_stocks.robinhood.urls import *
 
 
 @login_required
-def load_account_profile(info=None):
+def load_account_profile(account_number=None, info=None):
     """Gets the information associated with the accounts profile,including day
     trading information and cash being held by Robinhood.
 
+    :param acccount_number: the robinhood account number.
+    :type acccount_number: Optional[str]
     :param info: The name of the key whose value is to be returned from the function.
     :type info: Optional[str]
     :returns: The function returns a dictionary of key/value pairs. \
     If a string is passed in to the info parameter, then the function will return \
     a string corresponding to the value of the key whose name matches the info parameter.
     :Dictionary Keys: * url
                       * portfolio_cash
@@ -55,16 +57,19 @@
                       * option_trading_on_expiration_enabled
                       * cash_held_for_options_collateral
                       * fractional_position_closing_only
                       * user_id
                       * rhs_stock_loan_consent_status
 
     """
-    url = account_profile_url()
-    data = request_get(url, 'indexzero')
+    url = account_profile_url(account_number)
+    if account_number is not None:
+         data = request_get(url)
+    else:
+        data = request_get(url, 'indexzero')
     return(filter_data(data, info))
 
 
 @login_required
 def load_basic_profile(info=None):
     """Gets the information associated with the personal profile,
     such as phone number, city, marital status, and date of birth.
```

### Comparing `robin_stocks-2.1.0/robin_stocks/robinhood/stocks.py` & `robin_stocks-3.0.0/robin_stocks/robinhood/stocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """Contains information in regards to stocks."""
+from functools import cache
+
 from robin_stocks.robinhood.helper import *
 from robin_stocks.robinhood.urls import *
 
 def get_quotes(inputSymbols, info=None):
     """Takes any number of stock tickers and returns information pertaining to its price.
 
     :param inputSymbols: May be a single stock ticker or a list of stock tickers.
@@ -223,15 +225,15 @@
                     prices.append(item['last_trade_price'])
                 else:
                     prices.append(item['last_extended_hours_trade_price'])
         else:
             prices.append(None)
     return(prices)
 
-
+@cache
 @convert_none_to_string
 def get_name_by_symbol(symbol):
     """Returns the name of a stock from the stock ticker.
 
     :param symbol: The ticker of the stock as a string.
     :type symbol: str
     :returns: [str] Returns the simple name of the stock. If the simple name does not exist then returns the full name.
@@ -251,14 +253,15 @@
     # If stock doesn't have a simple name attribute then get the full name.
     filter = filter_data(data, info='simple_name')
     if not filter or filter == "":
         filter = filter_data(data, info='name')
     return(filter)
 
 
+@cache
 @convert_none_to_string
 def get_name_by_url(url):
     """Returns the name of a stock from the instrument url. Should be located at ``https://api.robinhood.com/instruments/<id>``
     where <id> is the id of the stock.
 
     :param url: The url of the stock as a string.
     :type url: str
@@ -271,14 +274,15 @@
     # If stock doesn't have a simple name attribute then get the full name.
     filter = filter_data(data, info='simple_name')
     if not filter or filter == "":
         filter = filter_data(data, info='name')
     return(filter)
 
 
+@cache
 @convert_none_to_string
 def get_symbol_by_url(url):
     """Returns the symbol of a stock from the instrument url. Should be located at ``https://api.robinhood.com/instruments/<id>``
     where <id> is the id of the stock.
 
     :param url: The url of the stock as a string.
     :type url: str
```

### Comparing `robin_stocks-2.1.0/robin_stocks/robinhood/urls.py` & `robin_stocks-3.0.0/robin_stocks/robinhood/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 def challenge_url(challenge_id):
     return('https://api.robinhood.com/challenge/{0}/respond/'.format(challenge_id))
 
 # Profiles
 
 
-def account_profile_url():
-    return('https://api.robinhood.com/accounts/')
+def account_profile_url(account_number=None):
+    return('https://api.robinhood.com/accounts/'+account_number)
 
 
 def basic_profile_url():
     return('https://api.robinhood.com/user/basic_info/')
 
 
 def investment_profile_url():
@@ -82,16 +82,16 @@
     return('https://api.robinhood.com/instruments/{0}/splits/'.format(id_for_stock(symbol)))
 
 # account
 
 def phoenix_url():
     return('https://phoenix.robinhood.com/accounts/unified')
 
-def positions_url():
-    return('https://api.robinhood.com/positions/')
+def positions_url(account_number=None):
+    return('https://api.robinhood.com/positions/?account_number='+account_number)
 
 def banktransfers_url(direction=None):
     if direction == 'received':
         return('https://api.robinhood.com/ach/received/transfers/')
     else:
         return('https://api.robinhood.com/ach/transfers/')
 
@@ -208,16 +208,16 @@
 def option_orders_url(orderID=None):
     if orderID:
         return('https://api.robinhood.com/options/orders/{0}/'.format(orderID))
     else:
         return('https://api.robinhood.com/options/orders/')
 
 
-def option_positions_url():
-    return('https://api.robinhood.com/options/positions/')
+def option_positions_url(account_number):
+    return('https://api.robinhood.com/options/positions/?account_numbers='+account_number)
 
 
 def marketdata_options_url():
     return('https://api.robinhood.com/marketdata/options/')
 
 # pricebook
```

### Comparing `robin_stocks-2.1.0/robin_stocks/tda/__init__.py` & `robin_stocks-3.0.0/robin_stocks/tda/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/tda/accounts.py` & `robin_stocks-3.0.0/robin_stocks/tda/accounts.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/tda/authentication.py` & `robin_stocks-3.0.0/robin_stocks/tda/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/tda/globals.py` & `robin_stocks-3.0.0/robin_stocks/tda/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/tda/helper.py` & `robin_stocks-3.0.0/robin_stocks/tda/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/tda/markets.py` & `robin_stocks-3.0.0/robin_stocks/tda/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/tda/orders.py` & `robin_stocks-3.0.0/robin_stocks/tda/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/tda/stocks.py` & `robin_stocks-3.0.0/robin_stocks/tda/stocks.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks/tda/urls.py` & `robin_stocks-3.0.0/robin_stocks/tda/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/robin_stocks.egg-info/PKG-INFO` & `robin_stocks-3.0.0/robin_stocks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robin-stocks
-Version: 2.1.0
+Version: 3.0.0
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
 Description: .. image:: docs/source/_static/pics/title.PNG
         
@@ -97,9 +97,9 @@
         .. _Gemini Documentation: gemini.rst
         .. _TDA Documentation: tda.rst
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
 Platform: UNKNOWN
 Requires: requests
 Requires: pyotp
 Requires: cryptography
-Requires-Python: >=3
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
```

### Comparing `robin_stocks-2.1.0/robin_stocks.egg-info/SOURCES.txt` & `robin_stocks-3.0.0/robin_stocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/setup.py` & `robin_stocks-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='robin_stocks',
-      version='2.1.0',
+      version='3.0.0',
       description='A Python wrapper around the Robinhood API',
       long_description=long_description,
       long_description_content_type='text/x-rst',
       url='https://github.com/jmfernandes/robin_stocks',
       author='Josh Fernandes',
       author_email='joshfernandes@mac.com',
       keywords=['robinhood','robin stocks','finance app','stocks','options','trading','investing'],
       license='MIT',
-      python_requires='>=3',
+      python_requires='>=3.9',
       packages=find_packages(),
       requires=['requests', 'pyotp', 'cryptography'],
       install_requires=[
           'requests',
           'pyotp',
           'python-dotenv',
           'cryptography'
```

### Comparing `robin_stocks-2.1.0/tests/app_tests.py` & `robin_stocks-3.0.0/tests/app_tests.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/tests/test_gemini.py` & `robin_stocks-3.0.0/tests/test_gemini.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-2.1.0/tests/test_robinhood.py` & `robin_stocks-3.0.0/tests/test_robinhood.py`

 * *Files 2% similar despite different names*

```diff
@@ -810,7 +810,30 @@
         assert profile
 
     @pytest.mark.xfail()
     def test_login_failed(self):
         r.logout()
         profile = r.load_account_profile(info=None)
         assert profile
+
+class TestOrders:
+    @classmethod
+    def setup_class(cls):
+        totp  = pyotp.TOTP(os.environ['robin_mfa']).now()
+        login = r.login(os.environ['robin_username'], os.environ['robin_password'], mfa_code=totp)
+    
+    def test_find_stock_orders(cls):
+        def isFloat(f):
+            try:
+                float(f)
+                return True
+            except ValueError:
+                return False
+
+        orderHistory = r.find_stock_orders()
+        assert orderHistory
+
+        for order in orderHistory:
+            assert isFloat(order['quantity'])
+            assert isFloat(order['cumulative_quantity'])
+            if(order['state'] == 'filled'):
+                assert (order['quantity'] == order['cumulative_quantity'])
```

### Comparing `robin_stocks-2.1.0/tests/test_tda.py` & `robin_stocks-3.0.0/tests/test_tda.py`

 * *Files identical despite different names*

