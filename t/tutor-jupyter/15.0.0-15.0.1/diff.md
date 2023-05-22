# Comparing `tmp/tutor-jupyter-15.0.0.tar.gz` & `tmp/tutor-jupyter-15.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-jupyter-15.0.0.tar", last modified: Tue May 16 13:48:49 2023, max compression
+gzip compressed data, was "dist/tutor-jupyter-15.0.1.tar", last modified: Mon May 22 07:45:20 2023, max compression
```

## Comparing `tutor-jupyter-15.0.0.tar` & `tutor-jupyter-15.0.1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     5843 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     4942 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1774 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutor_jupyter.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     5843 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutor_jupyter.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1134 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutor_jupyter.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutor_jupyter.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutor_jupyter.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutor_jupyter.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       13 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutor_jupyter.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/
--rw-r--r--   0 ci        (1000) ci        (1000)       23 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/dev-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      297 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      464 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      193 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/openedx-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/patches/openedx-dockerfile-post-python-requirements
--rw-r--r--   0 ci        (1000) ci        (1000)     4145 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/apps/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/apps/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)     4185 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/hub/
--rw-r--r--   0 ci        (1000) ci        (1000)      606 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/hub/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/lab/
--rw-r--r--   0 ci        (1000) ci        (1000)      838 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/lab/Dockerfile
--rw-r--r--   0 ci        (1000) ci        (1000)      295 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/lab/config.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/jobs/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:49.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/jobs/init/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/jobs/init/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/jobs/init/jupyterhub.sh
--rw-r--r--   0 ci        (1000) ci        (1000)      862 2023-05-16 13:48:39.000000 tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/jobs/init/mysql.sh
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     6018 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     5117 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1774 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutor_jupyter.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6018 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutor_jupyter.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1149 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutor_jupyter.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutor_jupyter.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutor_jupyter.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       48 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutor_jupyter.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       13 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutor_jupyter.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/
+-rw-r--r--   0 ci        (1000) ci        (1000)       23 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)       78 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)       84 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/dev-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      297 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      464 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      193 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/openedx-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      176 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/patches/openedx-dockerfile-post-python-requirements
+-rw-r--r--   0 ci        (1000) ci        (1000)     4145 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/apps/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/apps/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)     4185 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/hub/
+-rw-r--r--   0 ci        (1000) ci        (1000)      606 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/hub/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/lab/
+-rw-r--r--   0 ci        (1000) ci        (1000)      838 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/lab/Dockerfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      295 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/lab/config.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/jobs/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:20.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/jobs/init/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/jobs/init/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/jobs/init/jupyterhub.sh
+-rw-r--r--   0 ci        (1000) ci        (1000)      862 2023-05-22 07:45:07.000000 tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/jobs/init/mysql.sh
```

### Comparing `tutor-jupyter-15.0.0/LICENSE.txt` & `tutor-jupyter-15.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.0/PKG-INFO` & `tutor-jupyter-15.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-jupyter
-Version: 15.0.0
+Version: 15.0.1
 Summary: Jupyter Notebook plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-jupyter
 Author: Overhang.IO
 Maintainer: Régis Behmo
 Maintainer-email: regis@overhang.io
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-jupyter
@@ -59,19 +59,24 @@
 
     tutor local launch
 
 Print the default passport ID::
 
     echo "$(tutor config printvalue JUPYTER_DEFAULT_PASSPORT_ID):$(tutor config printvalue JUPYTER_LTI_CLIENT_KEY):$(tutor config printvalue JUPYTER_LTI_CLIENT_SECRET)"
 
-Make a note of the printed value. Go to the Studio Tools ➡️ Advanced Settings ➡️ LTI Passports. Insert the passport value.
+Make a note of the printed value. Go to the Studio Tools ➡️ Advanced Settings ➡️ LTI Passports. Insert the passport value:
 
-In "Advanced Module List" add "jupyter" (with quotes)::
+.. image:: https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings-lti.png
+     :alt: Studio advanced settings
 
-![jupyter xblock advanced settings](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings.png)
+
+In "Advanced Module List" add "jupyter" (with quotes):
+
+.. image:: https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings.png
+     :alt: Studio advanced settings
 
 You should then be able to create an advanced Jupyter XBlock in the Studio:
 
 > Add New Component ➡️ Advanced ➡️ Jupyter notebook
 
 The default `"hello" <https://github.com/overhangio/jupyter-xblock/blob/main/static/notebooks/hello.ipynb>`__  notebook will be pulled from the jupyter-block repository and displayed in the studio.
