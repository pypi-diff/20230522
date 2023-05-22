# Comparing `tmp/idem-spotinst-0.1.0.tar.gz` & `tmp/idem-spotinst-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idem-spotinst-0.1.0.tar", last modified: Mon Oct 24 19:44:39 2022, max compression
+gzip compressed data, was "idem-spotinst-0.2.0.tar", last modified: Mon May 22 15:18:30 2023, max compression
```

## Comparing `idem-spotinst-0.1.0.tar` & `idem-spotinst-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/
--rw-r--r--   0 root         (0) root         (0)    11336 2022-10-24 19:44:27.000000 idem-spotinst-0.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6478 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5681 2022-10-24 19:44:27.000000 idem-spotinst-0.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/idem_spotinst/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/idem_spotinst/acct/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/idem_spotinst/acct/spotinst/
--rw-r--r--   0 root         (0) root         (0)      536 2022-10-24 19:44:27.000000 idem-spotinst-0.1.0/idem_spotinst/acct/spotinst/init.py
--rw-r--r--   0 root         (0) root         (0)     1351 2022-10-24 19:44:27.000000 idem-spotinst-0.1.0/idem_spotinst/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/idem_spotinst/exec/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/idem_spotinst/exec/spotinst/
--rw-r--r--   0 root         (0) root         (0)      231 2022-10-24 19:44:27.000000 idem-spotinst-0.1.0/idem_spotinst/exec/spotinst/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/idem_spotinst/states/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/idem_spotinst/states/spotinst/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/idem_spotinst/states/spotinst/ocean/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/idem_spotinst/states/spotinst/ocean/aws/
--rw-r--r--   0 root         (0) root         (0)    20532 2022-10-24 19:44:27.000000 idem-spotinst-0.1.0/idem_spotinst/states/spotinst/ocean/aws/k8s_cluster.py
--rw-r--r--   0 root         (0) root         (0)    22969 2022-10-24 19:44:27.000000 idem-spotinst-0.1.0/idem_spotinst/states/spotinst/ocean/aws/launch_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/idem_spotinst/tool/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/
--rw-r--r--   0 root         (0) root         (0)     1080 2022-10-24 19:44:27.000000 idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/comment_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/ocean/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/ocean/aws/
--rw-r--r--   0 root         (0) root         (0)     2862 2022-10-24 19:44:27.000000 idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/ocean/aws/conversion_utils.py
--rw-r--r--   0 root         (0) root         (0)     2830 2022-10-24 19:44:27.000000 idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/ocean/aws/k8s_cluster_utils.py
--rw-r--r--   0 root         (0) root         (0)      906 2022-10-24 19:44:27.000000 idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/ocean/aws/tag_utils.py
--rw-r--r--   0 root         (0) root         (0)     3145 2022-10-24 19:44:27.000000 idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/state_comparison_utils.py
--rw-r--r--   0 root         (0) root         (0)      856 2022-10-24 19:44:27.000000 idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/state_utils.py
--rw-r--r--   0 root         (0) root         (0)       18 2022-10-24 19:44:39.000000 idem-spotinst-0.1.0/idem_spotinst/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/idem_spotinst.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6478 2022-10-24 19:44:39.000000 idem-spotinst-0.1.0/idem_spotinst.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      800 2022-10-24 19:44:39.000000 idem-spotinst-0.1.0/idem_spotinst.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-10-24 19:44:39.000000 idem-spotinst-0.1.0/idem_spotinst.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-10-24 19:44:39.000000 idem-spotinst-0.1.0/idem_spotinst.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       61 2022-10-24 19:44:39.000000 idem-spotinst-0.1.0/idem_spotinst.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2022-10-24 19:44:39.000000 idem-spotinst-0.1.0/idem_spotinst.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-10-24 19:44:39.710445 idem-spotinst-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2720 2022-10-24 19:44:27.000000 idem-spotinst-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)    11336 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6174 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5377 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/acct/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/acct/spotinst/
+-rw-r--r--   0 root         (0) root         (0)      536 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/acct/spotinst/init.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/exec/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/exec/spotinst/
+-rw-r--r--   0 root         (0) root         (0)      231 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/exec/spotinst/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/states/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/states/spotinst/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/states/spotinst/ocean/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/states/spotinst/ocean/aws/
+-rw-r--r--   0 root         (0) root         (0)    20832 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/states/spotinst/ocean/aws/k8s_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    23325 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/states/spotinst/ocean/aws/launch_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/tool/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/comment_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/aws/
+-rw-r--r--   0 root         (0) root         (0)     2862 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/aws/conversion_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/aws/k8s_cluster_utils.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/aws/tag_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3145 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/state_comparison_utils.py
+-rw-r--r--   0 root         (0) root         (0)      856 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/state_utils.py
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-22 15:18:30.000000 idem-spotinst-0.2.0/idem_spotinst/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/idem_spotinst.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6174 2023-05-22 15:18:30.000000 idem-spotinst-0.2.0/idem_spotinst.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      800 2023-05-22 15:18:30.000000 idem-spotinst-0.2.0/idem_spotinst.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 15:18:30.000000 idem-spotinst-0.2.0/idem_spotinst.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-05-22 15:18:30.000000 idem-spotinst-0.2.0/idem_spotinst.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-05-22 15:18:30.000000 idem-spotinst-0.2.0/idem_spotinst.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-22 15:18:30.000000 idem-spotinst-0.2.0/idem_spotinst.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-22 15:18:30.921814 idem-spotinst-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-05-22 15:18:17.000000 idem-spotinst-0.2.0/setup.py
```

### Comparing `idem-spotinst-0.1.0/LICENSE` & `idem-spotinst-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.1.0/PKG-INFO` & `idem-spotinst-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-spotinst
-Version: 0.1.0
+Version: 0.2.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Prerna
 Author-email: prjain@vmware.com
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
-    Idem plugin to manage Spotinst resources
+The Idem spot instance provider
 
 About
 =====
 
-Spotinst Provider Idem plugin
+An Idem plugin to manage spot instance resources. A spot instance is an instance deployed at a discount on spare EC2 capacity.
 
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
+You can install ``idem-spotinst`` with the Python package installer (PyPI) or from source.
+
+Install from PyPI
++++++++++++++++++
 
-   If wanting to contribute to the project, and setup your local development
-   environment, see the ``CONTRIBUTING.rst`` document in the source repository
-   for this project.
+.. code-block:: bash
 
