# Comparing `tmp/twb_project-1.0.0.tar.gz` & `tmp/twb_project-1.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twb_project-1.0.0.tar", max compression
+gzip compressed data, was "twb_project-1.0.1a0.tar", max compression
```

## Comparing `twb_project-1.0.0.tar` & `twb_project-1.0.1a0.tar`

### file list

```diff
@@ -1,18 +1,16 @@
--rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-1.0.0/LICENSE
--rw-r--r--   0        0        0     1547 2023-02-27 01:45:34.838817 twb_project-1.0.0/README.md
--rw-r--r--   0        0        0      760 2023-05-06 15:59:06.172123 twb_project-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      218 2023-05-02 04:53:16.027176 twb_project-1.0.0/twb/__init__.py
--rw-r--r--   0        0        0      788 2023-02-26 15:18:15.849792 twb_project-1.0.0/twb/bip.py
--rw-r--r--   0        0        0    20033 2023-05-06 15:57:13.965716 twb_project-1.0.0/twb/builder.py
--rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-1.0.0/twb/builder_helpers.py
--rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-1.0.0/twb/decompressor.py
--rw-r--r--   0        0        0     9493 2023-03-26 18:01:42.380403 twb_project-1.0.0/twb/downloader.py
--rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-1.0.0/twb/logger.py
--rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 twb_project-1.0.0/twb/logger_init.py
--rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-1.0.0/twb/modifier.py
--rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-1.0.0/twb/parallelization.py
--rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-1.0.0/twb/reader.py
--rw-r--r--   0        0        0     6203 2023-04-20 00:32:02.529127 twb_project-1.0.0/twb/utils.py
--rw-r--r--   0        0        0     5878 2023-05-05 14:46:34.743706 twb_project-1.0.0/twb/warehouse.py
--rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 twb_project-1.0.0/setup.py
--rw-r--r--   0        0        0     2590 1970-01-01 00:00:00.000000 twb_project-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    18092 2023-02-26 13:10:42.136159 twb_project-1.0.1a0/LICENSE
+-rw-r--r--   0        0        0     1547 2023-05-21 20:04:40.510524 twb_project-1.0.1a0/README.md
+-rw-r--r--   0        0        0      791 2023-05-21 22:13:19.964052 twb_project-1.0.1a0/pyproject.toml
+-rw-r--r--   0        0        0      143 2023-05-07 20:45:45.325589 twb_project-1.0.1a0/twb/__init__.py
+-rw-r--r--   0        0        0    17182 2023-05-21 22:12:03.290444 twb_project-1.0.1a0/twb/builder.py
+-rw-r--r--   0        0        0      227 2023-05-03 04:36:18.661146 twb_project-1.0.1a0/twb/builder_helpers.py
+-rw-r--r--   0        0        0     4614 2023-03-26 18:02:08.247223 twb_project-1.0.1a0/twb/decompressor.py
+-rw-r--r--   0        0        0     3794 2023-04-20 07:59:01.227219 twb_project-1.0.1a0/twb/logger.py
+-rw-r--r--   0        0        0     1817 2023-05-04 17:42:59.712780 twb_project-1.0.1a0/twb/logger_init.py
+-rw-r--r--   0        0        0    10603 2023-05-02 23:19:18.752689 twb_project-1.0.1a0/twb/modifier.py
+-rw-r--r--   0        0        0     9161 2023-04-20 02:54:12.926181 twb_project-1.0.1a0/twb/parallelization.py
+-rw-r--r--   0        0        0     5527 2023-05-02 04:49:02.953589 twb_project-1.0.1a0/twb/reader.py
+-rw-r--r--   0        0        0     6171 2023-05-07 20:45:49.998705 twb_project-1.0.1a0/twb/utils.py
+-rw-r--r--   0        0        0     3869 2023-05-21 22:12:25.266159 twb_project-1.0.1a0/twb/warehouse.py
+-rw-r--r--   0        0        0     2571 1970-01-01 00:00:00.000000 twb_project-1.0.1a0/setup.py
+-rw-r--r--   0        0        0     2574 1970-01-01 00:00:00.000000 twb_project-1.0.1a0/PKG-INFO
```

### Comparing `twb_project-1.0.0/LICENSE` & `twb_project-1.0.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `twb_project-1.0.0/README.md` & `twb_project-1.0.1a0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />
+<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/007bbe1a-fc2b-4135-e9a6-0d8784004c00/HD" alt="TWB" />
 
 # Temporal Wikipedia Blocks (TWB)
 
 Temporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.
 
 The package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.
```

