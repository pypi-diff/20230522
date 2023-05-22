# Comparing `tmp/idem-core-functions-0.2.2.tar.gz` & `tmp/idem-core-functions-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-core-functions-0.2.2.tar", last modified: Thu Dec  8 21:14:20 2022, max compression
+gzip compressed data, was "idem-core-functions-0.3.0.tar", last modified: Mon May 22 15:13:45 2023, max compression
```

## Comparing `idem-core-functions-0.2.2.tar` & `idem-core-functions-0.3.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 21:14:20.533621 idem-core-functions-0.2.2/
--rw-r--r--   0 root         (0) root         (0)    11345 2022-12-08 21:14:01.000000 idem-core-functions-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6550 2022-12-08 21:14:20.533621 idem-core-functions-0.2.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5736 2022-12-08 21:14:01.000000 idem-core-functions-0.2.2/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 21:14:20.533621 idem-core-functions-0.2.2/idem_core_functions/
--rw-r--r--   0 root         (0) root         (0)     1271 2022-12-08 21:14:01.000000 idem-core-functions-0.2.2/idem_core_functions/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 21:14:20.533621 idem-core-functions-0.2.2/idem_core_functions/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 21:14:20.533621 idem-core-functions-0.2.2/idem_core_functions/exec/core/
--rw-r--r--   0 root         (0) root         (0)     2465 2022-12-08 21:14:01.000000 idem-core-functions-0.2.2/idem_core_functions/exec/core/collection.py
--rw-r--r--   0 root         (0) root         (0)     5567 2022-12-08 21:14:01.000000 idem-core-functions-0.2.2/idem_core_functions/exec/core/conversion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 21:14:20.533621 idem-core-functions-0.2.2/idem_core_functions/exec/core/encoder/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-08 21:14:01.000000 idem-core-functions-0.2.2/idem_core_functions/exec/core/encoder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1751 2022-12-08 21:14:01.000000 idem-core-functions-0.2.2/idem_core_functions/exec/core/encoder/base64.py
--rw-r--r--   0 root         (0) root         (0)      649 2022-12-08 21:14:01.000000 idem-core-functions-0.2.2/idem_core_functions/exec/core/encoding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 21:14:20.533621 idem-core-functions-0.2.2/idem_core_functions/exec/core/encryption/
--rw-r--r--   0 root         (0) root         (0)     6190 2022-12-08 21:14:01.000000 idem-core-functions-0.2.2/idem_core_functions/exec/core/encryption/gpg.py
--rw-r--r--   0 root         (0) root         (0)      989 2022-12-08 21:14:01.000000 idem-core-functions-0.2.2/idem_core_functions/exec/core/string.py
--rw-r--r--   0 root         (0) root         (0)       18 2022-12-08 21:14:20.000000 idem-core-functions-0.2.2/idem_core_functions/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-08 21:14:20.533621 idem-core-functions-0.2.2/idem_core_functions.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6550 2022-12-08 21:14:20.000000 idem-core-functions-0.2.2/idem_core_functions.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      672 2022-12-08 21:14:20.000000 idem-core-functions-0.2.2/idem_core_functions.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-08 21:14:20.000000 idem-core-functions-0.2.2/idem_core_functions.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-12-08 21:14:20.000000 idem-core-functions-0.2.2/idem_core_functions.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       70 2022-12-08 21:14:20.000000 idem-core-functions-0.2.2/idem_core_functions.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-12-08 21:14:20.000000 idem-core-functions-0.2.2/idem_core_functions.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-12-08 21:14:20.533621 idem-core-functions-0.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2749 2022-12-08 21:14:01.000000 idem-core-functions-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)    11345 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6551 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5737 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/idem_core_functions/
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/idem_core_functions/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/idem_core_functions/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/idem_core_functions/exec/core/
+-rw-r--r--   0 root         (0) root         (0)     5094 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/idem_core_functions/exec/core/collection.py
+-rw-r--r--   0 root         (0) root         (0)     7624 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/idem_core_functions/exec/core/conversion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/idem_core_functions/exec/core/encoder/
+-rw-r--r--   0 root         (0) root         (0)     2774 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/idem_core_functions/exec/core/encoder/base64.py
+-rw-r--r--   0 root         (0) root         (0)     1877 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/idem_core_functions/exec/core/encoding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/idem_core_functions/exec/core/encryption/
+-rw-r--r--   0 root         (0) root         (0)     7334 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/idem_core_functions/exec/core/encryption/gpg.py
+-rw-r--r--   0 root         (0) root         (0)     1611 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/idem_core_functions/exec/core/string.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-22 15:13:44.000000 idem-core-functions-0.3.0/idem_core_functions/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/idem_core_functions.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6551 2023-05-22 15:13:45.000000 idem-core-functions-0.3.0/idem_core_functions.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      622 2023-05-22 15:13:45.000000 idem-core-functions-0.3.0/idem_core_functions.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 15:13:45.000000 idem-core-functions-0.3.0/idem_core_functions.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-22 15:13:45.000000 idem-core-functions-0.3.0/idem_core_functions.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-22 15:13:45.000000 idem-core-functions-0.3.0/idem_core_functions.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-22 15:13:45.000000 idem-core-functions-0.3.0/idem_core_functions.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-22 15:13:45.054485 idem-core-functions-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2749 2023-05-22 15:13:31.000000 idem-core-functions-0.3.0/setup.py
```

### Comparing `idem-core-functions-0.2.2/LICENSE` & `idem-core-functions-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-core-functions-0.2.2/PKG-INFO` & `idem-core-functions-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-core-functions
-Version: 0.2.2
+Version: 0.3.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Barnali Rakshit
 Author-email: brakshit@vmware.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Console