-If wanting to use ``idem-spotinst``, you can do so from source.
+      pip install idem-spotinst
 
-Install from source
+Install from Source
 +++++++++++++++++++
 
 .. code-block:: bash
 
    # clone repo
    git clone git@<your-project-path>/idem-spotinst.git
    cd idem-spotinst
@@ -89,89 +88,67 @@
    python3 -m venv .venv
    source .venv/bin/activate
    pip install -e .
 
 Usage
 =====
 
-Credentials Setup
------------------
+Setup
+-----
 
-After installation, the spotinst Idem execution and state modules will be accessible to the pop `hub`.
-In order to use them, we need to set up our credentials.
+After installation, ``idem-spotinst`` execution and state modules are accessible to the pop *hub*.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
 * `pop hub <https://pop-book.readthedocs.io/en/latest/main/hub.html#>`__
 
-Create a new file called `credentials.yaml` and populate it with credentials.
-The `default` profile will be picked up automatically by `idem`.
-
-There are multiple authentication backends for `idem-spotinst` which each have their own unique set of parameters.
-The following examples show the parameters that can be used to define credential profiles.
+To use ``idem-spotinst`` execution and state modules to manage spot instance resources, set up a credentials.yaml file for authentication. There are multiple authentication backends for ``idem-spotinst``, where each has its own unique set of parameters. For example:
 
 credentials.yaml:
 
 ..  code:: sls
 
     spotinst:
       default:
         account_id: act-11c833de
         token: b5460afe3c29a30c28abd54d190d1aa923587574321e75925cfc8268b54b4562
 
-Next step is to encrypt the credentials file, and add the encryption key and encrypted file
-path to the ENVIRONMENT.
+For more about Idem credentials files, including recommended steps for encryption and environment variables, see `Authenticating with Idem <https://docs.idemproject.io/getting-started/en/latest/topics/gettingstarted/authenticating.html>`__
 
-Encrypt the credential file:
+You are now ready to use idem-spotinst.
 
-.. code:: bash
+States
+------
 
-    Idem encrypt credentials.yaml
+Idem SLS files use states to ensure that resources are in a desired configuration. An idem-spotinst SLS file supports three state functions: *present*, *absent*, and *describe*.
 
-This will generate a credentials.yaml.fernet file and a command line output token::
+present
++++++++
 
-    -AXFSEFSSEjsfdG_lb333kVhCVSCDyOFH4eABCDEFNwI=
+The *present* function ensures that a resource exists. If a resource doesn't exist, running *present* creates it. If the resource already exists, running *present* might leave it unchanged, or update it if there are any configuration changes.
 
-Add these to your environment:
+You can only update values that the spotinst REST API supports.
 
-.. code:: bash
+absent
+++++++
+
+The *absent* function ensures that a resource does not exist. If the resource exists, running *absent* deletes it. If the resource doesn't exist, running *absent* has no effect.
 
-    export ACCT_KEY="-AXFSEFSSEjsfdG_lb333kVhCVSCDyOFH4eABCDEFNwI="
-    export ACCT_FILE=$PWD/credentials.yaml.fernet
+describe
+++++++++
 
+The *describe* function returns a list of all resources of the specified type under the spotinst account ID from your credentials.yaml profile.
 
-You are ready to use idem-spotinst!!!
+Accessing States
+----------------
 
-STATES
---------
-Idem states are used to make sure resources are in a desired state.
-The desired state of a resource can be specified in sls file.
-In Idem-spotinst, three states are supported: `present`, `absent`, `describe`
-
-present state
-+++++++++++++
-`present` state makes sure a resource exists in a desired state. If a resource does
-not exist, running `present` will create the resource on the provider. If a resource
-exists, running `present` will update the resource on the provider. (Only the values
-that the spotinst REST api supports can be updated.)
-
-absent state
-++++++++++++
-`absent` state makes sure a resource does not exist. If a resource exits, running
-`absent` will delete the resource. If a resource does not exist, running `absent`
-is a no-operation.
-
-describe state
-++++++++++++++
-`describe` state lists all the current resources of the same resource type
-under the spotinst account id specified in the credential profile.
+States can be accessed by their relative location in ``idem-spotinst/idem_spotinst/states``.
 
-States can be accessed by their relative location in `idem-spotinst/idem_spotinst/states`.
-For example, in the state sls yaml file below, spotinst launch specification state can be created with the `present` function.
+For example, a spotinst launch specification state can be created with the *present* function as shown in the following SLS file.
 
 my_resource_launch_spec_state.sls:
 
 .. code:: sls
 
     my_resource_launch_spec:
         spotinst.ocean.aws.launch_spec.present:
@@ -195,28 +172,30 @@
               value: value1
             - key: tag2
               value: value2
           - instance_types:
             - t2.micro
           - image_id: ami-0c02fb55956c7d318
 
-The state sls file can be executed with:
+The Idem command to create the preceding state is:
 
 .. code:: bash
 
     idem state $PWD/my_resource_launch_spec_state.sls
 
-The resource parameters in an sls yaml file follow the exact structure as
-what's in the `Spotinst REST api doc <https://docs.spot.io/api/>`__ . URI Parameters
-should be specified in snake case with "- " in front. All parameters of the api request body
-should be specified in exactly the same way as what's in the spotinst REST api.
+Your SLS should follow the resource parameter structure shown in the `Spotinst REST API <https://docs.spot.io/api/>`__.
+
+* Specify URI parameters in snake case with a leading dash and space "- ".
 
-Current Supported Resources states
-++++++++++++++++++++++++++++++++++
+* Specify all parameters of the API request body exactly as shown in the the `Spotinst REST API <https://docs.spot.io/api/>`__.
+
+Current Supported Resource States
+---------------------------------
 
 ocean_aws
-"""""""""""""
-k8s_cluser
++++++++++
+
+k8s_cluster
 
 launch_spec
```

### Comparing `idem-spotinst-0.1.0/README.rst` & `idem-spotinst-0.2.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -6,57 +6,56 @@
    :alt: Made with pop, a Python implementation of Plugin Oriented Programming
    :target: https://pop.readthedocs.io/
 
 .. image:: https://img.shields.io/badge/made%20with-python-yellow
    :alt: Made with Python
    :target: https://www.python.org/
 