### Comparing `twb_project-1.0.0/pyproject.toml` & `twb_project-1.0.1a0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 [tool.poetry]
 name = "twb-project"
-version = "1.0.0"
+version = "1.0.1a0"
 description = "An unified tool for the research in extracting information from Wikipedia Edit History chunk."
 authors = ["Lingxi Li <hi@lingxi.li>"]
 license = "GNU GPL"
 readme = "README.md"
 packages = [
     { include = "twb" },
 ]
 homepage = "https://twb.lingxi.li/"
 repository = "https://github.com/lilingxi01/twb-project"
-documentation = "https://twb.lingxi.li/docs/"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4"
 py7zr = "^0.20.5"
 xmltodict = "^0.13.0"
 jsonlines = "^3.1.0"
 zstandard = "^0.21.0"
 psutil = "^5.9.5"
-requests = "^2.28.2"
+requests = "^2.30.0"
 beautifulsoup4 = "^4.12.2"
+tqdm = "^4.65.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 
+[tool.poetry.scripts]
+benchmark = "tests.benchmark:main"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `twb_project-1.0.0/twb/decompressor.py` & `twb_project-1.0.1a0/twb/decompressor.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.0.0/twb/logger.py` & `twb_project-1.0.1a0/twb/logger.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.0.0/twb/logger_init.py` & `twb_project-1.0.1a0/twb/logger_init.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.0.0/twb/modifier.py` & `twb_project-1.0.1a0/twb/modifier.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.0.0/twb/parallelization.py` & `twb_project-1.0.1a0/twb/parallelization.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.0.0/twb/reader.py` & `twb_project-1.0.1a0/twb/reader.py`

 * *Files identical despite different names*

### Comparing `twb_project-1.0.0/twb/utils.py` & `twb_project-1.0.1a0/twb/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
+import logging
 import os
 from typing import List, Callable, Union
 import zstandard as zstd
 import py7zr
 import shutil
 import psutil
 from importlib.metadata import version, PackageNotFoundError
 import multiprocessing as mp
 
-from twb.logger import twb_logger
-
 
 def get_curr_version():
     """
     Get the version of the package.
     """
     try:
         return version('twb-project')
