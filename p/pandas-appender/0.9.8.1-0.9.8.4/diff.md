# Comparing `tmp/pandas_appender-0.9.8.1.tar.gz` & `tmp/pandas_appender-0.9.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas_appender-0.9.8.1.tar", last modified: Sun Dec 11 07:12:15 2022, max compression
+gzip compressed data, was "pandas_appender-0.9.8.4.tar", last modified: Mon May 22 16:49:10 2023, max compression
```

## Comparing `pandas_appender-0.9.8.1.tar` & `pandas_appender-0.9.8.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 astrogreg  (2081) astrogreg  (2082)        0 2022-12-11 07:12:15.019573 pandas_appender-0.9.8.1/
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)      247 2022-12-11 06:48:33.000000 pandas_appender-0.9.8.1/.editorconfig
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)       66 2022-12-11 06:56:32.000000 pandas_appender-0.9.8.1/.gitignore
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)    11357 2022-12-11 05:51:12.000000 pandas_appender-0.9.8.1/LICENSE
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)      774 2022-12-11 06:29:52.000000 pandas_appender-0.9.8.1/Makefile
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     4198 2022-12-11 07:12:15.019573 pandas_appender-0.9.8.1/PKG-INFO
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     3039 2022-12-11 05:51:12.000000 pandas_appender-0.9.8.1/README.md
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     1997 2022-12-11 06:51:03.000000 pandas_appender-0.9.8.1/azure-pipelines.yml
-drwxrwxr-x   0 astrogreg  (2081) astrogreg  (2082)        0 2022-12-11 07:12:15.015573 pandas_appender-0.9.8.1/pandas_appender/
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)       34 2022-12-11 05:51:12.000000 pandas_appender-0.9.8.1/pandas_appender/__init__.py
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     4631 2022-12-11 05:56:15.000000 pandas_appender-0.9.8.1/pandas_appender/appender.py
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)      818 2022-12-11 05:51:12.000000 pandas_appender-0.9.8.1/pandas_appender/hints.py
-drwxrwxr-x   0 astrogreg  (2081) astrogreg  (2082)        0 2022-12-11 07:12:15.019573 pandas_appender-0.9.8.1/pandas_appender.egg-info/
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     4198 2022-12-11 07:12:14.000000 pandas_appender-0.9.8.1/pandas_appender.egg-info/PKG-INFO
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)      413 2022-12-11 07:12:14.000000 pandas_appender-0.9.8.1/pandas_appender.egg-info/SOURCES.txt
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)        1 2022-12-11 07:12:14.000000 pandas_appender-0.9.8.1/pandas_appender.egg-info/dependency_links.txt
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)       62 2022-12-11 07:12:14.000000 pandas_appender-0.9.8.1/pandas_appender.egg-info/requires.txt
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)       16 2022-12-11 07:12:14.000000 pandas_appender-0.9.8.1/pandas_appender.egg-info/top_level.txt
-drwxrwxr-x   0 astrogreg  (2081) astrogreg  (2082)        0 2022-12-11 07:12:15.019573 pandas_appender-0.9.8.1/scripts/
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     1792 2022-12-11 05:51:12.000000 pandas_appender-0.9.8.1/scripts/tuner.py
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)       38 2022-12-11 07:12:15.019573 pandas_appender-0.9.8.1/setup.cfg
--rwxrwxr-x   0 astrogreg  (2081) astrogreg  (2082)     2040 2022-12-11 07:11:35.000000 pandas_appender-0.9.8.1/setup.py
-drwxrwxr-x   0 astrogreg  (2081) astrogreg  (2082)        0 2022-12-11 07:12:15.019573 pandas_appender-0.9.8.1/test/
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     7418 2022-12-11 07:00:57.000000 pandas_appender-0.9.8.1/test/test_appender.py
--rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     1211 2022-12-11 07:00:38.000000 pandas_appender-0.9.8.1/test/test_hints.py
+drwxrwxr-x   0 astrogreg  (2081) astrogreg  (2082)        0 2023-05-22 16:49:10.001569 pandas_appender-0.9.8.4/
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)      247 2022-12-11 06:48:33.000000 pandas_appender-0.9.8.4/.editorconfig
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)       66 2022-12-11 06:56:32.000000 pandas_appender-0.9.8.4/.gitignore
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)    11357 2022-12-11 05:51:12.000000 pandas_appender-0.9.8.4/LICENSE
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)      793 2023-05-22 16:45:53.000000 pandas_appender-0.9.8.4/Makefile
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     4196 2023-05-22 16:49:10.001569 pandas_appender-0.9.8.4/PKG-INFO
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     3039 2022-12-11 05:51:12.000000 pandas_appender-0.9.8.4/README.md
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     2355 2022-12-11 19:46:15.000000 pandas_appender-0.9.8.4/azure-pipelines.yml
+drwxrwxr-x   0 astrogreg  (2081) astrogreg  (2082)        0 2023-05-22 16:49:10.001569 pandas_appender-0.9.8.4/pandas_appender/
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)       34 2022-12-11 05:51:12.000000 pandas_appender-0.9.8.4/pandas_appender/__init__.py
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     4631 2022-12-11 05:56:15.000000 pandas_appender-0.9.8.4/pandas_appender/appender.py
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)      818 2022-12-11 05:51:12.000000 pandas_appender-0.9.8.4/pandas_appender/hints.py
+drwxrwxr-x   0 astrogreg  (2081) astrogreg  (2082)        0 2023-05-22 16:49:10.001569 pandas_appender-0.9.8.4/pandas_appender.egg-info/
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     4196 2023-05-22 16:49:09.000000 pandas_appender-0.9.8.4/pandas_appender.egg-info/PKG-INFO
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)      413 2023-05-22 16:49:09.000000 pandas_appender-0.9.8.4/pandas_appender.egg-info/SOURCES.txt
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)        1 2023-05-22 16:49:09.000000 pandas_appender-0.9.8.4/pandas_appender.egg-info/dependency_links.txt
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)       64 2023-05-22 16:49:09.000000 pandas_appender-0.9.8.4/pandas_appender.egg-info/requires.txt
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)       16 2023-05-22 16:49:09.000000 pandas_appender-0.9.8.4/pandas_appender.egg-info/top_level.txt
+drwxrwxr-x   0 astrogreg  (2081) astrogreg  (2082)        0 2023-05-22 16:49:10.001569 pandas_appender-0.9.8.4/scripts/
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     1792 2022-12-11 05:51:12.000000 pandas_appender-0.9.8.4/scripts/tuner.py
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)       38 2023-05-22 16:49:10.001569 pandas_appender-0.9.8.4/setup.cfg
+-rwxrwxr-x   0 astrogreg  (2081) astrogreg  (2082)     2052 2023-05-22 16:45:53.000000 pandas_appender-0.9.8.4/setup.py
+drwxrwxr-x   0 astrogreg  (2081) astrogreg  (2082)        0 2023-05-22 16:49:10.001569 pandas_appender-0.9.8.4/test/
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     7418 2022-12-11 07:00:57.000000 pandas_appender-0.9.8.4/test/test_appender.py
+-rw-rw-r--   0 astrogreg  (2081) astrogreg  (2082)     1211 2022-12-11 07:00:38.000000 pandas_appender-0.9.8.4/test/test_hints.py
```

### Comparing `pandas_appender-0.9.8.1/LICENSE` & `pandas_appender-0.9.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas_appender-0.9.8.1/Makefile` & `pandas_appender-0.9.8.4/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -17,12 +17,13 @@
 
 distcheck: distclean
 	python ./setup.py sdist
 	twine check dist/*
 
 dist: distclean
 	echo "reminder, you must have tagged this commit or you'll end up failing"
+	echo "  git push"
 	echo "  git tag v0.x.x"
 	echo "  git push --tags"
 	python ./setup.py sdist
 	twine check dist/*
 	twine upload dist/* -r pypi
```

### Comparing `pandas_appender-0.9.8.1/PKG-INFO` & `pandas_appender-0.9.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas_appender
-Version: 0.9.8.1
+Version: 0.9.8.4
 Summary: A helper class that makes appending to a Pandas DataFrame efficient
 Home-page: https://github.com/wumpus/pandas-appender
 Author: Greg Lindahl and others
 Author-email: lindahl@pbm.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # pandas-appender
 
 [![Build Status](https://dev.azure.com/lindahl0577/pandas-appender/_apis/build/status/wumpus.pandas-appender?branchName=main)](https://dev.azure.com/lindahl0577/pandas-appender/_build/latest?definitionId=2&branchName=main) [![Coverage](https://coveralls.io/repos/github/wumpus/pandas-appender/badge.svg?branch=main)](https://coveralls.io/github/wumpus/pandas-appender?branch=main) [![Apache License 2.0](https://img.shields.io/github/license/wumpus/pandas-appender.svg)](LICENSE)
```

### Comparing `pandas_appender-0.9.8.1/README.md` & `pandas_appender-0.9.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pandas_appender-0.9.8.1/azure-pipelines.yml` & `pandas_appender-0.9.8.4/azure-pipelines.yml`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,38 @@
   # https://github.com/actions/python-versions/blob/main/versions-manifest.json
   - job: linux
     pool:
       vmImage: 'ubuntu-latest'
     strategy:
       matrix:
         # Python 3.6 is not available on ubuntu 22.04 (latest)
+        #Python36:
+          # specifying the vmImage here does not work
+          #vmImage: 'ubuntu-20.4'
+          #python.version: '3.6'
         Python37:
           python.version: '3.7'
         Python38:
           python.version: '3.8'
         Python39:
           python.version: '3.9'
         Python310:
           python.version: '3.10'
         Python311:
           python.version: '3.11'
+        #Python312:
+          # requires allowUnstable
+          # as of 3.12.0-alpha.3, no pandas or numpy wheels, pandas build fails after 19 minutes
+          #python.version: '3.12-dev'
 
     steps:
     - task: UsePythonVersion@0
       inputs:
         versionSpec: '$(python.version)'
+        allowUnstable: true
       displayName: 'Use Python $(python.version)'
 
     - script: |
         python -m pip install --upgrade pip
         pip install . .[test]
       displayName: 'Install dependencies'
```

### Comparing `pandas_appender-0.9.8.1/pandas_appender/appender.py` & `pandas_appender-0.9.8.4/pandas_appender/appender.py`

 * *Files identical despite different names*

### Comparing `pandas_appender-0.9.8.1/pandas_appender/hints.py` & `pandas_appender-0.9.8.4/pandas_appender/hints.py`

 * *Files identical despite different names*

### Comparing `pandas_appender-0.9.8.1/pandas_appender.egg-info/PKG-INFO` & `pandas_appender-0.9.8.4/pandas_appender.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-appender
-Version: 0.9.8.1
+Version: 0.9.8.4
 Summary: A helper class that makes appending to a Pandas DataFrame efficient
 Home-page: https://github.com/wumpus/pandas-appender
 Author: Greg Lindahl and others
 Author-email: lindahl@pbm.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6.*
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # pandas-appender
 
 [![Build Status](https://dev.azure.com/lindahl0577/pandas-appender/_apis/build/status/wumpus.pandas-appender?branchName=main)](https://dev.azure.com/lindahl0577/pandas-appender/_build/latest?definitionId=2&branchName=main) [![Coverage](https://coveralls.io/repos/github/wumpus/pandas-appender/badge.svg?branch=main)](https://coveralls.io/github/wumpus/pandas-appender?branch=main) [![Apache License 2.0](https://img.shields.io/github/license/wumpus/pandas-appender.svg)](LICENSE)
```

### Comparing `pandas_appender-0.9.8.1/scripts/tuner.py` & `pandas_appender-0.9.8.4/scripts/tuner.py`

 * *Files identical despite different names*

### Comparing `pandas_appender-0.9.8.1/setup.py` & `pandas_appender-0.9.8.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 packages = [
     'pandas_appender',
 ]
 
 test_requirements = ['pytest', 'pytest-cov', 'pytest-sugar', 'coveralls', 'numpy']
 
 requires = [
-    'pandas'
+    'pandas<2'  # DataFrame.append() disappears in v2
 ]
 
 extras_require = {
     'test': test_requirements,  # setup no longer tests, so make them an extra
 }
 
 setup_requires = ['setuptools_scm']
@@ -32,15 +32,15 @@
     description='A helper class that makes appending to a Pandas DataFrame efficient',
     long_description=description,
     long_description_content_type='text/markdown',
     author='Greg Lindahl and others',
     author_email='lindahl@pbm.com',
     url='https://github.com/wumpus/pandas-appender',
     packages=packages,
-    python_requires=">=3.6.*",
+    python_requires=">=3.6",
     extras_require=extras_require,
     setup_requires=setup_requires,
     install_requires=requires,
     scripts=scripts,
     license='Apache 2.0',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
@@ -49,15 +49,15 @@
         'Environment :: MacOS X',
         'Intended Audience :: Information Technology',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
         #'Programming Language :: Python :: 3.5',  # setuptools_scm 6 dropped Py 3.5 and somehow I can't ask for an old version?
-        'Programming Language :: Python :: 3.6',  # can't CI on azure 22.04
+        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3 :: Only',
     ],
```

### Comparing `pandas_appender-0.9.8.1/test/test_appender.py` & `pandas_appender-0.9.8.4/test/test_appender.py`

 * *Files identical despite different names*

### Comparing `pandas_appender-0.9.8.1/test/test_hints.py` & `pandas_appender-0.9.8.4/test/test_hints.py`

 * *Files identical despite different names*

