# Comparing `tmp/ghevaluator-2.0.0.tar.gz` & `tmp/ghevaluator-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghevaluator-2.0.0.tar", last modified: Thu May 11 14:39:26 2023, max compression
+gzip compressed data, was "ghevaluator-2.1.0.tar", last modified: Mon May 22 09:46:08 2023, max compression
```

## Comparing `ghevaluator-2.0.0.tar` & `ghevaluator-2.1.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 14:39:26.661398 ghevaluator-2.0.0/
--rw-r--r--   0 bebatut    (502) staff       (20)     1066 2023-05-11 09:08:31.000000 ghevaluator-2.0.0/LICENSE
--rw-r--r--   0 bebatut    (502) staff       (20)       52 2023-05-11 09:08:31.000000 ghevaluator-2.0.0/MANIFEST.in
--rw-r--r--   0 bebatut    (502) staff       (20)     4197 2023-05-11 14:39:26.660374 ghevaluator-2.0.0/PKG-INFO
--rw-r--r--   0 bebatut    (502) staff       (20)     2237 2023-05-11 14:38:57.000000 ghevaluator-2.0.0/README.md
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 14:39:26.634285 ghevaluator-2.0.0/docs/
--rw-r--r--   0 bebatut    (502) staff       (20)      230 2023-05-11 14:26:46.000000 ghevaluator-2.0.0/docs/.buildinfo
--rw-r--r--   0 bebatut    (502) staff       (20)        0 2023-05-11 14:35:03.000000 ghevaluator-2.0.0/docs/.nojekyll
--rw-r--r--   0 bebatut    (502) staff       (20)     3678 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/api_documentation.html
--rw-r--r--   0 bebatut    (502) staff       (20)     9913 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/contributing.html
--rw-r--r--   0 bebatut    (502) staff       (20)     3624 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/genindex.html
--rw-r--r--   0 bebatut    (502) staff       (20)     5790 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/index.html
--rw-r--r--   0 bebatut    (502) staff       (20)     4377 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/installation.html
--rw-r--r--   0 bebatut    (502) staff       (20)      371 2023-05-11 14:26:46.000000 ghevaluator-2.0.0/docs/objects.inv
--rw-r--r--   0 bebatut    (502) staff       (20)     3503 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/py-modindex.html
--rw-r--r--   0 bebatut    (502) staff       (20)     3235 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/search.html
--rw-r--r--   0 bebatut    (502) staff       (20)     5577 2023-05-11 14:26:46.000000 ghevaluator-2.0.0/docs/searchindex.js
--rw-r--r--   0 bebatut    (502) staff       (20)     8118 2023-05-11 14:26:45.000000 ghevaluator-2.0.0/docs/usage.html
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 14:39:26.645951 ghevaluator-2.0.0/ghevaluator/
--rw-r--r--   0 bebatut    (502) staff       (20)    11385 2023-05-11 09:08:31.000000 ghevaluator-2.0.0/ghevaluator/__init__.py
--rw-r--r--   0 bebatut    (502) staff       (20)     1241 2023-05-11 09:08:31.000000 ghevaluator-2.0.0/ghevaluator/__main__.py
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 14:39:26.656834 ghevaluator-2.0.0/ghevaluator.egg-info/
--rw-r--r--   0 bebatut    (502) staff       (20)     4197 2023-05-11 14:39:26.000000 ghevaluator-2.0.0/ghevaluator.egg-info/PKG-INFO
--rw-r--r--   0 bebatut    (502) staff       (20)      579 2023-05-11 14:39:26.000000 ghevaluator-2.0.0/ghevaluator.egg-info/SOURCES.txt
--rw-r--r--   0 bebatut    (502) staff       (20)        1 2023-05-11 14:39:26.000000 ghevaluator-2.0.0/ghevaluator.egg-info/dependency_links.txt
--rw-r--r--   0 bebatut    (502) staff       (20)       58 2023-05-11 14:39:26.000000 ghevaluator-2.0.0/ghevaluator.egg-info/entry_points.txt
--rw-r--r--   0 bebatut    (502) staff       (20)       18 2023-05-11 14:39:26.000000 ghevaluator-2.0.0/ghevaluator.egg-info/requires.txt
--rw-r--r--   0 bebatut    (502) staff       (20)       42 2023-05-11 14:39:26.000000 ghevaluator-2.0.0/ghevaluator.egg-info/top_level.txt
--rw-r--r--   0 bebatut    (502) staff       (20)      981 2023-05-11 14:07:39.000000 ghevaluator-2.0.0/pyproject.toml
--rw-r--r--   0 bebatut    (502) staff       (20)       38 2023-05-11 14:39:26.661579 ghevaluator-2.0.0/setup.cfg
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 14:39:26.394776 ghevaluator-2.0.0/src/
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 14:39:26.657613 ghevaluator-2.0.0/src/docs/
--rw-r--r--   0 bebatut    (502) staff       (20)     1115 2023-05-11 14:25:17.000000 ghevaluator-2.0.0/src/docs/conf.py
-drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-11 14:39:26.659678 ghevaluator-2.0.0/tests/
--rw-r--r--   0 bebatut    (502) staff       (20)     9636 2023-05-11 09:08:31.000000 ghevaluator-2.0.0/tests/test_ghevaluator.py
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-22 09:46:08.989394 ghevaluator-2.1.0/
+-rw-r--r--   0 bebatut    (502) staff       (20)     1066 2023-05-11 09:08:31.000000 ghevaluator-2.1.0/LICENSE
+-rw-r--r--   0 bebatut    (502) staff       (20)       52 2023-05-11 09:08:31.000000 ghevaluator-2.1.0/MANIFEST.in
+-rw-r--r--   0 bebatut    (502) staff       (20)     4253 2023-05-22 09:46:08.988940 ghevaluator-2.1.0/PKG-INFO
+-rw-r--r--   0 bebatut    (502) staff       (20)     2293 2023-05-22 09:44:16.000000 ghevaluator-2.1.0/README.md
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-22 09:46:08.971939 ghevaluator-2.1.0/docs/
+-rw-r--r--   0 bebatut    (502) staff       (20)      230 2023-05-22 09:28:28.000000 ghevaluator-2.1.0/docs/.buildinfo
+-rw-r--r--   0 bebatut    (502) staff       (20)     3678 2023-05-22 09:28:27.000000 ghevaluator-2.1.0/docs/api_documentation.html
+-rw-r--r--   0 bebatut    (502) staff       (20)    10043 2023-05-22 09:44:16.000000 ghevaluator-2.1.0/docs/contributing.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     3624 2023-05-22 09:28:28.000000 ghevaluator-2.1.0/docs/genindex.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     5817 2023-05-22 09:44:16.000000 ghevaluator-2.1.0/docs/index.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     4377 2023-05-22 09:28:27.000000 ghevaluator-2.1.0/docs/installation.html
+-rw-r--r--   0 bebatut    (502) staff       (20)      371 2023-05-22 09:28:28.000000 ghevaluator-2.1.0/docs/objects.inv
+-rw-r--r--   0 bebatut    (502) staff       (20)     3503 2023-05-22 09:28:28.000000 ghevaluator-2.1.0/docs/py-modindex.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     3235 2023-05-22 09:28:28.000000 ghevaluator-2.1.0/docs/search.html
+-rw-r--r--   0 bebatut    (502) staff       (20)     5570 2023-05-22 09:44:16.000000 ghevaluator-2.1.0/docs/searchindex.js
+-rw-r--r--   0 bebatut    (502) staff       (20)     8176 2023-05-22 09:44:16.000000 ghevaluator-2.1.0/docs/usage.html
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-22 09:46:08.975711 ghevaluator-2.1.0/ghevaluator/
+-rw-r--r--   0 bebatut    (502) staff       (20)    12098 2023-05-22 09:44:16.000000 ghevaluator-2.1.0/ghevaluator/__init__.py
+-rw-r--r--   0 bebatut    (502) staff       (20)     1241 2023-05-11 14:54:26.000000 ghevaluator-2.1.0/ghevaluator/__main__.py
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-22 09:46:08.985492 ghevaluator-2.1.0/ghevaluator.egg-info/
+-rw-r--r--   0 bebatut    (502) staff       (20)     4253 2023-05-22 09:46:08.000000 ghevaluator-2.1.0/ghevaluator.egg-info/PKG-INFO
+-rw-r--r--   0 bebatut    (502) staff       (20)      564 2023-05-22 09:46:08.000000 ghevaluator-2.1.0/ghevaluator.egg-info/SOURCES.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)        1 2023-05-22 09:46:08.000000 ghevaluator-2.1.0/ghevaluator.egg-info/dependency_links.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)       58 2023-05-22 09:46:08.000000 ghevaluator-2.1.0/ghevaluator.egg-info/entry_points.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)       18 2023-05-22 09:46:08.000000 ghevaluator-2.1.0/ghevaluator.egg-info/requires.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)       45 2023-05-22 09:46:08.000000 ghevaluator-2.1.0/ghevaluator.egg-info/top_level.txt
+-rw-r--r--   0 bebatut    (502) staff       (20)      981 2023-05-22 09:31:24.000000 ghevaluator-2.1.0/pyproject.toml
+-rw-r--r--   0 bebatut    (502) staff       (20)       38 2023-05-22 09:46:08.989509 ghevaluator-2.1.0/setup.cfg
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-22 09:46:08.958589 ghevaluator-2.1.0/src/
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-22 09:46:08.986025 ghevaluator-2.1.0/src/docs/
+-rw-r--r--   0 bebatut    (502) staff       (20)     1115 2023-05-11 14:25:17.000000 ghevaluator-2.1.0/src/docs/conf.py
+drwxr-xr-x   0 bebatut    (502) staff       (20)        0 2023-05-22 09:46:08.986795 ghevaluator-2.1.0/tests/
+-rw-r--r--   0 bebatut    (502) staff       (20)    10637 2023-05-22 09:44:16.000000 ghevaluator-2.1.0/tests/test_ghevaluator.py
```

### Comparing `ghevaluator-2.0.0/LICENSE` & `ghevaluator-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.0.0/PKG-INFO` & `ghevaluator-2.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghevaluator
-Version: 2.0.0
+Version: 2.1.0
 Summary: A command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON report file.
 Author: Teresa Müller
 Author-email: Siyu Chen <chensy96@gmail.com>, Bérénice Batut <berenice.batut@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Siyu Chen
         
