# Comparing `tmp/robin_stocks-3.0.0.tar.gz` & `tmp/robin_stocks-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/robin_stocks-3.0.0.tar", last modified: Mon May 22 01:15:38 2023, max compression
+gzip compressed data, was "robin_stocks-3.0.1.tar", last modified: Mon May 22 03:03:17 2023, max compression
```

## Comparing `robin_stocks-3.0.0.tar` & `robin_stocks-3.0.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 01:15:38.451269 robin_stocks-3.0.0/
--rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.0.0/LICENSE.txt
--rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.0.0/MANIFEST.in
--rw-r--r--   0 josh       (501) staff       (20)     5803 2023-05-22 01:15:38.450786 robin_stocks-3.0.0/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/README.rst
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 01:15:38.430340 robin_stocks-3.0.0/robin_stocks/
--rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/__init__.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 01:15:38.435842 robin_stocks-3.0.0/robin_stocks/gemini/
--rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/account.py
--rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/gemini/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 01:15:38.442599 robin_stocks-3.0.0/robin_stocks/robinhood/
--rw-r--r--   0 josh       (501) staff       (20)     5012 2021-02-23 04:31:10.000000 robin_stocks-3.0.0/robin_stocks/robinhood/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)    30654 2023-05-22 00:46:39.000000 robin_stocks-3.0.0/robin_stocks/robinhood/account.py
--rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.0.0/robin_stocks/robinhood/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.0.0/robin_stocks/robinhood/crypto.py
--rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.0.0/robin_stocks/robinhood/export.py
--rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/robinhood/globals.py
--rw-r--r--   0 josh       (501) staff       (20)    13217 2021-02-23 04:29:35.000000 robin_stocks-3.0.0/robin_stocks/robinhood/helper.py
--rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.0.0/robin_stocks/robinhood/markets.py
--rw-r--r--   0 josh       (501) staff       (20)    20319 2023-05-22 00:46:39.000000 robin_stocks-3.0.0/robin_stocks/robinhood/options.py
--rw-r--r--   0 josh       (501) staff       (20)    63387 2023-05-22 01:12:04.000000 robin_stocks-3.0.0/robin_stocks/robinhood/orders.py
--rw-r--r--   0 josh       (501) staff       (20)     9622 2023-05-22 00:46:39.000000 robin_stocks-3.0.0/robin_stocks/robinhood/profiles.py
--rw-r--r--   0 josh       (501) staff       (20)    25261 2023-05-22 01:12:04.000000 robin_stocks-3.0.0/robin_stocks/robinhood/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     7284 2023-05-22 00:46:39.000000 robin_stocks-3.0.0/robin_stocks/robinhood/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 01:15:38.446627 robin_stocks-3.0.0/robin_stocks/tda/
--rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/accounts.py
--rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/authentication.py
--rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/globals.py
--rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/helper.py
--rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/markets.py
--rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/orders.py
--rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.0.0/robin_stocks/tda/stocks.py
--rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/robin_stocks/tda/urls.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 01:15:38.432279 robin_stocks-3.0.0/robin_stocks.egg-info/
--rw-r--r--   0 josh       (501) staff       (20)     5803 2023-05-22 01:15:38.000000 robin_stocks-3.0.0/robin_stocks.egg-info/PKG-INFO
--rw-r--r--   0 josh       (501) staff       (20)     1330 2023-05-22 01:15:38.000000 robin_stocks-3.0.0/robin_stocks.egg-info/SOURCES.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2023-05-22 01:15:38.000000 robin_stocks-3.0.0/robin_stocks.egg-info/dependency_links.txt
--rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.0.0/robin_stocks.egg-info/not-zip-safe
--rw-r--r--   0 josh       (501) staff       (20)       42 2023-05-22 01:15:38.000000 robin_stocks-3.0.0/robin_stocks.egg-info/requires.txt
--rw-r--r--   0 josh       (501) staff       (20)       19 2023-05-22 01:15:38.000000 robin_stocks-3.0.0/robin_stocks.egg-info/top_level.txt
--rw-r--r--   0 josh       (501) staff       (20)       38 2023-05-22 01:15:38.451448 robin_stocks-3.0.0/setup.cfg
--rw-r--r--   0 josh       (501) staff       (20)      931 2023-05-22 01:12:25.000000 robin_stocks-3.0.0/setup.py
-drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 01:15:38.449585 robin_stocks-3.0.0/tests/
--rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.0.0/tests/__init__.py
--rw-r--r--   0 josh       (501) staff       (20)     9780 2021-10-20 03:47:23.000000 robin_stocks-3.0.0/tests/app_tests.py
--rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/tests/test_gemini.py
--rw-r--r--   0 josh       (501) staff       (20)    33003 2023-05-22 01:12:04.000000 robin_stocks-3.0.0/tests/test_robinhood.py
--rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.0.0/tests/test_tda.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 03:03:17.538196 robin_stocks-3.0.1/
+-rw-r--r--   0 josh       (501) staff       (20)     1062 2018-10-17 16:32:18.000000 robin_stocks-3.0.1/LICENSE.txt
+-rw-r--r--   0 josh       (501) staff       (20)       88 2018-09-27 04:22:53.000000 robin_stocks-3.0.1/MANIFEST.in
+-rw-r--r--   0 josh       (501) staff       (20)     5087 2023-05-22 03:03:17.537774 robin_stocks-3.0.1/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     4629 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/README.rst
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 03:03:17.518837 robin_stocks-3.0.1/robin_stocks/
+-rw-r--r--   0 josh       (501) staff       (20)       47 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/__init__.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 03:03:17.524616 robin_stocks-3.0.1/robin_stocks/gemini/
+-rw-r--r--   0 josh       (501) staff       (20)      789 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    12995 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     2499 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)    10801 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)      585 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     6140 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    18993 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     3859 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/gemini/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 03:03:17.530730 robin_stocks-3.0.1/robin_stocks/robinhood/
+-rw-r--r--   0 josh       (501) staff       (20)     5012 2021-02-23 04:31:10.000000 robin_stocks-3.0.1/robin_stocks/robinhood/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)    30654 2023-05-22 00:46:39.000000 robin_stocks-3.0.1/robin_stocks/robinhood/account.py
+-rw-r--r--   0 josh       (501) staff       (20)     8596 2021-10-20 03:38:49.000000 robin_stocks-3.0.1/robin_stocks/robinhood/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)     9715 2021-05-12 02:09:12.000000 robin_stocks-3.0.1/robin_stocks/robinhood/crypto.py
+-rw-r--r--   0 josh       (501) staff       (20)     6602 2023-05-22 00:46:39.000000 robin_stocks-3.0.1/robin_stocks/robinhood/export.py
+-rw-r--r--   0 josh       (501) staff       (20)      902 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/robinhood/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)    13217 2021-02-23 04:29:35.000000 robin_stocks-3.0.1/robin_stocks/robinhood/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)    11649 2021-02-27 17:30:21.000000 robin_stocks-3.0.1/robin_stocks/robinhood/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)    20319 2023-05-22 00:46:39.000000 robin_stocks-3.0.1/robin_stocks/robinhood/options.py
+-rw-r--r--   0 josh       (501) staff       (20)    63387 2023-05-22 01:12:04.000000 robin_stocks-3.0.1/robin_stocks/robinhood/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)     9622 2023-05-22 00:46:39.000000 robin_stocks-3.0.1/robin_stocks/robinhood/profiles.py
+-rw-r--r--   0 josh       (501) staff       (20)    25261 2023-05-22 01:12:04.000000 robin_stocks-3.0.1/robin_stocks/robinhood/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     7567 2023-05-22 02:23:50.000000 robin_stocks-3.0.1/robin_stocks/robinhood/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 03:03:17.534925 robin_stocks-3.0.1/robin_stocks/tda/
+-rw-r--r--   0 josh       (501) staff       (20)      713 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     4761 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/accounts.py
+-rw-r--r--   0 josh       (501) staff       (20)     6608 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/authentication.py
+-rw-r--r--   0 josh       (501) staff       (20)      753 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/globals.py
+-rw-r--r--   0 josh       (501) staff       (20)     9765 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/helper.py
+-rw-r--r--   0 josh       (501) staff       (20)     3433 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/markets.py
+-rw-r--r--   0 josh       (501) staff       (20)     4714 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/orders.py
+-rw-r--r--   0 josh       (501) staff       (20)    12030 2021-02-20 06:33:23.000000 robin_stocks-3.0.1/robin_stocks/tda/stocks.py
+-rw-r--r--   0 josh       (501) staff       (20)     3161 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/robin_stocks/tda/urls.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 03:03:17.520827 robin_stocks-3.0.1/robin_stocks.egg-info/
+-rw-r--r--   0 josh       (501) staff       (20)     5087 2023-05-22 03:03:17.000000 robin_stocks-3.0.1/robin_stocks.egg-info/PKG-INFO
+-rw-r--r--   0 josh       (501) staff       (20)     1330 2023-05-22 03:03:17.000000 robin_stocks-3.0.1/robin_stocks.egg-info/SOURCES.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2023-05-22 03:03:17.000000 robin_stocks-3.0.1/robin_stocks.egg-info/dependency_links.txt
+-rw-r--r--   0 josh       (501) staff       (20)        1 2018-02-23 03:52:33.000000 robin_stocks-3.0.1/robin_stocks.egg-info/not-zip-safe
+-rw-r--r--   0 josh       (501) staff       (20)       42 2023-05-22 03:03:17.000000 robin_stocks-3.0.1/robin_stocks.egg-info/requires.txt
+-rw-r--r--   0 josh       (501) staff       (20)       19 2023-05-22 03:03:17.000000 robin_stocks-3.0.1/robin_stocks.egg-info/top_level.txt
+-rw-r--r--   0 josh       (501) staff       (20)       38 2023-05-22 03:03:17.538312 robin_stocks-3.0.1/setup.cfg
+-rw-r--r--   0 josh       (501) staff       (20)      931 2023-05-22 03:00:44.000000 robin_stocks-3.0.1/setup.py
+drwxr-xr-x   0 josh       (501) staff       (20)        0 2023-05-22 03:03:17.537151 robin_stocks-3.0.1/tests/
+-rw-r--r--   0 josh       (501) staff       (20)        0 2020-06-15 04:00:04.000000 robin_stocks-3.0.1/tests/__init__.py
+-rw-r--r--   0 josh       (501) staff       (20)     9843 2023-05-22 02:31:15.000000 robin_stocks-3.0.1/tests/app_tests.py
+-rw-r--r--   0 josh       (501) staff       (20)     2157 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/tests/test_gemini.py
+-rw-r--r--   0 josh       (501) staff       (20)    32945 2023-05-22 02:32:23.000000 robin_stocks-3.0.1/tests/test_robinhood.py
+-rw-r--r--   0 josh       (501) staff       (20)      571 2021-02-20 06:32:12.000000 robin_stocks-3.0.1/tests/test_tda.py
```

### Comparing `robin_stocks-3.0.0/LICENSE.txt` & `robin_stocks-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/PKG-INFO` & `robin_stocks-3.0.1/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,105 +1,90 @@
-Metadata-Version: 2.1
-Name: robin_stocks
-Version: 3.0.0
-Summary: A Python wrapper around the Robinhood API
-Home-page: https://github.com/jmfernandes/robin_stocks
-Author: Josh Fernandes
-Author-email: joshfernandes@mac.com
-License: MIT
-Description: .. image:: docs/source/_static/pics/title.PNG
-        
-        Robin-Stocks API Library
-        ========================
-        This library provides a pure python interface to interact with the Robinhood API, Gemini API,
-        and TD Ameritrade API. The code is simple to use, easy to understand, and easy to modify.
-        With this library you can view information on stocks, options, and crypto-currencies in real time, 
-        create your own robo-investor or trading algorithm, and improve your programming skills.
-        
-        To join our Slack channel where you can discuss trading and coding, click the link https://join.slack.com/t/robin-stocks/shared_invite/zt-7up2htza-wNSil5YDa3zrAglFFSxRIA
-        
-        Supported APIs
-        ==============
-        The supported APIs are Robinhood, Gemini, and TD Ameritrade. For more information about how to use the different APIs, visit the README
-        documents for `Robinhood Documentation`_, `Gemini Documentation`_, and `TDA Documentation`_.
-        
-        Below are examples on how to call each of those modules.
-        
-        >>> import robin_stocks.robinhood as rh
-        >>> import robin_stocks.gemini as gem
-        >>> import robin_stocks.tda as tda
-        >>> # Here are some example calls
-        >>> gem.get_pubticker("btcusd") # gets ticker information for Bitcoin from Gemini
-        >>> rh.get_all_open_crypto_orders() # gets all cypto orders from Robinhood
-        >>> tda.get_price_history("tsla") # get price history from TD Ameritrade 
-        
-        Contributing
-        ============
-        If you would like to contribute to this project, follow our contributing guidelines `Here <https://github.com/jmfernandes/robin_stocks/blob/master/contributing.md>`_.
-        
-        Automatic Testing
-        ^^^^^^^^^^^^^^^^^
-        
-        If you are contributing to this project and would like to use automatic testing for your changes, you will need to install pytest and pytest-dotenv. To do this type into terminal or command prompt:
-        
-        >>> pip install pytest
-        >>> pip install pytest-dotenv
-        
-        You will also need to fill out all the fields in .test.env. I recommend that you rename the file as .env once you are done adding in all your personal information. After that, you can simply run:
-        
-        >>> pytest
-        
-        to run all the tests. If you would like to run specific tests or run all the tests in a specific class then type:
-        
-        >>> pytest tests/test_robinhood.py -k test_name_apple # runs only the 1 test
-        >>> pytest tests/test_gemini.py -k TestTrades # runs every test in TestTrades but nothing else
-        
-        Finally, if you would like the API calls to print out to terminal, then add the -s flag to any of the above pytest calls.
-        
-        
-        Installing
-        ========================
-        There is no need to download these files directly. This project is published on PyPi,
-        so it can be installed by typing into terminal (on Mac) or into command prompt (on PC):
-        
-        >>> pip install robin_stocks
-        
-        Also be sure that Python 3 is installed. If you need to install python you can download it from `Python.org <https://www.python.org/downloads/>`_.
-        Pip is the package installer for python, and is automatically installed when you install python. To learn more about Pip, you can go to `PyPi.org <https://pypi.org/project/pip/>`_.
-        
-        If you would like to be able to make changes to the package yourself, clone the repository onto your computer by typing into terminal or command prompt:
-        
-        >>> git clone https://github.com/jmfernandes/robin_stocks.git
-        >>> cd robin_stocks
-        
-        Now that you have cd into the repository you can type
-        
-        >>> pip install .
-        
-        and this will install whatever you changed in the local files. This will allow you to make changes and experiment with your own code.
-        
-        List of Functions and Example Usage
-        ===================================
-        
-        For a complete list of all Robinhood API functions and what the different parameters mean, 
-        go to `robin-stocks.com Robinhood Page <http://www.robin-stocks.com/en/latest/robinhood.html>`_. If you would like to
-        see some example code and instructions on how to set up two-factor authorization for Robinhood,
-        go to the `Robinhood Documentation`_.
-        
-        For a complete list of all TD Ameritrade API functions and what the different parameters mean, 
-        go to `robin-stocks.com TDA Page <http://www.robin-stocks.com/en/latest/tda.html>`_. For detailed instructions on 
-        how to generate API keys for TD Ameritrade and how to use the API, go to the `TDA Documentation`_.
-        
-        For a complete list of all Gemini API functions and what the different parameters mean, 
-        go to `robin-stocks.com Gemeni Page <http://www.robin-stocks.com/en/latest/gemini.html>`_. For detailed instructions on 
-        how to generate API keys for Gemini and how to use both the private and public API, go to the `Gemini Documentation`_.
-        
-        .. _Robinhood Documentation: Robinhood.rst
-        .. _Gemini Documentation: gemini.rst
-        .. _TDA Documentation: tda.rst
-Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
-Platform: UNKNOWN
-Requires: requests
-Requires: pyotp
-Requires: cryptography
-Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+.. image:: docs/source/_static/pics/title.PNG
+
+Robin-Stocks API Library
+========================
+This library provides a pure python interface to interact with the Robinhood API, Gemini API,
+and TD Ameritrade API. The code is simple to use, easy to understand, and easy to modify.
+With this library you can view information on stocks, options, and crypto-currencies in real time, 
+create your own robo-investor or trading algorithm, and improve your programming skills.
+
+To join our Slack channel where you can discuss trading and coding, click the link https://join.slack.com/t/robin-stocks/shared_invite/zt-7up2htza-wNSil5YDa3zrAglFFSxRIA
+
+Supported APIs
+==============
+The supported APIs are Robinhood, Gemini, and TD Ameritrade. For more information about how to use the different APIs, visit the README
+documents for `Robinhood Documentation`_, `Gemini Documentation`_, and `TDA Documentation`_.
+
+Below are examples on how to call each of those modules.
+
+>>> import robin_stocks.robinhood as rh
+>>> import robin_stocks.gemini as gem
+>>> import robin_stocks.tda as tda
+>>> # Here are some example calls
+>>> gem.get_pubticker("btcusd") # gets ticker information for Bitcoin from Gemini
+>>> rh.get_all_open_crypto_orders() # gets all cypto orders from Robinhood
+>>> tda.get_price_history("tsla") # get price history from TD Ameritrade 
+
+Contributing
+============
+If you would like to contribute to this project, follow our contributing guidelines `Here <https://github.com/jmfernandes/robin_stocks/blob/master/contributing.md>`_.
+
+Automatic Testing
+^^^^^^^^^^^^^^^^^
+
+If you are contributing to this project and would like to use automatic testing for your changes, you will need to install pytest and pytest-dotenv. To do this type into terminal or command prompt:
+
+>>> pip install pytest
+>>> pip install pytest-dotenv
+
+You will also need to fill out all the fields in .test.env. I recommend that you rename the file as .env once you are done adding in all your personal information. After that, you can simply run:
+
+>>> pytest
+
+to run all the tests. If you would like to run specific tests or run all the tests in a specific class then type:
+
+>>> pytest tests/test_robinhood.py -k test_name_apple # runs only the 1 test
+>>> pytest tests/test_gemini.py -k TestTrades # runs every test in TestTrades but nothing else
+
+Finally, if you would like the API calls to print out to terminal, then add the -s flag to any of the above pytest calls.
+
+
+Installing
+========================
+There is no need to download these files directly. This project is published on PyPi,
+so it can be installed by typing into terminal (on Mac) or into command prompt (on PC):
+
+>>> pip install robin_stocks
+
+Also be sure that Python 3 is installed. If you need to install python you can download it from `Python.org <https://www.python.org/downloads/>`_.
+Pip is the package installer for python, and is automatically installed when you install python. To learn more about Pip, you can go to `PyPi.org <https://pypi.org/project/pip/>`_.
+
+If you would like to be able to make changes to the package yourself, clone the repository onto your computer by typing into terminal or command prompt:
+
+>>> git clone https://github.com/jmfernandes/robin_stocks.git
+>>> cd robin_stocks
+
+Now that you have cd into the repository you can type
+
+>>> pip install .
+
+and this will install whatever you changed in the local files. This will allow you to make changes and experiment with your own code.
+
+List of Functions and Example Usage
+===================================
+
+For a complete list of all Robinhood API functions and what the different parameters mean, 
+go to `robin-stocks.com Robinhood Page <http://www.robin-stocks.com/en/latest/robinhood.html>`_. If you would like to
+see some example code and instructions on how to set up two-factor authorization for Robinhood,
+go to the `Robinhood Documentation`_.
+
+For a complete list of all TD Ameritrade API functions and what the different parameters mean, 
+go to `robin-stocks.com TDA Page <http://www.robin-stocks.com/en/latest/tda.html>`_. For detailed instructions on 
+how to generate API keys for TD Ameritrade and how to use the API, go to the `TDA Documentation`_.
+
+For a complete list of all Gemini API functions and what the different parameters mean, 
+go to `robin-stocks.com Gemeni Page <http://www.robin-stocks.com/en/latest/gemini.html>`_. For detailed instructions on 
+how to generate API keys for Gemini and how to use both the private and public API, go to the `Gemini Documentation`_.
+
+.. _Robinhood Documentation: Robinhood.rst
+.. _Gemini Documentation: gemini.rst
+.. _TDA Documentation: tda.rst
```

### Comparing `robin_stocks-3.0.0/README.rst` & `robin_stocks-3.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: robin_stocks
+Version: 3.0.1
+Summary: A Python wrapper around the Robinhood API
+Home-page: https://github.com/jmfernandes/robin_stocks
+Author: Josh Fernandes
+Author-email: joshfernandes@mac.com
+License: MIT
+Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
+Requires: requests
+Requires: pyotp
+Requires: cryptography
+Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
 .. image:: docs/source/_static/pics/title.PNG
 
 Robin-Stocks API Library
 ========================
 This library provides a pure python interface to interact with the Robinhood API, Gemini API,
 and TD Ameritrade API. The code is simple to use, easy to understand, and easy to modify.
 With this library you can view information on stocks, options, and crypto-currencies in real time, 
