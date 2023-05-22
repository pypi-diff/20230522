# Comparing `tmp/pytest-tally-1.3.0.tar.gz` & `tmp/pytest-tally-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-tally-1.3.0.tar", last modified: Mon May 22 05:39:53 2023, max compression
+gzip compressed data, was "pytest-tally-1.3.1.tar", last modified: Mon May 22 05:52:11 2023, max compression
```

## Comparing `pytest-tally-1.3.0.tar` & `pytest-tally-1.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:39:53.667449 pytest-tally-1.3.0/
--rw-r--r--   0 jwr003   (623385768) 542971493      139 2023-04-15 00:11:14.000000 pytest-tally-1.3.0/.flake8
--rw-r--r--   0 jwr003   (623385768) 542971493     1900 2023-04-19 18:50:46.000000 pytest-tally-1.3.0/.gitignore
--rw-r--r--   0 jwr003   (623385768) 542971493       25 2023-04-15 00:11:48.000000 pytest-tally-1.3.0/.isort.cfg
--rw-r--r--   0 jwr003   (623385768) 542971493      419 2023-04-15 03:02:55.000000 pytest-tally-1.3.0/.pre-commit-config.yaml
--rw-r--r--   0 jwr003   (623385768) 542971493     1068 2023-03-03 22:12:17.000000 pytest-tally-1.3.0/LICENSE
--rw-r--r--   0 jwr003   (623385768) 542971493     5802 2023-05-22 05:39:53.666384 pytest-tally-1.3.0/PKG-INFO
--rw-r--r--   0 jwr003   (623385768) 542971493     4885 2023-05-22 05:38:40.000000 pytest-tally-1.3.0/README.md
--rw-r--r--   0 jwr003   (623385768) 542971493       30 2023-03-05 22:13:29.000000 pytest-tally-1.3.0/conftest.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:39:53.560828 pytest-tally-1.3.0/misc/
--rw-r--r--   0 jwr003   (623385768) 542971493     1390 2023-05-22 05:09:41.000000 pytest-tally-1.3.0/misc/CHANGELOG.md
--rw-r--r--   0 jwr003   (623385768) 542971493     1698 2023-04-14 05:16:42.000000 pytest-tally-1.3.0/misc/RELEASE_INSTRUCTIONS
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:39:53.567956 pytest-tally-1.3.0/pytest_tally/
--rw-r--r--   0 jwr003   (623385768) 542971493      144 2023-03-06 07:36:18.000000 pytest-tally-1.3.0/pytest_tally/__init__.py
--rw-r--r--   0 jwr003   (623385768) 542971493     3466 2023-04-20 02:27:46.000000 pytest-tally-1.3.0/pytest_tally/classes.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:39:53.612155 pytest-tally-1.3.0/pytest_tally/clients/
--rw-r--r--   0 jwr003   (623385768) 542971493     3200 2023-05-20 07:39:29.000000 pytest-tally-1.3.0/pytest_tally/clients/app.py
--rw-r--r--   0 jwr003   (623385768) 542971493    11206 2023-05-21 18:28:51.000000 pytest-tally-1.3.0/pytest_tally/clients/rich_dashboard.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:39:53.645177 pytest-tally-1.3.0/pytest_tally/clients/templates/
--rw-r--r--   0 jwr003   (623385768) 542971493    11749 2023-05-20 07:39:29.000000 pytest-tally-1.3.0/pytest_tally/clients/templates/index.html
--rw-r--r--   0 jwr003   (623385768) 542971493    11817 2023-05-22 05:23:07.000000 pytest-tally-1.3.0/pytest_tally/clients/tk_client.py
--rw-r--r--   0 jwr003   (623385768) 542971493     8250 2023-05-20 07:39:29.000000 pytest-tally-1.3.0/pytest_tally/plugin.py
--rw-r--r--   0 jwr003   (623385768) 542971493     2826 2023-04-13 09:21:48.000000 pytest-tally-1.3.0/pytest_tally/pytest_reportlog.py
--rw-r--r--   0 jwr003   (623385768) 542971493     2687 2023-04-19 18:51:00.000000 pytest-tally-1.3.0/pytest_tally/utils.py
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:39:53.592701 pytest-tally-1.3.0/pytest_tally.egg-info/
--rw-r--r--   0 jwr003   (623385768) 542971493     5802 2023-05-22 05:39:53.000000 pytest-tally-1.3.0/pytest_tally.egg-info/PKG-INFO
--rw-r--r--   0 jwr003   (623385768) 542971493      750 2023-05-22 05:39:53.000000 pytest-tally-1.3.0/pytest_tally.egg-info/SOURCES.txt
--rw-r--r--   0 jwr003   (623385768) 542971493        1 2023-05-22 05:39:53.000000 pytest-tally-1.3.0/pytest_tally.egg-info/dependency_links.txt
--rw-r--r--   0 jwr003   (623385768) 542971493      210 2023-05-22 05:39:53.000000 pytest-tally-1.3.0/pytest_tally.egg-info/entry_points.txt
--rw-r--r--   0 jwr003   (623385768) 542971493      130 2023-05-22 05:39:53.000000 pytest-tally-1.3.0/pytest_tally.egg-info/requires.txt
--rw-r--r--   0 jwr003   (623385768) 542971493       13 2023-05-22 05:39:53.000000 pytest-tally-1.3.0/pytest_tally.egg-info/top_level.txt
-drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:39:53.664806 pytest-tally-1.3.0/requirements/
--rw-r--r--   0 jwr003   (623385768) 542971493       99 2023-04-15 00:12:58.000000 pytest-tally-1.3.0/requirements/requirements-dev.in
--rw-r--r--   0 jwr003   (623385768) 542971493     2882 2023-05-20 07:39:29.000000 pytest-tally-1.3.0/requirements/requirements-dev.txt
--rw-r--r--   0 jwr003   (623385768) 542971493       95 2023-05-22 05:06:21.000000 pytest-tally-1.3.0/requirements/requirements.in
--rw-r--r--   0 jwr003   (623385768) 542971493      987 2023-05-20 07:39:29.000000 pytest-tally-1.3.0/requirements/requirements.txt
--rw-r--r--   0 jwr003   (623385768) 542971493       38 2023-05-22 05:39:53.667693 pytest-tally-1.3.0/setup.cfg
--rw-r--r--   0 jwr003   (623385768) 542971493     1982 2023-05-22 05:20:24.000000 pytest-tally-1.3.0/setup.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:52:11.059532 pytest-tally-1.3.1/
+-rw-r--r--   0 jwr003   (623385768) 542971493      139 2023-04-15 00:11:14.000000 pytest-tally-1.3.1/.flake8
+-rw-r--r--   0 jwr003   (623385768) 542971493     1900 2023-04-19 18:50:46.000000 pytest-tally-1.3.1/.gitignore
+-rw-r--r--   0 jwr003   (623385768) 542971493       25 2023-04-15 00:11:48.000000 pytest-tally-1.3.1/.isort.cfg
+-rw-r--r--   0 jwr003   (623385768) 542971493      419 2023-04-15 03:02:55.000000 pytest-tally-1.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 jwr003   (623385768) 542971493     1068 2023-03-03 22:12:17.000000 pytest-tally-1.3.1/LICENSE
+-rw-r--r--   0 jwr003   (623385768) 542971493     5802 2023-05-22 05:52:11.058438 pytest-tally-1.3.1/PKG-INFO
+-rw-r--r--   0 jwr003   (623385768) 542971493     4885 2023-05-22 05:38:40.000000 pytest-tally-1.3.1/README.md
+-rw-r--r--   0 jwr003   (623385768) 542971493       30 2023-03-05 22:13:29.000000 pytest-tally-1.3.1/conftest.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:52:11.010552 pytest-tally-1.3.1/misc/
+-rw-r--r--   0 jwr003   (623385768) 542971493     1450 2023-05-22 05:51:05.000000 pytest-tally-1.3.1/misc/CHANGELOG.md
+-rw-r--r--   0 jwr003   (623385768) 542971493     1698 2023-04-14 05:16:42.000000 pytest-tally-1.3.1/misc/RELEASE_INSTRUCTIONS
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:52:11.015622 pytest-tally-1.3.1/pytest_tally/
+-rw-r--r--   0 jwr003   (623385768) 542971493      144 2023-03-06 07:36:18.000000 pytest-tally-1.3.1/pytest_tally/__init__.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     3466 2023-04-20 02:27:46.000000 pytest-tally-1.3.1/pytest_tally/classes.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:52:11.028965 pytest-tally-1.3.1/pytest_tally/clients/
+-rw-r--r--   0 jwr003   (623385768) 542971493     3200 2023-05-20 07:39:29.000000 pytest-tally-1.3.1/pytest_tally/clients/app.py
+-rw-r--r--   0 jwr003   (623385768) 542971493    11206 2023-05-21 18:28:51.000000 pytest-tally-1.3.1/pytest_tally/clients/rich_dashboard.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:52:11.048437 pytest-tally-1.3.1/pytest_tally/clients/templates/
+-rw-r--r--   0 jwr003   (623385768) 542971493    11749 2023-05-20 07:39:29.000000 pytest-tally-1.3.1/pytest_tally/clients/templates/index.html
+-rw-r--r--   0 jwr003   (623385768) 542971493    11817 2023-05-22 05:23:07.000000 pytest-tally-1.3.1/pytest_tally/clients/tk_client.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     8250 2023-05-20 07:39:29.000000 pytest-tally-1.3.1/pytest_tally/plugin.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     2826 2023-04-13 09:21:48.000000 pytest-tally-1.3.1/pytest_tally/pytest_reportlog.py
+-rw-r--r--   0 jwr003   (623385768) 542971493     2687 2023-04-19 18:51:00.000000 pytest-tally-1.3.1/pytest_tally/utils.py
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:52:11.024643 pytest-tally-1.3.1/pytest_tally.egg-info/
+-rw-r--r--   0 jwr003   (623385768) 542971493     5802 2023-05-22 05:52:10.000000 pytest-tally-1.3.1/pytest_tally.egg-info/PKG-INFO
+-rw-r--r--   0 jwr003   (623385768) 542971493      750 2023-05-22 05:52:10.000000 pytest-tally-1.3.1/pytest_tally.egg-info/SOURCES.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493        1 2023-05-22 05:52:10.000000 pytest-tally-1.3.1/pytest_tally.egg-info/dependency_links.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493      210 2023-05-22 05:52:10.000000 pytest-tally-1.3.1/pytest_tally.egg-info/entry_points.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493      146 2023-05-22 05:52:10.000000 pytest-tally-1.3.1/pytest_tally.egg-info/requires.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493       13 2023-05-22 05:52:10.000000 pytest-tally-1.3.1/pytest_tally.egg-info/top_level.txt
+drwxr-xr-x   0 jwr003   (623385768) 542971493        0 2023-05-22 05:52:11.056455 pytest-tally-1.3.1/requirements/
+-rw-r--r--   0 jwr003   (623385768) 542971493       99 2023-04-15 00:12:58.000000 pytest-tally-1.3.1/requirements/requirements-dev.in
+-rw-r--r--   0 jwr003   (623385768) 542971493     2882 2023-05-22 05:48:31.000000 pytest-tally-1.3.1/requirements/requirements-dev.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493      132 2023-05-22 05:47:41.000000 pytest-tally-1.3.1/requirements/requirements.in
+-rw-r--r--   0 jwr003   (623385768) 542971493     1045 2023-05-22 05:48:28.000000 pytest-tally-1.3.1/requirements/requirements.txt
+-rw-r--r--   0 jwr003   (623385768) 542971493       38 2023-05-22 05:52:11.059741 pytest-tally-1.3.1/setup.cfg
+-rw-r--r--   0 jwr003   (623385768) 542971493     2009 2023-05-22 05:47:19.000000 pytest-tally-1.3.1/setup.py
```

### Comparing `pytest-tally-1.3.0/.gitignore` & `pytest-tally-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.3.0/LICENSE` & `pytest-tally-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.3.0/PKG-INFO` & `pytest-tally-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-tally
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Pytest plugin to generate realtime summary stats, and display them in-console using a text-based dashboard.
 Home-page: https://github.com/jeffwright13/pytest-tally
 Author: Jeff Wright
 Author-email: jeff.washcloth@gmail.com
 License: MIT
 Keywords: pytest pytest-plugin testing tui rich blessed
 Classifier: Framework :: Pytest