@@ -30,57 +30,56 @@
    :alt: Made with pop, a Python implementation of Plugin Oriented Programming
    :target: https://pop.readthedocs.io/
 
 .. image:: https://img.shields.io/badge/made%20with-python-yellow
    :alt: Made with Python
    :target: https://www.python.org/
 
-.. note::
-    Idem plugin with set of common functions that can be executed with exec.run state.
+Idem plugin with built-in functions
 
 About
 =====
 
-Idem plugin with built-in functions
+An Idem plugin containing common functions that you can run with the ``exec.run`` state. You can use argument binding to pass the output of these common functions to other Idem plugin resource states, such as in ``idem-aws``, ``idem-k8s``, or other Idem plugins.
 
 What is POP?
 ------------
 
-This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based
-implementation of *Plugin Oriented Programming (POP)*. POP seeks to bring
-together concepts and wisdom from the history of computing in new ways to solve
-modern computing problems.
+This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based implementation of *Plugin Oriented Programming (POP)*. POP seeks to bring together concepts and wisdom from the history of computing in new ways to solve modern computing problems.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
 * `pop-awesome <https://gitlab.com/saltstack/pop/pop-awesome>`__
 * `pop-create <https://gitlab.com/saltstack/pop/pop-create/>`__
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
 * Python 3.7+
-* git *(if installing from source, or contributing to the project)*
+* git *(if installing from source or contributing to the project)*
+
+  To contribute to the project and set up your local development environment, see ``CONTRIBUTING.rst`` in the source repository for this project.
 
 Installation
 ------------
 
-.. note::
+You can install ``idem-core-functions`` with the Python package installer (PyPI) or from source.
 
-   If wanting to contribute to the project, and setup your local development
-   environment, see the ``CONTRIBUTING.rst`` document in the source repository
-   for this project.
+Install from PyPI
++++++++++++++++++
 
-If wanting to use ``idem-core-functions``, you can do so from source.
+.. code-block:: bash
+
+      pip install idem-core-functions
 
-Install from source
+Install from Source
 +++++++++++++++++++
 
 .. code-block:: bash
 
    # clone repo
    git clone git@<your-project-path>/idem-core-functions.git
    cd idem-core-functions
@@ -88,50 +87,70 @@
    # Setup venv
    python3 -m venv .venv
    source .venv/bin/activate
    pip install -e .
 
 Usage
 =====
-This Idem plugin functions can be executed with exec.run state that can then be used with other idem plugin like idem-aws, idem-k8s etc as arg-binding.
 
 Setup
