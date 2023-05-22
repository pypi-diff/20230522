# Comparing `tmp/otools-rpc-0.2.4.tar.gz` & `tmp/otools-rpc-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otools-rpc-0.2.4.tar", last modified: Mon May 22 12:57:54 2023, max compression
+gzip compressed data, was "otools-rpc-0.2.5.tar", last modified: Mon May 22 13:48:11 2023, max compression
```

## Comparing `otools-rpc-0.2.4.tar` & `otools-rpc-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 12:57:54.355006 otools-rpc-0.2.4/
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     1074 2023-05-22 09:23:28.000000 otools-rpc-0.2.4/LICENSE.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     2791 2023-05-22 12:57:54.355006 otools-rpc-0.2.4/PKG-INFO
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     2297 2023-05-22 12:57:46.000000 otools-rpc-0.2.4/README.md
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 12:57:54.355006 otools-rpc-0.2.4/otools_rpc/
--rw-rw-r--   0 opennet   (1000) opennet   (1000)        0 2023-05-22 09:21:22.000000 otools-rpc-0.2.4/otools_rpc/__init__.py
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 12:57:54.355006 otools-rpc-0.2.4/otools_rpc/external_api/
--rw-rw-r--   0 opennet   (1000) opennet   (1000)       37 2023-05-22 12:56:56.000000 otools-rpc-0.2.4/otools_rpc/external_api/__init__.py
--rw-rw-r--   0 opennet   (1000) opennet   (1000)      959 2023-05-22 08:31:48.000000 otools-rpc-0.2.4/otools_rpc/external_api/common.py
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     4812 2023-05-22 12:56:56.000000 otools-rpc-0.2.4/otools_rpc/external_api/environment.py
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     6037 2023-05-22 09:13:04.000000 otools-rpc-0.2.4/otools_rpc/external_api/recordset.py
-drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 12:57:54.355006 otools-rpc-0.2.4/otools_rpc.egg-info/
--rw-rw-r--   0 opennet   (1000) opennet   (1000)     2791 2023-05-22 12:57:54.000000 otools-rpc-0.2.4/otools_rpc.egg-info/PKG-INFO
--rw-rw-r--   0 opennet   (1000) opennet   (1000)      368 2023-05-22 12:57:54.000000 otools-rpc-0.2.4/otools_rpc.egg-info/SOURCES.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)        1 2023-05-22 12:57:54.000000 otools-rpc-0.2.4/otools_rpc.egg-info/dependency_links.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)       46 2023-05-22 12:57:54.000000 otools-rpc-0.2.4/otools_rpc.egg-info/requires.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)       11 2023-05-22 12:57:54.000000 otools-rpc-0.2.4/otools_rpc.egg-info/top_level.txt
--rw-rw-r--   0 opennet   (1000) opennet   (1000)       38 2023-05-22 12:57:54.355006 otools-rpc-0.2.4/setup.cfg
--rw-rw-r--   0 opennet   (1000) opennet   (1000)      828 2023-05-22 12:57:46.000000 otools-rpc-0.2.4/setup.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:48:11.495314 otools-rpc-0.2.5/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     1074 2023-05-22 13:36:09.000000 otools-rpc-0.2.5/LICENSE.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     2841 2023-05-22 13:48:11.495314 otools-rpc-0.2.5/PKG-INFO
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)     2348 2023-05-22 13:47:55.000000 otools-rpc-0.2.5/README.md
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:48:11.495314 otools-rpc-0.2.5/otools_rpc/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:36:09.000000 otools-rpc-0.2.5/otools_rpc/__init__.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:48:11.495314 otools-rpc-0.2.5/otools_rpc/external_api/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       37 2023-05-22 13:36:09.000000 otools-rpc-0.2.5/otools_rpc/external_api/__init__.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)      959 2023-05-22 13:36:09.000000 otools-rpc-0.2.5/otools_rpc/external_api/common.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     4812 2023-05-22 13:47:55.000000 otools-rpc-0.2.5/otools_rpc/external_api/environment.py
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     6037 2023-05-22 13:36:09.000000 otools-rpc-0.2.5/otools_rpc/external_api/recordset.py
+drwxrwxr-x   0 opennet   (1000) opennet   (1000)        0 2023-05-22 13:48:11.495314 otools-rpc-0.2.5/otools_rpc.egg-info/
+-rw-r--r--   0 opennet   (1000) opennet   (1000)     2841 2023-05-22 13:48:11.000000 otools-rpc-0.2.5/otools_rpc.egg-info/PKG-INFO
+-rw-r--r--   0 opennet   (1000) opennet   (1000)      368 2023-05-22 13:48:11.000000 otools-rpc-0.2.5/otools_rpc.egg-info/SOURCES.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)        1 2023-05-22 13:48:11.000000 otools-rpc-0.2.5/otools_rpc.egg-info/dependency_links.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       46 2023-05-22 13:48:11.000000 otools-rpc-0.2.5/otools_rpc.egg-info/requires.txt
+-rw-r--r--   0 opennet   (1000) opennet   (1000)       11 2023-05-22 13:48:11.000000 otools-rpc-0.2.5/otools_rpc.egg-info/top_level.txt
+-rw-rw-r--   0 opennet   (1000) opennet   (1000)       38 2023-05-22 13:48:11.495314 otools-rpc-0.2.5/setup.cfg
+-rw-r--r--   0 opennet   (1000) opennet   (1000)      828 2023-05-22 13:47:55.000000 otools-rpc-0.2.5/setup.py
```

### Comparing `otools-rpc-0.2.4/LICENSE.txt` & `otools-rpc-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `otools-rpc-0.2.4/PKG-INFO` & `otools-rpc-0.2.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otools-rpc
-Version: 0.2.4
+Version: 0.2.5
 Summary: A tool to interact with Odoo's external API.
 Home-page: https://github.com/MrFaBemol/otools-rpc
 Author: Gautier Casabona
 Author-email: gcasabona.pro@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # otools-rpc
 
-[![Version](https://img.shields.io/badge/version-0.2.4-blue.svg)](https://pypi.org/project/otools-rpc/)
+[![Version](https://img.shields.io/badge/version-0.2.5-blue.svg)](https://pypi.org/project/otools-rpc/)
 [![Status](https://img.shields.io/badge/status-alpha-orange.svg)](https://pypi.org/project/otools-rpc/)
 
 otools-rpc is a Python package for interacting with the Odoo ERP system through XML-RPC requests. It provides a convenient way to communicate with Odoo and perform various operations. Please note that the package is currently in the testing/alpha phase, and further improvements and updates are expected.
 
 ## Features
 
 [//]: # (### Environnement Class)
@@ -36,26 +36,28 @@
 
 You can install otools-rpc using pip:
 
 ```console
 $ pip install otools-rpc
 ```
 
+See on pypi: https://pypi.org/project/otools-rpc/
+
 ## Usage
 Here are some examples of how to use otools-rpc to interact with the Odoo ERP system via the external API:
 
 ```python
