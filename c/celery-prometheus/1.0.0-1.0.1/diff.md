# Comparing `tmp/celery_prometheus-1.0.0.tar.gz` & `tmp/celery_prometheus-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celery_prometheus-1.0.0.tar", max compression
+gzip compressed data, was "celery_prometheus-1.0.1.tar", max compression
```

## Comparing `celery_prometheus-1.0.0.tar` & `celery_prometheus-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1494 2023-03-07 08:50:46.497950 celery_prometheus-1.0.0/LICENSE
--rw-r--r--   0        0        0     2443 2023-03-08 10:13:51.239360 celery_prometheus-1.0.0/README.md
--rw-r--r--   0        0        0      677 2023-03-08 10:19:12.101502 celery_prometheus-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      250 2023-03-03 18:22:42.131998 celery_prometheus-1.0.0/src/celery_prometheus/__init__.py
--rw-r--r--   0        0        0     2040 2023-03-08 09:52:16.463608 celery_prometheus-1.0.0/src/celery_prometheus/prometheus_bootstep.py
--rw-r--r--   0        0        0        0 2023-03-03 16:11:01.458612 celery_prometheus-1.0.0/src/celery_prometheus/py.typed
--rw-r--r--   0        0        0     3220 1970-01-01 00:00:00.000000 celery_prometheus-1.0.0/setup.py
--rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 celery_prometheus-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1494 2023-03-06 13:47:40.505128 celery_prometheus-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2443 2023-05-22 08:49:38.167956 celery_prometheus-1.0.1/README.md
+-rw-r--r--   0        0        0      677 2023-05-22 11:21:32.784290 celery_prometheus-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      250 2023-05-22 08:49:38.167956 celery_prometheus-1.0.1/src/celery_prometheus/__init__.py
+-rw-r--r--   0        0        0     2088 2023-05-22 11:21:01.117187 celery_prometheus-1.0.1/src/celery_prometheus/prometheus_bootstep.py
+-rw-r--r--   0        0        0        0 2023-05-22 08:49:38.167956 celery_prometheus-1.0.1/src/celery_prometheus/py.typed
+-rw-r--r--   0        0        0     3081 1970-01-01 00:00:00.000000 celery_prometheus-1.0.1/PKG-INFO
```

### Comparing `celery_prometheus-1.0.0/LICENSE` & `celery_prometheus-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `celery_prometheus-1.0.0/README.md` & `celery_prometheus-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `celery_prometheus-1.0.0/pyproject.toml` & `celery_prometheus-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "celery-prometheus"
-version = "1.0.0"
+version = "1.0.1"
 description = "Celery with your own prometheus metrics"
 authors = ["Guillaume Gauvrit <guillaume@gandi.net>"]
 readme = "README.md"
 license = "BSD-Derived"
 
 [tool.poetry.dependencies]
 python = "^3.7"