------------------
-After installation, the idem-core-functions execution modules will be accessible to the pop `hub`.
+-----
+
+After installation, ``idem-core-functions`` execution modules are accessible to the pop *hub*.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
 * `pop hub <https://pop-book.readthedocs.io/en/latest/main/hub.html#>`__
 
-You are ready to use idem-core-functions!!!
+You are now ready to use idem-core-functions.
 
 Exec Module
 -----------
-Exec modules can be run from SLS using the "exec.run" state. The return from the exec module is put in the state's "new_state", so it can be used in arg_binding. The desired state of a resource can be specified in sls file.
-The "core.encoding.base64encode" to apply Base64 encoding to a string.
-The "core.encoding.base64decode" takes a string containing a Base64 character sequence and returns the original string.
-The "core.conversion.to_json" to serialize an object to a string of JSON
-The "core.collection.distinct" to return a new list with any duplicate elements removed for a given list.
-The "core.collection.flatten" to eplaces any elements that are lists with a flattened sequence of the list for a given list.
-The "core.collection.element" to retrieve a single element from a list.
-The "core.collection.length" to  determine the length of a given list, map, or string.
 
-Request Syntax:
+An SLS file specifies the desired state of a resource. You can run an exec module within an SLS file using the ``exec.run`` state, where the exec module returns a new state that can be referenced with argument binding.
 
-..  code:: sls
+* ``core.encoding.base64encode``
+
+  Apply Base64 encoding to a string.
+
+* ``core.encoding.base64decode``
+
+  Restore a Base64 encoded character string to the original string.
+
+* ``core.conversion.to_json``
+
+  Serialize an object to a string of JSON.
 
+* ``core.collection.distinct``
+
+  For a given list, return a new list with any duplicate elements removed.
+
+* ``core.collection.flatten``
+
+  For a given list, replace any elements that are lists with a flattened sequence of that list.
+
+* ``core.collection.element``
+
+  Retrieve a single element from a list.
+
+* ``core.collection.length``
+
+  Determine the length of a given list, map, or string.
+
+Syntax:
+
+..  code:: sls
 
     [Idem-state-name]:
       exec.run:
         - path: core.encoder.base64.encode
         - kwargs:
             data: test-user-name:test-password
 
-
     [Idem-state-name]:
       exec.run:
         - path: core.encoder.base64.decode
         - kwargs:
             encoded_data: dGVzdC11c2VyLW5hbWU6dGVzdC1wYXNzd29yZA==
 
     [Idem-state-name]:
@@ -145,15 +164,15 @@
 
     [Idem-state-name]:
       exec.run:
         - path: core.encryption.gpg.encrypt
         - kwargs:
             data: test-data-for-encryption
 
-Examples Usage:
+Examples:
 
 ..  code:: sls
 
         vault_generic_secret.example-creds.search:
           vault.secrets.kv_v1.secret.search:
             - path: "example/projects.registry.example.com"
 
@@ -181,25 +200,26 @@
 
         idem.core.encryption.gpg.encrypt.test-1:
           exec.run:
             - path: core.encryption.gpg.encrypt
             - kwargs:
                 data: test-data-for-encryption
 
-It can be specified from command line when calling exec module as below
+Idem command line examples:
 
 .. code:: bash
 
      idem exec exec.core.encoding.base64encode data=sample-data
      idem exec exec.core.encoding.base64decode encoded_data=dGVzdC11c2VyLW5hbWU6dGVzdC1wYXNzd29yZA==
 
-Current Supported exec functions
-++++++++++++++++++++++++++++++++++
+Current Supported Exec Functions
+--------------------------------
 
 core
-"""""""""""""
+++++
+
 * conversion
 * collection
 * encoder
 * encryption
```

### Comparing `idem-core-functions-0.2.2/README.rst` & `idem-core-functions-0.3.0/idem_core_functions.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,85 @@
+Metadata-Version: 2.1
+Name: idem-core-functions
+Version: 0.3.0
+Summary: UNKNOWN
+Home-page: UNKNOWN
+Author: Barnali Rakshit
+Author-email: brakshit@vmware.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Information Technology
+Classifier: Intended Audience :: System Administrators
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 ===================
 idem-core-functions
 ===================
 
 .. image:: https://img.shields.io/badge/made%20with-pop-teal
    :alt: Made with pop, a Python implementation of Plugin Oriented Programming
    :target: https://pop.readthedocs.io/
 
 .. image:: https://img.shields.io/badge/made%20with-python-yellow
    :alt: Made with Python
    :target: https://www.python.org/
 