@@ -83,8 +99,8 @@
 
 For a complete list of all Gemini API functions and what the different parameters mean, 
 go to `robin-stocks.com Gemeni Page <http://www.robin-stocks.com/en/latest/gemini.html>`_. For detailed instructions on 
 how to generate API keys for Gemini and how to use both the private and public API, go to the `Gemini Documentation`_.
 
 .. _Robinhood Documentation: Robinhood.rst
 .. _Gemini Documentation: gemini.rst
-.. _TDA Documentation: tda.rst
+.. _TDA Documentation: tda.rst
```

### Comparing `robin_stocks-3.0.0/robin_stocks/gemini/__init__.py` & `robin_stocks-3.0.1/robin_stocks/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/gemini/account.py` & `robin_stocks-3.0.1/robin_stocks/gemini/account.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/gemini/authentication.py` & `robin_stocks-3.0.1/robin_stocks/gemini/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/gemini/crypto.py` & `robin_stocks-3.0.1/robin_stocks/gemini/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/gemini/globals.py` & `robin_stocks-3.0.1/robin_stocks/gemini/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/gemini/helper.py` & `robin_stocks-3.0.1/robin_stocks/gemini/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/gemini/orders.py` & `robin_stocks-3.0.1/robin_stocks/gemini/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/gemini/urls.py` & `robin_stocks-3.0.1/robin_stocks/gemini/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/robinhood/__init__.py` & `robin_stocks-3.0.1/robin_stocks/robinhood/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/robinhood/account.py` & `robin_stocks-3.0.1/robin_stocks/robinhood/account.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/robinhood/authentication.py` & `robin_stocks-3.0.1/robin_stocks/robinhood/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/robinhood/crypto.py` & `robin_stocks-3.0.1/robin_stocks/robinhood/crypto.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/robinhood/export.py` & `robin_stocks-3.0.1/robin_stocks/robinhood/export.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/robinhood/globals.py` & `robin_stocks-3.0.1/robin_stocks/robinhood/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/robinhood/helper.py` & `robin_stocks-3.0.1/robin_stocks/robinhood/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/robinhood/markets.py` & `robin_stocks-3.0.1/robin_stocks/robinhood/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/robinhood/options.py` & `robin_stocks-3.0.1/robin_stocks/robinhood/options.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/robinhood/orders.py` & `robin_stocks-3.0.1/robin_stocks/robinhood/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/robinhood/profiles.py` & `robin_stocks-3.0.1/robin_stocks/robinhood/profiles.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/robinhood/stocks.py` & `robin_stocks-3.0.1/robin_stocks/robinhood/stocks.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/robinhood/urls.py` & `robin_stocks-3.0.1/robin_stocks/robinhood/urls.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 def challenge_url(challenge_id):
     return('https://api.robinhood.com/challenge/{0}/respond/'.format(challenge_id))
 
 # Profiles
 
 
 def account_profile_url(account_number=None):