```

### Comparing `celery_prometheus-1.0.0/src/celery_prometheus/prometheus_bootstep.py` & `celery_prometheus-1.0.1/src/celery_prometheus/prometheus_bootstep.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Helper for celery."""
 import logging
 from argparse import ArgumentParser
 from typing import Any, Mapping, Optional, cast
 
 from celery import VERSION as celery_version  # type: ignore
 from celery import Celery
-from prometheus_client import REGISTRY, start_http_server
+from prometheus_client import CollectorRegistry, start_http_server
 from prometheus_client.multiprocess import MultiProcessCollector
 
 log = logging.getLogger(__name__)
 
 
 if celery_version.major < 5:
     from celery.signals import user_preload_options  # type: ignore
@@ -49,11 +49,12 @@
         app.steps["worker"].add(PrometheusBootstep)
 
 
 def attach_prometheus_registry(app: Celery, prometheus_addr: Optional[str]) -> None:
     """Celery loader based on yaml file."""
 
     if prometheus_addr:
-        MultiProcessCollector(REGISTRY)
+        registry = CollectorRegistry()
+        MultiProcessCollector(registry)
         prom_addr, prom_port = prometheus_addr.rsplit(":")
         port = int(prom_port)
-        start_http_server(port, prom_addr, REGISTRY)
+        start_http_server(port, prom_addr, registry)
```

### Comparing `celery_prometheus-1.0.0/setup.py` & `celery_prometheus-1.0.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,95 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: celery-prometheus
+Version: 1.0.1
+Summary: Celery with your own prometheus metrics
+License: BSD-Derived
+Author: Guillaume Gauvrit
+Author-email: guillaume@gandi.net
+Requires-Python: >=3.7,<4.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: celery (>=4)
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Celery Prometheus
 
-packages = \
-['celery_prometheus']
+This module expose the Prometheus HTTP server to expose metrics of your Celery backends.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['celery>=4']
-
-setup_kwargs = {
-    'name': 'celery-prometheus',
-    'version': '1.0.0',
-    'description': 'Celery with your own prometheus metrics',
-    'long_description': "# Celery Prometheus\n\nThis module expose the Prometheus HTTP server to expose metrics of your Celery backends.\n\nTo install `celery-prometheus` with pip, use the command:\n\n```\npip install celery-prometheus\n```\n\nWith Poetry:\n\n```\npoetry add celery-prometheus\n```\n\n## Usage\n\nTo setup `celery-prometheus` to your backend, simply call the method `add_prometheus_option`\nafter the init of the `Celery` object.\n\nExample:\n\n```python\n\nfrom celery import Celery\nfrom celery_prometheus import add_prometheus_option\n\napp = Celery()\nadd_prometheus_option(app)\n\n# Rest of your code ...\n\n```\n\nBefore starting your backend, you will need to expose the `PROMETHEUS_MULTIPROC_DIR` environment\nvariable to indicate which folder the Prometheus Client will use to store the metrics\n(see [Multiprocess Mode (E.g. Gunicorn) of the Promehteus Client documentation](https://github.com/prometheus/client_python#multiprocess-mode-eg-gunicorn)).\n\nTo start and expose the Prometheus HTTP Server, you need to use the `--prometheus-collector-addr`\nargument when starting your Celery backend:\n\n```bash\nexport PROMETHEUS_MULTIPROC_DIR=/var/cache/my_celery_app\ncelery worker -A my_celery_backend.backend --prometheus-collector-addr 0.0.0.0:6543\n```\n\nNow that your backend is started, you can configure your Prometheus scrappers to scrappe your\nCelery backend.\n\n## Contributions\n\nThis project is open to external contributions. Feel free to submit us a\n[Pull request](https://github.com/Gandi/celery-prometheus/pulls) if you want to contribute and\nimprove with us this project.\n\nIn order to maintain an overall good code quality, this project use the following tools:\n\n - [Black](https://github.com/psf/black)\n - [Isort](https://github.com/PyCQA/isort)\n - [Flake8](https://flake8.pycqa.org/en/latest/)\n\nLinting and formatting tools are configured to match the [current default rules of Black](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html).\n\nWe also use [Mypy](https://mypy.readthedocs.io/en/stable/) as a static type checker.\n\nPlease ensure to run these tools before commiting and submiting a Pull request. In case one of\nthese mentionned tools report an error, the CI will automatically fail.\n\nIf you're making your first contribution to this project, please add your name to the\n[contributors list](CONTRIBUTORS.txt).\n\n## License\n\nThis project is released by [Gandi.net](https://www.gandi.net/en) tech team under the\n[BSD-3 license](LICENSE).\n",
-    'author': 'Guillaume Gauvrit',
-    'author_email': 'guillaume@gandi.net',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+To install `celery-prometheus` with pip, use the command:
 
+```
+pip install celery-prometheus
+```
+
+With Poetry:
+
+```
+poetry add celery-prometheus
+```
+
+## Usage
+
+To setup `celery-prometheus` to your backend, simply call the method `add_prometheus_option`
+after the init of the `Celery` object.
+
+Example:
+
+```python
+
+from celery import Celery
+from celery_prometheus import add_prometheus_option
+
+app = Celery()
+add_prometheus_option(app)
+
+# Rest of your code ...
+
+```
+
+Before starting your backend, you will need to expose the `PROMETHEUS_MULTIPROC_DIR` environment
+variable to indicate which folder the Prometheus Client will use to store the metrics
+(see [Multiprocess Mode (E.g. Gunicorn) of the Promehteus Client documentation](https://github.com/prometheus/client_python#multiprocess-mode-eg-gunicorn)).
+
+To start and expose the Prometheus HTTP Server, you need to use the `--prometheus-collector-addr`
+argument when starting your Celery backend:
+
+```bash
+export PROMETHEUS_MULTIPROC_DIR=/var/cache/my_celery_app
+celery worker -A my_celery_backend.backend --prometheus-collector-addr 0.0.0.0:6543
+```
+
+Now that your backend is started, you can configure your Prometheus scrappers to scrappe your
+Celery backend.
+
+## Contributions
+
+This project is open to external contributions. Feel free to submit us a
+[Pull request](https://github.com/Gandi/celery-prometheus/pulls) if you want to contribute and
+improve with us this project.
+
+In order to maintain an overall good code quality, this project use the following tools:
+
+ - [Black](https://github.com/psf/black)
+ - [Isort](https://github.com/PyCQA/isort)
+ - [Flake8](https://flake8.pycqa.org/en/latest/)
+
+Linting and formatting tools are configured to match the [current default rules of Black](https://black.readthedocs.io/en/stable/the_black_code_style/current_style.html).
+
+We also use [Mypy](https://mypy.readthedocs.io/en/stable/) as a static type checker.
+
+Please ensure to run these tools before commiting and submiting a Pull request. In case one of
+these mentionned tools report an error, the CI will automatically fail.
+
+If you're making your first contribution to this project, please add your name to the
+[contributors list](CONTRIBUTORS.txt).
+
+## License
+
+This project is released by [Gandi.net](https://www.gandi.net/en) tech team under the
+[BSD-3 license](LICENSE).
 
-setup(**setup_kwargs)
```

