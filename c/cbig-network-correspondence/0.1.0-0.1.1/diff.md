# Comparing `tmp/cbig_network_correspondence-0.1.0.tar.gz` & `tmp/cbig_network_correspondence-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbig_network_correspondence-0.1.0.tar", max compression
+gzip compressed data, was "cbig_network_correspondence-0.1.1.tar", max compression
```

## Comparing `cbig_network_correspondence-0.1.0.tar` & `cbig_network_correspondence-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    16811 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/README.md
--rw-r--r--   0        0        0     2303 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      490 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/__init__.py
--rw-r--r--   0        0        0    14151 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/compute_overlap_with_atlases.py
--rw-r--r--   0        0        0     3143 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/grab_data_info.py
--rw-r--r--   0        0        0      429 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/load_example.py
--rw-r--r--   0        0        0        0 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/py.typed
--rw-r--r--   0        0        0    12032 2023-04-18 12:01:59.446442 cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/visualize_overlap_lib.py
--rw-r--r--   0        0        0    18205 1970-01-01 00:00:00.000000 cbig_network_correspondence-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    16956 2023-05-22 08:41:24.908590 cbig_network_correspondence-0.1.1/README.md
+-rw-r--r--   0        0        0     2303 2023-05-22 08:41:24.908590 cbig_network_correspondence-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      490 2023-05-22 08:41:24.908590 cbig_network_correspondence-0.1.1/src/cbig_network_correspondence/__init__.py
+-rw-r--r--   0        0        0    14151 2023-05-22 08:41:24.908590 cbig_network_correspondence-0.1.1/src/cbig_network_correspondence/compute_overlap_with_atlases.py
+-rw-r--r--   0        0        0     3143 2023-05-22 08:41:24.908590 cbig_network_correspondence-0.1.1/src/cbig_network_correspondence/grab_data_info.py
+-rw-r--r--   0        0        0      429 2023-05-22 08:41:24.908590 cbig_network_correspondence-0.1.1/src/cbig_network_correspondence/load_example.py
+-rw-r--r--   0        0        0        0 2023-05-22 08:41:24.908590 cbig_network_correspondence-0.1.1/src/cbig_network_correspondence/py.typed
+-rw-r--r--   0        0        0    12032 2023-05-22 08:41:24.908590 cbig_network_correspondence-0.1.1/src/cbig_network_correspondence/visualize_overlap_lib.py
+-rw-r--r--   0        0        0    18252 1970-01-01 00:00:00.000000 cbig_network_correspondence-0.1.1/PKG-INFO
```

### Comparing `cbig_network_correspondence-0.1.0/README.md` & `cbig_network_correspondence-0.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cbig_network_correspondence?style=flat-square)](https://pypi.python.org/pypi/cbig_network_correspondence/)
 [![PyPI - License](https://img.shields.io/pypi/l/cbig_network_correspondence?style=flat-square)](https://pypi.python.org/pypi/cbig_network_correspondence/)
 [![Coookiecutter - Wolt](https://img.shields.io/badge/cookiecutter-Wolt-00c2e8?style=flat-square&logo=cookiecutter&logoColor=D4AA00&link=https://github.com/woltapp/wolt-python-package-cookiecutter)](https://github.com/woltapp/wolt-python-package-cookiecutter)
 
 
 ---
 
+**Documentation**: [https://rubykong.github.io/cbig_network_correspondence](https://rubykong.github.io/cbig_network_correspondence)
+
 **Source Code**: [https://github.com/rubykong/cbig_network_correspondence](https://github.com/rubykong/cbig_network_correspondence)
 
 **PyPI**: [https://pypi.org/project/cbig_network_correspondence/](https://pypi.org/project/cbig_network_correspondence/)
 
 ---
 
 This toolbox was used to explore the network correspondence between networks across different atlases. 
@@ -32,15 +34,15 @@
 
 We will provide detailed usage of these function in the following sections.
 
 ### Atlases we included
 
 Check this list for the atlases we have included. We use abbreviations for the atlases. Here we provide the decription for each atlas. If you want us to include your atlas, please contact me (roo.cone@gmail.com).
 
-![networkcorrespondence](https://user-images.githubusercontent.com/20438248/232702654-3f334164-bb13-41af-a7aa-8f29bae9fca7.jpg)
+![networkcorrespondence](https://github.com/rubykong/cbig_network_correspondence_data/assets/20438248/b430f2fe-4b78-49f2-9084-5a43d450dba1)
 
 These atlases should be automatically downloaded when you install the toolbox. If you want to download the atlases manually, you can find the atlases here: https://github.com/rubykong/cbig_network_correspondence_data. The atlas data will be automatically downloaded in your python package directory: `cbig_network_correspondence/src/cbig_network_correspondence/data`.
 
 ### Config file
 
 In this toolbox, the information for each atlas was constructed as config file. We have included the config files for each atlas. The config files will be automatically downloaded when you install the toolbox. If you want to check the config files manually, you can find the config files in your python package directory: `cbig_network_correspondence/src/cbig_network_correspondence/data/atlas_config`. If you want to use your own atlas, you can create your own config file, check next sections for details.
```

### Comparing `cbig_network_correspondence-0.1.0/pyproject.toml` & `cbig_network_correspondence-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cbig_network_correspondence"
-version = "0.1.0"
+version = "0.1.1"
 description = "A toolbox for exploring network correspondence across atlases"
 authors = [
     "Ruby Kong <roo.cone@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/compute_overlap_with_atlases.py` & `cbig_network_correspondence-0.1.1/src/cbig_network_correspondence/compute_overlap_with_atlases.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/grab_data_info.py` & `cbig_network_correspondence-0.1.1/src/cbig_network_correspondence/grab_data_info.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.1.0/src/cbig_network_correspondence/visualize_overlap_lib.py` & `cbig_network_correspondence-0.1.1/src/cbig_network_correspondence/visualize_overlap_lib.py`

 * *Files identical despite different names*

### Comparing `cbig_network_correspondence-0.1.0/PKG-INFO` & `cbig_network_correspondence-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbig-network-correspondence
-Version: 0.1.0
+Version: 0.1.1
 Summary: A toolbox for exploring network correspondence across atlases
 Home-page: https://rubykong.github.io/cbig_network_correspondence
 License: MIT
 Author: Ruby Kong
 Author-email: roo.cone@gmail.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -12,18 +12,16 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: gitpython (>=3.1.27,<4.0.0)
 Requires-Dist: natsort (>=8.3.1,<9.0.0)
 Requires-Dist: nibabel (>=5.0.1,<6.0.0)
 Requires-Dist: numpy (>=1.20.3,<2.0.0)
 Requires-Dist: scipy (>=1.9.0,<2.0.0)
@@ -37,14 +35,16 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/cbig_network_correspondence?style=flat-square)](https://pypi.python.org/pypi/cbig_network_correspondence/)
 [![PyPI - License](https://img.shields.io/pypi/l/cbig_network_correspondence?style=flat-square)](https://pypi.python.org/pypi/cbig_network_correspondence/)
 [![Coookiecutter - Wolt](https://img.shields.io/badge/cookiecutter-Wolt-00c2e8?style=flat-square&logo=cookiecutter&logoColor=D4AA00&link=https://github.com/woltapp/wolt-python-package-cookiecutter)](https://github.com/woltapp/wolt-python-package-cookiecutter)
 
 
 ---
 
+**Documentation**: [https://rubykong.github.io/cbig_network_correspondence](https://rubykong.github.io/cbig_network_correspondence)
+
 **Source Code**: [https://github.com/rubykong/cbig_network_correspondence](https://github.com/rubykong/cbig_network_correspondence)
 
 **PyPI**: [https://pypi.org/project/cbig_network_correspondence/](https://pypi.org/project/cbig_network_correspondence/)
 
 ---
 
 This toolbox was used to explore the network correspondence between networks across different atlases. 
@@ -65,15 +65,15 @@
 
 We will provide detailed usage of these function in the following sections.
 
 ### Atlases we included
 
 Check this list for the atlases we have included. We use abbreviations for the atlases. Here we provide the decription for each atlas. If you want us to include your atlas, please contact me (roo.cone@gmail.com).
 
-![networkcorrespondence](https://user-images.githubusercontent.com/20438248/232702654-3f334164-bb13-41af-a7aa-8f29bae9fca7.jpg)
+![networkcorrespondence](https://github.com/rubykong/cbig_network_correspondence_data/assets/20438248/b430f2fe-4b78-49f2-9084-5a43d450dba1)
 
 These atlases should be automatically downloaded when you install the toolbox. If you want to download the atlases manually, you can find the atlases here: https://github.com/rubykong/cbig_network_correspondence_data. The atlas data will be automatically downloaded in your python package directory: `cbig_network_correspondence/src/cbig_network_correspondence/data`.
 
 ### Config file
 
 In this toolbox, the information for each atlas was constructed as config file. We have included the config files for each atlas. The config files will be automatically downloaded when you install the toolbox. If you want to check the config files manually, you can find the config files in your python package directory: `cbig_network_correspondence/src/cbig_network_correspondence/data/atlas_config`. If you want to use your own atlas, you can create your own config file, check next sections for details.
```

