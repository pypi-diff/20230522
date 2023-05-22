# Comparing `tmp/pytest-tally-1.2.0.tar.gz` & `tmp/pytest-tally-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-tally-1.2.0.tar", last modified: Sat May 20 07:40:22 2023, max compression
+gzip compressed data, was "pytest-tally-1.3.0.tar", last modified: Mon May 22 05:39:53 2023, max compression
```

## Comparing `pytest-tally-1.2.0.tar` & `pytest-tally-1.3.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-20 07:40:22.064190 pytest-tally-1.2.0/
--rw-r--r--   0 jwr003   (623385768) 542971493      139 2023-04-15 00:11:14.000000 pytest-tally-1.2.0/.flake8
--rw-r--r--   0 jwr003   (623385768) 542971493     1900 2023-04-19 18:50:46.000000 pytest-tally-1.2.0/.gitignore
--rw-r--r--   0 jwr003   (623385768) 542971493       25 2023-04-15 00:11:48.000000 pytest-tally-1.2.0/.isort.cfg
--rw-r--r--   0 jwr003   (623385768) 542971493      419 2023-04-15 03:02:55.000000 pytest-tally-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 jwr003   (623385768) 542971493     1068 2023-03-03 22:12:17.000000 pytest-tally-1.2.0/LICENSE
--rw-r--r--   0 jwr003   (623385768) 542971493     4841 2023-05-20 07:40:22.063186 pytest-tally-1.2.0/PKG-INFO
--rw-r--r--   0 jwr003   (623385768) 542971493     3924 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/README.md
--rw-r--r--   0 jwr003   (623385768) 542971493       30 2023-03-05 22:13:29.000000 pytest-tally-1.2.0/conftest.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-20 07:40:21.955987 pytest-tally-1.2.0/misc/
--rw-r--r--   0 jwr003   (623385768) 542971493     1346 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/misc/CHANGELOG.md
--rw-r--r--   0 jwr003   (623385768) 542971493     1698 2023-04-14 05:16:42.000000 pytest-tally-1.2.0/misc/RELEASE_INSTRUCTIONS
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-20 07:40:21.961205 pytest-tally-1.2.0/pytest_tally/
--rw-r--r--   0 jwr003   (623385768) 542971493      144 2023-03-06 07:36:18.000000 pytest-tally-1.2.0/pytest_tally/__init__.py
--rw-r--r--   0 jwr003   (623385768) 542971493     3466 2023-04-20 02:27:46.000000 pytest-tally-1.2.0/pytest_tally/classes.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-20 07:40:22.006699 pytest-tally-1.2.0/pytest_tally/clients/
--rw-r--r--   0 jwr003   (623385768) 542971493     3200 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/pytest_tally/clients/app.py
--rw-r--r--   0 jwr003   (623385768) 542971493    11206 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/pytest_tally/clients/rich_dashboard.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-20 07:40:22.039559 pytest-tally-1.2.0/pytest_tally/clients/templates/
--rw-r--r--   0 jwr003   (623385768) 542971493    11749 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/pytest_tally/clients/templates/index.html
--rw-r--r--   0 jwr003   (623385768) 542971493     8250 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/pytest_tally/plugin.py
--rw-r--r--   0 jwr003   (623385768) 542971493     2826 2023-04-13 09:21:48.000000 pytest-tally-1.2.0/pytest_tally/pytest_reportlog.py
--rw-r--r--   0 jwr003   (623385768) 542971493     2687 2023-04-19 18:51:00.000000 pytest-tally-1.2.0/pytest_tally/utils.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-20 07:40:21.970415 pytest-tally-1.2.0/pytest_tally.egg-info/
--rw-r--r--   0 jwr003   (623385768) 542971493     4841 2023-05-20 07:40:21.000000 pytest-tally-1.2.0/pytest_tally.egg-info/PKG-INFO
--rw-r--r--   0 jwr003   (623385768) 542971493      716 2023-05-20 07:40:21.000000 pytest-tally-1.2.0/pytest_tally.egg-info/SOURCES.txt
--rw-r--r--   0 jwr003   (623385768) 542971493        1 2023-05-20 07:40:21.000000 pytest-tally-1.2.0/pytest_tally.egg-info/dependency_links.txt
--rw-r--r--   0 jwr003   (623385768) 542971493      163 2023-05-20 07:40:21.000000 pytest-tally-1.2.0/pytest_tally.egg-info/entry_points.txt
--rw-r--r--   0 jwr003   (623385768) 542971493      130 2023-05-20 07:40:21.000000 pytest-tally-1.2.0/pytest_tally.egg-info/requires.txt
--rw-r--r--   0 jwr003   (623385768) 542971493       13 2023-05-20 07:40:21.000000 pytest-tally-1.2.0/pytest_tally.egg-info/top_level.txt
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-20 07:40:22.061710 pytest-tally-1.2.0/requirements/
--rw-r--r--   0 jwr003   (623385768) 542971493       99 2023-04-15 00:12:58.000000 pytest-tally-1.2.0/requirements/requirements-dev.in
--rw-r--r--   0 jwr003   (623385768) 542971493     2882 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/requirements/requirements-dev.txt
--rw-r--r--   0 jwr003   (623385768) 542971493       95 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/requirements/requirements.in
--rw-r--r--   0 jwr003   (623385768) 542971493      987 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/requirements/requirements.txt
--rw-r--r--   0 jwr003   (623385768) 542971493       38 2023-05-20 07:40:22.064406 pytest-tally-1.2.0/setup.cfg
--rw-r--r--   0 jwr003   (623385768) 542971493     1920 2023-05-20 07:39:29.000000 pytest-tally-1.2.0/setup.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:39:53.667449 pytest-tally-1.3.0/
+-rw-r--r--   0 jwr003   (623385768) 542971493      139 2023-04-15 00:11:14.000000 pytest-tally-1.3.0/.flake8
+-rw-r--r--   0 jwr003   (623385768) 542971493     1900 2023-04-19 18:50:46.000000 pytest-tally-1.3.0/.gitignore
+-rw-r--r--   0 jwr003   (623385768) 542971493       25 2023-04-15 00:11:48.000000 pytest-tally-1.3.0/.isort.cfg
+-rw-r--r--   0 jwr003   (623385768) 542971493      419 2023-04-15 03:02:55.000000 pytest-tally-1.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 jwr003   (623385768) 542971493     1068 2023-03-03 22:12:17.000000 pytest-tally-1.3.0/LICENSE
+-rw-r--r--   0 jwr003   (623385768) 542971493     5802 2023-05-22 05:39:53.666384 pytest-tally-1.3.0/PKG-INFO
+-rw-r--r--   0 jwr003   (623385768) 542971493     4885 2023-05-22 05:38:40.000000 pytest-tally-1.3.0/README.md
+-rw-r--r--   0 jwr003   (623385768) 542971493       30 2023-03-05 22:13:29.000000 pytest-tally-1.3.0/conftest.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:39:53.560828 pytest-tally-1.3.0/misc/
+-rw-r--r--   0 jwr003   (623385768) 542971493     1390 2023-05-22 05:09:41.000000 pytest-tally-1.3.0/misc/CHANGELOG.md
+-rw-r--r--   0 jwr003   (623385768) 542971493     1698 2023-04-14 05:16:42.000000 pytest-tally-1.3.0/misc/RELEASE_INSTRUCTIONS
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:39:53.567956 pytest-tally-1.3.0/pytest_tally/
+-rw-r--r--   0 jwr003   (623385768) 542971493      144 2023-03-06 07:36:18.000000 pytest-tally-1.3.0/pytest_tally/__init__.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     3466 2023-04-20 02:27:46.000000 pytest-tally-1.3.0/pytest_tally/classes.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:39:53.612155 pytest-tally-1.3.0/pytest_tally/clients/
+-rw-r--r--   0 jwr003   (623385768) 542971493     3200 2023-05-20 07:39:29.000000 pytest-tally-1.3.0/pytest_tally/clients/app.py
+-rw-r--r--   0 jwr003   (623385768) 542971493    11206 2023-05-21 18:28:51.000000 pytest-tally-1.3.0/pytest_tally/clients/rich_dashboard.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:39:53.645177 pytest-tally-1.3.0/pytest_tally/clients/templates/
+-rw-r--r--   0 jwr003   (623385768) 542971493    11749 2023-05-20 07:39:29.000000 pytest-tally-1.3.0/pytest_tally/clients/templates/index.html
+-rw-r--r--   0 jwr003   (623385768) 542971493    11817 2023-05-22 05:23:07.000000 pytest-tally-1.3.0/pytest_tally/clients/tk_client.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     8250 2023-05-20 07:39:29.000000 pytest-tally-1.3.0/pytest_tally/plugin.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     2826 2023-04-13 09:21:48.000000 pytest-tally-1.3.0/pytest_tally/pytest_reportlog.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     2687 2023-04-19 18:51:00.000000 pytest-tally-1.3.0/pytest_tally/utils.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:39:53.592701 pytest-tally-1.3.0/pytest_tally.egg-info/
+-rw-r--r--   0 jwr003   (623385768) 542971493     5802 2023-05-22 05:39:53.000000 pytest-tally-1.3.0/pytest_tally.egg-info/PKG-INFO
+-rw-r--r--   0 jwr003   (623385768) 542971493      750 2023-05-22 05:39:53.000000 pytest-tally-1.3.0/pytest_tally.egg-info/SOURCES.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493        1 2023-05-22 05:39:53.000000 pytest-tally-1.3.0/pytest_tally.egg-info/dependency_links.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493      210 2023-05-22 05:39:53.000000 pytest-tally-1.3.0/pytest_tally.egg-info/entry_points.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493      130 2023-05-22 05:39:53.000000 pytest-tally-1.3.0/pytest_tally.egg-info/requires.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493       13 2023-05-22 05:39:53.000000 pytest-tally-1.3.0/pytest_tally.egg-info/top_level.txt
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:39:53.664806 pytest-tally-1.3.0/requirements/
+-rw-r--r--   0 jwr003   (623385768) 542971493       99 2023-04-15 00:12:58.000000 pytest-tally-1.3.0/requirements/requirements-dev.in
+-rw-r--r--   0 jwr003   (623385768) 542971493     2882 2023-05-20 07:39:29.000000 pytest-tally-1.3.0/requirements/requirements-dev.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493       95 2023-05-22 05:06:21.000000 pytest-tally-1.3.0/requirements/requirements.in
+-rw-r--r--   0 jwr003   (623385768) 542971493      987 2023-05-20 07:39:29.000000 pytest-tally-1.3.0/requirements/requirements.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493       38 2023-05-22 05:39:53.667693 pytest-tally-1.3.0/setup.cfg
+-rw-r--r--   0 jwr003   (623385768) 542971493     1982 2023-05-22 05:20:24.000000 pytest-tally-1.3.0/setup.py
```

### Comparing `pytest-tally-1.2.0/.gitignore` & `pytest-tally-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.2.0/LICENSE` & `pytest-tally-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.2.0/PKG-INFO` & `pytest-tally-1.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,44 @@
-Metadata-Version: 2.1
-Name: pytest-tally
-Version: 1.2.0
-Summary: A Pytest plugin to generate realtime summary stats, and display them in-console using a text-based dashboard.
-Home-page: https://github.com/jeffwright13/pytest-tally
-Author: Jeff Wright
-Author-email: jeff.washcloth@gmail.com
-License: MIT
-Keywords: pytest pytest-plugin testing tui rich blessed
-Classifier: Framework :: Pytest
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Testing
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # pytest-tally
 