```

### Comparing `pytest-tally-1.3.0/README.md` & `pytest-tally-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.3.0/misc/CHANGELOG.md` & `pytest-tally-1.3.1/misc/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project tries to adhere to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## 1.3.1 - 2023-05-20
+- Added missing watchdog dependency.
+
 ## 1.3.0 - 2023-05-20
 - Added Tkinter app.
 
 ## 1.2.0 - 2023-05-20
 - Added web app support via Flask
 - Fixed broekn'ds Rich app
```

### Comparing `pytest-tally-1.3.0/misc/RELEASE_INSTRUCTIONS` & `pytest-tally-1.3.1/misc/RELEASE_INSTRUCTIONS`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.3.0/pytest_tally/classes.py` & `pytest-tally-1.3.1/pytest_tally/classes.py`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.3.0/pytest_tally/clients/app.py` & `pytest-tally-1.3.1/pytest_tally/clients/app.py`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.3.0/pytest_tally/clients/rich_dashboard.py` & `pytest-tally-1.3.1/pytest_tally/clients/rich_dashboard.py`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.3.0/pytest_tally/clients/templates/index.html` & `pytest-tally-1.3.1/pytest_tally/clients/templates/index.html`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.3.0/pytest_tally/clients/tk_client.py` & `pytest-tally-1.3.1/pytest_tally/clients/tk_client.py`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.3.0/pytest_tally/plugin.py` & `pytest-tally-1.3.1/pytest_tally/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.3.0/pytest_tally/pytest_reportlog.py` & `pytest-tally-1.3.1/pytest_tally/pytest_reportlog.py`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.3.0/pytest_tally/utils.py` & `pytest-tally-1.3.1/pytest_tally/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.3.0/pytest_tally.egg-info/PKG-INFO` & `pytest-tally-1.3.1/pytest_tally.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-tally
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Pytest plugin to generate realtime summary stats, and display them in-console using a text-based dashboard.
 Home-page: https://github.com/jeffwright13/pytest-tally
 Author: Jeff Wright
 Author-email: jeff.washcloth@gmail.com
 License: MIT
 Keywords: pytest pytest-plugin testing tui rich blessed
 Classifier: Framework :: Pytest
```