@@ -35,36 +35,36 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Galaxy History Evaluator
 ========================
 
-Galaxy History Evaluator or `ghevaluator` is a command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON report file.
+Galaxy History Evaluator or `ghevaluator` is a command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON and HTML report files.
 
 ## Context
 
 [Galaxy](https://galaxyproject.org/) is an **open, web-based platform for data-intensive computational research**.
 
 When running their data analysis, Galaxy users create histories storing their data, but also the steps of the data analysis, i.e. the tools used, their versions and parameters.
 
 Galaxy is also used for training where participants follow step-by-step tutorials, stored in Galaxy histories. At the end, participants might want to know if they followed correctly the tutorial and instructors might need to evaluate histories to give feedback and deliver certificates.
 **Evaluating histories manually can be painful and error prone**.
 
-Galaxy History Evaluator aims to solve this by providing a command-line tool to compare a Galaxy history to a templare workflow and generate a report in JSON with difference between the provided history and the expected workflow.
+Galaxy History Evaluator aims to solve this by providing a command-line tool to compare a Galaxy history to a templare workflow and generate a report in JSON and HTML with difference between the provided history and the expected workflow.
 
 ## Usage
 
 Galaxy History Evaluator can be used via command-line
 
 ```bash
 $ ghevaluator --help
 usage: ghevaluator [-h] -u HISTORY_URL -w WORKFLOW_URL -a APIKEY [-o OUTPUT]
 
-Compare a Galaxy history to a template workflow and generate a JSON report file
+Compare a Galaxy history to a template workflow and generate the JSON and HTML report files
 
 options:
   -h, --help            show this help message and exit
   -u HISTORY_URL, --history_url HISTORY_URL
                         URL to Galaxy history
   -w WORKFLOW_URL, --workflow_url WORKFLOW_URL
                         URL to template workflow
@@ -83,21 +83,21 @@
 ```
 
 ## Tests
 
 1. Export the Galaxy API key as environment variable
 
   ```bash
-  $ export GALAXY_APIKEY = <>
+  $ export GALAXY_API_KEY=<REPLACE_WITH_GALAXY_API_KEY>
   ```
 
 2. Run the unit tests
 
   ```bash
-  $ make tests
+  $ make test
   ```
 
 
 ## Documentation
 
 
 Documentation could be found at https://streetscience.community/ghevaluator/
```

### Comparing `ghevaluator-2.0.0/README.md` & `ghevaluator-2.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Galaxy History Evaluator
 ========================
 
-Galaxy History Evaluator or `ghevaluator` is a command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON report file.
+Galaxy History Evaluator or `ghevaluator` is a command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON and HTML report files.
 
 ## Context
 
 [Galaxy](https://galaxyproject.org/) is an **open, web-based platform for data-intensive computational research**.
 
 When running their data analysis, Galaxy users create histories storing their data, but also the steps of the data analysis, i.e. the tools used, their versions and parameters.
 
 Galaxy is also used for training where participants follow step-by-step tutorials, stored in Galaxy histories. At the end, participants might want to know if they followed correctly the tutorial and instructors might need to evaluate histories to give feedback and deliver certificates.
 **Evaluating histories manually can be painful and error prone**.
 
-Galaxy History Evaluator aims to solve this by providing a command-line tool to compare a Galaxy history to a templare workflow and generate a report in JSON with difference between the provided history and the expected workflow.
+Galaxy History Evaluator aims to solve this by providing a command-line tool to compare a Galaxy history to a templare workflow and generate a report in JSON and HTML with difference between the provided history and the expected workflow.
 
 ## Usage
 
 Galaxy History Evaluator can be used via command-line
 
 ```bash
 $ ghevaluator --help
 usage: ghevaluator [-h] -u HISTORY_URL -w WORKFLOW_URL -a APIKEY [-o OUTPUT]
 
-Compare a Galaxy history to a template workflow and generate a JSON report file
+Compare a Galaxy history to a template workflow and generate the JSON and HTML report files
 
 options:
   -h, --help            show this help message and exit
   -u HISTORY_URL, --history_url HISTORY_URL
                         URL to Galaxy history
   -w WORKFLOW_URL, --workflow_url WORKFLOW_URL
                         URL to template workflow
@@ -45,21 +45,21 @@
 ```
 
 ## Tests
 
 1. Export the Galaxy API key as environment variable
 
   ```bash
-  $ export GALAXY_APIKEY = <>
+  $ export GALAXY_API_KEY=<REPLACE_WITH_GALAXY_API_KEY>
   ```
 
 2. Run the unit tests
 
   ```bash
-  $ make tests
+  $ make test
   ```
 
 
 ## Documentation
 
 
 Documentation could be found at https://streetscience.community/ghevaluator/
```

### Comparing `ghevaluator-2.0.0/docs/api_documentation.html` & `ghevaluator-2.1.0/docs/api_documentation.html`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.0.0/docs/contributing.html` & `ghevaluator-2.1.0/docs/contributing.html`

 * *Files 4% similar despite different names*

```diff
@@ -81,19 +81,27 @@
 </li>
 </ol>
 </section>
 <section id="tests">
 <h2>Tests<a class="headerlink" href="#tests" title="Permalink to this heading">¶</a></h2>
 <p>The code and individual functions are covered by tests, using <cite>unittests</cite>.</p>
 <p>We also recommend to run them locally before pushing to GitHub with:</p>
+<ol class="arabic">
+<li><p>Export the Galaxy API key as environment variable</p>
+<div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>$<span class="w"> </span><span class="nb">export</span><span class="w"> </span><span class="nv">GALAXY_API_KEY</span><span class="o">=</span>&lt;REPLACE_WITH_GALAXY_API_KEY&gt;
+</pre></div>
+</div>
+</li>
+<li><p>Run the unit tests</p>
 <div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>$<span class="w"> </span>make<span class="w"> </span><span class="nb">test</span>
 </pre></div>
 </div>
-<p>After adding new function or making changes to an existing function, make sure to make changes to the unittest files under the <cite>test</cite> folder.</p>
-<p>In addition to unit tests, the overall functionality and the intergration of the tool is tested via <cite>subprocess</cite> under the <cite>integration test</cite> folder. It also runs automatically everytime someone pushes or commits to the git repository.</p>
+</li>
+</ol>
+<p>After adding new function or making changes to an existing function, make sure to make changes to the tests in the <cite>test</cite> folder.</p>
 </section>
 <section id="documentation">
 <h2>Documentation<a class="headerlink" href="#documentation" title="Permalink to this heading">¶</a></h2>
 <p>This documentation is generated using Sphinx.</p>
 <p>To update it:</p>
 <ol class="arabic">
 <li><p>Make the changes in <cite>src/docs</cite></p></li>
```

#### html2text {}

```diff
@@ -57,20 +57,20 @@
       $ make develop
    3. Runghevaluator
       $ ghevaluator ...
 
 ***** TestsÂ¶ *****
 The code and individual functions are covered by tests, usingunittests.
 We also recommend to run them locally before pushing to GitHub with:
-$ make test
+   1. Export the Galaxy API key as environment variable
+      $ export GALAXY_API_KEY=<REPLACE_WITH_GALAXY_API_KEY>
+   2. Run the unit tests
+      $ make test
 After adding new function or making changes to an existing function, make sure
-to make changes to the unittest files under thetestfolder.
-In addition to unit tests, the overall functionality and the intergration of
-the tool is tested viasubprocessunder theintegration testfolder. It also runs
-automatically everytime someone pushes or commits to the git repository.
+to make changes to the tests in thetestfolder.
 
 ***** DocumentationÂ¶ *****
 This documentation is generated using Sphinx.
 To update it:
    1. Make the changes insrc/docs
    2. Generate the doc with
       $ make doc
```

### Comparing `ghevaluator-2.0.0/docs/genindex.html` & `ghevaluator-2.1.0/docs/genindex.html`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.0.0/docs/index.html` & `ghevaluator-2.1.0/docs/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,17 @@
         <div class="bodywrapper">
           
 
           <div class="body" role="main">
             
   <section id="welcome-to-galaxy-history-evaluator-s-documentation">
 <h1>Welcome to Galaxy History Evaluator’s documentation!<a class="headerlink" href="#welcome-to-galaxy-history-evaluator-s-documentation" title="Permalink to this heading">¶</a></h1>
-<p>A command-line tool to evaluate a Galaxy history, by comparing the history’s corresponding workflow with a reference workflow. The output result is a JSON file reporting the differences between the two histories/workflows.</p>
+<p>A command-line tool to evaluate a Galaxy history, by comparing the history’s corresponding workflow
+with a reference workflow.</p>
+<p>The output result are a JSON and HTML report files, reporting the differences between the history and the workflow.</p>
 <div class="toctree-wrapper compound">
 <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="usage.html#output">Output</a></li>
 </ul>
 </li>
```

#### html2text {}

```diff
@@ -4,16 +4,17 @@
 
 
 
 
 
 ****** Welcome to Galaxy History Evaluatorâs documentation!Â¶ ******
 A command-line tool to evaluate a Galaxy history, by comparing the historyâs
-corresponding workflow with a reference workflow. The output result is a JSON
-file reporting the differences between the two histories/workflows.
+corresponding workflow with a reference workflow.
+The output result are a JSON and HTML report files, reporting the differences
+between the history and the workflow.
 Contents:
     * Usage
           o Output
     * Installation
           o Requirements
           o Installation_via_pip
     * API_documentation
```

### Comparing `ghevaluator-2.0.0/docs/installation.html` & `ghevaluator-2.1.0/docs/installation.html`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.0.0/docs/py-modindex.html` & `ghevaluator-2.1.0/docs/py-modindex.html`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.0.0/docs/search.html` & `ghevaluator-2.1.0/docs/search.html`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.0.0/docs/searchindex.js` & `ghevaluator-2.1.0/docs/searchindex.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -48,30 +48,30 @@
         "still": 1,
         "one": 1,
         "against": 1,
         "order": 1,
         "realiz": 1,
         "goal": 1,
         "simpli": 1,
-        "two": [1, 2],
+        "two": 1,
         "some": 1,
         "modif": 1,
         "done": 1,
         "For": [1, 4],
         "exampl": [1, 4],
         "structur": 1,
         "final": 1,
         "ha": 1,
         "alterd": 1,
         "becaus": 1,
         "onli": 1,
         "track": 1,
         "which": 1,
         "part": 1,
-        "ar": 1,
+        "ar": [1, 2],
         "miss": 1,
         "wrong": 1,
         "In": 1,
         "anoth": 1,
         "word": 1,
         "standard": 1,
         "so": 1,
@@ -151,57 +151,54 @@
         "run": 1,
         "individu": 1,
         "function": 1,
         "cover": 1,
         "unittest": 1,
         "also": [1, 4],
         "recommend": 1,
+        "export": 1,
+        "api": [1, 2, 4],
+        "kei": [1, 4],
+        "environ": 1,
+        "variabl": 1,
+        "galaxy_api_kei": 1,
+        "replace_with_galaxy_api_kei": 1,
+        "unit": 1,
         "ad": 1,
         "sure": 1,
-        "under": 1,
-        "addit": 1,
-        "unit": 1,
-        "overal": 1,
-        "intergr": 1,
-        "subprocess": 1,
-        "integr": 1,
-        "everytim": 1,
-        "someon": 1,
-        "git": 1,
         "gener": [1, 4],
         "src": 1,
         "doc": 1,
         "check": 1,
         "open": 1,
         "index": [1, 2],
-        "html": 1,
+        "html": [1, 2, 4],
         "web": 1,
         "browser": 1,
         "usag": [1, 2],
         "mai": 1,
         "refer": [1, 2, 4],
         "here": [1, 4],
         "www": 1,
         "org": [1, 4],
         "en": 1,
         "A": 2,
         "correspond": [2, 4],
         "output": 2,
         "result": 2,
-        "i": [2, 4],
         "json": [2, 4],
         "report": [2, 4],
         "between": 2,
         "instal": 2,
         "requir": 2,
         "pip": 2,
-        "api": [2, 4],
         "contribut": 2,
         "what": 2,
         "should": [2, 4],
+        "i": [2, 4],
         "know": 2,
         "befor": 2,
         "get": [2, 4],
         "start": 2,
         "how": 2,
         "can": [2, 4],
         "develop": 2,
@@ -218,15 +215,14 @@
         "apikei": 4,
         "o": 4,
         "option": 4,
         "show": 4,
         "messag": 4,
         "exit": 4,
         "url": 4,
-        "kei": 4,
         "path": 4,
         "input": 4,
         "publish": 4,
         "your": 4,
         "share": 4,
         "link": 4,
         "explain": 4,
@@ -321,38 +317,14 @@
         "sphinx.domains.std": 2,
         "sphinx": 57
     },
     "alltitles": {
         "API documentation": [
             [0, "module-__main__"]
         ],
-        "Contributing": [
-            [1, "contributing"]
-        ],
-        "What should I know before I get started?": [
-            [1, "what-should-i-know-before-i-get-started"]
-        ],
-        "How can I contribute?": [
-            [1, "how-can-i-contribute"]
-        ],
-        "Reporting mistakes or errors": [
-            [1, "reporting-mistakes-or-errors"]
-        ],
-        "Your first content contribution": [
-            [1, "your-first-content-contribution"]
-        ],
-        "Development": [
-            [1, "development"]
-        ],
-        "Tests": [
-            [1, "tests"]
-        ],
-        "Documentation": [
-            [1, "documentation"]
-        ],
         "Welcome to Galaxy History Evaluator\u2019s documentation!": [
             [2, "welcome-to-galaxy-history-evaluator-s-documentation"]
         ],
         "Contents:": [
             [2, null]
         ],
         "Indices and tables": [
@@ -368,14 +340,38 @@
             [3, "installation-via-pip"]
         ],
         "Usage": [
             [4, "usage"]
         ],
         "Output": [
             [4, "output"]
+        ],
+        "Contributing": [
+            [1, "contributing"]
+        ],
+        "What should I know before I get started?": [
+            [1, "what-should-i-know-before-i-get-started"]
+        ],
+        "How can I contribute?": [
+            [1, "how-can-i-contribute"]
+        ],
+        "Reporting mistakes or errors": [
+            [1, "reporting-mistakes-or-errors"]
+        ],
+        "Your first content contribution": [
+            [1, "your-first-content-contribution"]
+        ],
+        "Development": [
+            [1, "development"]
+        ],
+        "Tests": [
+            [1, "tests"]
+        ],
+        "Documentation": [
+            [1, "documentation"]
         ]
     },
     "indexentries": {
         "__main__": [
             [0, "module-__main__"]
         ],
         "module": [
```

### Comparing `ghevaluator-2.0.0/docs/usage.html` & `ghevaluator-2.1.0/docs/usage.html`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             
   <section id="usage">
 <h1>Usage<a class="headerlink" href="#usage" title="Permalink to this heading">¶</a></h1>
 <p>Galaxy History Evaluator can be used via command-line</p>
 <div class="highlight-bash notranslate"><div class="highlight"><pre><span></span>$<span class="w"> </span>ghevaluator<span class="w"> </span>--help
 usage:<span class="w"> </span>ghevaluator<span class="w"> </span><span class="o">[</span>-h<span class="o">]</span><span class="w"> </span>-u<span class="w"> </span>HISTORY_URL<span class="w"> </span>-w<span class="w"> </span>WORKFLOW_URL<span class="w"> </span>-a<span class="w"> </span>APIKEY<span class="w"> </span><span class="o">[</span>-o<span class="w"> </span>OUTPUT<span class="o">]</span>
 
-Compare<span class="w"> </span>a<span class="w"> </span>Galaxy<span class="w"> </span><span class="nb">history</span><span class="w"> </span>to<span class="w"> </span>a<span class="w"> </span>template<span class="w"> </span>workflow<span class="w"> </span>and<span class="w"> </span>generate<span class="w"> </span>a<span class="w"> </span>JSON<span class="w"> </span>report<span class="w"> </span>file
+Compare<span class="w"> </span>a<span class="w"> </span>Galaxy<span class="w"> </span><span class="nb">history</span><span class="w"> </span>to<span class="w"> </span>a<span class="w"> </span>template<span class="w"> </span>workflow<span class="w"> </span>and<span class="w"> </span>generate<span class="w"> </span>the<span class="w"> </span>JSON<span class="w"> </span>and<span class="w"> </span>HTML<span class="w"> </span>report<span class="w"> </span>files
 
 options:
 -h,<span class="w"> </span>--help<span class="w">            </span>show<span class="w"> </span>this<span class="w"> </span><span class="nb">help</span><span class="w"> </span>message<span class="w"> </span>and<span class="w"> </span><span class="nb">exit</span>
 -u<span class="w"> </span>HISTORY_URL,<span class="w"> </span>--history_url<span class="w"> </span>HISTORY_URL
 <span class="w">                        </span>URL<span class="w"> </span>to<span class="w"> </span>Galaxy<span class="w"> </span><span class="nb">history</span>
 -w<span class="w"> </span>WORKFLOW_URL,<span class="w"> </span>--workflow_url<span class="w"> </span>WORKFLOW_URL
 <span class="w">                        </span>URL<span class="w"> </span>to<span class="w"> </span>template<span class="w"> </span>workflow
```

#### html2text {}

```diff
@@ -8,15 +8,16 @@
 
 
 ****** UsageÂ¶ ******
 Galaxy History Evaluator can be used via command-line
 $ ghevaluator --help
 usage: ghevaluator [-h] -u HISTORY_URL -w WORKFLOW_URL -a APIKEY [-o OUTPUT]
 
-Compare a Galaxy history to a template workflow and generate a JSON report file
+Compare a Galaxy history to a template workflow and generate the JSON and HTML
+report files
 
 options:
 -h, --help            show this help message and exit
 -u HISTORY_URL, --history_url HISTORY_URL
                         URL to Galaxy history
 -w WORKFLOW_URL, --workflow_url WORKFLOW_URL
                         URL to template workflow
```

### Comparing `ghevaluator-2.0.0/ghevaluator/__init__.py` & `ghevaluator-2.1.0/ghevaluator/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import json
 import requests
 
 from bioblend.galaxy import GalaxyInstance
+from jinja2 import Environment, PackageLoader, select_autoescape
 from pathlib import Path
 from urllib import parse
 
 
 def get_hist_info(hist_url):
     """
     Get history name and Galaxy URL from history URL
@@ -176,19 +177,19 @@
 def fill_step_comparison(ref_step, hist_step, key):
     """
     Compare reference and history steps for a specific key
 
     :param ref_step: dictionary with reference step
     :param hist_step: dictionary with history step
     :param key: key of values to compare
-    :return: dictionary with expected, history, same
+    :return: dictionary with workflow, history, same
     """
     hist_value = hist_step[key] if hist_step is not None else None
     return {
-        'expected': ref_step[key],
+        'workflow': ref_step[key],
         'history': hist_value,
         'same': bool(ref_step[key] == hist_value)
     }
 
 
 def fill_step_report(ref_step, hist_step=None):
     """
@@ -202,27 +203,27 @@
         "tool": fill_step_comparison(ref_step, hist_step, 'tool'),
         "id": fill_step_comparison(ref_step, hist_step, 'id'),
         "owner": fill_step_comparison(ref_step, hist_step, 'owner'),
         "version": fill_step_comparison(ref_step, hist_step, 'version'),
         "order": fill_step_comparison(ref_step, hist_step, 'order'),
         "parameters": {
             'number': {
-                'expected': len(ref_step['parameters']),
+                'workflow': len(ref_step['parameters']),
                 'history': len(hist_step['parameters']) if hist_step is not None else None,
                 'same': bool(len(ref_step['parameters']) == len(hist_step['parameters'])) if hist_step is not None else False
             },
             'wrong': len(ref_step['parameters']),
             'details': {}
         },
         "inputs_connection": fill_step_comparison(ref_step, hist_step, 'inputs_connection')
     }
     # compare parameters
     for p in ref_step['parameters']:
         s_report['parameters']['details'][p] = {
-            'expected': ref_step['parameters'][p],
+            'workflow': ref_step['parameters'][p],
             'history': hist_step['parameters'][p] if hist_step is not None and p in hist_step['parameters'] else None,
             'same': bool(ref_step['parameters'][p] == hist_step['parameters'][p]) if hist_step is not None and p in hist_step['parameters'] else False
         }
         if s_report['parameters']['details'][p]['same']:
             s_report['parameters']['wrong'] -= 1
     return s_report
 
@@ -245,74 +246,93 @@
             h_step_count += 1
         else:
             print("Need to implement input connection comparison so order is similar")
             comparison[i] = fill_step_report(ref_step, None)
     return comparison
 
 
-def compare_workflows(hist_wf, ref_wf):
+def compare_workflows(hist_wf, ref_wf, report):
     """
     Compare a user workflow to a reference workflow and generate a report
 
     :param hist_wf: dictorionary with history extracted workflow
     :param ref_wf: dictionary with reference workflow
     :return: dictionary with report
     """
-    report = {}
     hist_wf = hist_wf['steps']
     ref_wf = ref_wf['steps']
     # Reformate workflows
     ordered_hist_wf, hist_wf_by_tool = reformate_workflows(hist_wf)
     ordered_ref_wf, ref_wf_by_tool = reformate_workflows(ref_wf)
     report['reference_wf'] = ordered_ref_wf
     report['history_wf'] = ordered_hist_wf
     # Compare inputs in both workflows
     hist_wf_input_nb = count_wf_inputs(hist_wf)
     ref_wf_input_nb = count_wf_inputs(ref_wf)
     report['data_inputs'] = {
-        "expected": ref_wf_input_nb,
+        "workflow": ref_wf_input_nb,
         "history": hist_wf_input_nb,
         "same": bool(ref_wf_input_nb == hist_wf_input_nb)
     }
     # Compare number of steps in both workflows
     hist_step_nb = len(hist_wf) - hist_wf_input_nb
     ref_step_nb = len(ref_wf) - ref_wf_input_nb
     report['steps'] = {
-        'expected': ref_step_nb,
+        'workflow': ref_step_nb,
         'history': hist_step_nb,
         'same': bool(ref_step_nb == hist_step_nb)
     }
     # Compare ordered workflows
     report['comparison_given_reference_workflow_order'] = compare_ordered_steps(ordered_ref_wf, ordered_hist_wf)
     # Compare workflows by tools
     comparison = {}
     for tool in ref_wf_by_tool:
         comparison[tool] = {
             'number': {
-                'expected': len(ref_wf_by_tool[tool]),
+                'workflow': len(ref_wf_by_tool[tool]),
                 'history': len(hist_wf_by_tool[tool]) if tool in hist_wf_by_tool else 0,
                 'same': bool(len(ref_wf_by_tool[tool]) == len(hist_wf_by_tool[tool])) if tool in hist_wf_by_tool else False
             },
             'details': compare_ordered_steps(ref_wf_by_tool[tool], hist_wf_by_tool[tool] if tool in hist_wf_by_tool else None)
         }
     report['comparison_by_reference_workflow_tools'] = comparison
     return report
 
 
+def generate_html_report_content(data):
+    """
+    Generate HTML report
+
+    :param data: dictionary holding the information of the status of key features of user history
+    """
+    env = Environment(
+        loader=PackageLoader("ghevaluator", "templates"),
+        autoescape=select_autoescape()
+    )
+    template = env.get_template("report.html")
+    return template.render(report=data)
+
+
 def generate_report_files(data, output_dp):
     """
-    Convert the report dictionary into a JSON file
+    Convert the report dictionary into a JSON file and a HTML file
 
     :param data: dictionary holding the information of the status of key features of user history
     :param output_dp: Path object of the output directory
     """
+    output_dp.mkdir(parents=True, exist_ok=True)
+
     json_fp = output_dp / Path("report.json")
     with json_fp.open('w') as out_f:
         json.dump(data, out_f, ensure_ascii=False, indent=4)
 
+    html_fp = output_dp / Path("report.html")
+    with html_fp.open('w') as out_f:
+        out_f.write(generate_html_report_content(data))
+
 
 def ghevaluator(hist_url, wf_url, apikey, output_dp):
     """
     The main function
 
     This function serves as the driver and connection between all major parts of the program:
 
@@ -323,9 +343,9 @@
     :param hist_url: URL to Galaxy history
     :param wf_url: URL to template workflow
     :param apikey: a Galaxy API key obtained prehand
     :param output_dp: Path object of the output report
     """
     hist_wf = get_workflow_from_history(hist_url, apikey)
     ref_wf = get_standard_workflow(wf_url)
-    report = compare_workflows(hist_wf, ref_wf)
+    report = compare_workflows(hist_wf, ref_wf, {'inputs': {'history': hist_url, 'workflow': wf_url}})
     generate_report_files(report, output_dp)
```

### Comparing `ghevaluator-2.0.0/ghevaluator/__main__.py` & `ghevaluator-2.1.0/ghevaluator/__main__.py`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.0.0/ghevaluator.egg-info/PKG-INFO` & `ghevaluator-2.1.0/ghevaluator.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghevaluator
-Version: 2.0.0
+Version: 2.1.0
 Summary: A command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON report file.
 Author: Teresa Müller
 Author-email: Siyu Chen <chensy96@gmail.com>, Bérénice Batut <berenice.batut@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Siyu Chen
         
@@ -35,36 +35,36 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Galaxy History Evaluator
 ========================
 
-Galaxy History Evaluator or `ghevaluator` is a command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON report file.
+Galaxy History Evaluator or `ghevaluator` is a command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON and HTML report files.
 
 ## Context
 
 [Galaxy](https://galaxyproject.org/) is an **open, web-based platform for data-intensive computational research**.
 
 When running their data analysis, Galaxy users create histories storing their data, but also the steps of the data analysis, i.e. the tools used, their versions and parameters.
 
 Galaxy is also used for training where participants follow step-by-step tutorials, stored in Galaxy histories. At the end, participants might want to know if they followed correctly the tutorial and instructors might need to evaluate histories to give feedback and deliver certificates.
 **Evaluating histories manually can be painful and error prone**.
 
-Galaxy History Evaluator aims to solve this by providing a command-line tool to compare a Galaxy history to a templare workflow and generate a report in JSON with difference between the provided history and the expected workflow.
+Galaxy History Evaluator aims to solve this by providing a command-line tool to compare a Galaxy history to a templare workflow and generate a report in JSON and HTML with difference between the provided history and the expected workflow.
 
 ## Usage
 
 Galaxy History Evaluator can be used via command-line
 
 ```bash
 $ ghevaluator --help
 usage: ghevaluator [-h] -u HISTORY_URL -w WORKFLOW_URL -a APIKEY [-o OUTPUT]
 
-Compare a Galaxy history to a template workflow and generate a JSON report file
+Compare a Galaxy history to a template workflow and generate the JSON and HTML report files
 
 options:
   -h, --help            show this help message and exit
   -u HISTORY_URL, --history_url HISTORY_URL
                         URL to Galaxy history
   -w WORKFLOW_URL, --workflow_url WORKFLOW_URL
                         URL to template workflow
@@ -83,21 +83,21 @@
 ```
 
 ## Tests
 
 1. Export the Galaxy API key as environment variable
 
   ```bash
-  $ export GALAXY_APIKEY = <>
+  $ export GALAXY_API_KEY=<REPLACE_WITH_GALAXY_API_KEY>
   ```
 
 2. Run the unit tests
 
   ```bash
-  $ make tests
+  $ make test
   ```
 
 
 ## Documentation
 
 
 Documentation could be found at https://streetscience.community/ghevaluator/
```

### Comparing `ghevaluator-2.0.0/ghevaluator.egg-info/SOURCES.txt` & `ghevaluator-2.1.0/ghevaluator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 docs/.buildinfo
-docs/.nojekyll
 docs/api_documentation.html
 docs/contributing.html
 docs/genindex.html
 docs/index.html
 docs/installation.html
 docs/objects.inv
 docs/py-modindex.html
```

### Comparing `ghevaluator-2.0.0/pyproject.toml` & `ghevaluator-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghevaluator"
-version = "2.0.0"
+version = "2.1.0"
 authors = [
   { name="Siyu Chen", email="chensy96@gmail.com" },
   { name="Teresa Müller" },
   { name="Bérénice Batut", email="berenice.batut@gmail.com" },
 ]
 description = "A command-line Python tool to compare Galaxy histories to a template workflow and generate a JSON report file."
 readme = "README.md"
```

### Comparing `ghevaluator-2.0.0/src/docs/conf.py` & `ghevaluator-2.1.0/src/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ghevaluator-2.0.0/tests/test_ghevaluator.py` & `ghevaluator-2.1.0/tests/test_ghevaluator.py`

 * *Files 8% similar despite different names*

```diff
@@ -169,18 +169,18 @@
     """
     """
     key = 'key'
     value = 1
     ref_step = {key: value}
     comparison = ghevaluator.fill_step_comparison(ref_step, None, key)
     assert isinstance(comparison, dict)
-    assert 'expected' in comparison
+    assert 'workflow' in comparison
     assert 'history' in comparison
     assert 'same' in comparison
-    assert comparison['expected'] == value
+    assert comparison['workflow'] == value
     assert comparison['history'] is None
     assert not comparison['same']
     comparison = ghevaluator.fill_step_comparison(ref_step, ref_step, key)
     assert comparison['history'] == value
     assert comparison['same']
     comparison = ghevaluator.fill_step_comparison(ref_step, {key: value + 1}, key)
     assert comparison['history'] == value + 1
@@ -207,25 +207,25 @@
     assert "id" in report
     assert "owner" in report
     assert "version" in report
     assert "parameters" in report
     assert "inputs_connection" in report
     assert "order" in report
     assert isinstance(report['tool'], dict)
-    assert "expected" in report['tool']
-    assert report['tool']['expected'] == 'tool'
+    assert "workflow" in report['tool']
+    assert report['tool']['workflow'] == 'tool'
     assert report['tool']['history'] is None
     assert isinstance(report['parameters'], dict)
     assert "number" in report['parameters']
     assert isinstance(report['parameters']['number'], dict)
-    assert report['parameters']['number']['expected'] == 1
+    assert report['parameters']['number']['workflow'] == 1
     assert report['parameters']['number']['history'] is None
     assert isinstance(report['parameters']['details'], dict)
     assert "p1" in report['parameters']['details']
-    assert report['parameters']['details']['p1']['expected'] == 'p1'
+    assert report['parameters']['details']['p1']['workflow'] == 'p1'
     assert report['parameters']['details']['p1']['history'] is None
     report = ghevaluator.fill_step_report(ref_step, ref_step)
     assert report['tool']['history'] == 'tool'
     assert report['parameters']['number']['history'] == 1
     assert report['parameters']['details']['p1']['history'] == 'p1'
 
 
@@ -271,43 +271,65 @@
 
 
 def test_compare_workflows():
     """
     """
     ref_wf = ghevaluator.get_standard_workflow(WF_URL)
     hist_wf = ghevaluator.get_workflow_from_history(HIST_URL, APIKEY)
-    report = ghevaluator.compare_workflows(hist_wf, ref_wf)
+    report = ghevaluator.compare_workflows(hist_wf, ref_wf, {})
     assert isinstance(report, dict)
     assert "reference_wf" in report
     assert "history_wf" in report
     assert "data_inputs" in report
     assert isinstance(report['data_inputs'], dict)
-    assert 'expected' in report['data_inputs']
-    assert report['data_inputs']['expected'] == 1
+    assert 'workflow' in report['data_inputs']
+    assert report['data_inputs']['workflow'] == 1
     assert report['data_inputs']['history'] == 1
     assert report['data_inputs']['same']
     assert "steps" in report
     assert isinstance(report['steps'], dict)
-    assert 'expected' in report['steps']
-    assert report['steps']['expected'] == 3
+    assert 'workflow' in report['steps']
+    assert report['steps']['workflow'] == 3
     assert report['steps']['history'] == 3
     assert report['steps']['same']
     assert "comparison_given_reference_workflow_order" in report
     assert isinstance(report["comparison_given_reference_workflow_order"], dict)
     assert "comparison_by_reference_workflow_tools" in report
     assert isinstance(report["comparison_by_reference_workflow_tools"], dict)
 
 
+def test_generate_html_report_content():
+    """
+    """
+    ref_wf = ghevaluator.get_standard_workflow(WF_URL)
+    hist_wf = ghevaluator.get_workflow_from_history(HIST_URL, APIKEY)
+    report = ghevaluator.compare_workflows(hist_wf, ref_wf, {'inputs': {'history': HIST_URL, 'workflow': WF_URL}})
+    content = ghevaluator.generate_html_report_content(report)
+    assert 'Galaxy History Evaluator report' in content
+    assert 'fa-check-square' in content
+    assert 'fa-exclamation-triangle' in content
+    assert 'FastQC' in content
+    assert '1.0.2+galaxy0' in content
+    assert 'Occurence 1' in content
+
+
 def test_generate_report_files():
     """
     """
-    ghevaluator.generate_report_files({}, Path("."))
+    ref_wf = ghevaluator.get_standard_workflow(WF_URL)
+    hist_wf = ghevaluator.get_workflow_from_history(HIST_URL, APIKEY)
+    report = ghevaluator.compare_workflows(hist_wf, ref_wf, {'inputs': {'history': HIST_URL, 'workflow': WF_URL}})
+    ghevaluator.generate_report_files(report, Path("."))
     assert Path("report.json").exists
     Path("report.json").unlink()
+    assert Path("report.html").exists
+    Path("report.html").unlink()
 
 
 def test_ghevaluator():
     """
     """
     ghevaluator.ghevaluator(HIST_URL, WF_URL, APIKEY, Path("."))
     assert Path("report.json").exists
     Path("report.json").unlink()
+    assert Path("report.html").exists
+    Path("report.html").unlink()
```

