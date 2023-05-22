# Comparing `tmp/askCO-0.0.2.tar.gz` & `tmp/askCO-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "askCO-0.0.2.tar", last modified: Thu May 18 02:24:02 2023, max compression
+gzip compressed data, was "askCO-0.0.3.tar", last modified: Mon May 22 02:24:03 2023, max compression
```

## Comparing `askCO-0.0.2.tar` & `askCO-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 02:24:02.791366 askCO-0.0.2/
--rw-rw-rw-   0        0        0      622 2023-05-18 02:24:02.791366 askCO-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3048 2023-05-17 02:06:05.000000 askCO-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 02:24:02.791366 askCO-0.0.2/askCO.egg-info/
--rw-rw-rw-   0        0        0      622 2023-05-18 02:24:02.000000 askCO-0.0.2/askCO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      134 2023-05-18 02:24:02.000000 askCO-0.0.2/askCO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 02:24:02.000000 askCO-0.0.2/askCO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 02:24:02.000000 askCO-0.0.2/askCO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 02:24:02.791366 askCO-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      826 2023-05-18 01:54:17.000000 askCO-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 02:24:03.554121 askCO-0.0.3/
+-rw-rw-rw-   0        0        0     3769 2023-05-22 02:24:03.554121 askCO-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3199 2023-05-22 02:18:06.000000 askCO-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 02:24:03.554121 askCO-0.0.3/askCO.egg-info/
+-rw-rw-rw-   0        0        0     3769 2023-05-22 02:24:03.000000 askCO-0.0.3/askCO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      162 2023-05-22 02:24:03.000000 askCO-0.0.3/askCO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 02:24:03.000000 askCO-0.0.3/askCO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-22 02:24:03.000000 askCO-0.0.3/askCO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 02:24:03.000000 askCO-0.0.3/askCO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 02:24:03.554121 askCO-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      806 2023-05-22 02:23:00.000000 askCO-0.0.3/setup.py
```

### Comparing `askCO-0.0.2/README.md` & `askCO-0.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 This script provides an interface for getting data from the Museum of New Zealand Te Papa Tongarewa. With it, you can run searches and request individual records, which are returned as python objects.
 
 See the [API documentation](https://data.tepapa.govt.nz/docs/) for what's available and how to construct searches.
 
 Te Papa's API requires a registration key in the headers of each request – go to https://data.tepapa.govt.nz/docs/register.html to register. I recommend adding the API key to an environment variable called 'TE-PAPA-KEY', and then calling that from your script to pass to askCO.
 
 ## Installation
-Clone this repo using `git clone`. Install the following packages:
-- Requests
+Install using pip: `pip install askCO`
 
-## Run a query
+askCO requires the `requests` module.
+
+## Run a search query
 The `tryCO.py` file lays out a prepared search for a page of `Myosotis` specimen records in the `Plants` collection. It calls the API key, sets functional and query parameters, and sets up then runs the search request.
 
 A `Search` request object uses:
 - `quiet`: Can be `True` or `False`. If False, askCO prints messages to the console like the URL being requested.
 - `timeout`: How long in seconds before the query times out.
 - `attempts`: How many times a single query will be retried after an error like a timeout or connection error.
 - `endpoint`: Which API endpoint to query. Defaults to `object` but others like `agent`, `taxon`, and `place` are available.
@@ -25,20 +26,24 @@
 - `start`: Where to begin the page of results. Useful when requesting subsequent pages of a search.
 
 The `Scroll` request object is similar, though it finds and returns all records, not just a page. It uses most of the same parameters, but not `start`. Scrolling works well with a `size` of `1000`. It can also use:
 - `duration`: How long to keep the scroll query alive for on the API side. Defaults to `1` minute.
 - `max_records`: How many records to retrieve, if you don't want everything.
 - `sleep`: How long to wait between requests for scroll pages. Set this to `0.1` to ensure you avoid getting rate limited.
 
-Search and scroll results are stored as a list of json objects in the `records` variable of the request object.
+Search and scroll results are stored as a list of dictionaries in the `records` attribute of the request object.
+
+HTTP status is stored as an integer in the `status_code` attribute.
 
 ## Get a record
 When requesting a single record, the `Resource` request object still uses:
 - `api_key`
 - `quiet`
 - `timeout`
 - `attempts`
 - `endpoint`
 
 It also takes an `irn` parameter, the specific number for that record within the endpoint. Make sure you've set the correct endpoint - /object/123456 isn't the same as /agent/123456.
 
-The record's data is stored as a json object in the `response_text` variable of the request object.
+The record's data is stored as a dictionary in the `response_text` attribute of the request object.
+
+HTTP status is stored as an integer in the `status_code` attribute.
```