-.. note::
-    Idem plugin with set of common functions that can be executed with exec.run state.
+Idem plugin with built-in functions
 
 About
 =====
 
-Idem plugin with built-in functions
+An Idem plugin containing common functions that you can run with the ``exec.run`` state. You can use argument binding to pass the output of these common functions to other Idem plugin resource states, such as in ``idem-aws``, ``idem-k8s``, or other Idem plugins.
 
 What is POP?
 ------------
 
-This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based
-implementation of *Plugin Oriented Programming (POP)*. POP seeks to bring
-together concepts and wisdom from the history of computing in new ways to solve
-modern computing problems.
+This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based implementation of *Plugin Oriented Programming (POP)*. POP seeks to bring together concepts and wisdom from the history of computing in new ways to solve modern computing problems.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
 * `pop-awesome <https://gitlab.com/saltstack/pop/pop-awesome>`__
 * `pop-create <https://gitlab.com/saltstack/pop/pop-create/>`__
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
 * Python 3.7+
-* git *(if installing from source, or contributing to the project)*
+* git *(if installing from source or contributing to the project)*
+
+  To contribute to the project and set up your local development environment, see ``CONTRIBUTING.rst`` in the source repository for this project.
 
 Installation
 ------------
 
-.. note::
+You can install ``idem-core-functions`` with the Python package installer (PyPI) or from source.
 
-   If wanting to contribute to the project, and setup your local development
-   environment, see the ``CONTRIBUTING.rst`` document in the source repository
-   for this project.
+Install from PyPI
++++++++++++++++++
 
-If wanting to use ``idem-core-functions``, you can do so from source.
+.. code-block:: bash
+
+      pip install idem-core-functions
 
-Install from source
+Install from Source
 +++++++++++++++++++
 
 .. code-block:: bash
 
    # clone repo
    git clone git@<your-project-path>/idem-core-functions.git
    cd idem-core-functions
@@ -64,50 +87,70 @@
    # Setup venv
    python3 -m venv .venv
    source .venv/bin/activate
    pip install -e .
 
 Usage
 =====
-This Idem plugin functions can be executed with exec.run state that can then be used with other idem plugin like idem-aws, idem-k8s etc as arg-binding.
 
 Setup
------------------
-After installation, the idem-core-functions execution modules will be accessible to the pop `hub`.
+-----
+
+After installation, ``idem-core-functions`` execution modules are accessible to the pop *hub*.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
 * `pop hub <https://pop-book.readthedocs.io/en/latest/main/hub.html#>`__
 
-You are ready to use idem-core-functions!!!
+You are now ready to use idem-core-functions.
 
 Exec Module
 -----------
-Exec modules can be run from SLS using the "exec.run" state. The return from the exec module is put in the state's "new_state", so it can be used in arg_binding. The desired state of a resource can be specified in sls file.
-The "core.encoding.base64encode" to apply Base64 encoding to a string.
-The "core.encoding.base64decode" takes a string containing a Base64 character sequence and returns the original string.
-The "core.conversion.to_json" to serialize an object to a string of JSON
-The "core.collection.distinct" to return a new list with any duplicate elements removed for a given list.
-The "core.collection.flatten" to eplaces any elements that are lists with a flattened sequence of the list for a given list.
-The "core.collection.element" to retrieve a single element from a list.
-The "core.collection.length" to  determine the length of a given list, map, or string.
 
-Request Syntax:
+An SLS file specifies the desired state of a resource. You can run an exec module within an SLS file using the ``exec.run`` state, where the exec module returns a new state that can be referenced with argument binding.
 
-..  code:: sls
+* ``core.encoding.base64encode``
+
+  Apply Base64 encoding to a string.
+
+* ``core.encoding.base64decode``
+
+  Restore a Base64 encoded character string to the original string.
+
+* ``core.conversion.to_json``
+
+  Serialize an object to a string of JSON.
+
+* ``core.collection.distinct``
 