-.. note::
-    Idem plugin to manage Spotinst resources
+The Idem spot instance provider
 
 About
 =====
 
-Spotinst Provider Idem plugin
+An Idem plugin to manage spot instance resources. A spot instance is an instance deployed at a discount on spare EC2 capacity.
 
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
+You can install ``idem-spotinst`` with the Python package installer (PyPI) or from source.
+
+Install from PyPI
++++++++++++++++++
 
-   If wanting to contribute to the project, and setup your local development
-   environment, see the ``CONTRIBUTING.rst`` document in the source repository
-   for this project.
+.. code-block:: bash
 
-If wanting to use ``idem-spotinst``, you can do so from source.
+      pip install idem-spotinst
 
-Install from source
+Install from Source
 +++++++++++++++++++
 
 .. code-block:: bash
 
    # clone repo
    git clone git@<your-project-path>/idem-spotinst.git
    cd idem-spotinst
@@ -65,89 +64,67 @@
    python3 -m venv .venv
    source .venv/bin/activate
    pip install -e .
 
 Usage
 =====
 
-Credentials Setup
------------------
+Setup
+-----
 
-After installation, the spotinst Idem execution and state modules will be accessible to the pop `hub`.
-In order to use them, we need to set up our credentials.
+After installation, ``idem-spotinst`` execution and state modules are accessible to the pop *hub*.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
 * `pop hub <https://pop-book.readthedocs.io/en/latest/main/hub.html#>`__
 
-Create a new file called `credentials.yaml` and populate it with credentials.
-The `default` profile will be picked up automatically by `idem`.
-
-There are multiple authentication backends for `idem-spotinst` which each have their own unique set of parameters.
-The following examples show the parameters that can be used to define credential profiles.
+To use ``idem-spotinst`` execution and state modules to manage spot instance resources, set up a credentials.yaml file for authentication. There are multiple authentication backends for ``idem-spotinst``, where each has its own unique set of parameters. For example:
 
 credentials.yaml:
 
 ..  code:: sls
 
     spotinst:
       default:
         account_id: act-11c833de
         token: b5460afe3c29a30c28abd54d190d1aa923587574321e75925cfc8268b54b4562
 
-Next step is to encrypt the credentials file, and add the encryption key and encrypted file
-path to the ENVIRONMENT.
+For more about Idem credentials files, including recommended steps for encryption and environment variables, see `Authenticating with Idem <https://docs.idemproject.io/getting-started/en/latest/topics/gettingstarted/authenticating.html>`__
 
-Encrypt the credential file:
+You are now ready to use idem-spotinst.
 
-.. code:: bash
+States
+------
 
-    Idem encrypt credentials.yaml
+Idem SLS files use states to ensure that resources are in a desired configuration. An idem-spotinst SLS file supports three state functions: *present*, *absent*, and *describe*.
 
-This will generate a credentials.yaml.fernet file and a command line output token::
+present
++++++++
 
-    -AXFSEFSSEjsfdG_lb333kVhCVSCDyOFH4eABCDEFNwI=
+The *present* function ensures that a resource exists. If a resource doesn't exist, running *present* creates it. If the resource already exists, running *present* might leave it unchanged, or update it if there are any configuration changes.
 
-Add these to your environment:
+You can only update values that the spotinst REST API supports.
 
-.. code:: bash
+absent
+++++++
+
+The *absent* function ensures that a resource does not exist. If the resource exists, running *absent* deletes it. If the resource doesn't exist, running *absent* has no effect.
 
-    export ACCT_KEY="-AXFSEFSSEjsfdG_lb333kVhCVSCDyOFH4eABCDEFNwI="
-    export ACCT_FILE=$PWD/credentials.yaml.fernet
+describe
+++++++++
 
+The *describe* function returns a list of all resources of the specified type under the spotinst account ID from your credentials.yaml profile.
 
-You are ready to use idem-spotinst!!!
+Accessing States
+----------------
 
-STATES
---------
-Idem states are used to make sure resources are in a desired state.
-The desired state of a resource can be specified in sls file.
-In Idem-spotinst, three states are supported: `present`, `absent`, `describe`
-
-present state
-+++++++++++++
-`present` state makes sure a resource exists in a desired state. If a resource does
-not exist, running `present` will create the resource on the provider. If a resource
-exists, running `present` will update the resource on the provider. (Only the values
-that the spotinst REST api supports can be updated.)
-
-absent state
-++++++++++++
-`absent` state makes sure a resource does not exist. If a resource exits, running
-`absent` will delete the resource. If a resource does not exist, running `absent`
-is a no-operation.
-
-describe state
-++++++++++++++
-`describe` state lists all the current resources of the same resource type
-under the spotinst account id specified in the credential profile.
+States can be accessed by their relative location in ``idem-spotinst/idem_spotinst/states``.
 
-States can be accessed by their relative location in `idem-spotinst/idem_spotinst/states`.
-For example, in the state sls yaml file below, spotinst launch specification state can be created with the `present` function.
+For example, a spotinst launch specification state can be created with the *present* function as shown in the following SLS file.
 
 my_resource_launch_spec_state.sls:
 
 .. code:: sls
 
     my_resource_launch_spec:
         spotinst.ocean.aws.launch_spec.present:
@@ -171,26 +148,28 @@
               value: value1
             - key: tag2
               value: value2
           - instance_types:
             - t2.micro
           - image_id: ami-0c02fb55956c7d318
 
-The state sls file can be executed with:
+The Idem command to create the preceding state is:
 
 .. code:: bash
 
     idem state $PWD/my_resource_launch_spec_state.sls
 
-The resource parameters in an sls yaml file follow the exact structure as
-what's in the `Spotinst REST api doc <https://docs.spot.io/api/>`__ . URI Parameters
-should be specified in snake case with "- " in front. All parameters of the api request body
-should be specified in exactly the same way as what's in the spotinst REST api.
+Your SLS should follow the resource parameter structure shown in the `Spotinst REST API <https://docs.spot.io/api/>`__.
+
+* Specify URI parameters in snake case with a leading dash and space "- ".
 
-Current Supported Resources states
-++++++++++++++++++++++++++++++++++
+* Specify all parameters of the API request body exactly as shown in the the `Spotinst REST API <https://docs.spot.io/api/>`__.
+
+Current Supported Resource States
+---------------------------------
 
 ocean_aws