-    return('https://api.robinhood.com/accounts/'+account_number)
+    if account_number:
+        return('https://api.robinhood.com/accounts/'+account_number)
+    else:
+        return('https://api.robinhood.com/accounts/')
 
 
 def basic_profile_url():
     return('https://api.robinhood.com/user/basic_info/')
 
 
 def investment_profile_url():
@@ -83,15 +86,18 @@
 
 # account
 
 def phoenix_url():
     return('https://phoenix.robinhood.com/accounts/unified')
 
 def positions_url(account_number=None):
-    return('https://api.robinhood.com/positions/?account_number='+account_number)
+    if account_number:
+        return('https://api.robinhood.com/positions/?account_number='+account_number)
+    else:
+        return('https://api.robinhood.com/positions/')
 
 def banktransfers_url(direction=None):
     if direction == 'received':
         return('https://api.robinhood.com/ach/received/transfers/')
     else:
         return('https://api.robinhood.com/ach/transfers/')
 
@@ -209,15 +215,18 @@
     if orderID:
         return('https://api.robinhood.com/options/orders/{0}/'.format(orderID))
     else:
         return('https://api.robinhood.com/options/orders/')
 
 
 def option_positions_url(account_number):
-    return('https://api.robinhood.com/options/positions/?account_numbers='+account_number)
+    if account_number:
+        return('https://api.robinhood.com/options/positions/?account_numbers='+account_number)
+    else:
+        return('https://api.robinhood.com/options/positions/')
 
 
 def marketdata_options_url():
     return('https://api.robinhood.com/marketdata/options/')
 
 # pricebook
