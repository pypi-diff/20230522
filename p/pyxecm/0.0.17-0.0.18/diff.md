# Comparing `tmp/pyxecm-0.0.17.tar.gz` & `tmp/pyxecm-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxecm-0.0.17.tar", last modified: Mon May 22 10:44:53 2023, max compression
+gzip compressed data, was "pyxecm-0.0.18.tar", last modified: Mon May 22 11:45:37 2023, max compression
```

## Comparing `pyxecm-0.0.17.tar` & `pyxecm-0.0.18.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:44:53.725262 pyxecm-0.0.17/
--rw-rw-rw-   0 root         (0) root         (0)    11360 2023-05-22 10:44:36.000000 pyxecm-0.0.17/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1680 2023-05-22 10:44:53.725262 pyxecm-0.0.17/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      853 2023-05-22 10:44:36.000000 pyxecm-0.0.17/README.md
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-22 10:44:43.000000 pyxecm-0.0.17/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:44:53.723262 pyxecm-0.0.17/pyxecm/
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    33694 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/k8s.py
--rw-rw-rw-   0 root         (0) root         (0)    15046 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/llm.py
--rw-rw-rw-   0 root         (0) root         (0)    77524 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/m365.py
--rw-rw-rw-   0 root         (0) root         (0)    50994 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/main.py
--rw-rw-rw-   0 root         (0) root         (0)     9554 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/otac.py
--rw-rw-rw-   0 root         (0) root         (0)   256092 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/otcs.py
--rw-rw-rw-   0 root         (0) root         (0)   117829 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/otds.py
--rw-rw-rw-   0 root         (0) root         (0)     1627 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/otiv.py
--rw-rw-rw-   0 root         (0) root         (0)    10240 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/otpd.py
--rw-rw-rw-   0 root         (0) root         (0)   250685 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/payload.py
--rw-rw-rw-   0 root         (0) root         (0)     5986 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/sap.py
--rw-rw-rw-   0 root         (0) root         (0)     2718 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/translate.py
--rw-rw-rw-   0 root         (0) root         (0)     2719 2023-05-22 10:44:36.000000 pyxecm-0.0.17/pyxecm/web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 10:44:53.725262 pyxecm-0.0.17/pyxecm.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1680 2023-05-22 10:44:53.000000 pyxecm-0.0.17/pyxecm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-22 10:44:53.000000 pyxecm-0.0.17/pyxecm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 10:44:53.000000 pyxecm-0.0.17/pyxecm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       78 2023-05-22 10:44:53.000000 pyxecm-0.0.17/pyxecm.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-22 10:44:53.000000 pyxecm-0.0.17/pyxecm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 10:44:53.725262 pyxecm-0.0.17/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-22 10:44:36.000000 pyxecm-0.0.17/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:45:37.626434 pyxecm-0.0.18/
+-rw-rw-rw-   0 root         (0) root         (0)    11360 2023-05-22 11:45:09.000000 pyxecm-0.0.18/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-05-22 11:45:37.625434 pyxecm-0.0.18/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      853 2023-05-22 11:45:09.000000 pyxecm-0.0.18/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-05-22 11:45:22.000000 pyxecm-0.0.18/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:45:37.623434 pyxecm-0.0.18/pyxecm/
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    33694 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/k8s.py
+-rw-rw-rw-   0 root         (0) root         (0)    15046 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/llm.py
+-rw-rw-rw-   0 root         (0) root         (0)    77524 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/m365.py
+-rw-rw-rw-   0 root         (0) root         (0)    50994 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/main.py
+-rw-rw-rw-   0 root         (0) root         (0)     9554 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/otac.py
+-rw-rw-rw-   0 root         (0) root         (0)   256092 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/otcs.py
+-rw-rw-rw-   0 root         (0) root         (0)   117829 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/otds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1627 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/otiv.py
+-rw-rw-rw-   0 root         (0) root         (0)    10240 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/otpd.py
+-rw-rw-rw-   0 root         (0) root         (0)   250685 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/payload.py
+-rw-rw-rw-   0 root         (0) root         (0)     5986 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/sap.py
+-rw-rw-rw-   0 root         (0) root         (0)     2718 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/translate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2719 2023-05-22 11:45:09.000000 pyxecm-0.0.18/pyxecm/web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 11:45:37.625434 pyxecm-0.0.18/pyxecm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1680 2023-05-22 11:45:37.000000 pyxecm-0.0.18/pyxecm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      408 2023-05-22 11:45:37.000000 pyxecm-0.0.18/pyxecm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 11:45:37.000000 pyxecm-0.0.18/pyxecm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       78 2023-05-22 11:45:37.000000 pyxecm-0.0.18/pyxecm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-22 11:45:37.000000 pyxecm-0.0.18/pyxecm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-22 11:45:37.626434 pyxecm-0.0.18/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      418 2023-05-22 11:45:09.000000 pyxecm-0.0.18/setup.py
```

### Comparing `pyxecm-0.0.17/LICENSE` & `pyxecm-0.0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/PKG-INFO` & `pyxecm-0.0.18/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.17
+Version: 0.0.18
 Summary: A Python library to interact with Opentext Extended ECM REST API
 Home-page: https://pypi.org/project/pyxecm/
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://github.com/opentext/pyxecm
 Keywords: opentext extendedecm contentserver otds appworks archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyxecm-0.0.17/README.md` & `pyxecm-0.0.18/README.md`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/pyproject.toml` & `pyxecm-0.0.18/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [project]
   classifiers = ["Development Status :: 4 - Beta", "Programming Language :: Python :: 3", "License :: OSI Approved :: Apache Software License", "Operating System :: OS Independent", "Intended Audience :: Developers", "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"]
   dependencies = ["requests < 3", "requests_toolbelt", "setuptools", "kubernetes", "python-hcl2", "zipfile36", "suds"]
   description = "A Python library to interact with Opentext Extended ECM REST API"
   name = "pyxecm"
   readme = "README.md"
   requires-python = ">=3.10"
-  version = "0.0.17"
+  version = "0.0.18"
 
   [[project.authors]]
     email = "kgatzweiler@opentext.com"
     name = "Kai Gatzweiler"
 
   [[project.authors]]
     email = "mdiefenb@opentext.com"
```