-"""""""""""""
-k8s_cluser
++++++++++
+
+k8s_cluster
 
 launch_spec
```

### Comparing `idem-spotinst-0.1.0/idem_spotinst/acct/spotinst/init.py` & `idem-spotinst-0.2.0/idem_spotinst/acct/spotinst/init.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.1.0/idem_spotinst/conf.py` & `idem-spotinst-0.2.0/idem_spotinst/conf.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.1.0/idem_spotinst/states/spotinst/ocean/aws/k8s_cluster.py` & `idem-spotinst-0.2.0/idem_spotinst/states/spotinst/ocean/aws/k8s_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""State module for managing Ocean AWS k8s cluster."""
 import base64
 import copy
 import json
 from typing import Any
 from typing import Dict
 
 __contracts__ = ["resource"]
@@ -19,95 +20,100 @@
     logging: Dict = None,
     scheduling: Dict = None,
     security: Dict = None,
     strategy: Dict = None,
     auto_scaler=None,
     update_policy: Dict = None,
 ) -> Dict[str, Any]:
-    r"""
+    """Create a Ocean k8s Cluster.
 
-    Create a Ocean k8s Cluster.
+    Refer the `Spot Create Ocean Cluster documentation <https://docs.spot.io/api/#operation/OceanAWSClusterCreate>`_
+    to get insight of functionality and input parameters
 
-    Please refer the `Spot Create Ocean Cluster documentation <https://docs.spot.io/api/#operation/OceanAWSClusterCreate>`_ to get insight of functionality and input parameters
     Args:
 
-        name(Text): ocean cluster name.
-        resource_id(Text, optional): The ocean cluster identifier.
-        auto_scaler(Dict, optional): The automatic scaling mechanism used in Ocean for Kubernetes.
-        capacity (Dict, optional): The overall capability of the Ocean cluster expressed as number of instances and specified with a minimum,
-                                   a maximum, and a target number of running instances.
-        compute (Dict, optional):
+        name(str): ocean cluster name.
+        resource_id(str, Optional): The ocean cluster identifier.
+        auto_scaler(dict, Optional): The automatic scaling mechanism used in Ocean for Kubernetes.
+        capacity (dict, Optional):
+            The overall capability of the Ocean cluster expressed as number of instances and specified with a minimum,
+            a maximum, and a target number of running instances.
+        compute (dict, Optional):
             Compute specifications for the Ocean cluster. This is required for greenfield and optional for brownfield.
-        controller_cluster_id(string, required): Reporting identifier for the Ocean Controller.
-        logging	(Dict, optional):  Logging configuration for ocean aws cluster.
-        region(string, required): Region for the Ocean cluster to run in.
-        scheduling(Dict, optional)	: An object used to define times for a task such as a shutdown to be activated.
-        security(Dict, optional): Object for cluster security features.
-        strategy(Dict, optional): An object defining the cluster strategy with regard to waiting periods and utilization of on-demand and reserved instances.
-        update_policy(Dict, optional): Configures the cluster update policy. You can configure to start the roll on update and run it in defined batches.
+        controller_cluster_id(str): Reporting identifier for the Ocean Controller.
+        logging	(dict, Optional):  Logging configuration for ocean aws cluster.
+        region(str): Region for the Ocean cluster to run in.
+        scheduling(dict, Optional)	: An object used to define times for a task such as a shutdown to be activated.
+        security(dict, Optional): Object for cluster security features.
+        strategy(dict, Optional):
+            An object defining the cluster strategy with regard to waiting periods
+            and utilization of on-demand and reserved instances.
+        update_policy(dict, Optional): Configures the cluster update policy.
+            You can configure to start the roll on update and run it in defined batches.
 
     Request Syntax:
-       [spotinst.ocean.aws.k8s_cluster-state-id]:
-             spotinst.ocean.aws.k8s_cluster.present:
-              - name: 'string'
-              - controller_cluster_id: 'string'
-              - region: 'string'
-              - update_policy:
-                  shouldRoll: boolean
-                  roll:
-                     batchSizePercentage: Integer
-                     comment: 'string'
-                     batchMinHealthyPercentage: Integer
-              - compute:
-                  launchSpecification:
-                    keyPair: 'string'
-                    imageId: 'string'
-                    associatePublicIpAddress: boolean
-                    rootVolumeSize: Integer
-                    iamInstanceProfile:
-                        arn: 'string'
-                    userData: 'string'
-                    tags:
-                    - tagKey: 'string'
-                      tagValue: 'string'
-                    - tagKey: 'string'
-                      tagValue: 'string'
-                    securityGroupIds:
+        .. code-block:: sls
+
+            [spotinst.ocean.aws.k8s_cluster-state-id]:
+               spotinst.ocean.aws.k8s_cluster.present:
+                  - name: 'string'
+                  - controller_cluster_id: 'string'
+                  - region: 'string'
+                  - update_policy:
+                      shouldRoll: boolean
+                      roll:
+                         batchSizePercentage: Integer
+                         comment: 'string'
+                         batchMinHealthyPercentage: Integer
+                  - compute:
+                      launchSpecification:
+                        keyPair: 'string'
+                        imageId: 'string'
+                        associatePublicIpAddress: boolean
+                        rootVolumeSize: Integer
+                        iamInstanceProfile:
+                            arn: 'string'
+                        userData: 'string'
+                        tags:
+                        - tagKey: 'string'
+                          tagValue: 'string'
+                        - tagKey: 'string'
+                          tagValue: 'string'
+                        securityGroupIds:
+                            - 'string'
+                      subnetIds:
+                         - 'string'
+                      instanceTypes:
+                        whitelist:
                         - 'string'
-                  subnetIds:
-                     - 'string'
-                  instanceTypes:
-                    whitelist:
-                    - 'string'
-              - strategy:
-                  fallbackToOd: boolean
-                  spotPercentage: Integer
-                  utilizeReservedInstances: boolean
-              - auto_scaler:
-                  isEnabled: boolean
-                  isAutoConfig: boolean
-                  cooldown: Integer
-                  headroom:
-                    cpuPerUnit: Integer
-                    memoryPerUnit: Integer
-                    numOfUnits: Integer
-                  down:
-                    maxScaleDownPercentage: Integer
-              - resourceLimits:
-                  maxMemoryGib: Integer
-                  maxVCpu: Integer
-              - capacity:
-                  maximum: Integer
-                  minimum: Integer
+                  - strategy:
+                      fallbackToOd: boolean
+                      spotPercentage: Integer
+                      utilizeReservedInstances: boolean
+                  - auto_scaler:
+                      isEnabled: boolean
+                      isAutoConfig: boolean
+                      cooldown: Integer
+                      headroom:
+                        cpuPerUnit: Integer
+                        memoryPerUnit: Integer
+                        numOfUnits: Integer
+                      down:
+                        maxScaleDownPercentage: Integer
+                  - resourceLimits:
+                      maxMemoryGib: Integer
+                      maxVCpu: Integer
+                  - capacity:
+                      maximum: Integer
+                      minimum: Integer
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             ocean_cluster:
               spotinst.ocean.aws.k8s_cluster.present:
               - name: idem-test
               - controller_cluster_id: idem-test
               - region: ap-east-1
@@ -158,15 +164,14 @@
                     maxMemoryGib: 20000
                     maxVCpu: 100000
               - capacity:
                   maximum: 1000
                   minimum: 1
 
     """