```

### Comparing `robin_stocks-3.0.0/robin_stocks/tda/__init__.py` & `robin_stocks-3.0.1/robin_stocks/tda/__init__.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/tda/accounts.py` & `robin_stocks-3.0.1/robin_stocks/tda/accounts.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/tda/authentication.py` & `robin_stocks-3.0.1/robin_stocks/tda/authentication.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/tda/globals.py` & `robin_stocks-3.0.1/robin_stocks/tda/globals.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/tda/helper.py` & `robin_stocks-3.0.1/robin_stocks/tda/helper.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/tda/markets.py` & `robin_stocks-3.0.1/robin_stocks/tda/markets.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/tda/orders.py` & `robin_stocks-3.0.1/robin_stocks/tda/orders.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/tda/stocks.py` & `robin_stocks-3.0.1/robin_stocks/tda/stocks.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks/tda/urls.py` & `robin_stocks-3.0.1/robin_stocks/tda/urls.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/robin_stocks.egg-info/PKG-INFO` & `robin_stocks-3.0.1/robin_stocks.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,105 +1,106 @@
 Metadata-Version: 2.1
 Name: robin-stocks
-Version: 3.0.0
+Version: 3.0.1
 Summary: A Python wrapper around the Robinhood API
 Home-page: https://github.com/jmfernandes/robin_stocks
 Author: Josh Fernandes
 Author-email: joshfernandes@mac.com
 License: MIT