+  For a given list, return a new list with any duplicate elements removed.
+
+* ``core.collection.flatten``
+
+  For a given list, replace any elements that are lists with a flattened sequence of that list.
+
+* ``core.collection.element``
+
+  Retrieve a single element from a list.
+
+* ``core.collection.length``
+
+  Determine the length of a given list, map, or string.
+
+Syntax:
+
+..  code:: sls
 
     [Idem-state-name]:
       exec.run:
         - path: core.encoder.base64.encode
         - kwargs:
             data: test-user-name:test-password
 
-
     [Idem-state-name]:
       exec.run:
         - path: core.encoder.base64.decode
         - kwargs:
             encoded_data: dGVzdC11c2VyLW5hbWU6dGVzdC1wYXNzd29yZA==
 
     [Idem-state-name]:
@@ -121,15 +164,15 @@
 
     [Idem-state-name]:
       exec.run:
         - path: core.encryption.gpg.encrypt
         - kwargs:
             data: test-data-for-encryption
 
-Examples Usage:
+Examples:
 
 ..  code:: sls
 
         vault_generic_secret.example-creds.search:
           vault.secrets.kv_v1.secret.search:
             - path: "example/projects.registry.example.com"
 
@@ -157,23 +200,26 @@
 
         idem.core.encryption.gpg.encrypt.test-1:
           exec.run:
             - path: core.encryption.gpg.encrypt
             - kwargs:
                 data: test-data-for-encryption
 
-It can be specified from command line when calling exec module as below
+Idem command line examples:
 
 .. code:: bash
 
      idem exec exec.core.encoding.base64encode data=sample-data
      idem exec exec.core.encoding.base64decode encoded_data=dGVzdC11c2VyLW5hbWU6dGVzdC1wYXNzd29yZA==
 
-Current Supported exec functions
-++++++++++++++++++++++++++++++++++
+Current Supported Exec Functions
+--------------------------------
 
 core
-"""""""""""""
+++++
+
 * conversion
 * collection
 * encoder
 * encryption
+
+
```

### Comparing `idem-core-functions-0.2.2/idem_core_functions/conf.py` & `idem-core-functions-0.3.0/idem_core_functions/conf.py`

 * *Files identical despite different names*

### Comparing `idem-core-functions-0.2.2/idem_core_functions/exec/core/encryption/gpg.py` & `idem-core-functions-0.3.0/idem_core_functions/exec/core/encryption/gpg.py`

 * *Files 13% similar despite different names*

```diff
@@ -45,14 +45,37 @@
             If True is specified, then the default cipher algorithm (CAST5) is used.
             The cipher-algorithm to use (for example, 'AES256') can also be specified.
         extra_args(list[str], Optional):
             A list of additional arguments to pass to the gpg executable.
             For example, Pass extra_args=['-z', '0'] to disable compression
         public_key(str, Optional):
             Public key of the recipient. This public key will be imported and trusted, if not already.
+
+    Returns:
+        .. code-block:: python
+
+            {"result": True|False, "comment": list, "ret": None|dict}
+
+    Examples:
+        Calling this exec module function from the cli
+
+        .. code-block:: bash
+
+            idem exec core.encryption.gpg.encrypt data=test-data-for-encryption
+
+        Using in a state:
+
+        .. code-block:: yaml
+
+            Idem-state-name:
+              exec.run:
+                - path: core.encryption.gpg.encrypt
+                - kwargs:
+                    data: test-data-for-encryption
+
     """
     result = dict(comment=[], ret=None, result=True)
     if not data:
         result["result"] = False
         result["comment"].append("data for gpg_encrypt is empty")
         return result
 
@@ -115,14 +138,37 @@
             A passphrase to use when accessing the keyrings.
         output(str, Optional):
             The name of an output file to write to.
         extra_args(list[str], Optional):
             A list of additional arguments to pass to the gpg executable.
         private_key(str, Optional):
             The private key of the recipient for decryption. This private key will be imported and trusted, if not already.
+
+    Returns:
+        .. code-block:: python
+
+            {"result": True|False, "comment": list, "ret": None|dict}
+
+    Examples:
+        Calling this exec module function from the cli
+
+        .. code-block:: bash
+
+            idem exec core.encryption.gpg.decrypt message="This is for decryption test" passphrase="test"
+
+        Using in a state:
+
+        .. code-block:: yaml
+
+            Idem-state-name:
+              exec.run:
+                - path: core.encryption.gpg.decrypt
+                - kwargs:
+                    message: This is for decryption test
+                    passphrase: test
     """
     result = dict(comment=[], ret=None, result=True)
     if not message:
         result["result"] = False
         result["comment"].append("message for gpg_decrypt is empty")
         return result