-
     if auto_scaler is None:
         auto_scaler = {}
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
 
     # If userdata is set in compute, encode userData to base64
     if (
         compute
@@ -395,44 +400,45 @@
 
 async def absent(
     hub,
     ctx,
     name: str,
     resource_id: str = None,
 ) -> Dict[str, Any]:
-    r"""
+    """Deletes the specified Ocean cluster.
 
-    Deletes the specified Ocean cluster.
     When this call completes, the cluster is no longer available for use.
 
-    Please refer the `Spot Delete Ocean Cluster documentation <https://docs.spot.io/api/#operation/OceanAWSClusterDelete>`_ to get insight of functionality and input parameters
+    Refer the `Spot Delete Ocean Cluster documentation <https://docs.spot.io/api/#operation/OceanAWSClusterDelete>`_
+    to get insight of functionality and input parameters
 
     Args:
-        name(Text): An idem name of the ocean cluster.
-        resource_id(Text): The ID of the ocean cluster.
+        name(str): An idem name of the ocean cluster.
+        resource_id(str, Optional): The ID of the ocean cluster.
 
     Request Syntax:
-       [k8s_cluster-resource-id]:
-              spotinst.ocean.aws.k8s_cluster.absent:
-              - name: 'string'
-              - resource_id: 'string'
+        .. code-block:: sls
+
+           [k8s_cluster-resource-id]:
+             spotinst.ocean.aws.k8s_cluster.absent:
+               - name: 'string'
+               - resource_id: 'string'
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             idem-test-k8s_cluster:
               spotinst.ocean.aws.k8s_cluster.absent:
                 - name: idem-test-k8s_cluster
                 - resource_id:idem-test-k8s_cluster
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     if not resource_id:
         result["comment"] = hub.tool.spotinst.comment_utils.already_absent_comment(
             resource_type="spotinst.ocean.aws.k8s_cluster", name=name
         )
         return result
 
@@ -495,31 +501,30 @@
         result["result"] = False
         result["comment"] = before["comment"]
 
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""
+    """Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
-    Describe the resource in a way that can be recreated/managed with the corresponding "present" function
     Gets information about the ocean clusters.
 
-    Please refer the `Spot Listing Ocean Cluster documentation <https://docs.spot.io/api/#operation/OceanAWSClusterList>`_ to get insight of functionality and input parameters
+    Refer the `Spot Listing Ocean Cluster documentation <https://docs.spot.io/api/#operation/OceanAWSClusterList>`_
+    to get insight of functionality and input parameters
 
     Returns:
         Dict[str, Dict[str, Any]]
 
     Examples:
-
         .. code-block:: bash
 
             $ idem describe spotinst.ocean.aws.k8s_cluster
-    """
 
+    """
     result = {}
     url = (
         f"{hub.exec.spotinst.URL}/ocean/aws/k8s/cluster?accountId={ctx.acct.account_id}"
     )
     ret = await hub.exec.request.json.get(
         ctx,
         url=url,
```

### Comparing `idem-spotinst-0.1.0/idem_spotinst/states/spotinst/ocean/aws/launch_spec.py` & `idem-spotinst-0.2.0/idem_spotinst/states/spotinst/ocean/aws/launch_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""State module for managing Ocean AWS LaunchSpec."""
 import base64
 import copy
 import json
 from typing import Any
 from typing import Dict
 from typing import List
 
@@ -33,118 +34,118 @@
     elastic_ip_pool: Dict = None,
     auto_scale: Dict = None,
     block_device_mappings: List = None,
     associate_public_ip_address: bool = None,
     scheduling: Dict = None,
     instance_metadata_options: Dict = None,
 ) -> Dict[str, Any]:
-    r"""
+    """Create a Launch Spec(Virtual Node Group).
 
-     Create a Virtual Node Group.
+    Refer the `Spot Create Launch Spec(Virtual Node Group) documentation <https://docs.spot.io/api/#operation/OceanAWSLaunchSpecCreate>`_
+    to get insight of functionality and input parameters
 