-Description: .. image:: docs/source/_static/pics/title.PNG
-        
-        Robin-Stocks API Library
-        ========================
-        This library provides a pure python interface to interact with the Robinhood API, Gemini API,
-        and TD Ameritrade API. The code is simple to use, easy to understand, and easy to modify.
-        With this library you can view information on stocks, options, and crypto-currencies in real time, 
-        create your own robo-investor or trading algorithm, and improve your programming skills.
-        
-        To join our Slack channel where you can discuss trading and coding, click the link https://join.slack.com/t/robin-stocks/shared_invite/zt-7up2htza-wNSil5YDa3zrAglFFSxRIA
-        
-        Supported APIs
-        ==============
-        The supported APIs are Robinhood, Gemini, and TD Ameritrade. For more information about how to use the different APIs, visit the README
-        documents for `Robinhood Documentation`_, `Gemini Documentation`_, and `TDA Documentation`_.
-        
-        Below are examples on how to call each of those modules.
-        
-        >>> import robin_stocks.robinhood as rh
-        >>> import robin_stocks.gemini as gem
-        >>> import robin_stocks.tda as tda
-        >>> # Here are some example calls
-        >>> gem.get_pubticker("btcusd") # gets ticker information for Bitcoin from Gemini
-        >>> rh.get_all_open_crypto_orders() # gets all cypto orders from Robinhood
-        >>> tda.get_price_history("tsla") # get price history from TD Ameritrade 
-        
-        Contributing
-        ============
-        If you would like to contribute to this project, follow our contributing guidelines `Here <https://github.com/jmfernandes/robin_stocks/blob/master/contributing.md>`_.
-        
-        Automatic Testing
-        ^^^^^^^^^^^^^^^^^
-        
-        If you are contributing to this project and would like to use automatic testing for your changes, you will need to install pytest and pytest-dotenv. To do this type into terminal or command prompt:
-        
-        >>> pip install pytest
-        >>> pip install pytest-dotenv
-        
-        You will also need to fill out all the fields in .test.env. I recommend that you rename the file as .env once you are done adding in all your personal information. After that, you can simply run:
-        
-        >>> pytest
-        
-        to run all the tests. If you would like to run specific tests or run all the tests in a specific class then type:
-        
-        >>> pytest tests/test_robinhood.py -k test_name_apple # runs only the 1 test
-        >>> pytest tests/test_gemini.py -k TestTrades # runs every test in TestTrades but nothing else
-        
-        Finally, if you would like the API calls to print out to terminal, then add the -s flag to any of the above pytest calls.
-        
-        
-        Installing
-        ========================
-        There is no need to download these files directly. This project is published on PyPi,
-        so it can be installed by typing into terminal (on Mac) or into command prompt (on PC):
-        
-        >>> pip install robin_stocks
-        
-        Also be sure that Python 3 is installed. If you need to install python you can download it from `Python.org <https://www.python.org/downloads/>`_.
-        Pip is the package installer for python, and is automatically installed when you install python. To learn more about Pip, you can go to `PyPi.org <https://pypi.org/project/pip/>`_.
-        
-        If you would like to be able to make changes to the package yourself, clone the repository onto your computer by typing into terminal or command prompt:
-        
-        >>> git clone https://github.com/jmfernandes/robin_stocks.git
-        >>> cd robin_stocks
-        
-        Now that you have cd into the repository you can type
-        
-        >>> pip install .
-        
-        and this will install whatever you changed in the local files. This will allow you to make changes and experiment with your own code.
-        
-        List of Functions and Example Usage
-        ===================================
-        
-        For a complete list of all Robinhood API functions and what the different parameters mean, 
-        go to `robin-stocks.com Robinhood Page <http://www.robin-stocks.com/en/latest/robinhood.html>`_. If you would like to
-        see some example code and instructions on how to set up two-factor authorization for Robinhood,
-        go to the `Robinhood Documentation`_.
-        
-        For a complete list of all TD Ameritrade API functions and what the different parameters mean, 
-        go to `robin-stocks.com TDA Page <http://www.robin-stocks.com/en/latest/tda.html>`_. For detailed instructions on 
-        how to generate API keys for TD Ameritrade and how to use the API, go to the `TDA Documentation`_.
-        
-        For a complete list of all Gemini API functions and what the different parameters mean, 
-        go to `robin-stocks.com Gemeni Page <http://www.robin-stocks.com/en/latest/gemini.html>`_. For detailed instructions on 
-        how to generate API keys for Gemini and how to use both the private and public API, go to the `Gemini Documentation`_.
-        
-        .. _Robinhood Documentation: Robinhood.rst
-        .. _Gemini Documentation: gemini.rst
-        .. _TDA Documentation: tda.rst
 Keywords: robinhood,robin stocks,finance app,stocks,options,trading,investing