```

### Comparing `tutor-jupyter-15.0.0/README.rst` & `tutor-jupyter-15.0.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -36,19 +36,24 @@
 
     tutor local launch
 
 Print the default passport ID::
 
     echo "$(tutor config printvalue JUPYTER_DEFAULT_PASSPORT_ID):$(tutor config printvalue JUPYTER_LTI_CLIENT_KEY):$(tutor config printvalue JUPYTER_LTI_CLIENT_SECRET)"
 
-Make a note of the printed value. Go to the Studio Tools ➡️ Advanced Settings ➡️ LTI Passports. Insert the passport value.
+Make a note of the printed value. Go to the Studio Tools ➡️ Advanced Settings ➡️ LTI Passports. Insert the passport value:
 
-In "Advanced Module List" add "jupyter" (with quotes)::
+.. image:: https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings-lti.png
+     :alt: Studio advanced settings
 
-![jupyter xblock advanced settings](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings.png)
+
+In "Advanced Module List" add "jupyter" (with quotes):
+
+.. image:: https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings.png
+     :alt: Studio advanced settings
 
 You should then be able to create an advanced Jupyter XBlock in the Studio:
 
 > Add New Component ➡️ Advanced ➡️ Jupyter notebook
 
 The default `"hello" <https://github.com/overhangio/jupyter-xblock/blob/main/static/notebooks/hello.ipynb>`__  notebook will be pulled from the jupyter-block repository and displayed in the studio.
```

### Comparing `tutor-jupyter-15.0.0/setup.py` & `tutor-jupyter-15.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.0/tutor_jupyter.egg-info/PKG-INFO` & `tutor-jupyter-15.0.1/tutor_jupyter.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-jupyter
-Version: 15.0.0
+Version: 15.0.1
 Summary: Jupyter Notebook plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-jupyter
 Author: Overhang.IO
 Maintainer: Régis Behmo
 Maintainer-email: regis@overhang.io
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-jupyter
@@ -59,19 +59,24 @@
 
     tutor local launch
 
 Print the default passport ID::
 
     echo "$(tutor config printvalue JUPYTER_DEFAULT_PASSPORT_ID):$(tutor config printvalue JUPYTER_LTI_CLIENT_KEY):$(tutor config printvalue JUPYTER_LTI_CLIENT_SECRET)"
 
-Make a note of the printed value. Go to the Studio Tools ➡️ Advanced Settings ➡️ LTI Passports. Insert the passport value.
+Make a note of the printed value. Go to the Studio Tools ➡️ Advanced Settings ➡️ LTI Passports. Insert the passport value:
 
-In "Advanced Module List" add "jupyter" (with quotes)::
+.. image:: https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings-lti.png
+     :alt: Studio advanced settings
 
-![jupyter xblock advanced settings](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings.png)
+
+In "Advanced Module List" add "jupyter" (with quotes):
+
+.. image:: https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings.png
+     :alt: Studio advanced settings
 
 You should then be able to create an advanced Jupyter XBlock in the Studio:
 
 > Add New Component ➡️ Advanced ➡️ Jupyter notebook
 
 The default `"hello" <https://github.com/overhangio/jupyter-xblock/blob/main/static/notebooks/hello.ipynb>`__  notebook will be pulled from the jupyter-block repository and displayed in the studio.
```

### Comparing `tutor-jupyter-15.0.0/tutor_jupyter.egg-info/SOURCES.txt` & `tutor-jupyter-15.0.1/tutor_jupyter.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.py
 tutor_jupyter.egg-info/PKG-INFO
 tutor_jupyter.egg-info/SOURCES.txt
 tutor_jupyter.egg-info/dependency_links.txt
 tutor_jupyter.egg-info/entry_points.txt
 tutor_jupyter.egg-info/requires.txt
 tutor_jupyter.egg-info/top_level.txt
```

### Comparing `tutor-jupyter-15.0.0/tutorjupyter/plugin.py` & `tutor-jupyter-15.0.1/tutorjupyter/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py` & `tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/apps/jupyterhub_config.py`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/hub/Dockerfile` & `tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/hub/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/build/lab/Dockerfile` & `tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/build/lab/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-jupyter-15.0.0/tutorjupyter/templates/jupyter/jobs/init/mysql.sh` & `tutor-jupyter-15.0.1/tutorjupyter/templates/jupyter/jobs/init/mysql.sh`

 * *Files identical despite different names*