-from otools_rpc.external_api import Environnement
+from otools_rpc.external_api import Environment
 
 url = "http://localhost:8069/"
 username = "admin"
 password = "admin"
 
 # Create an instance of the environment
-env = Environnement(url, username, password, db='my_odoo')
+env = Environment(url, username, password, db='my_odoo')
 env = env.with_context(lang='en_US')
 print(env)
 
 # Example: Create an invoice for a specific partner
 partner_id = env['res.partner'].search([('name', '=', 'Mitchell Admin')], limit=1)
 invoice_vals = {
     'partner_id': partner_id.id,
@@ -77,8 +79,8 @@
 invoice_id = env['account.move'].create(invoice_vals)
 print("Created invoice:", invoice_id)
 
 # Posting the invoice
 invoice_id.action_post()
 ```
 
-More details are coming soon
+More details are coming soon...
```

### Comparing `otools-rpc-0.2.4/README.md` & `otools-rpc-0.2.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # otools-rpc
 
-[![Version](https://img.shields.io/badge/version-0.2.4-blue.svg)](https://pypi.org/project/otools-rpc/)
+[![Version](https://img.shields.io/badge/version-0.2.5-blue.svg)](https://pypi.org/project/otools-rpc/)
 [![Status](https://img.shields.io/badge/status-alpha-orange.svg)](https://pypi.org/project/otools-rpc/)
 
 otools-rpc is a Python package for interacting with the Odoo ERP system through XML-RPC requests. It provides a convenient way to communicate with Odoo and perform various operations. Please note that the package is currently in the testing/alpha phase, and further improvements and updates are expected.
 
 ## Features
 
 [//]: # (### Environnement Class)
@@ -20,26 +20,28 @@
 
 You can install otools-rpc using pip:
 
 ```console
 $ pip install otools-rpc
 ```
 
+See on pypi: https://pypi.org/project/otools-rpc/
+
 ## Usage
 Here are some examples of how to use otools-rpc to interact with the Odoo ERP system via the external API:
 
 ```python
-from otools_rpc.external_api import Environnement
+from otools_rpc.external_api import Environment
 
 url = "http://localhost:8069/"
 username = "admin"
 password = "admin"
 
 # Create an instance of the environment
-env = Environnement(url, username, password, db='my_odoo')
+env = Environment(url, username, password, db='my_odoo')
 env = env.with_context(lang='en_US')
 print(env)
 
 # Example: Create an invoice for a specific partner
 partner_id = env['res.partner'].search([('name', '=', 'Mitchell Admin')], limit=1)
 invoice_vals = {
     'partner_id': partner_id.id,
@@ -61,8 +63,8 @@
 invoice_id = env['account.move'].create(invoice_vals)
 print("Created invoice:", invoice_id)
 
 # Posting the invoice
 invoice_id.action_post()
 ```
 
-More details are coming soon
+More details are coming soon...
```

### Comparing `otools-rpc-0.2.4/otools_rpc/external_api/common.py` & `otools-rpc-0.2.5/otools_rpc/external_api/common.py`

 * *Files identical despite different names*

### Comparing `otools-rpc-0.2.4/otools_rpc/external_api/environment.py` & `otools-rpc-0.2.5/otools_rpc/external_api/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     def with_context(self, **kw):
         self._context = self._context | kw
         return self
 
 
     def log_request(self, recordset, *args, **kwargs):
         # Todo: add more infos about performance.
-        self.logger.debug(f"Executing {args[0]} on {recordset} with args: {args[1:]} / kwargs: {kwargs}")
+        self.logger.trace(f"Executing {args[0]} on {recordset} with args: {args[1:]} / kwargs: {kwargs}")
         self.requests.append({
             'model': recordset._name,
             'method': args[0],
             'args': args[1:],
             'kwargs': kwargs
         })
```

### Comparing `otools-rpc-0.2.4/otools_rpc/external_api/recordset.py` & `otools-rpc-0.2.5/otools_rpc/external_api/recordset.py`

 * *Files identical despite different names*

### Comparing `otools-rpc-0.2.4/otools_rpc.egg-info/PKG-INFO` & `otools-rpc-0.2.5/otools_rpc.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otools-rpc
-Version: 0.2.4
+Version: 0.2.5
 Summary: A tool to interact with Odoo's external API.
 Home-page: https://github.com/MrFaBemol/otools-rpc
 Author: Gautier Casabona
 Author-email: gcasabona.pro@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -12,15 +12,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # otools-rpc
 
-[![Version](https://img.shields.io/badge/version-0.2.4-blue.svg)](https://pypi.org/project/otools-rpc/)
+[![Version](https://img.shields.io/badge/version-0.2.5-blue.svg)](https://pypi.org/project/otools-rpc/)
 [![Status](https://img.shields.io/badge/status-alpha-orange.svg)](https://pypi.org/project/otools-rpc/)
 
 otools-rpc is a Python package for interacting with the Odoo ERP system through XML-RPC requests. It provides a convenient way to communicate with Odoo and perform various operations. Please note that the package is currently in the testing/alpha phase, and further improvements and updates are expected.
 
 ## Features
 
 [//]: # (### Environnement Class)
@@ -36,26 +36,28 @@
 
 You can install otools-rpc using pip:
 
 ```console
 $ pip install otools-rpc
 ```
 
+See on pypi: https://pypi.org/project/otools-rpc/
+
 ## Usage
 Here are some examples of how to use otools-rpc to interact with the Odoo ERP system via the external API:
 
 ```python
-from otools_rpc.external_api import Environnement
+from otools_rpc.external_api import Environment
 
 url = "http://localhost:8069/"
 username = "admin"
 password = "admin"
 
 # Create an instance of the environment
-env = Environnement(url, username, password, db='my_odoo')
+env = Environment(url, username, password, db='my_odoo')
 env = env.with_context(lang='en_US')
 print(env)
 
 # Example: Create an invoice for a specific partner
 partner_id = env['res.partner'].search([('name', '=', 'Mitchell Admin')], limit=1)
 invoice_vals = {
     'partner_id': partner_id.id,
@@ -77,8 +79,8 @@
 invoice_id = env['account.move'].create(invoice_vals)
 print("Created invoice:", invoice_id)
 
 # Posting the invoice
 invoice_id.action_post()
 ```
 
-More details are coming soon
+More details are coming soon...
```

### Comparing `otools-rpc-0.2.4/setup.py` & `otools-rpc-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="otools-rpc",
-    version="0.2.4",
+    version="0.2.5",
     description="A tool to interact with Odoo's external API.",
     packages=find_packages(exclude=["tests"]),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MrFaBemol/otools-rpc",
     author="Gautier Casabona",
     author_email="gcasabona.pro@gmail.com",
```