-Platform: UNKNOWN
 Requires: requests
 Requires: pyotp
 Requires: cryptography
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
+
+.. image:: docs/source/_static/pics/title.PNG
+
+Robin-Stocks API Library
+========================
+This library provides a pure python interface to interact with the Robinhood API, Gemini API,
+and TD Ameritrade API. The code is simple to use, easy to understand, and easy to modify.
+With this library you can view information on stocks, options, and crypto-currencies in real time, 
+create your own robo-investor or trading algorithm, and improve your programming skills.
+
+To join our Slack channel where you can discuss trading and coding, click the link https://join.slack.com/t/robin-stocks/shared_invite/zt-7up2htza-wNSil5YDa3zrAglFFSxRIA
+
+Supported APIs
+==============
+The supported APIs are Robinhood, Gemini, and TD Ameritrade. For more information about how to use the different APIs, visit the README
+documents for `Robinhood Documentation`_, `Gemini Documentation`_, and `TDA Documentation`_.
+
+Below are examples on how to call each of those modules.
+
+>>> import robin_stocks.robinhood as rh
+>>> import robin_stocks.gemini as gem
+>>> import robin_stocks.tda as tda
+>>> # Here are some example calls
+>>> gem.get_pubticker("btcusd") # gets ticker information for Bitcoin from Gemini
+>>> rh.get_all_open_crypto_orders() # gets all cypto orders from Robinhood
+>>> tda.get_price_history("tsla") # get price history from TD Ameritrade 
+
+Contributing
+============
+If you would like to contribute to this project, follow our contributing guidelines `Here <https://github.com/jmfernandes/robin_stocks/blob/master/contributing.md>`_.
+
+Automatic Testing
+^^^^^^^^^^^^^^^^^
+
+If you are contributing to this project and would like to use automatic testing for your changes, you will need to install pytest and pytest-dotenv. To do this type into terminal or command prompt:
+
+>>> pip install pytest
+>>> pip install pytest-dotenv
+
+You will also need to fill out all the fields in .test.env. I recommend that you rename the file as .env once you are done adding in all your personal information. After that, you can simply run:
+
+>>> pytest
+
+to run all the tests. If you would like to run specific tests or run all the tests in a specific class then type:
+
+>>> pytest tests/test_robinhood.py -k test_name_apple # runs only the 1 test
+>>> pytest tests/test_gemini.py -k TestTrades # runs every test in TestTrades but nothing else
+
+Finally, if you would like the API calls to print out to terminal, then add the -s flag to any of the above pytest calls.
+
+
+Installing
+========================
+There is no need to download these files directly. This project is published on PyPi,
+so it can be installed by typing into terminal (on Mac) or into command prompt (on PC):
+
+>>> pip install robin_stocks
+
+Also be sure that Python 3 is installed. If you need to install python you can download it from `Python.org <https://www.python.org/downloads/>`_.
+Pip is the package installer for python, and is automatically installed when you install python. To learn more about Pip, you can go to `PyPi.org <https://pypi.org/project/pip/>`_.
+
+If you would like to be able to make changes to the package yourself, clone the repository onto your computer by typing into terminal or command prompt:
+
+>>> git clone https://github.com/jmfernandes/robin_stocks.git
+>>> cd robin_stocks
+
+Now that you have cd into the repository you can type
+
+>>> pip install .
+
+and this will install whatever you changed in the local files. This will allow you to make changes and experiment with your own code.
+
+List of Functions and Example Usage
+===================================
+
+For a complete list of all Robinhood API functions and what the different parameters mean, 
+go to `robin-stocks.com Robinhood Page <http://www.robin-stocks.com/en/latest/robinhood.html>`_. If you would like to
+see some example code and instructions on how to set up two-factor authorization for Robinhood,
+go to the `Robinhood Documentation`_.
+
+For a complete list of all TD Ameritrade API functions and what the different parameters mean, 
+go to `robin-stocks.com TDA Page <http://www.robin-stocks.com/en/latest/tda.html>`_. For detailed instructions on 
+how to generate API keys for TD Ameritrade and how to use the API, go to the `TDA Documentation`_.
+
+For a complete list of all Gemini API functions and what the different parameters mean, 
+go to `robin-stocks.com Gemeni Page <http://www.robin-stocks.com/en/latest/gemini.html>`_. For detailed instructions on 
+how to generate API keys for Gemini and how to use both the private and public API, go to the `Gemini Documentation`_.
+
+.. _Robinhood Documentation: Robinhood.rst
+.. _Gemini Documentation: gemini.rst
+.. _TDA Documentation: tda.rst
```

### Comparing `robin_stocks-3.0.0/robin_stocks.egg-info/SOURCES.txt` & `robin_stocks-3.0.1/robin_stocks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/setup.py` & `robin_stocks-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='robin_stocks',
-      version='3.0.0',
+      version='3.0.1',
       description='A Python wrapper around the Robinhood API',
       long_description=long_description,
       long_description_content_type='text/x-rst',
       url='https://github.com/jmfernandes/robin_stocks',
       author='Josh Fernandes',
       author_email='joshfernandes@mac.com',
       keywords=['robinhood','robin stocks','finance app','stocks','options','trading','investing'],