-     Please refer the `Spot Create Launch Spec(Virtual Node Group) documentation <https://docs.spot.io/api/#operation/OceanAWSLaunchSpecCreate>`_ to get insight of functionality and input parameters
-
-     Args:
-         name(Text): launch specification name.
-         image_id(Text): AWS image identifier.
-         ocean_id(Text): The Ocean cluster identifier. Required for Launch Spec creation
-         resource_id(Text, optional): The virtual node group identifier.
-         iam_instance_profile(Dict, optional): The instance profile iamRole object.
-         taints(List, optional): Add taints to Launch Spec.
-         tags(List, optional): List of kay-value pairs of tags.
-         subnet_ids(List, optional): Set subnets in launchSpec. Each element in the array is a subnet identifier.
-         user_data(Text, optional): Set user data script.
-         security_group_ids(List, optional): Set security groups. Each element in the array is a security group identifier.
-         root_volume_size(Integer, optional): Set root volume size (in GB). This field and blockDeviceMappings cannot be used in the same specification.
-         strategy(Dict, optional): Similar to a strategy for an Ocean cluster, but applying only to a virtual node group.
-         restrict_scale_down(Boolean, optional): When set to “True”, VNG nodes will be treated as if all pods running have the restrict-scale-down label. Therefore, Ocean will not scale nodes down unless empty.
-         resource_limits(Dict, optional): Option to set a maximum/minimum number of instances per launch specification.
-         labels(List, optional): An array of labels to add to the VNG nodes. Only custom user labels are allowed, and not Kubernetes built-in labels or Spot internal labels.
-         instance_types(List, optional): A list of instance types allowed to be provisioned for pods pending for the launch specification.
-         preferred_spot_types(List, optional): When Ocean scales up instances, it takes your preferred types into consideration while maintaining a variety of machine types running for optimized distribution.
-         elastic_ip_pool(Dict, optional): Assign an Elastic IP to the instances launched by the launch spec.
-         auto_scale(Dict, optional): Object specifying the automatic scaling of an Ocean VNG.
-         block_device_mappings(List, optional):
+    Args:
+         name(str): launch specification name.
+         image_id(str): AWS image identifier.
+         ocean_id(str): The Ocean cluster identifier. Required for Launch Spec creation
+         resource_id(str, Optional): The virtual node group identifier.
+         iam_instance_profile(dict, Optional): The instance profile iamRole object.
+         taints(list, Optional): Add taints to Launch Spec.
+         tags(list, Optional): List of kay-value pairs of tags.
+         subnet_ids(list, Optional): Set subnets in launchSpec. Each element in the array is a subnet identifier.
+         user_data(str, Optional): Set user data script.
+         security_group_ids(list, Optional): Set security groups. Each element in the array is a security group identifier.
+         root_volume_size(int, Optional): Set root volume size (in GB). This field and blockDeviceMappings cannot be used in the same specification.
+         strategy(dict, Optional): Similar to a strategy for an Ocean cluster, but applying only to a virtual node group.
+         restrict_scale_down(bool, Optional): When set to “True”, VNG nodes will be treated as if all pods running have the restrict-scale-down label. Therefore, Ocean will not scale nodes down unless empty.
+         resource_limits(dict, Optional): Option to set a maximum/minimum number of instances per launch specification.
+         labels(list, Optional): An array of labels to add to the VNG nodes. Only custom user labels are allowed, and not Kubernetes built-in labels or Spot internal labels.
+         instance_types(list, Optional): A list of instance types allowed to be provisioned for pods pending for the launch specification.
+         preferred_spot_types(list, Optional): When Ocean scales up instances, it takes your preferred types into consideration while maintaining a variety of machine types running for optimized distribution.
+         elastic_ip_pool(dict, Optional): Assign an Elastic IP to the instances launched by the launch spec.
+         auto_scale(dict, Optional): Object specifying the automatic scaling of an Ocean VNG.
+         block_device_mappings(list, Optional):
             Block devices that are exposed to the instance. You can specify virtual devices and EBS volumes.
             This parameter and rootVolumeSize cannot be in the spec at the same time.
             This parameter can be null, but if not null, it must contain at least one block device.
-         associate_public_ip_address(Boolean, optional): Configure public IP address allocation.
-         scheduling(Dict, optional): An object used to define scheduled tasks such as a manual headroom update.
-         instance_metadata_options(Dict, optional): Ocean instance metadata options object for IMDSv2.
+         associate_public_ip_address(bool, Optional): Configure public IP address allocation.
+         scheduling(dict, Optional): An object used to define scheduled tasks such as a manual headroom update.
+         instance_metadata_options(dict, Optional): Ocean instance metadata options object for IMDSv2.
 
     Request Syntax:
-        [spotinst.ocean.aws.launch_spec-resource-id]:
-             spotinst.ocean.aws.launch_spec.present:
-               - name: 'string'
-               - resource_id: 'string'
-               - taints:
-                 - effect: 'string'
-                   key: 'string'
-                   value: 'string'
-               - tags:
-                 - tagKey: 'string'
-                   tagValue: 'string'
-                 - tagKey: 'string'
-                   tagValue: 'string'
-               - subnet_ids:
-                 - 'string'
-               - user_data: 'string'
-               - security_group_ids:
-                 - 'string'
-               - root_volume_size: Integer
-               - resource_limits:
-                   maxInstanceCount: Integer
-               - ocean_id: 'string'
-               - labels:
-                 - key: 'string'
-                   value: 'string'
-                 - key: 'string'
-                   value: 'string'
-               - instance_types:
-                 - 'string'
-               - image_id: 'string'
-               - iam_instance_profile:
-                   arn: 'string'
-               - associate_public_ip_address: true/false
-               - preferred_spot_types:
-                 - 'string'
-               - elastic_ip_pool:
-                   tagSelector:
-                     tagKey: 'string'
-                     tagValue: 'string'
-               - auto_scale:
-                   headrooms:
-                    - cpuPerUnit: Integer
-                      memoryPerUnit: Integer
-                      numOfUnits: Integer
-               - block_device_mappings:
-                - deviceName: 'string'
-                  ebs:
-                    deleteOnTermination: true/false
-                    encrypted: true/false
-                    volumeSize: Integer
-                    volumeType: 'string'
-                - scheduling:
-                    tasks:
-                      - isEnabled: true/false
-                        cronExpression: 'string'
-                        taskType: 'string'
-                    shutdownHours:
-                      timeWindows:
-                        - 'string'
-                    isEnabled: true/false
-                - instanceMetadataOptions:
-                            httpTokens: 'string'
-                            httpPutResponseHopLimit: Integer
+        .. code-block:: sls
 
-     Returns:
-         Dict[str, Any]
+            [spotinst.ocean.aws.launch_spec-resource-id]:
+                spotinst.ocean.aws.launch_spec.present:
+                   - name: 'string'
+                   - resource_id: 'string'
+                   - taints:
+                     - effect: 'string'
+                       key: 'string'
+                       value: 'string'
+                   - tags:
+                     - tagKey: 'string'
+                       tagValue: 'string'
+                     - tagKey: 'string'
+                       tagValue: 'string'
+                   - subnet_ids:
+                     - 'string'
+                   - user_data: 'string'
+                   - security_group_ids:
+                     - 'string'
+                   - root_volume_size: Integer
+                   - resource_limits:
+                       maxInstanceCount: Integer
+                   - ocean_id: 'string'
+                   - labels:
+                     - key: 'string'
+                       value: 'string'
+                     - key: 'string'
+                       value: 'string'
+                   - instance_types:
+                     - 'string'
+                   - image_id: 'string'
+                   - iam_instance_profile:
+                       arn: 'string'
+                   - associate_public_ip_address: true/false
+                   - preferred_spot_types:
+                     - 'string'
+                   - elastic_ip_pool:
+                       tagSelector:
+                         tagKey: 'string'
+                         tagValue: 'string'
+                   - auto_scale:
+                       headrooms:
+                        - cpuPerUnit: Integer
+                          memoryPerUnit: Integer
+                          numOfUnits: Integer
+                   - block_device_mappings:
+                    - deviceName: 'string'
+                      ebs:
+                        deleteOnTermination: true/false
+                        encrypted: true/false
+                        volumeSize: Integer
+                        volumeType: 'string'
+                    - scheduling:
+                        tasks:
+                          - isEnabled: true/false
+                            cronExpression: 'string'
+                            taskType: 'string'
+                        shutdownHours:
+                          timeWindows:
+                            - 'string'
+                        isEnabled: true/false
+                    - instanceMetadataOptions:
+                                httpTokens: 'string'
+                                httpPutResponseHopLimit: Integer
 
