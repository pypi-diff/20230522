# Comparing `tmp/jupyter-xblock-15.0.0.tar.gz` & `tmp/jupyter-xblock-15.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-xblock-15.0.0.tar", last modified: Wed Mar 29 02:50:47 2023, max compression
+gzip compressed data, was "jupyter-xblock-15.0.1.tar", last modified: Mon May 22 05:01:15 2023, max compression
```

## Comparing `jupyter-xblock-15.0.0.tar` & `jupyter-xblock-15.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-03-29 02:50:47.449866 jupyter-xblock-15.0.0/
--rw-rw-r--   0 regis     (1000) regis     (1000)    35139 2023-03-29 02:48:07.000000 jupyter-xblock-15.0.0/LICENSE.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       41 2023-03-29 02:48:07.000000 jupyter-xblock-15.0.0/MANIFEST.in
--rw-rw-r--   0 regis     (1000) regis     (1000)     4488 2023-03-29 02:50:47.449866 jupyter-xblock-15.0.0/PKG-INFO
--rw-rw-r--   0 regis     (1000) regis     (1000)     3788 2023-03-29 02:48:07.000000 jupyter-xblock-15.0.0/README.md
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-03-29 02:50:47.445866 jupyter-xblock-15.0.0/jupyter_xblock.egg-info/
--rw-rw-r--   0 regis     (1000) regis     (1000)     4488 2023-03-29 02:50:47.000000 jupyter-xblock-15.0.0/jupyter_xblock.egg-info/PKG-INFO
--rw-rw-r--   0 regis     (1000) regis     (1000)      359 2023-03-29 02:50:47.000000 jupyter-xblock-15.0.0/jupyter_xblock.egg-info/SOURCES.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)        1 2023-03-29 02:50:47.000000 jupyter-xblock-15.0.0/jupyter_xblock.egg-info/dependency_links.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       58 2023-03-29 02:50:47.000000 jupyter-xblock-15.0.0/jupyter_xblock.egg-info/entry_points.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       21 2023-03-29 02:50:47.000000 jupyter-xblock-15.0.0/jupyter_xblock.egg-info/requires.txt
--rw-rw-r--   0 regis     (1000) regis     (1000)       14 2023-03-29 02:50:47.000000 jupyter-xblock-15.0.0/jupyter_xblock.egg-info/top_level.txt
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-03-29 02:50:47.445866 jupyter-xblock-15.0.0/jupyterxblock/
--rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-03-29 02:48:07.000000 jupyter-xblock-15.0.0/jupyterxblock/__init__.py
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-03-29 02:50:47.445866 jupyter-xblock-15.0.0/jupyterxblock/static/
-drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-03-29 02:50:47.449866 jupyter-xblock-15.0.0/jupyterxblock/static/css/
--rw-rw-r--   0 regis     (1000) regis     (1000)       95 2023-03-29 02:48:07.000000 jupyter-xblock-15.0.0/jupyterxblock/static/css/student.css
--rw-rw-r--   0 regis     (1000) regis     (1000)     3816 2023-03-29 02:48:07.000000 jupyter-xblock-15.0.0/jupyterxblock/xblock.py
--rw-rw-r--   0 regis     (1000) regis     (1000)       38 2023-03-29 02:50:47.449866 jupyter-xblock-15.0.0/setup.cfg
--rwxrwxr-x   0 regis     (1000) regis     (1000)     1148 2023-03-29 02:50:07.000000 jupyter-xblock-15.0.0/setup.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-22 05:01:15.148287 jupyter-xblock-15.0.1/
+-rw-rw-r--   0 regis     (1000) regis     (1000)    35139 2023-05-22 04:46:45.000000 jupyter-xblock-15.0.1/LICENSE.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)       41 2023-05-22 04:46:44.000000 jupyter-xblock-15.0.1/MANIFEST.in
+-rw-rw-r--   0 regis     (1000) regis     (1000)     4574 2023-05-22 05:01:15.148287 jupyter-xblock-15.0.1/PKG-INFO
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3874 2023-05-22 04:49:23.000000 jupyter-xblock-15.0.1/README.md
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-22 05:01:15.148287 jupyter-xblock-15.0.1/jupyter_xblock.egg-info/
+-rw-rw-r--   0 regis     (1000) regis     (1000)     4574 2023-05-22 05:01:15.000000 jupyter-xblock-15.0.1/jupyter_xblock.egg-info/PKG-INFO
+-rw-rw-r--   0 regis     (1000) regis     (1000)      359 2023-05-22 05:01:15.000000 jupyter-xblock-15.0.1/jupyter_xblock.egg-info/SOURCES.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)        1 2023-05-22 05:01:15.000000 jupyter-xblock-15.0.1/jupyter_xblock.egg-info/dependency_links.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)       58 2023-05-22 05:01:15.000000 jupyter-xblock-15.0.1/jupyter_xblock.egg-info/entry_points.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)       21 2023-05-22 05:01:15.000000 jupyter-xblock-15.0.1/jupyter_xblock.egg-info/requires.txt
+-rw-rw-r--   0 regis     (1000) regis     (1000)       14 2023-05-22 05:01:15.000000 jupyter-xblock-15.0.1/jupyter_xblock.egg-info/top_level.txt
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-22 05:01:15.148287 jupyter-xblock-15.0.1/jupyterxblock/
+-rw-rw-r--   0 regis     (1000) regis     (1000)        0 2023-05-22 04:46:44.000000 jupyter-xblock-15.0.1/jupyterxblock/__init__.py
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-22 05:01:15.144287 jupyter-xblock-15.0.1/jupyterxblock/static/
+drwxrwxr-x   0 regis     (1000) regis     (1000)        0 2023-05-22 05:01:15.148287 jupyter-xblock-15.0.1/jupyterxblock/static/css/
+-rw-rw-r--   0 regis     (1000) regis     (1000)       95 2023-05-22 04:46:44.000000 jupyter-xblock-15.0.1/jupyterxblock/static/css/student.css
+-rw-rw-r--   0 regis     (1000) regis     (1000)     3830 2023-05-22 04:46:44.000000 jupyter-xblock-15.0.1/jupyterxblock/xblock.py
+-rw-rw-r--   0 regis     (1000) regis     (1000)       38 2023-05-22 05:01:15.148287 jupyter-xblock-15.0.1/setup.cfg
+-rwxrwxr-x   0 regis     (1000) regis     (1000)     1148 2023-05-22 05:00:51.000000 jupyter-xblock-15.0.1/setup.py
```

### Comparing `jupyter-xblock-15.0.0/LICENSE.txt` & `jupyter-xblock-15.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyter-xblock-15.0.0/PKG-INFO` & `jupyter-xblock-15.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-xblock
-Version: 15.0.0
+Version: 15.0.1
 Summary: Jupyter XBlock for Open edX
 Home-page: UNKNOWN
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
@@ -18,37 +18,35 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Jupyter XBlock
 
 This is an [XBlock](https://edx.readthedocs.io/projects/xblock-tutorial/en/latest/overview/introduction.html) to integrate JupyterHub notebooks to your [Open edX](https://openedx.org) learning management system (LMS).
 
-> ⚠️ THIS IS A WORK-IN_PROGRESS! We expect to release a first stable version sometime in March 2023.
-
 Features:
 
 * Integrate [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) notebooks to the Open edX courseware.
 * Fully editable notebooks and student workspaces.
 * Simple integration of notebooks from public git repositories.
 
 Here is a screenshot of the Jupyter XBlock in action:
 
-![](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/screenshots/lms.png)
+![](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/lms.png)
 
 ## Usage
 
 Install this xblock with [Tutor](https://docs.tutor.overhang.io/) (Olive release):
 
     echo "jupyter-xblock>=15.0.0,<16.0.0" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
     tutor images build openedx
     tutor local start -d
 
 In your course "Advanced Settings", add "jupyter" to the "Advanced Module List":
 
-![](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/screenshots/studio-advanced-settings.png)
+![Studio advanced module list](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings.png)
 
 ## Configuration
 
 ### JupyterHub base URL
 
 The JupyterHub cluster can be configured separately for every XBlock, but this can be quite tedious for course instructors. Instead, a default JupyterHub cluster URL can be defined globally by adding the `LTI_DEFAULT_JUPYTER_HUB_URL` setting to both the LMS and CMS settings.
 
@@ -62,15 +60,17 @@
 
 Similarly, the LTI passport ID can be defined globally for all Jupyter XBlock instances. When a passport ID is not explicitely defined in an XBlock, it will default to the `LTI_DEFAULT_JUPYTER_PASSPORT_ID` setting. If this setting is also undefined, then it will default to `LTI_DEFAULT_PASSPORT_ID`. The fallback value is "jupyterhub".
 
 To define a global LTI passport ID to be used by all Jupyter XBlock instances, add to your LMS/CMS settings:
 
     LTI_DEFAULT_JUPYTER_PASSPORT_ID = "myjupyterhub"
 
-Then, the corresponding passport must be created in the course advanced settings, as described in the [Open edX documentation](https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/latest/exercises_tools/lti_component.html#creating-an-lti-passport-string).
+Then, the corresponding passport must be created in the course advanced settings, as described in the [Open edX documentation](https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/latest/exercises_tools/lti_component.html#creating-an-lti-passport-string):
+
+![Studio advanced LTI settings](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings-lti.png)
 
 ## Configuring JupyterHub
 
 You will have to launch your own JupyterHub cluster separately from Open edX. Your cluster should support:
 
 - LTI authentication via [ltiauthenticator](https://github.com/jupyterhub/ltiauthenticator/).
 - LTI authentication must accept the key and secret defined in the course LTI passport (see above).
```

### Comparing `jupyter-xblock-15.0.0/README.md` & `jupyter-xblock-15.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 # Jupyter XBlock
 
 This is an [XBlock](https://edx.readthedocs.io/projects/xblock-tutorial/en/latest/overview/introduction.html) to integrate JupyterHub notebooks to your [Open edX](https://openedx.org) learning management system (LMS).
 
-> ⚠️ THIS IS A WORK-IN_PROGRESS! We expect to release a first stable version sometime in March 2023.
-
 Features:
 
 * Integrate [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) notebooks to the Open edX courseware.
 * Fully editable notebooks and student workspaces.
 * Simple integration of notebooks from public git repositories.
 
 Here is a screenshot of the Jupyter XBlock in action:
 
-![](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/screenshots/lms.png)
+![](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/lms.png)
 
 ## Usage
 
 Install this xblock with [Tutor](https://docs.tutor.overhang.io/) (Olive release):
 
     echo "jupyter-xblock>=15.0.0,<16.0.0" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
     tutor images build openedx
     tutor local start -d
 
 In your course "Advanced Settings", add "jupyter" to the "Advanced Module List":
 
-![](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/screenshots/studio-advanced-settings.png)
+![Studio advanced module list](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings.png)
 
 ## Configuration
 
 ### JupyterHub base URL
 
 The JupyterHub cluster can be configured separately for every XBlock, but this can be quite tedious for course instructors. Instead, a default JupyterHub cluster URL can be defined globally by adding the `LTI_DEFAULT_JUPYTER_HUB_URL` setting to both the LMS and CMS settings.
 
@@ -42,15 +40,17 @@
 
 Similarly, the LTI passport ID can be defined globally for all Jupyter XBlock instances. When a passport ID is not explicitely defined in an XBlock, it will default to the `LTI_DEFAULT_JUPYTER_PASSPORT_ID` setting. If this setting is also undefined, then it will default to `LTI_DEFAULT_PASSPORT_ID`. The fallback value is "jupyterhub".
 
 To define a global LTI passport ID to be used by all Jupyter XBlock instances, add to your LMS/CMS settings:
 
     LTI_DEFAULT_JUPYTER_PASSPORT_ID = "myjupyterhub"
 
-Then, the corresponding passport must be created in the course advanced settings, as described in the [Open edX documentation](https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/latest/exercises_tools/lti_component.html#creating-an-lti-passport-string).
+Then, the corresponding passport must be created in the course advanced settings, as described in the [Open edX documentation](https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/latest/exercises_tools/lti_component.html#creating-an-lti-passport-string):
+
+![Studio advanced LTI settings](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings-lti.png)
 
 ## Configuring JupyterHub
 
 You will have to launch your own JupyterHub cluster separately from Open edX. Your cluster should support:
 
 - LTI authentication via [ltiauthenticator](https://github.com/jupyterhub/ltiauthenticator/).
 - LTI authentication must accept the key and secret defined in the course LTI passport (see above).
```

### Comparing `jupyter-xblock-15.0.0/jupyter_xblock.egg-info/PKG-INFO` & `jupyter-xblock-15.0.1/jupyter_xblock.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter-xblock
-Version: 15.0.0
+Version: 15.0.1
 Summary: Jupyter XBlock for Open edX
 Home-page: UNKNOWN
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: Overhang.IO
 Maintainer-email: regis@overhang.io
 License: AGPLv3
@@ -18,37 +18,35 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Jupyter XBlock
 
 This is an [XBlock](https://edx.readthedocs.io/projects/xblock-tutorial/en/latest/overview/introduction.html) to integrate JupyterHub notebooks to your [Open edX](https://openedx.org) learning management system (LMS).
 
-> ⚠️ THIS IS A WORK-IN_PROGRESS! We expect to release a first stable version sometime in March 2023.
-
 Features:
 
 * Integrate [JupyterLab](https://jupyterlab.readthedocs.io/en/stable/) notebooks to the Open edX courseware.
 * Fully editable notebooks and student workspaces.
 * Simple integration of notebooks from public git repositories.
 
 Here is a screenshot of the Jupyter XBlock in action:
 
-![](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/screenshots/lms.png)
+![](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/lms.png)
 
 ## Usage
 
 Install this xblock with [Tutor](https://docs.tutor.overhang.io/) (Olive release):
 
     echo "jupyter-xblock>=15.0.0,<16.0.0" >> "$(tutor config printroot)/env/build/openedx/requirements/private.txt"
     tutor images build openedx
     tutor local start -d
 
 In your course "Advanced Settings", add "jupyter" to the "Advanced Module List":
 
-![](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/screenshots/studio-advanced-settings.png)
+![Studio advanced module list](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings.png)
 
 ## Configuration
 
 ### JupyterHub base URL
 
 The JupyterHub cluster can be configured separately for every XBlock, but this can be quite tedious for course instructors. Instead, a default JupyterHub cluster URL can be defined globally by adding the `LTI_DEFAULT_JUPYTER_HUB_URL` setting to both the LMS and CMS settings.
 
@@ -62,15 +60,17 @@
 
 Similarly, the LTI passport ID can be defined globally for all Jupyter XBlock instances. When a passport ID is not explicitely defined in an XBlock, it will default to the `LTI_DEFAULT_JUPYTER_PASSPORT_ID` setting. If this setting is also undefined, then it will default to `LTI_DEFAULT_PASSPORT_ID`. The fallback value is "jupyterhub".
 
 To define a global LTI passport ID to be used by all Jupyter XBlock instances, add to your LMS/CMS settings:
 
     LTI_DEFAULT_JUPYTER_PASSPORT_ID = "myjupyterhub"
 
-Then, the corresponding passport must be created in the course advanced settings, as described in the [Open edX documentation](https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/latest/exercises_tools/lti_component.html#creating-an-lti-passport-string).
+Then, the corresponding passport must be created in the course advanced settings, as described in the [Open edX documentation](https://edx.readthedocs.io/projects/open-edx-building-and-running-a-course/en/latest/exercises_tools/lti_component.html#creating-an-lti-passport-string):
+
+![Studio advanced LTI settings](https://raw.githubusercontent.com/overhangio/jupyter-xblock/main/static/screenshots/studio-advanced-settings-lti.png)
 
 ## Configuring JupyterHub
 
 You will have to launch your own JupyterHub cluster separately from Open edX. Your cluster should support:
 
 - LTI authentication via [ltiauthenticator](https://github.com/jupyterhub/ltiauthenticator/).
 - LTI authentication must accept the key and secret defined in the course LTI passport (see above).
```

### Comparing `jupyter-xblock-15.0.0/jupyterxblock/xblock.py` & `jupyter-xblock-15.0.1/jupyterxblock/xblock.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,27 @@
         scope=Scope.settings,
         default=_("Jupyter notebook"),
     )
 
     # Jupyter git repo attributes
     nb_git_repo = String(
         display_name=_("Notebook git repository"),
-        help="For example: https://github.com/binder-examples/requirements.git",
+        help="For example: https://github.com/overhangio/jupyter-xblock.git",
         default="",
         scope=Scope.settings,
     )
     nb_git_branch = String(
         display_name=_("Notebook git branch"),
         default="main",
         scope=Scope.settings,
     )
     nb_git_file = String(
         display_name=_("Notebook file"),
         help="Path relative to the repository root",
-        default="index.ipynb",
+        default="static/notebooks/hello.ipynb",
         scope=Scope.settings,
     )
 
     # LTI attributes
     lti_id = String(
         display_name=_("LTI ID"),
         help=LtiConsumerXBlock.lti_id.help,
```

### Comparing `jupyter-xblock-15.0.0/setup.py` & `jupyter-xblock-15.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with io.open(os.path.join(here, "README.md"), "rt", encoding="utf8") as f:
     readme = f.read()
 
 setup(
     name="jupyter-xblock",
-    version="15.0.0",
+    version="15.0.1",
     description="Jupyter XBlock for Open edX",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Overhang.IO",
     author_email="contact@overhang.io",
     maintainer="Overhang.IO",
     maintainer_email="regis@overhang.io",
```

