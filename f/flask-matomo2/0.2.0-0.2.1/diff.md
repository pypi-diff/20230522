# Comparing `tmp/flask_matomo2-0.2.0.tar.gz` & `tmp/flask_matomo2-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_matomo2-0.2.0.tar", max compression
+gzip compressed data, was "flask_matomo2-0.2.1.tar", max compression
```

## Comparing `flask_matomo2-0.2.0.tar` & `flask_matomo2-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-05-15 10:56:36.633278 flask_matomo2-0.2.0/LICENSE
--rw-r--r--   0        0        0     4473 2023-05-22 08:19:15.716732 flask_matomo2-0.2.0/README.md
--rw-r--r--   0        0        0      176 2023-05-16 11:48:09.342069 flask_matomo2-0.2.0/flask_matomo/__init__.py
--rw-r--r--   0        0        0     8723 2023-05-22 08:20:03.780851 flask_matomo2-0.2.0/flask_matomo/core.py
--rw-r--r--   0        0        0     1057 2023-05-22 08:20:46.828179 flask_matomo2-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5422 1970-01-01 00:00:00.000000 flask_matomo2-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-15 10:56:36.633278 flask_matomo2-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4491 2023-05-22 08:28:32.297042 flask_matomo2-0.2.1/README.md
+-rw-r--r--   0        0        0      114 2023-05-22 08:27:37.428989 flask_matomo2-0.2.1/flask_matomo2/__init__.py
+-rw-r--r--   0        0        0     8650 2023-05-22 08:31:03.560264 flask_matomo2-0.2.1/flask_matomo2/core.py
+-rw-r--r--   0        0        0     1250 2023-05-22 08:32:23.265051 flask_matomo2-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     5628 1970-01-01 00:00:00.000000 flask_matomo2-0.2.1/PKG-INFO
```

### Comparing `flask_matomo2-0.2.0/LICENSE` & `flask_matomo2-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_matomo2-0.2.0/README.md` & `flask_matomo2-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 pip install flask-matomo
 ```
 
 ## Usage
 
 ```python
 from flask import Flask, jsonify
-from flask_matomo import *
+from flask_matomo2 import Matomo
 
 app = Flask(__name__)
 matomo = Matomo(app, matomo_url="https://matomo.mydomain.com",
                 id_site=5, token_auth="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX")
 
 @app.route("/")
 def index():
@@ -41,15 +41,15 @@
 
 ### Adding details to route
 
 You can provide details to a route in 2 ways, first by using the `matomo.details` decorator:
 
 ```python
 from flask import Flask, jsonify
-from flask_matomo import *
+from flask_matomo2 import Matomo
 
 app = Flask(__name__)
 matomo = Matomo(app, matomo_url="https://matomo.mydomain.com",
                 id_site=5, token_auth="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX")
 
 @app.route("/foo")
 @matomo.details(action_name="Foo")
@@ -59,15 +59,15 @@
 if __name__ == "__main__":
   app.run()
 ```
 
 or by giving details to the Matomo constructor:
 ```python
 from flask import Flask, jsonify
-from flask_matomo import *
+from flask_matomo2 import Matomo
 
 app = Flask(__name__)
 matomo = Matomo(
   app,
   matomo_url="https://matomo.mydomain.com",
   id_site=5,
   token_auth="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
```

### Comparing `flask_matomo2-0.2.0/flask_matomo/core.py` & `flask_matomo2-0.2.1/flask_matomo2/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 import json
 import logging
 import random
 import re
 import time
 import typing
 import urllib.parse
-from threading import Thread
 
 import flask
 import httpx
-from flask import current_app, g, request
+from flask import g, request
 