```

### Comparing `robin_stocks-3.0.0/tests/app_tests.py` & `robin_stocks-3.0.1/tests/app_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,19 +7,21 @@
 load_dotenv()
 import requests
 
 import robin_stocks.robinhood as r
 import robin_stocks.gemini as g
 import robin_stocks.tda as t
 
+single_stock = 'AAPL'
 
 totp  = pyotp.TOTP(os.environ['robin_mfa']).now()
 print("Current OTP:", totp)
 login = r.login(os.environ['robin_username'], os.environ['robin_password'], store_session=True, mfa_code=totp)
 print("login data is ", login)
+print(r.load_account_profile(info=None))
 exit()
 # print("===")
 # print("running test at {}".format(datetime.datetime.now()))
 # print("===")
 
 # order = r.get_watchlist_by_name("test")
 # print(order)
```

### Comparing `robin_stocks-3.0.0/tests/test_gemini.py` & `robin_stocks-3.0.1/tests/test_gemini.py`

 * *Files identical despite different names*

### Comparing `robin_stocks-3.0.0/tests/test_robinhood.py` & `robin_stocks-3.0.1/tests/test_robinhood.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     # Set up variables for class
     single_stock = 'AAPL'
     event_stock = 'USO1'
     fake_stock = 'thisisfake'
     instrument = 'https://api.robinhood.com/instruments/450dfc6d-5510-4d40-abfb-f633b7d9be3e/'
     fake_instrument = 'https://api.robinhood.com/instruments/aaaaaaaa-0000-0000-0000-aaaaaaaaaaaa/'
     id = '450dfc6d-5510-4d40-abfb-f633b7d9be3e'
