# Comparing `tmp/pyxecm-llm-0.0.0.tar.gz` & `tmp/pyxecm-llm-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxecm-llm-0.0.0.tar", last modified: Mon May 22 17:51:06 2023, max compression
+gzip compressed data, was "pyxecm-llm-0.0.1.tar", last modified: Mon May 22 18:05:56 2023, max compression
```

## Comparing `pyxecm-llm-0.0.0.tar` & `pyxecm-llm-0.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kgatzweiler   (501) staff       (20)        0 2023-05-22 17:51:06.152806 pyxecm-llm-0.0.0/
--rw-r--r--   0 kgatzweiler   (501) staff       (20)    11360 2023-05-22 17:43:50.000000 pyxecm-llm-0.0.0/LICENSE
--rw-r--r--   0 kgatzweiler   (501) staff       (20)     7008 2023-05-22 17:51:06.152637 pyxecm-llm-0.0.0/PKG-INFO
--rw-r--r--   0 kgatzweiler   (501) staff       (20)     6205 2023-05-22 17:39:04.000000 pyxecm-llm-0.0.0/README.md
--rw-r--r--   0 kgatzweiler   (501) staff       (20)      879 2023-05-22 17:48:44.000000 pyxecm-llm-0.0.0/pyproject.toml
-drwxr-xr-x   0 kgatzweiler   (501) staff       (20)        0 2023-05-22 17:51:06.151474 pyxecm-llm-0.0.0/pyxecm-llm/
--rw-r--r--   0 kgatzweiler   (501) staff       (20)    15046 2023-05-22 17:48:03.000000 pyxecm-llm-0.0.0/pyxecm-llm/llm.py
-drwxr-xr-x   0 kgatzweiler   (501) staff       (20)        0 2023-05-22 17:51:06.152381 pyxecm-llm-0.0.0/pyxecm_llm.egg-info/
--rw-r--r--   0 kgatzweiler   (501) staff       (20)     7008 2023-05-22 17:51:06.000000 pyxecm-llm-0.0.0/pyxecm_llm.egg-info/PKG-INFO
--rw-r--r--   0 kgatzweiler   (501) staff       (20)      228 2023-05-22 17:51:06.000000 pyxecm-llm-0.0.0/pyxecm_llm.egg-info/SOURCES.txt
--rw-r--r--   0 kgatzweiler   (501) staff       (20)        1 2023-05-22 17:51:06.000000 pyxecm-llm-0.0.0/pyxecm_llm.egg-info/dependency_links.txt
--rw-r--r--   0 kgatzweiler   (501) staff       (20)       85 2023-05-22 17:51:06.000000 pyxecm-llm-0.0.0/pyxecm_llm.egg-info/requires.txt
--rw-r--r--   0 kgatzweiler   (501) staff       (20)       11 2023-05-22 17:51:06.000000 pyxecm-llm-0.0.0/pyxecm_llm.egg-info/top_level.txt
--rw-r--r--   0 kgatzweiler   (501) staff       (20)       38 2023-05-22 17:51:06.152855 pyxecm-llm-0.0.0/setup.cfg
--rw-r--r--   0 kgatzweiler   (501) staff       (20)      437 2023-05-22 17:40:22.000000 pyxecm-llm-0.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:05:56.604909 pyxecm-llm-0.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2023-05-22 18:05:25.000000 pyxecm-llm-0.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     7008 2023-05-22 18:05:56.604909 pyxecm-llm-0.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6205 2023-05-22 18:05:25.000000 pyxecm-llm-0.0.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      878 2023-05-22 18:05:45.000000 pyxecm-llm-0.0.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:05:56.602909 pyxecm-llm-0.0.1/pyxecm-llm/
+-rw-rw-rw-   0 root         (0) root         (0)    15046 2023-05-22 18:05:25.000000 pyxecm-llm-0.0.1/pyxecm-llm/llm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 18:05:56.603909 pyxecm-llm-0.0.1/pyxecm_llm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7008 2023-05-22 18:05:56.000000 pyxecm-llm-0.0.1/pyxecm_llm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      228 2023-05-22 18:05:56.000000 pyxecm-llm-0.0.1/pyxecm_llm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 18:05:56.000000 pyxecm-llm-0.0.1/pyxecm_llm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-22 18:05:56.000000 pyxecm-llm-0.0.1/pyxecm_llm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-22 18:05:56.000000 pyxecm-llm-0.0.1/pyxecm_llm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 18:05:56.604909 pyxecm-llm-0.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      437 2023-05-22 18:05:25.000000 pyxecm-llm-0.0.1/setup.py
```

### Comparing `pyxecm-llm-0.0.0/LICENSE` & `pyxecm-llm-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxecm-llm-0.0.0/PKG-INFO` & `pyxecm-llm-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm-llm
-Version: 0.0.0
+Version: 0.0.1
 Summary: A Python library to interact with Opentext Extended ECM REST API
 Home-page: https://pypi.org/project/pyxecm-llm/
 Author-email: "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://gitlab.otxlab.net/ecm/pyxecm-llm
 Keywords: opentext extendedecm contentserver otds appworks archivecenter openai
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyxecm-llm-0.0.0/README.md` & `pyxecm-llm-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyxecm-llm-0.0.0/pyproject.toml` & `pyxecm-llm-0.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,20 @@
+
 [build-system]