-from flask_matomo import MatomoError
-
-logger = logging.getLogger("flask_matomo")
+logger = logging.getLogger("flask_matomo2")
 
 
 class Matomo:
     """The Matomo object provides the central interface for interacting with Matomo.
 
     Parameters
     ----------
@@ -135,35 +132,35 @@
         if self.routes_details.get(action_name) and self.routes_details.get(action_name, {}).get(
             "action_name"
         ):
             data["action_name"] = self.routes_details.get(action_name, {}).get("action_name")
 
         # Create new thread with request, because otherwise the original request will be blocked
         # Thread(target=self.track, kwargs=keyword_arguments).start()
-        g.flask_matomo = {
+        g.flask_matomo2 = {
             "tracking": True,
             "start_ns": time.perf_counter_ns(),
             "tracking_data": data,
         }
 
     def after_request(self, response: flask.Response):
         """Collect tracking data about current request."""
-        tracking_state = g.get("flask_matomo", {})
+        tracking_state = g.get("flask_matomo2", {})
         if not tracking_state.get("tracking", False):
             return response
 
         end_ns = time.perf_counter_ns()
-        gt_ms = (end_ns - g.flask_matomo["start_ns"]) / 1000
-        g.flask_matomo["tracking_data"]["gt_ms"] = gt_ms
-        g.flask_matomo["tracking_data"]["cvar"]["http_status_code"] = response.status_code
+        gt_ms = (end_ns - g.flask_matomo2["start_ns"]) / 1000
+        g.flask_matomo2["tracking_data"]["gt_ms"] = gt_ms
+        g.flask_matomo2["tracking_data"]["cvar"]["http_status_code"] = response.status_code
 
         return response
 
     def teardown_request(self, exc: typing.Optional[Exception] = None) -> None:
-        tracking_state = g.get("flask_matomo", {})
+        tracking_state = g.get("flask_matomo2", {})
         if not tracking_state.get("tracking", False):
             return
 
         tracking_data = tracking_state["tracking_data"]
         for key, value in tracking_state.get("custom_tracking_data", {}).items():
             if key == "cvar" and "cvar" in tracking_data:
                 tracking_data["cvar"].update(value)
```

### Comparing `flask_matomo2-0.2.0/pyproject.toml` & `flask_matomo2-0.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 [tool.poetry]
 name = "flask-matomo2"
-version = "0.2.0"
+version = "0.2.1"
 description = "Track requests to your Flask server with Matomo"
 authors = ["Kristoffer Andersson <kristoffer.andersson@gu.se>"]
 license = "MIT"
 readme = "README.md"
-packages = [{include = "flask_matomo"}]
+packages = [{include = "flask_matomo2"}]
 classifiers=[
     "Environment :: Web Environment",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
+homepage = "https://spraakbanken.gu.se"
+repository = "https://github.com/spraakbanken/flask-matomo2"
+
+[tool.poetry.urls]
+"Bug Tracker" = "https://github.com/spraakbanken/flask-matomo2/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Flask = "^2"
 httpx = "^0.24.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `flask_matomo2-0.2.0/PKG-INFO` & `flask_matomo2-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: flask-matomo2
-Version: 0.2.0
+Version: 0.2.1
 Summary: Track requests to your Flask server with Matomo
+Home-page: https://spraakbanken.gu.se
 License: MIT
 Author: Kristoffer Andersson
 Author-email: kristoffer.andersson@gu.se
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -16,14 +17,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Flask (>=2,<3)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Project-URL: Bug Tracker, https://github.com/spraakbanken/flask-matomo2/issues
+Project-URL: Repository, https://github.com/spraakbanken/flask-matomo2
 Description-Content-Type: text/markdown
 
 # Flask-Matomo
 
 ![](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)
 [![PyPI](https://img.shields.io/pypi/v/flask-matomo2.svg?style=flat-square&colorB=dfb317)](https://pypi.org/project/flask-matomo2/)
 <!-- [![Docs](https://img.shields.io/badge/docs-readthedocs-red.svg?style=flat-square)](https://flask-matomo.readthedocs.io) -->
@@ -37,15 +40,15 @@
 pip install flask-matomo
 ```
 
 ## Usage
 
 ```python
 from flask import Flask, jsonify
-from flask_matomo import *
+from flask_matomo2 import Matomo
 
 app = Flask(__name__)
 matomo = Matomo(app, matomo_url="https://matomo.mydomain.com",
                 id_site=5, token_auth="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX")
 
 @app.route("/")
 def index():
@@ -65,15 +68,15 @@
 
 ### Adding details to route
 
 You can provide details to a route in 2 ways, first by using the `matomo.details` decorator:
 
 ```python
 from flask import Flask, jsonify
-from flask_matomo import *
+from flask_matomo2 import Matomo
 
 app = Flask(__name__)
 matomo = Matomo(app, matomo_url="https://matomo.mydomain.com",
                 id_site=5, token_auth="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX")
 
 @app.route("/foo")
 @matomo.details(action_name="Foo")
@@ -83,15 +86,15 @@
 if __name__ == "__main__":
   app.run()
 ```
 
 or by giving details to the Matomo constructor:
 ```python
 from flask import Flask, jsonify
-from flask_matomo import *
+from flask_matomo2 import Matomo
 
 app = Flask(__name__)
 matomo = Matomo(
   app,
   matomo_url="https://matomo.mydomain.com",
   id_site=5,
   token_auth="XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX",
```