-     Examples:
+    Returns:
+         Dict[str, Any]
 
+    Examples:
          .. code-block:: sls
 
              ols-77e27034:
                spotinst.ocean.aws.launch_spec.present:
                - name: cluster-arm
                - resource_id: ols-77e27034
                - taints:
@@ -197,16 +198,16 @@
                     shutdownHours:
                       timeWindows:
                         - "Sat:08:00-Sun:08:00"
                     isEnabled: true
                 - instanceMetadataOptions:
                             httpTokens: optional
                             httpPutResponseHopLimit: 12
-    """
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     user_data_base64 = None
     if user_data:
         try:
             user_data_base64 = base64.b64encode(user_data.encode("utf-8")).decode(
                 "utf-8"
             )
@@ -424,44 +425,46 @@
             resource_type="spotinst.ocean.aws.launch_spec", name=name
         )
 
     return result
 
 
 async def absent(hub, ctx, name: str, resource_id: str = None) -> Dict[str, Any]:
-    r"""
-    Deletes the specified launch Spec.
+    """Deletes the specified launch Spec.
+
     When this call completes, the launch configuration is no longer available for use.
 
-    Please refer the `Spot Delete Launch Spec(Virtual Node Group) documentation <https://docs.spot.io/api/#operation/OceanAWSLaunchSpecDelete>`_ to get insight of functionality and input parameters
+    Refer the `Spot Delete Launch Spec(Virtual Node Group) documentation <https://docs.spot.io/api/#operation/OceanAWSLaunchSpecDelete>`_
+    to get insight of functionality and input parameters
 
 
     Args:
-        name(Text): An idem name of the launch spec.
-        resource_id(Text): The AWS ID of the launch spec.
+        name(str): An idem name of the launch spec.
+        resource_id(str, Optional): The AWS ID of the launch spec.
 
     Request Syntax:
-       [launch_spec-resource-id]:
-              spotinst.ocean.aws.launch_spec.absent:
-              - name: 'string'
-              - resource_id: 'string'
+         .. code-block:: sls
+
+           [launch_spec-resource-id]:
+                  spotinst.ocean.aws.launch_spec.absent:
+                  - name: 'string'
+                  - resource_id: 'string'
 
     Returns:
         Dict[str, Any]
 
     Examples:
-
         .. code-block:: sls
 
             idem-test-launch_spec:
               spotinst.ocean.aws.launch_spec.absent:
                 - name: idem-test-launch_spec
-                - resource_id:idem-test-launch_spec
-    """
+                - resource_id: idem-test-launch_spec
 
+    """
     result = dict(comment=(), old_state=None, new_state=None, name=name, result=True)
     if not resource_id:
         result["comment"] = hub.tool.spotinst.comment_utils.already_absent_comment(
             resource_type="spotinst.ocean.aws.launch_spec", name=name
         )
         return result
 
@@ -525,31 +528,29 @@
         result["result"] = False
         result["comment"] = before["comment"]
 
     return result
 
 
 async def describe(hub, ctx) -> Dict[str, Dict[str, Any]]:
-    r"""
+    """Describe the resource in a way that can be recreated/managed with the corresponding "present" function.
 
-    Describe the resource in a way that can be recreated/managed with the corresponding "present" function
     Gets information about the virtual node groups for the cluster.
 
     Please refer the `Spot Listing Launch Spec(Virtual Node Group) documentation <https://docs.spot.io/api/#operation/OceanAWSLaunchSpecList>`_ to get insight of functionality and input parameters
 
     Returns:
         Dict[str, Dict[str, Any]]
 
     Examples:
-
         .. code-block:: bash
 
             $ idem describe spotinst.ocean.aws.launch_spec
-    """
 