-    list_stocks = ['tsla', 'f', 'plug', 'fB', 'SPY', 'botz', 'jnug']
+    list_stocks = ['tsla', 'f', 'plug', 'meTA', 'SPY', 'botz', 'jnug']
     fake_stocks = ['87627273', 'ffffffffff']
 
     @classmethod
     def setup_class(cls):
         totp  = pyotp.TOTP(os.environ['robin_mfa']).now()
         login = r.login(os.environ['robin_username'], os.environ['robin_password'], mfa_code=totp)
 
@@ -684,15 +684,14 @@
         assert ('eligible_for_drip' in profile)
         assert ('eligible_for_cash_management' in profile)
         assert ('cash_management_enabled' in profile)
         assert ('option_trading_on_expiration_enabled' in profile)
         assert ('cash_held_for_options_collateral' in profile)
         assert ('fractional_position_closing_only' in profile)
         assert ('user_id' in profile)
-        assert ('rhs_stock_loan_consent_status' in profile)
 
     def test_basic_profile(self):
         profile = r.load_basic_profile(info=None)
         assert profile
         assert ('user' in profile)
         assert ('address' in profile)
         assert ('city' in profile)
```

### Comparing `robin_stocks-3.0.0/tests/test_tda.py` & `robin_stocks-3.0.1/tests/test_tda.py`

 * *Files identical despite different names*