@@ -157,32 +156,32 @@
     """
     with open(path, 'r') as f:
         f.seek(position)
         return f.readline()
 
 
 def _rmtree_error_handler(func, path, exc_info):
-    twb_logger.error(f"Error occurred while calling {func.__name__} on {path}")
-    twb_logger.error(f"Error details: {exc_info}")
+    logging.error(f"Error occurred while calling {func.__name__} on {path}")
+    logging.error(f"Error details: {exc_info}")
 
     # TODO: We might be able to attempt to resolve the issue based on exc_info and then retry the operation.
 
 
 def cleanup_dir(path: str, onerror: Union[Callable, None] = _rmtree_error_handler):
     """
     Clean up the directory.
     :param path: the directory path
     :param onerror: the error handler
     """
     if os.path.exists(path):
         try:
             shutil.rmtree(path, onerror=onerror)
         except Exception as e:
-            twb_logger.error(f"Error occurred while removing: {path}. Check next log for details.")
-            twb_logger.error(e)
+            logging.error(f"Error occurred while removing: {path}. Check next log for details.")
+            logging.error(e)
 
 
 def prepare_output_dir(output_dir: str):
     if os.path.exists(output_dir):
         cleanup_dir(output_dir)
     os.makedirs(output_dir)
```

### Comparing `twb_project-1.0.0/setup.py` & `twb_project-1.0.1a0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,29 +8,34 @@
 {'': ['*']}
 
 install_requires = \
 ['beautifulsoup4>=4.12.2,<5.0.0',
  'jsonlines>=3.1.0,<4.0.0',
  'psutil>=5.9.5,<6.0.0',
  'py7zr>=0.20.5,<0.21.0',
- 'requests>=2.28.2,<3.0.0',
+ 'requests>=2.30.0,<3.0.0',
+ 'tqdm>=4.65.0,<5.0.0',
  'xmltodict>=0.13.0,<0.14.0',
  'zstandard>=0.21.0,<0.22.0']
 
+entry_points = \
+{'console_scripts': ['benchmark = tests.benchmark:main']}
+
 setup_kwargs = {
     'name': 'twb-project',
-    'version': '1.0.0',
+    'version': '1.0.1a0',
     'description': 'An unified tool for the research in extracting information from Wikipedia Edit History chunk.',
-    'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />\n\n# Temporal Wikipedia Blocks (TWB)\n\nTemporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install twb-project\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
+    'long_description': '<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/007bbe1a-fc2b-4135-e9a6-0d8784004c00/HD" alt="TWB" />\n\n# Temporal Wikipedia Blocks (TWB)\n\nTemporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.\n\nThe package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.\n\n## Installation\n\nThe package is available on PyPI and can be installed using pip:\n\n```bash\npip install twb-project\n```\n\n## Benefits\n\n- **Efficient**: The package is designed to be memory-friendly and can be easily parallelized to process large datasets.\n- **Fast**: The package is designed to be fast and can be easily optimized to process large datasets.\n- **Flexible**: The package is designed to be flexible and can be easily extended to support other types of blocks.\n- **Composable**: The package is designed to be composable and can be easily combined with other packages to build other datasets.\n\n## Specification\n\n- Default compression method: ZStandard.\n',
     'author': 'Lingxi Li',
     'author_email': 'hi@lingxi.li',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://twb.lingxi.li/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'entry_points': entry_points,
     'python_requires': '>=3.8,<4',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `twb_project-1.0.0/PKG-INFO` & `twb_project-1.0.1a0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twb-project
-Version: 1.0.0
+Version: 1.0.1a0
 Summary: An unified tool for the research in extracting information from Wikipedia Edit History chunk.
 Home-page: https://twb.lingxi.li/
 License: GNU GPL
 Author: Lingxi Li
 Author-email: hi@lingxi.li
 Requires-Python: >=3.8,<4
 Classifier: License :: Other/Proprietary License
@@ -13,22 +13,22 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: psutil (>=5.9.5,<6.0.0)
 Requires-Dist: py7zr (>=0.20.5,<0.21.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Requires-Dist: zstandard (>=0.21.0,<0.22.0)
-Project-URL: Documentation, https://twb.lingxi.li/docs/
 Project-URL: Repository, https://github.com/lilingxi01/twb-project
 Description-Content-Type: text/markdown
 
-<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/49178640-2f6d-4c23-e56f-a48eca531200/HD" alt="TWB" />
+<img src="https://imagedelivery.net/Dr98IMl5gQ9tPkFM5JRcng/007bbe1a-fc2b-4135-e9a6-0d8784004c00/HD" alt="TWB" />
 
 # Temporal Wikipedia Blocks (TWB)
 
 Temporal Wikipedia Blocks (TWB) is a powerful Python package designed to process the extensive edit history of Wikipedia pages into easily manageable and memory-friendly blocks. The package is specifically developed to enable efficient parallelization and composition of these blocks to facilitate faster processing and analysis of large Wikipedia datasets. The original design of this package is to build other Wikipedia-oriented datasets on top of it.
 
 The package works by dividing the Wikipedia edit history into temporal blocks, which are essentially subsets of the complete dataset that are based on time intervals. These blocks can then be easily processed and analyzed without the need to load the entire dataset into memory.
```