+    """
     result = {}
 
     url = f"{hub.exec.spotinst.URL}/ocean/aws/k8s/launchSpec?accountId={ctx.acct.account_id}"
     ret = await hub.exec.request.json.get(
         ctx,
         url=url,
         success_codes=[200],
```

### Comparing `idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/comment_utils.py` & `idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/comment_utils.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/ocean/aws/conversion_utils.py` & `idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/aws/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/ocean/aws/k8s_cluster_utils.py` & `idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/aws/k8s_cluster_utils.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/ocean/aws/tag_utils.py` & `idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/ocean/aws/tag_utils.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/state_comparison_utils.py` & `idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/state_comparison_utils.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.1.0/idem_spotinst/tool/spotinst/state_utils.py` & `idem-spotinst-0.2.0/idem_spotinst/tool/spotinst/state_utils.py`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.1.0/idem_spotinst.egg-info/PKG-INFO` & `idem-spotinst-0.2.0/idem_spotinst.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idem-spotinst
-Version: 0.1.0
+Version: 0.2.0
 Summary: UNKNOWN
 Home-page: UNKNOWN
 Author: Prerna
 Author-email: prjain@vmware.com
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
-    Idem plugin to manage Spotinst resources
+The Idem spot instance provider
 
 About
 =====
 
-Spotinst Provider Idem plugin
+An Idem plugin to manage spot instance resources. A spot instance is an instance deployed at a discount on spare EC2 capacity.
 
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
+You can install ``idem-spotinst`` with the Python package installer (PyPI) or from source.
+
+Install from PyPI
++++++++++++++++++
 
-   If wanting to contribute to the project, and setup your local development
-   environment, see the ``CONTRIBUTING.rst`` document in the source repository
-   for this project.
+.. code-block:: bash
 
-If wanting to use ``idem-spotinst``, you can do so from source.
+      pip install idem-spotinst
 
-Install from source
+Install from Source
 +++++++++++++++++++
 
 .. code-block:: bash
 
    # clone repo
    git clone git@<your-project-path>/idem-spotinst.git
    cd idem-spotinst
@@ -89,89 +88,67 @@
    python3 -m venv .venv
    source .venv/bin/activate
    pip install -e .
 
 Usage
 =====
 
-Credentials Setup
------------------
+Setup
+-----
 
-After installation, the spotinst Idem execution and state modules will be accessible to the pop `hub`.
-In order to use them, we need to set up our credentials.
+After installation, ``idem-spotinst`` execution and state modules are accessible to the pop *hub*.
 
 For more information:
 
 * `Intro to Plugin Oriented Programming (POP) <https://pop-book.readthedocs.io/en/latest/>`__
 * `pop hub <https://pop-book.readthedocs.io/en/latest/main/hub.html#>`__
 
-Create a new file called `credentials.yaml` and populate it with credentials.
-The `default` profile will be picked up automatically by `idem`.
-
-There are multiple authentication backends for `idem-spotinst` which each have their own unique set of parameters.
-The following examples show the parameters that can be used to define credential profiles.
+To use ``idem-spotinst`` execution and state modules to manage spot instance resources, set up a credentials.yaml file for authentication. There are multiple authentication backends for ``idem-spotinst``, where each has its own unique set of parameters. For example:
 
 credentials.yaml:
 
 ..  code:: sls
 
     spotinst:
       default:
         account_id: act-11c833de
         token: b5460afe3c29a30c28abd54d190d1aa923587574321e75925cfc8268b54b4562
 
-Next step is to encrypt the credentials file, and add the encryption key and encrypted file
-path to the ENVIRONMENT.
+For more about Idem credentials files, including recommended steps for encryption and environment variables, see `Authenticating with Idem <https://docs.idemproject.io/getting-started/en/latest/topics/gettingstarted/authenticating.html>`__
 
-Encrypt the credential file:
+You are now ready to use idem-spotinst.
 
-.. code:: bash
+States
+------
 
-    Idem encrypt credentials.yaml
+Idem SLS files use states to ensure that resources are in a desired configuration. An idem-spotinst SLS file supports three state functions: *present*, *absent*, and *describe*.
 
-This will generate a credentials.yaml.fernet file and a command line output token::
+present
++++++++
 
-    -AXFSEFSSEjsfdG_lb333kVhCVSCDyOFH4eABCDEFNwI=
+The *present* function ensures that a resource exists. If a resource doesn't exist, running *present* creates it. If the resource already exists, running *present* might leave it unchanged, or update it if there are any configuration changes.
 
-Add these to your environment:
+You can only update values that the spotinst REST API supports.
 
-.. code:: bash
+absent
+++++++
+
+The *absent* function ensures that a resource does not exist. If the resource exists, running *absent* deletes it. If the resource doesn't exist, running *absent* has no effect.
 
-    export ACCT_KEY="-AXFSEFSSEjsfdG_lb333kVhCVSCDyOFH4eABCDEFNwI="
-    export ACCT_FILE=$PWD/credentials.yaml.fernet
+describe
+++++++++
 
+The *describe* function returns a list of all resources of the specified type under the spotinst account ID from your credentials.yaml profile.
 
-You are ready to use idem-spotinst!!!
+Accessing States
+----------------
 
-STATES
---------
-Idem states are used to make sure resources are in a desired state.
-The desired state of a resource can be specified in sls file.
-In Idem-spotinst, three states are supported: `present`, `absent`, `describe`
-
-present state
-+++++++++++++
-`present` state makes sure a resource exists in a desired state. If a resource does
-not exist, running `present` will create the resource on the provider. If a resource
-exists, running `present` will update the resource on the provider. (Only the values
-that the spotinst REST api supports can be updated.)
-
-absent state
-++++++++++++
-`absent` state makes sure a resource does not exist. If a resource exits, running
-`absent` will delete the resource. If a resource does not exist, running `absent`
-is a no-operation.
-
-describe state
-++++++++++++++
-`describe` state lists all the current resources of the same resource type
-under the spotinst account id specified in the credential profile.
+States can be accessed by their relative location in ``idem-spotinst/idem_spotinst/states``.
 
-States can be accessed by their relative location in `idem-spotinst/idem_spotinst/states`.
-For example, in the state sls yaml file below, spotinst launch specification state can be created with the `present` function.
+For example, a spotinst launch specification state can be created with the *present* function as shown in the following SLS file.
 
 my_resource_launch_spec_state.sls:
 
 .. code:: sls
 
     my_resource_launch_spec:
         spotinst.ocean.aws.launch_spec.present:
@@ -195,28 +172,30 @@
               value: value1
             - key: tag2
               value: value2
           - instance_types:
             - t2.micro
           - image_id: ami-0c02fb55956c7d318
 
-The state sls file can be executed with:
+The Idem command to create the preceding state is:
 
 .. code:: bash
 
     idem state $PWD/my_resource_launch_spec_state.sls
 
-The resource parameters in an sls yaml file follow the exact structure as
-what's in the `Spotinst REST api doc <https://docs.spot.io/api/>`__ . URI Parameters
-should be specified in snake case with "- " in front. All parameters of the api request body
-should be specified in exactly the same way as what's in the spotinst REST api.
+Your SLS should follow the resource parameter structure shown in the `Spotinst REST API <https://docs.spot.io/api/>`__.
+
+* Specify URI parameters in snake case with a leading dash and space "- ".
 
-Current Supported Resources states
-++++++++++++++++++++++++++++++++++
+* Specify all parameters of the API request body exactly as shown in the the `Spotinst REST API <https://docs.spot.io/api/>`__.
+
+Current Supported Resource States
+---------------------------------
 
 ocean_aws
-"""""""""""""
-k8s_cluser
++++++++++
+
+k8s_cluster
 
 launch_spec
```

### Comparing `idem-spotinst-0.1.0/idem_spotinst.egg-info/SOURCES.txt` & `idem-spotinst-0.2.0/idem_spotinst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idem-spotinst-0.1.0/setup.py` & `idem-spotinst-0.2.0/setup.py`

 * *Files identical despite different names*