-requires = ["setuptools >= 61.0"]
-build-backend = "setuptools.build_meta"
+  build-backend = "setuptools.build_meta"
+  requires = ["setuptools >= 61.0"]
 
 [project]
-name = "pyxecm-llm"
-version = "0.0.0"
-authors = [
-  { name = "Dr. Marc Diefenbruch", email = "mdiefenb@opentext.com" },
-]
-description = "A Python library to interact with Opentext Extended ECM REST API"
-readme = "README.md"
-requires-python = ">=3.10"
-classifiers = [
-  "Development Status :: 4 - Beta",
-  "Programming Language :: Python :: 3",
-  "License :: OSI Approved :: Apache Software License",
-  "Operating System :: OS Independent",
-  "Intended Audience :: Developers",
-  "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System",
-]
-dependencies = [
-  'requests < 3',
-  'requests_toolbelt',
-  'setuptools',
-  'kubernetes',
-  'python-hcl2',
-  'zipfile36',
-  'suds',
-  'pyxecm',
-]
+  classifiers = ["Development Status :: 4 - Beta", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"]
+  dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "python-hcl2", "zipfile36", "suds", "pyxecm"]
+  description = "A Python library to interact with Opentext Extended ECM REST API"
+  name = "pyxecm-llm"
+  readme = "README.md"
+  requires-python = ">=3.10"
+  version = "0.0.1"
+
+  [[project.authors]]
+    email = "mdiefenb@opentext.com"
+    name = "Dr. Marc Diefenbruch"
 
-[project.urls]
-"Homepage" = "https://gitlab.otxlab.net/ecm/pyxecm-llm"
+  [project.urls]
+    Homepage = "https://gitlab.otxlab.net/ecm/pyxecm-llm"
```

### Comparing `pyxecm-llm-0.0.0/pyxecm-llm/llm.py` & `pyxecm-llm-0.0.1/pyxecm-llm/llm.py`

 * *Files identical despite different names*

### Comparing `pyxecm-llm-0.0.0/pyxecm_llm.egg-info/PKG-INFO` & `pyxecm-llm-0.0.1/pyxecm_llm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm-llm
-Version: 0.0.0
+Version: 0.0.1
 Summary: A Python library to interact with Opentext Extended ECM REST API
 Home-page: https://pypi.org/project/pyxecm-llm/
 Author-email: "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://gitlab.otxlab.net/ecm/pyxecm-llm
 Keywords: opentext extendedecm contentserver otds appworks archivecenter openai
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