-### A Pytest plugin that displays test run progress in-console or in-browser.
+### A Pytest plugin that displays test run progress in-console, in-app or in-browser.
 
+## Using Rich:
 ![2023-04-14 18 34 48](https://user-images.githubusercontent.com/4308435/232174467-752c5d13-15e3-4c23-9430-1087050af0a4.gif)
+
+## Using Tkinter:
+![2023-05-21 23 33 27](https://github.com/jeffwright13/pytest-tally/assets/4308435/7bb98b54-f796-4249-81d0-f2c283a7c6a3)
+
+## Using Flask:
 ![2023-05-17 15 15 02](https://github.com/jeffwright13/pytest-tally/assets/4308435/a35151e2-64fe-40e2-bd2e-9a59033edcd3)
 
 
 ## Why?
 I run a lot of long-duration test campaigns that generate copious amounts of console output. I usually monitor their progress by periodically checking the terminal to see if anything has failed so far. This usually means scrolling back in the console, looking for that telltale FAILED indication. It can be a bit of a pain hunting for that information!
 
 This plugin writes up-to-date summary statistics for each test, as it executes, to a JSON file on disk. That file is then continually read by a small client that prints results to terminal or in-browser. That way I can split my screen and monitor both the raw console output from Pytest, and the client's summary output, at the same time. Mmmm. Life suddenly just became a little easier and brighter. :-)
 
-There are two clients so far:
-- Rich text-based client that runs in the terminal
-- HTML client that runs in the browser (via a Flask web-app)
+## Also - why??
+
+Because I'm a geek and I like learning new stuff about Python. This project made me learn about realtime file syncing, different ways of presenting data, how to get ChatGpt to write stuff for you, and a lot more!
 
 ## Install
 For most users: `pip install pytest-tally`
 For users who like to 'roll their own': `pip install -r requirements/requirements.txt && pip install pytest-tally`
 For power users who want the dev dependencies: `pip install -r requirements/requirements-dev.txt && pip install pytest-tally`
 
 ## Usage
 
+There are three clients included in this repo:
+- Rich text-based client that runs in the terminal
+- HTML client that runs in the browser (via a Flask web-app)
+- TkInter GUI
+
+Each of these has known issues (see below), but are functional. You are welcome to improve upon any of these, or write your own and submit a PR if you like.
+
 To use text-based Rich client to display test results in-console as the tests run, open another terminal session, activate your venv, and type in `tally` to start the text-based client. Press the "q" key to quit the text-based client.
 
 To use web-app Flask/HTML client to display test results in-browser as the tests run, open another terminal session, activate your venv, and type in `python pytest_tally/clients/app.py [-h] [--port PORT] JSON_FILE_PATH` to start the Flask web-app.
 
 Now, simply run Pytest like you normally would, but specify the `--tally` option: `pytest --tally`. This starts the Pytest run and populates the tally-data.json file with the information needed by the client to show the updateded test status as it occurs.
 
 
@@ -57,23 +47,26 @@
 
     pytest tally:
     --tally                   Enable the pytest-tally plugin. Writes live summary results
                               data to a JSON file for consumption by a dashboard client.
 
 ### Rich (text-based) Client:
 
-    usage: tally [-h] [-v] [-l] [-x MAX_ROWS] [-f FILE_PATH] [filename]
+    usage: tally-rich [-h] [-v] [-l] [-x MAX_ROWS] [-f FILE_PATH] [filename]
 
     options:
     -h, --help            show this help message and exit
     -v, --version         show program's version number and exit
     -l, --lines           draw separation [l]ines in between each table row (default: False)
     -x MAX_ROWS, --max_rows MAX_ROWS
                             ma[x] number of rows to display (default: 0 [no limit])
 
+_Limitations_
+- Non-default JSON file support not working.
+
 ### Flask (web-app) Client:
 
     usage: tally-flask [-h] [--port PORT] [--debug] [--log-level LOG_LEVEL] [--fetch-rate FETCH_RATE] [JSON_FILE]
 
     positional arguments:
     JSON_FILE             path to the JSON file (default: /Users/jwr003/coding/pytest-tally/tally-data.json)
 
@@ -81,7 +74,19 @@
     -h, --help            show this help message and exit
     --port PORT           listening port for the app
     --debug               enable debug mode
     --log-level LOG_LEVEL
                             log level for Werkzeug
     --fetch-rate FETCH_RATE
                             fetch rate (in ms) - effectively the update rate of the web app
+
+_Limitations_
+- Non-default JSON file support not working.
+
+### TkInter (GUI) Client:
+
+    usage: tally-tk
+
+
+_Limitations_
+- Non-default JSON file support not working.
+- No command line options. The intent is to provide all configuration through the app itself, but so far none are implemented.
```

### Comparing `pytest-tally-1.2.0/misc/CHANGELOG.md` & `pytest-tally-1.3.0/misc/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project tries to adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 1.3.0 - 2023-05-20
+- Added Tkinter app.
+
 ## 1.2.0 - 2023-05-20
 - Added web app support via Flask
 - Fixed broekn'ds Rich app
 
 ## [1.1.1] 2023-04-14
 - Implemented file-lock on shared JSON file to fix client stuttering issue.
 - Added support for CLI option '-l' (lines -separators).
```

### Comparing `pytest-tally-1.2.0/misc/RELEASE_INSTRUCTIONS` & `pytest-tally-1.3.0/misc/RELEASE_INSTRUCTIONS`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.2.0/pytest_tally/classes.py` & `pytest-tally-1.3.0/pytest_tally/classes.py`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.2.0/pytest_tally/clients/app.py` & `pytest-tally-1.3.0/pytest_tally/clients/app.py`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.2.0/pytest_tally/clients/rich_dashboard.py` & `pytest-tally-1.3.0/pytest_tally/clients/rich_dashboard.py`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.2.0/pytest_tally/clients/templates/index.html` & `pytest-tally-1.3.0/pytest_tally/clients/templates/index.html`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.2.0/pytest_tally/plugin.py` & `pytest-tally-1.3.0/pytest_tally/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.2.0/pytest_tally/pytest_reportlog.py` & `pytest-tally-1.3.0/pytest_tally/pytest_reportlog.py`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.2.0/pytest_tally/utils.py` & `pytest-tally-1.3.0/pytest_tally/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.2.0/pytest_tally.egg-info/PKG-INFO` & `pytest-tally-1.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-tally
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Pytest plugin to generate realtime summary stats, and display them in-console using a text-based dashboard.
 Home-page: https://github.com/jeffwright13/pytest-tally
 Author: Jeff Wright
 Author-email: jeff.washcloth@gmail.com
 License: MIT
 Keywords: pytest pytest-plugin testing tui rich blessed
 Classifier: Framework :: Pytest
@@ -19,36 +19,49 @@
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pytest-tally
 
-### A Pytest plugin that displays test run progress in-console or in-browser.
+### A Pytest plugin that displays test run progress in-console, in-app or in-browser.
 
+## Using Rich:
 ![2023-04-14 18 34 48](https://user-images.githubusercontent.com/4308435/232174467-752c5d13-15e3-4c23-9430-1087050af0a4.gif)
+
+## Using Tkinter:
+![2023-05-21 23 33 27](https://github.com/jeffwright13/pytest-tally/assets/4308435/7bb98b54-f796-4249-81d0-f2c283a7c6a3)
+
+## Using Flask:
 ![2023-05-17 15 15 02](https://github.com/jeffwright13/pytest-tally/assets/4308435/a35151e2-64fe-40e2-bd2e-9a59033edcd3)
 
 
 ## Why?
 I run a lot of long-duration test campaigns that generate copious amounts of console output. I usually monitor their progress by periodically checking the terminal to see if anything has failed so far. This usually means scrolling back in the console, looking for that telltale FAILED indication. It can be a bit of a pain hunting for that information!
 
 This plugin writes up-to-date summary statistics for each test, as it executes, to a JSON file on disk. That file is then continually read by a small client that prints results to terminal or in-browser. That way I can split my screen and monitor both the raw console output from Pytest, and the client's summary output, at the same time. Mmmm. Life suddenly just became a little easier and brighter. :-)
 
-There are two clients so far:
-- Rich text-based client that runs in the terminal
-- HTML client that runs in the browser (via a Flask web-app)
+## Also - why??
+
+Because I'm a geek and I like learning new stuff about Python. This project made me learn about realtime file syncing, different ways of presenting data, how to get ChatGpt to write stuff for you, and a lot more!
 
 ## Install
 For most users: `pip install pytest-tally`
 For users who like to 'roll their own': `pip install -r requirements/requirements.txt && pip install pytest-tally`
 For power users who want the dev dependencies: `pip install -r requirements/requirements-dev.txt && pip install pytest-tally`
 
 ## Usage
 
+There are three clients included in this repo:
+- Rich text-based client that runs in the terminal
+- HTML client that runs in the browser (via a Flask web-app)
+- TkInter GUI
+
+Each of these has known issues (see below), but are functional. You are welcome to improve upon any of these, or write your own and submit a PR if you like.
+
 To use text-based Rich client to display test results in-console as the tests run, open another terminal session, activate your venv, and type in `tally` to start the text-based client. Press the "q" key to quit the text-based client.
 
 To use web-app Flask/HTML client to display test results in-browser as the tests run, open another terminal session, activate your venv, and type in `python pytest_tally/clients/app.py [-h] [--port PORT] JSON_FILE_PATH` to start the Flask web-app.
 
 Now, simply run Pytest like you normally would, but specify the `--tally` option: `pytest --tally`. This starts the Pytest run and populates the tally-data.json file with the information needed by the client to show the updateded test status as it occurs.
 
 
@@ -57,23 +70,26 @@
 
     pytest tally:
     --tally                   Enable the pytest-tally plugin. Writes live summary results
                               data to a JSON file for consumption by a dashboard client.
 
 ### Rich (text-based) Client:
 
-    usage: tally [-h] [-v] [-l] [-x MAX_ROWS] [-f FILE_PATH] [filename]
+    usage: tally-rich [-h] [-v] [-l] [-x MAX_ROWS] [-f FILE_PATH] [filename]
 
     options:
     -h, --help            show this help message and exit
     -v, --version         show program's version number and exit
     -l, --lines           draw separation [l]ines in between each table row (default: False)
     -x MAX_ROWS, --max_rows MAX_ROWS
                             ma[x] number of rows to display (default: 0 [no limit])
 
+_Limitations_
+- Non-default JSON file support not working.
+
 ### Flask (web-app) Client:
 
     usage: tally-flask [-h] [--port PORT] [--debug] [--log-level LOG_LEVEL] [--fetch-rate FETCH_RATE] [JSON_FILE]
 
     positional arguments:
     JSON_FILE             path to the JSON file (default: /Users/jwr003/coding/pytest-tally/tally-data.json)
 
@@ -81,7 +97,19 @@
     -h, --help            show this help message and exit
     --port PORT           listening port for the app
     --debug               enable debug mode
     --log-level LOG_LEVEL
                             log level for Werkzeug
     --fetch-rate FETCH_RATE
                             fetch rate (in ms) - effectively the update rate of the web app
+
+_Limitations_
+- Non-default JSON file support not working.
+
+### TkInter (GUI) Client:
+
+    usage: tally-tk
+
+
+_Limitations_
+- Non-default JSON file support not working.
+- No command line options. The intent is to provide all configuration through the app itself, but so far none are implemented.
```

### Comparing `pytest-tally-1.2.0/pytest_tally.egg-info/SOURCES.txt` & `pytest-tally-1.3.0/pytest_tally.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,12 +17,13 @@
 pytest_tally.egg-info/SOURCES.txt
 pytest_tally.egg-info/dependency_links.txt
 pytest_tally.egg-info/entry_points.txt
 pytest_tally.egg-info/requires.txt
 pytest_tally.egg-info/top_level.txt
 pytest_tally/clients/app.py
 pytest_tally/clients/rich_dashboard.py
+pytest_tally/clients/tk_client.py
 pytest_tally/clients/templates/index.html
 requirements/requirements-dev.in
 requirements/requirements-dev.txt
 requirements/requirements.in
 requirements/requirements.txt
```

### Comparing `pytest-tally-1.2.0/requirements/requirements-dev.txt` & `pytest-tally-1.3.0/requirements/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.2.0/requirements/requirements.txt` & `pytest-tally-1.3.0/requirements/requirements.txt`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.2.0/setup.py` & `pytest-tally-1.3.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding="utf-8").read()
 
 
 setup(
     name="pytest-tally",
-    version="1.2.0",
+    version="1.3.0",
     author="Jeff Wright",
     author_email="jeff.washcloth@gmail.com",
     license="MIT",
     url="https://github.com/jeffwright13/pytest-tally",
     description=(
         "A Pytest plugin to generate realtime summary stats, and display them"
         " in-console using a text-based dashboard."
@@ -54,10 +54,11 @@
     ],
     keywords="pytest pytest-plugin testing tui rich blessed",
     entry_points={
         "pytest11": ["pytest_tally = pytest_tally.plugin"],
         "console_scripts": [
             "tally-rich = pytest_tally.clients.rich_dashboard:main",
             "tally-flask = pytest_tally.clients.app:main",
+            "tally-tk = pytest_tally.clients.tk_client:main",
         ],
     },
 )
```