```

### Comparing `idem-core-functions-0.2.2/idem_core_functions.egg-info/PKG-INFO` & `idem-core-functions-0.3.0/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,61 @@
-Metadata-Version: 2.1
-Name: idem-core-functions
-Version: 0.2.2
-Summary: UNKNOWN
-Home-page: UNKNOWN
-Author: Barnali Rakshit
-Author-email: brakshit@vmware.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 ===================
 idem-core-functions
 ===================
 
 .. image:: https://img.shields.io/badge/made%20with-pop-teal
    :alt: Made with pop, a Python implementation of Plugin Oriented Programming
    :target: https://pop.readthedocs.io/
 
 .. image:: https://img.shields.io/badge/made%20with-python-yellow
    :alt: Made with Python
    :target: https://www.python.org/
 
-.. note::
-    Idem plugin with set of common functions that can be executed with exec.run state.
+Idem plugin with built-in functions
 
 About
 =====
 
-Idem plugin with built-in functions
+An Idem plugin containing common functions that you can run with the ``exec.run`` state. You can use argument binding to pass the output of these common functions to other Idem plugin resource states, such as in ``idem-aws``, ``idem-k8s``, or other Idem plugins.
 
 What is POP?
 ------------
 
-This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based
-implementation of *Plugin Oriented Programming (POP)*. POP seeks to bring
-together concepts and wisdom from the history of computing in new ways to solve
-modern computing problems.
+This project is built with `pop <https://pop.readthedocs.io/>`__, a Python-based implementation of *Plugin Oriented Programming (POP)*. POP seeks to bring together concepts and wisdom from the history of computing in new ways to solve modern computing problems.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
 * `pop-awesome <https://gitlab.com/saltstack/pop/pop-awesome>`__
 * `pop-create <https://gitlab.com/saltstack/pop/pop-create/>`__
 
 Getting Started
 ===============
 
 Prerequisites
 -------------
 
 * Python 3.7+
-* git *(if installing from source, or contributing to the project)*
+* git *(if installing from source or contributing to the project)*
+
+  To contribute to the project and set up your local development environment, see ``CONTRIBUTING.rst`` in the source repository for this project.
 
 Installation
 ------------
 
-.. note::
+You can install ``idem-core-functions`` with the Python package installer (PyPI) or from source.
 
-   If wanting to contribute to the project, and setup your local development
-   environment, see the ``CONTRIBUTING.rst`` document in the source repository
-   for this project.
+Install from PyPI
++++++++++++++++++
 
-If wanting to use ``idem-core-functions``, you can do so from source.
+.. code-block:: bash
+
+      pip install idem-core-functions
 
-Install from source
+Install from Source
 +++++++++++++++++++
 
 .. code-block:: bash
 
    # clone repo
    git clone git@<your-project-path>/idem-core-functions.git
    cd idem-core-functions
@@ -88,50 +63,70 @@
    # Setup venv
    python3 -m venv .venv
    source .venv/bin/activate
    pip install -e .
 
 Usage
 =====
-This Idem plugin functions can be executed with exec.run state that can then be used with other idem plugin like idem-aws, idem-k8s etc as arg-binding.
 
 Setup
------------------
-After installation, the idem-core-functions execution modules will be accessible to the pop `hub`.
+-----
+
+After installation, ``idem-core-functions`` execution modules are accessible to the pop *hub*.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
 * `pop hub <https://pop-book.readthedocs.io/en/latest/main/hub.html#>`__
 
-You are ready to use idem-core-functions!!!
+You are now ready to use idem-core-functions.
 
 Exec Module
 -----------