### Comparing `pyxecm-0.0.17/pyxecm/k8s.py` & `pyxecm-0.0.18/pyxecm/k8s.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/pyxecm/llm.py` & `pyxecm-0.0.18/pyxecm/llm.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/pyxecm/m365.py` & `pyxecm-0.0.18/pyxecm/m365.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/pyxecm/main.py` & `pyxecm-0.0.18/pyxecm/main.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/pyxecm/otac.py` & `pyxecm-0.0.18/pyxecm/otac.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/pyxecm/otcs.py` & `pyxecm-0.0.18/pyxecm/otcs.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/pyxecm/otds.py` & `pyxecm-0.0.18/pyxecm/otds.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/pyxecm/otiv.py` & `pyxecm-0.0.18/pyxecm/otiv.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/pyxecm/otpd.py` & `pyxecm-0.0.18/pyxecm/otpd.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/pyxecm/payload.py` & `pyxecm-0.0.18/pyxecm/payload.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/pyxecm/sap.py` & `pyxecm-0.0.18/pyxecm/sap.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/pyxecm/translate.py` & `pyxecm-0.0.18/pyxecm/translate.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/pyxecm/web.py` & `pyxecm-0.0.18/pyxecm/web.py`

 * *Files identical despite different names*

### Comparing `pyxecm-0.0.17/pyxecm.egg-info/PKG-INFO` & `pyxecm-0.0.18/pyxecm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxecm
-Version: 0.0.17
+Version: 0.0.18
 Summary: A Python library to interact with Opentext Extended ECM REST API
 Home-page: https://pypi.org/project/pyxecm/
 Author-email: Kai Gatzweiler <kgatzweiler@opentext.com>, "Dr. Marc Diefenbruch" <mdiefenb@opentext.com>
 Project-URL: Homepage, https://github.com/opentext/pyxecm
 Keywords: opentext extendedecm contentserver otds appworks archivecenter
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