### Comparing `pytest-tally-1.3.0/pytest_tally.egg-info/SOURCES.txt` & `pytest-tally-1.3.1/pytest_tally.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-tally-1.3.0/requirements/requirements-dev.txt` & `pytest-tally-1.3.1/requirements/requirements-dev.txt`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     # via
     #   requests-toolbelt
     #   twine
 requests-toolbelt==0.10.1
     # via twine
 rfc3986==2.0.0
     # via twine
-rich==13.3.4
+rich==13.3.2
     # via
     #   -c requirements/requirements.txt
     #   twine
 six==1.16.0
     # via
     #   -c requirements/requirements.txt
     #   bleach
```

### Comparing `pytest-tally-1.3.0/requirements/requirements.txt` & `pytest-tally-1.3.1/requirements/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -28,19 +28,21 @@
     #   werkzeug
 mdurl==0.1.2
     # via markdown-it-py
 pygments==2.15.0
     # via rich
 quantiphy==2.19
     # via -r requirements/requirements.in
-rich==13.3.4
+rich==13.3.2
     # via -r requirements/requirements.in
 single-source==0.3.0
     # via -r requirements/requirements.in
 six==1.16.0
     # via blessed
 strip-ansi==0.1.1
     # via -r requirements/requirements.in
+watchdog==3.0.0
+    # via -r requirements/requirements.in
 wcwidth==0.2.6
     # via blessed
 werkzeug==2.3.4
     # via flask
```

### Comparing `pytest-tally-1.3.0/setup.py` & `pytest-tally-1.3.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return codecs.open(file_path, encoding="utf-8").read()
 
 
 setup(
     name="pytest-tally",
-    version="1.3.0",
+    version="1.3.1",
     author="Jeff Wright",
     author_email="jeff.washcloth@gmail.com",
     license="MIT",
     url="https://github.com/jeffwright13/pytest-tally",
     description=(
         "A Pytest plugin to generate realtime summary stats, and display them"
         " in-console using a text-based dashboard."
@@ -33,14 +33,15 @@
         "count-timer==0.3.8",
         "flask==2.3.2",
         "pytest>=6.2.5",
         "quantiphy==2.19",
         "rich==13.3.2",
         "single-source==0.3.0",
         "strip-ansi==0.1.1",
+        "watchdog==3.0.0",
     ],
     setup_requires=["setuptools_scm"],
     include_package_data=True,
     classifiers=[
         "Framework :: Pytest",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