-Exec modules can be run from SLS using the "exec.run" state. The return from the exec module is put in the state's "new_state", so it can be used in arg_binding. The desired state of a resource can be specified in sls file.
-The "core.encoding.base64encode" to apply Base64 encoding to a string.
-The "core.encoding.base64decode" takes a string containing a Base64 character sequence and returns the original string.
-The "core.conversion.to_json" to serialize an object to a string of JSON
-The "core.collection.distinct" to return a new list with any duplicate elements removed for a given list.
-The "core.collection.flatten" to eplaces any elements that are lists with a flattened sequence of the list for a given list.
-The "core.collection.element" to retrieve a single element from a list.
-The "core.collection.length" to  determine the length of a given list, map, or string.
 
-Request Syntax:
+An SLS file specifies the desired state of a resource. You can run an exec module within an SLS file using the ``exec.run`` state, where the exec module returns a new state that can be referenced with argument binding.
 
-..  code:: sls
+* ``core.encoding.base64encode``
+
+  Apply Base64 encoding to a string.
+
+* ``core.encoding.base64decode``
+
+  Restore a Base64 encoded character string to the original string.
+
+* ``core.conversion.to_json``
+
+  Serialize an object to a string of JSON.
+
+* ``core.collection.distinct``
 
+  For a given list, return a new list with any duplicate elements removed.
+
+* ``core.collection.flatten``
+
+  For a given list, replace any elements that are lists with a flattened sequence of that list.
+
+* ``core.collection.element``
+
+  Retrieve a single element from a list.
+
+* ``core.collection.length``
+
+  Determine the length of a given list, map, or string.
+
+Syntax:
+
+..  code:: sls
 
     [Idem-state-name]:
       exec.run:
         - path: core.encoder.base64.encode
         - kwargs:
             data: test-user-name:test-password
 
-
     [Idem-state-name]:
       exec.run:
         - path: core.encoder.base64.decode
         - kwargs:
             encoded_data: dGVzdC11c2VyLW5hbWU6dGVzdC1wYXNzd29yZA==
 
     [Idem-state-name]:
@@ -145,15 +140,15 @@
 
     [Idem-state-name]:
       exec.run:
         - path: core.encryption.gpg.encrypt
         - kwargs:
             data: test-data-for-encryption
 
-Examples Usage:
+Examples:
 
 ..  code:: sls
 
         vault_generic_secret.example-creds.search:
           vault.secrets.kv_v1.secret.search:
             - path: "example/projects.registry.example.com"
 
@@ -181,25 +176,24 @@
 
         idem.core.encryption.gpg.encrypt.test-1:
           exec.run:
             - path: core.encryption.gpg.encrypt
             - kwargs:
                 data: test-data-for-encryption
 
-It can be specified from command line when calling exec module as below
+Idem command line examples:
 
 .. code:: bash
 
      idem exec exec.core.encoding.base64encode data=sample-data
      idem exec exec.core.encoding.base64decode encoded_data=dGVzdC11c2VyLW5hbWU6dGVzdC1wYXNzd29yZA==
 
-Current Supported exec functions
-++++++++++++++++++++++++++++++++++
+Current Supported Exec Functions
+--------------------------------
 
 core
-"""""""""""""
+++++
+
 * conversion
 * collection
 * encoder
 * encryption
-
-
```

### Comparing `idem-core-functions-0.2.2/idem_core_functions.egg-info/SOURCES.txt` & `idem-core-functions-0.3.0/idem_core_functions.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -10,10 +10,9 @@
 idem_core_functions.egg-info/entry_points.txt
 idem_core_functions.egg-info/requires.txt
 idem_core_functions.egg-info/top_level.txt
 idem_core_functions/exec/core/collection.py
 idem_core_functions/exec/core/conversion.py
 idem_core_functions/exec/core/encoding.py
 idem_core_functions/exec/core/string.py
-idem_core_functions/exec/core/encoder/__init__.py
 idem_core_functions/exec/core/encoder/base64.py
 idem_core_functions/exec/core/encryption/gpg.py
```

### Comparing `idem-core-functions-0.2.2/setup.py` & `idem-core-functions-0.3.0/setup.py`

 * *Files identical despite different names*

