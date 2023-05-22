# Comparing `tmp/metroid-1.2.4.tar.gz` & `tmp/metroid-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metroid-1.2.4.tar", max compression
+gzip compressed data, was "metroid-1.3.0.tar", max compression
```

## Comparing `metroid-1.2.4.tar` & `metroid-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1068 2022-02-02 16:12:02.238015 metroid-1.2.4/LICENSE
--rw-r--r--   0        0        0     6176 2022-02-02 16:12:02.238015 metroid-1.2.4/README.md
--rw-r--r--   0        0        0      258 2022-02-02 16:12:02.238015 metroid-1.2.4/metroid/__init__.py
--rw-r--r--   0        0        0     4666 2022-02-02 16:12:02.238015 metroid-1.2.4/metroid/admin.py
--rw-r--r--   0        0        0      255 2022-02-02 16:12:02.238015 metroid-1.2.4/metroid/apps.py
--rw-r--r--   0        0        0     1948 2022-02-02 16:12:02.238015 metroid-1.2.4/metroid/celery.py
--rw-r--r--   0        0        0     7998 2022-02-02 16:12:02.238015 metroid-1.2.4/metroid/config.py
--rw-r--r--   0        0        0        0 2022-02-02 16:12:02.238015 metroid-1.2.4/metroid/management/__init__.py
--rw-r--r--   0        0        0        0 2022-02-02 16:12:02.238015 metroid-1.2.4/metroid/management/commands/__init__.py
--rw-r--r--   0        0        0     2579 2022-02-02 16:12:02.238015 metroid-1.2.4/metroid/management/commands/metroid.py
--rw-r--r--   0        0        0      936 2022-02-02 16:12:02.242015 metroid-1.2.4/metroid/migrations/0001_initial.py
--rw-r--r--   0        0        0      903 2022-02-02 16:12:02.242015 metroid-1.2.4/metroid/migrations/0002_failedpublishmessage.py
--rw-r--r--   0        0        0        0 2022-02-02 16:12:02.242015 metroid-1.2.4/metroid/migrations/__init__.py
--rw-r--r--   0        0        0     1265 2022-02-02 16:12:02.242015 metroid-1.2.4/metroid/models.py
--rw-r--r--   0        0        0     2732 2022-02-02 16:12:02.242015 metroid-1.2.4/metroid/publish.py
--rw-r--r--   0        0        0        0 2022-02-02 16:12:02.242015 metroid-1.2.4/metroid/py.typed
--rw-r--r--   0        0        0     1704 2022-02-02 16:12:02.242015 metroid-1.2.4/metroid/republish.py
--rw-r--r--   0        0        0     1832 2022-02-02 16:12:02.242015 metroid-1.2.4/metroid/rq.py
--rw-r--r--   0        0        0     4641 2022-02-02 16:12:02.242015 metroid-1.2.4/metroid/subscribe.py
--rw-r--r--   0        0        0      527 2022-02-02 16:12:02.242015 metroid-1.2.4/metroid/typing.py
--rw-r--r--   0        0        0      754 2022-02-02 16:12:02.242015 metroid-1.2.4/metroid/utils.py
--rw-r--r--   0        0        0     2469 2022-02-02 16:12:02.242015 metroid-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     7222 2022-02-02 16:12:12.084890 metroid-1.2.4/setup.py
--rw-r--r--   0        0        0     7579 2022-02-02 16:12:12.085458 metroid-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-22 10:52:04.011420 metroid-1.3.0/LICENSE
+-rw-r--r--   0        0        0     6176 2023-05-22 10:52:04.011420 metroid-1.3.0/README.md
+-rw-r--r--   0        0        0      258 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/__init__.py
+-rw-r--r--   0        0        0     4666 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/admin.py
+-rw-r--r--   0        0        0      255 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/apps.py
+-rw-r--r--   0        0        0     1948 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/celery.py
+-rw-r--r--   0        0        0     7978 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/config.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/management/commands/__init__.py
+-rw-r--r--   0        0        0     2579 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/management/commands/metroid.py
+-rw-r--r--   0        0        0      936 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/migrations/0001_initial.py
+-rw-r--r--   0        0        0      903 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/migrations/0002_failedpublishmessage.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/migrations/__init__.py
+-rw-r--r--   0        0        0     1265 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/models.py
+-rw-r--r--   0        0        0     2732 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/publish.py
+-rw-r--r--   0        0        0        0 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/py.typed
+-rw-r--r--   0        0        0     1705 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/republish.py
+-rw-r--r--   0        0        0     1832 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/rq.py
+-rw-r--r--   0        0        0     4641 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/subscribe.py
+-rw-r--r--   0        0        0      527 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/typing.py
+-rw-r--r--   0        0        0      754 2023-05-22 10:52:04.015420 metroid-1.3.0/metroid/utils.py
+-rw-r--r--   0        0        0     2490 2023-05-22 10:52:04.015420 metroid-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7720 1970-01-01 00:00:00.000000 metroid-1.3.0/PKG-INFO
```

### Comparing `metroid-1.2.4/LICENSE` & `metroid-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metroid-1.2.4/README.md` & `metroid-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `metroid-1.2.4/metroid/admin.py` & `metroid-1.3.0/metroid/admin.py`

 * *Files identical despite different names*

### Comparing `metroid-1.2.4/metroid/celery.py` & `metroid-1.3.0/metroid/celery.py`

 * *Files identical despite different names*

### Comparing `metroid-1.2.4/metroid/config.py` & `metroid-1.3.0/metroid/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Callable, List, Optional, Union
+from typing import Callable, List, Optional
 
 from django.conf import settings as django_settings
 from django.core.exceptions import ImproperlyConfigured
 from django.utils.module_loading import import_string
 
 from metroid.typing import MetroidSettings, Subscription, TopicPublishSettings
 
@@ -71,15 +71,15 @@
     @property
     def worker_type(self) -> str:
         """
         Returns the worker type.
         """
         return self.settings.get('worker_type', 'celery')
 
-    def get_x_metro_key(self, *, topic_name: str) -> Union[str, None]:
+    def get_x_metro_key(self, *, topic_name: str) -> str:
         """
         Fetches the x-metro-key based on topic
         """
         for topic in self.publish_settings:
             if topic['topic_name'] == topic_name:
                 return topic['x_metro_key']
         logger.critical('Unable to find a x-metro-key for %s', topic_name)
```

### Comparing `metroid-1.2.4/metroid/management/commands/metroid.py` & `metroid-1.3.0/metroid/management/commands/metroid.py`

 * *Files identical despite different names*

### Comparing `metroid-1.2.4/metroid/migrations/0001_initial.py` & `metroid-1.3.0/metroid/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `metroid-1.2.4/metroid/migrations/0002_failedpublishmessage.py` & `metroid-1.3.0/metroid/migrations/0002_failedpublishmessage.py`

 * *Files identical despite different names*

### Comparing `metroid-1.2.4/metroid/models.py` & `metroid-1.3.0/metroid/models.py`

 * *Files identical despite different names*

### Comparing `metroid-1.2.4/metroid/publish.py` & `metroid-1.3.0/metroid/publish.py`

 * *Files identical despite different names*

### Comparing `metroid-1.2.4/metroid/republish.py` & `metroid-1.3.0/metroid/republish.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 logger = logging.getLogger('metroid')
 
 
 def retry_failed_published_events() -> None:
     """
     Trys to publish all previously failed messages again.
 
-    It make a wrapper around this function based on your needs. If you implement posting to Metro at the end
+    It makes a wrapper around this function based on your needs. If you implement posting to Metro at the end
     of your API logic you might want to still return a 200 to the API user, even if a post to Metro should fail.
 
     :return: None - Metro gives empty response on valid posts
     :raises: requests.exceptions.HTTPError
     """
     for message in FailedPublishMessage.objects.all():
         formatted_data = {
```

### Comparing `metroid-1.2.4/metroid/rq.py` & `metroid-1.3.0/metroid/rq.py`

 * *Files identical despite different names*

### Comparing `metroid-1.2.4/metroid/subscribe.py` & `metroid-1.3.0/metroid/subscribe.py`

 * *Files identical despite different names*

### Comparing `metroid-1.2.4/metroid/typing.py` & `metroid-1.3.0/metroid/typing.py`

 * *Files identical despite different names*

### Comparing `metroid-1.2.4/metroid/utils.py` & `metroid-1.3.0/metroid/utils.py`

 * *Files identical despite different names*

### Comparing `metroid-1.2.4/pyproject.toml` & `metroid-1.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "metroid"
-version = "1.2.4"  # Remember to change in __init__.py as well
+version = "1.3.0"  # Remember to change in __init__.py as well
 description = "Metroid - Metro for Django"
 authors = ["Jonas Krüger Svensson <jonas.svensson@intility.no>"]
 maintainers = [
     "Ali Arfan <ali.arfan@intility.no>",
     "Ingvald Lorentzen <ingvald.lorentzen@intility.no",
     "Per Anders Stadheim <per.anders.stadheim@intility.no>",
 ]
@@ -29,38 +29,39 @@
     'Topic :: Software Development :: Libraries',
     'Topic :: Software Development :: Libraries :: Application Frameworks',
     'Topic :: Software Development :: Libraries :: Python Modules',
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-azure-servicebus = "^7.4.0"
-Django = "^3.1.1 || ^4.0"
+aiohttp = "^3.8.4"
+azure-servicebus = "^7.10.0"
+Django = "^3.2 || ^4.0"
 django-guid = "^3.2.0"
 
 [tool.poetry.dev-dependencies]
-pre-commit = "^2.9.3"
+pre-commit = "^3.3.2"
 python-decouple = "^3.4"
 redis = "^4.0.0"
-black = "^22.1.0"
-pytest = "^6.2.2"
-pytest-cov = "^3.0.0"
+black = "^23.3.0"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
 pytest-django = "^4.1.0"
-pytest-asyncio = "^0.17.0"
+pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.5.1"
 requests-mock = "^1.8.0"
 pytest-freezegun = "^0.4.2"
-celery = "^5.2.2"
+celery = "^5.3.0rc1"
 django-rq = "^2.4.1"
 redislite = "^6.0.674960"
 
 [tool.black]
 line-length = 120
 skip-string-normalization = true
-target-version = ['py37']
+target-version = ['py38']
 include = '\.pyi?$'
 exclude = '''
 (
     (\.eggs|\.git|\.hg|\.mypy_cache|\.tox|\.venv|\venv|\.github|\docs|\tests|\__pycache__)
 )
 '''
```

### Comparing `metroid-1.2.4/setup.py` & `metroid-1.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,215 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: metroid
+Version: 1.3.0
+Summary: Metroid - Metro for Django
+Home-page: https://github.com/intility/metroid
+Keywords: async,django,servicebus,task,celery,worker,rq
+Author: Jonas Krüger Svensson
+Author-email: jonas.svensson@intility.no
+Maintainer: Ali Arfan
+Maintainer-email: ali.arfan@intility.no
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.1
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: Django (>=3.2,<5.0)
+Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
+Requires-Dist: azure-servicebus (>=7.10.0,<8.0.0)
+Requires-Dist: django-guid (>=3.2.0,<4.0.0)
+Project-URL: Documentation, https://github.com/intility/metroid
+Project-URL: Repository, https://github.com/intility/metroid
+Description-Content-Type: text/markdown
+
+<h1 align="center">
+  <img src=".github/images/intility.png" width="124px"/><br/>
+  Metroid
+</h1>
+
+<p align="center">
+    <em>Subscribe, act, publish.</em>
+</p>
+<p align="center">
+    <a href="https://python.org">
+        <img src="https://img.shields.io/badge/python-v3.9+-blue.svg" alt="Python version">
+    </a>
+    <a href="https://djangoproject.com">
+        <img src="https://img.shields.io/badge/django-3.1.1+%20-blue.svg" alt="Django version">
+    </a>
+    <a href="https://docs.celeryproject.org/en/stable/">
+        <img src="https://img.shields.io/badge/celery-5.0.0+%20-blue.svg" alt="Celery version">
+    </a>
+    <a href="https://github.com/Azure/azure-sdk-for-python/tree/master/sdk/servicebus/azure-servicebus">
+        <img src="https://img.shields.io/badge/azure--servicebus-7.0.1+%20-blue.svg" alt="ServiceBus version">
+    </a>
+    <a href="https://github.com/snok/django-guid/">
+        <img src="https://img.shields.io/badge/django--guid-3.2.0+-blue.svg" alt="Django GUID version">
+    </a>
+</p>
+<p align="center">
+    <a href="https://codecov.io/gh/intility/metroid">
+        <img src="https://codecov.io/gh/intility/metroid/branch/main/graph/badge.svg" alt="Codecov">
+    </a>
+    <a href="https://github.com/pre-commit/pre-commit">
+        <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white" alt="Pre-commit">
+    </a>
+    <a href="https://github.com/psf/black">
+        <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">
+    </a>
+    <a href="http://mypy-lang.org">
+        <img src="http://www.mypy-lang.org/static/mypy_badge.svg" alt="mypy">
+    </a>
+    <a href="https://pycqa.github.io/isort/">
+        <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" alt="isort">
+    </a>
+</p>
+
+
+# Metroid - Metro for Django
+
+This app is intended to streamline integration with Metro for all Django+Celery users by:
+
+* Asynchronous handling of subscriptions and messages with one command
+* Execute Celery tasks based on message topics, defined in `settings.py`
+* Retry failed tasks through your admin dashboard when using the `MetroidTask` base
+
+## Overview
+* `python` >= 3.8
+* `django` >= 3.1.1 - For `asgiref`, settings
+* `django-guid` >= 3.2.0 - Storing correlation IDs for failed tasks in the database, making debugging easy
+* Choose one:
+   * `celery` >= 5.0.0 - Execute tasks based on a subject
+   * `rq` >= 2.4.1 - Execute tasks based on a subject
+
+### Implementation
+
+The `python manage.py metroid` app is fully asynchronous, and has no blocking code. It utilizes `Celery` to execute tasks.
+
+It works by:
+1. Going through all your configured subscriptions and start a new async connection for each one of them
+2. Metro sends messages on the subscriptions
+3. This app filters out messages matching subjects you have defined, and queues a celery task to execute
+   the function as specified for that subject  
+   3.1. If no task is found for that subject, the message is marked as complete
+4. The message is marked as complete after the Celery task has successfully been queued
+5. If the task is failed, an entry is automatically created in your database
+6. All failed tasks can be retried manually through the admin dashboard
+
+
+### Configure and install this package
+
+
+> **_Note_**
+> For a complete example, have a look in `demoproj/settings.py`.
+
+1. Create a `METROID` key in `settings.py` with all your subscriptions and handlers.
+Example settings:
+```python
+METROID = {
+    'subscriptions': [
+        {
+            'topic_name': 'metro-demo',
+            'subscription_name': 'sub-metrodemo-metrodemoerfett',
+            'connection_string': config('CONNECTION_STRING_METRO_DEMO', None),
+            'handlers': [
+               {
+                  'subject': 'MetroDemo/Type/GeekJokes',
+                  'regex': False,
+                  'handler_function': 'demoproj.demoapp.services.my_func'
+                }
+            ],
+        },
+    ],
+   'worker_type': 'celery', # default
+}
+```
+
+The `handler_function` is defined by providing the full dotted path as a string. For example,`from demoproj.demoapp.services import my_func` is provided as `'demoproj.demoapp.services.my_func'`.
+
+The handlers subject can be a regular expression or a string. If a regular expression is provided, the variable regex must be set to True. Example:
+ ```python
+'handlers': [{'subject': r'^MetroDemo/Type/.*$','regex':True,'handler_function': my_func}],
+ ```
+
+
 
-packages = \
-['metroid',
- 'metroid.management',
- 'metroid.management.commands',
- 'metroid.migrations']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['Django>=3.1.1,<5.0',
- 'azure-servicebus>=7.4.0,<8.0.0',
- 'django-guid>=3.2.0,<4.0.0']
-
-setup_kwargs = {
-    'name': 'metroid',
-    'version': '1.2.4',
-    'description': 'Metroid - Metro for Django',
-    'long_description': '<h1 align="center">\n  <img src=".github/images/intility.png" width="124px"/><br/>\n  Metroid\n</h1>\n\n<p align="center">\n    <em>Subscribe, act, publish.</em>\n</p>\n<p align="center">\n    <a href="https://python.org">\n        <img src="https://img.shields.io/badge/python-v3.9+-blue.svg" alt="Python version">\n    </a>\n    <a href="https://djangoproject.com">\n        <img src="https://img.shields.io/badge/django-3.1.1+%20-blue.svg" alt="Django version">\n    </a>\n    <a href="https://docs.celeryproject.org/en/stable/">\n        <img src="https://img.shields.io/badge/celery-5.0.0+%20-blue.svg" alt="Celery version">\n    </a>\n    <a href="https://github.com/Azure/azure-sdk-for-python/tree/master/sdk/servicebus/azure-servicebus">\n        <img src="https://img.shields.io/badge/azure--servicebus-7.0.1+%20-blue.svg" alt="ServiceBus version">\n    </a>\n    <a href="https://github.com/snok/django-guid/">\n        <img src="https://img.shields.io/badge/django--guid-3.2.0+-blue.svg" alt="Django GUID version">\n    </a>\n</p>\n<p align="center">\n    <a href="https://codecov.io/gh/intility/metroid">\n        <img src="https://codecov.io/gh/intility/metroid/branch/main/graph/badge.svg" alt="Codecov">\n    </a>\n    <a href="https://github.com/pre-commit/pre-commit">\n        <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white" alt="Pre-commit">\n    </a>\n    <a href="https://github.com/psf/black">\n        <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Black">\n    </a>\n    <a href="http://mypy-lang.org">\n        <img src="http://www.mypy-lang.org/static/mypy_badge.svg" alt="mypy">\n    </a>\n    <a href="https://pycqa.github.io/isort/">\n        <img src="https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336" alt="isort">\n    </a>\n</p>\n\n\n# Metroid - Metro for Django\n\nThis app is intended to streamline integration with Metro for all Django+Celery users by:\n\n* Asynchronous handling of subscriptions and messages with one command\n* Execute Celery tasks based on message topics, defined in `settings.py`\n* Retry failed tasks through your admin dashboard when using the `MetroidTask` base\n\n## Overview\n* `python` >= 3.8\n* `django` >= 3.1.1 - For `asgiref`, settings\n* `django-guid` >= 3.2.0 - Storing correlation IDs for failed tasks in the database, making debugging easy\n* Choose one:\n   * `celery` >= 5.0.0 - Execute tasks based on a subject\n   * `rq` >= 2.4.1 - Execute tasks based on a subject\n\n### Implementation\n\nThe `python manage.py metroid` app is fully asynchronous, and has no blocking code. It utilizes `Celery` to execute tasks.\n\nIt works by:\n1. Going through all your configured subscriptions and start a new async connection for each one of them\n2. Metro sends messages on the subscriptions\n3. This app filters out messages matching subjects you have defined, and queues a celery task to execute\n   the function as specified for that subject  \n   3.1. If no task is found for that subject, the message is marked as complete\n4. The message is marked as complete after the Celery task has successfully been queued\n5. If the task is failed, an entry is automatically created in your database\n6. All failed tasks can be retried manually through the admin dashboard\n\n\n### Configure and install this package\n\n\n> **_Note_**\n> For a complete example, have a look in `demoproj/settings.py`.\n\n1. Create a `METROID` key in `settings.py` with all your subscriptions and handlers.\nExample settings:\n```python\nMETROID = {\n    \'subscriptions\': [\n        {\n            \'topic_name\': \'metro-demo\',\n            \'subscription_name\': \'sub-metrodemo-metrodemoerfett\',\n            \'connection_string\': config(\'CONNECTION_STRING_METRO_DEMO\', None),\n            \'handlers\': [\n               {\n                  \'subject\': \'MetroDemo/Type/GeekJokes\',\n                  \'regex\': False,\n                  \'handler_function\': \'demoproj.demoapp.services.my_func\'\n                }\n            ],\n        },\n    ],\n   \'worker_type\': \'celery\', # default\n}\n```\n\nThe `handler_function` is defined by providing the full dotted path as a string. For example,`from demoproj.demoapp.services import my_func` is provided as `\'demoproj.demoapp.services.my_func\'`.\n\nThe handlers subject can be a regular expression or a string. If a regular expression is provided, the variable regex must be set to True. Example:\n ```python\n\'handlers\': [{\'subject\': r\'^MetroDemo/Type/.*$\',\'regex\':True,\'handler_function\': my_func}],\n ```\n\n\n\n2. Configure `Django-GUID`  by adding the app to your installed apps, to your middlewares and configuring logging\nas described [here](https://github.com/snok/django-guid#configuration).\nMake sure you enable the [`CeleryIntegration`](https://django-guid.readthedocs.io/en/latest/integrations.html#celery):\n```python\nfrom django_guid.integrations import CeleryIntegration\n\nDJANGO_GUID = {\n    \'INTEGRATIONS\': [\n        CeleryIntegration(\n            use_django_logging=True,\n            log_parent=True,\n        )\n    ],\n}\n```\n\n\n#### Creating your own handler functions\n\nYour functions will be called with keyword arguments for\n\n\n`message`, `topic_name`, `subscription_name` and `subject`. You function should in other words\nlook something like this:\n\n##### Celery\n```python\n@app.task(base=MetroidTask)\ndef my_func(*, message: dict, topic_name: str, subscription_name: str, subject: str) -> None:\n```\n\n##### rq\n```python\ndef my_func(*, message: dict, topic_name: str, subscription_name: str, subject: str) -> None:\n```\n\n\n### Running the project\n1. Ensure you have redis running:\n```bash\ndocker-compose up\n```\n2. Run migrations\n```bash\npython manage.py migrate\n```\n3. Create an admin account\n```bash\npython manage.py createsuperuser\n```\n4. Start a worker:\n```python\ncelery -A demoproj worker -l info\n```\n5. Run the subscriber:\n```python\npython manage.py metroid\n```\n6. Send messages to Metro. Example code can be found in [`demoproj/demoapp/services.py`](demoproj/demoapp/services.py)\n7. Run the webserver:\n```python\npython manage.py runserver 8000\n```\n8. See failed messages under `http://localhost:8080/admin`\n\nTo contribute, please see [`CONTRIBUTING.md`](CONTRIBUTING.md)\n',
-    'author': 'Jonas Krüger Svensson',
-    'author_email': 'jonas.svensson@intility.no',
-    'maintainer': 'Ali Arfan',
-    'maintainer_email': 'ali.arfan@intility.no',
-    'url': 'https://github.com/intility/metroid',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+2. Configure `Django-GUID`  by adding the app to your installed apps, to your middlewares and configuring logging
+as described [here](https://github.com/snok/django-guid#configuration).
+Make sure you enable the [`CeleryIntegration`](https://django-guid.readthedocs.io/en/latest/integrations.html#celery):
+```python
+from django_guid.integrations import CeleryIntegration
+
+DJANGO_GUID = {
+    'INTEGRATIONS': [
+        CeleryIntegration(
+            use_django_logging=True,
+            log_parent=True,
+        )
+    ],
 }
+```
+
+
+#### Creating your own handler functions
+
+Your functions will be called with keyword arguments for
+
+
+`message`, `topic_name`, `subscription_name` and `subject`. You function should in other words
+look something like this:
+
+##### Celery
+```python
+@app.task(base=MetroidTask)
+def my_func(*, message: dict, topic_name: str, subscription_name: str, subject: str) -> None:
+```
+
+##### rq
+```python
+def my_func(*, message: dict, topic_name: str, subscription_name: str, subject: str) -> None:
+```
+
+
+### Running the project
+1. Ensure you have redis running:
+```bash
+docker-compose up
+```
+2. Run migrations
+```bash
+python manage.py migrate
+```
+3. Create an admin account
+```bash
+python manage.py createsuperuser
+```
+4. Start a worker:
+```python
+celery -A demoproj worker -l info
+```
+5. Run the subscriber:
+```python
+python manage.py metroid
+```
+6. Send messages to Metro. Example code can be found in [`demoproj/demoapp/services.py`](demoproj/demoapp/services.py)
+7. Run the webserver:
+```python
+python manage.py runserver 8000
+```
+8. See failed messages under `http://localhost:8080/admin`
 
+To contribute, please see [`CONTRIBUTING.md`](CONTRIBUTING.md)
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,79 +1,82 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['metroid',
-'metroid.management', 'metroid.management.commands', 'metroid.migrations']
-package_data = \ {'': ['*']} install_requires = \ ['Django>=3.1.1,<5.0',
-'azure-servicebus>=7.4.0,<8.0.0', 'django-guid>=3.2.0,<4.0.0'] setup_kwargs =
-{ 'name': 'metroid', 'version': '1.2.4', 'description': 'Metroid - Metro for
-Django', 'long_description': '
-                    ****** \n [.github/images/intility.png]
-                              \n Metroid\n ******
-\n\n
-                         \n Subscribe, act, publish.\n
-\n
-\n \n_[Python_version]\n\n \n_[Django_version]\n\n \n_[Celery_version]\n\n \n_
-             [ServiceBus_version]\n\n \n_[Django_GUID_version]\n\n
-\n
-   \n \n_[Codecov]\n\n \n_[Pre-commit]\n\n \n_[Black]\n\n \n_[mypy]\n\n \n_
-                                  [isort]\n\n
-\n\n\n# Metroid - Metro for Django\n\nThis app is intended to streamline
-integration with Metro for all Django+Celery users by:\n\n* Asynchronous
-handling of subscriptions and messages with one command\n* Execute Celery tasks
-based on message topics, defined in `settings.py`\n* Retry failed tasks through
-your admin dashboard when using the `MetroidTask` base\n\n## Overview\n*
-`python` >= 3.8\n* `django` >= 3.1.1 - For `asgiref`, settings\n* `django-guid`
->= 3.2.0 - Storing correlation IDs for failed tasks in the database, making
-debugging easy\n* Choose one:\n * `celery` >= 5.0.0 - Execute tasks based on a
-subject\n * `rq` >= 2.4.1 - Execute tasks based on a subject\n\n###
-Implementation\n\nThe `python manage.py metroid` app is fully asynchronous, and
-has no blocking code. It utilizes `Celery` to execute tasks.\n\nIt works by:
-\n1. Going through all your configured subscriptions and start a new async
-connection for each one of them\n2. Metro sends messages on the
-subscriptions\n3. This app filters out messages matching subjects you have
-defined, and queues a celery task to execute\n the function as specified for
-that subject \n 3.1. If no task is found for that subject, the message is
-marked as complete\n4. The message is marked as complete after the Celery task
-has successfully been queued\n5. If the task is failed, an entry is
-automatically created in your database\n6. All failed tasks can be retried
-manually through the admin dashboard\n\n\n### Configure and install this
-package\n\n\n> **_Note_**\n> For a complete example, have a look in `demoproj/
-settings.py`.\n\n1. Create a `METROID` key in `settings.py` with all your
-subscriptions and handlers.\nExample settings:\n```python\nMETROID = {\n
-\'subscriptions\': [\n {\n \'topic_name\': \'metro-demo\',\n
-\'subscription_name\': \'sub-metrodemo-metrodemoerfett\',\n
-\'connection_string\': config(\'CONNECTION_STRING_METRO_DEMO\', None),\n
-\'handlers\': [\n {\n \'subject\': \'MetroDemo/Type/GeekJokes\',\n \'regex\':
-False,\n \'handler_function\': \'demoproj.demoapp.services.my_func\'\n }\n ],\n
-},\n ],\n \'worker_type\': \'celery\', # default\n}\n```\n\nThe
-`handler_function` is defined by providing the full dotted path as a string.
-For example,`from demoproj.demoapp.services import my_func` is provided as
-`\'demoproj.demoapp.services.my_func\'`.\n\nThe handlers subject can be a
-regular expression or a string. If a regular expression is provided, the
-variable regex must be set to True. Example:\n ```python\n\'handlers\': [
-{\'subject\': r\'^MetroDemo/Type/.*$\',\'regex\':True,\'handler_function\':
-my_func}],\n ```\n\n\n\n2. Configure `Django-GUID` by adding the app to your
-installed apps, to your middlewares and configuring logging\nas described
-[here](https://github.com/snok/django-guid#configuration).\nMake sure you
-enable the [`CeleryIntegration`](https://django-guid.readthedocs.io/en/latest/
-integrations.html#celery):\n```python\nfrom django_guid.integrations import
-CeleryIntegration\n\nDJANGO_GUID = {\n \'INTEGRATIONS\': [\n CeleryIntegration
-(\n use_django_logging=True,\n log_parent=True,\n )\n ],\n}\n```\n\n\n####
-Creating your own handler functions\n\nYour functions will be called with
-keyword arguments for\n\n\n`message`, `topic_name`, `subscription_name` and
-`subject`. You function should in other words\nlook something like this:
-\n\n##### Celery\n```python\n@app.task(base=MetroidTask)\ndef my_func(*,
-message: dict, topic_name: str, subscription_name: str, subject: str) -> None:
-\n```\n\n##### rq\n```python\ndef my_func(*, message: dict, topic_name: str,
-subscription_name: str, subject: str) -> None:\n```\n\n\n### Running the
-project\n1. Ensure you have redis running:\n```bash\ndocker-compose up\n```\n2.
-Run migrations\n```bash\npython manage.py migrate\n```\n3. Create an admin
-account\n```bash\npython manage.py createsuperuser\n```\n4. Start a worker:
-\n```python\ncelery -A demoproj worker -l info\n```\n5. Run the subscriber:
-\n```python\npython manage.py metroid\n```\n6. Send messages to Metro. Example
-code can be found in [`demoproj/demoapp/services.py`](demoproj/demoapp/
-services.py)\n7. Run the webserver:\n```python\npython manage.py runserver
-8000\n```\n8. See failed messages under `http://localhost:8080/admin`\n\nTo
-contribute, please see [`CONTRIBUTING.md`](CONTRIBUTING.md)\n', 'author':
-'Jonas KrÃ¼ger Svensson', 'author_email': 'jonas.svensson@intility.no',
-'maintainer': 'Ali Arfan', 'maintainer_email': 'ali.arfan@intility.no', 'url':
-'https://github.com/intility/metroid', 'packages': packages, 'package_data':
-package_data, 'install_requires': install_requires, 'python_requires':
-'>=3.8,<4.0', } setup(**setup_kwargs)
+Metadata-Version: 2.1 Name: metroid Version: 1.3.0 Summary: Metroid - Metro for
+Django Home-page: https://github.com/intility/metroid Keywords:
+async,django,servicebus,task,celery,worker,rq Author: Jonas KrÃ¼ger Svensson
+Author-email: jonas.svensson@intility.no Maintainer: Ali Arfan Maintainer-
+email: ali.arfan@intility.no Requires-Python: >=3.8,<4.0 Classifier:
+Development Status :: 5 - Production/Stable Classifier: Environment :: Web
+Environment Classifier: Framework :: Django Classifier: Framework :: Django ::
+3.1 Classifier: Intended Audience :: Developers Classifier: License :: OSI
+Approved :: BSD License Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python Classifier: Programming Language ::
+Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
+Topic :: Software Development Classifier: Topic :: Software Development ::
+Libraries Classifier: Topic :: Software Development :: Libraries :: Application
+Frameworks Classifier: Topic :: Software Development :: Libraries :: Python
+Modules Requires-Dist: Django (>=3.2,<5.0) Requires-Dist: aiohttp
+(>=3.8.4,<4.0.0) Requires-Dist: azure-servicebus (>=7.10.0,<8.0.0) Requires-
+Dist: django-guid (>=3.2.0,<4.0.0) Project-URL: Documentation, https://
+github.com/intility/metroid Project-URL: Repository, https://github.com/
+intility/metroid Description-Content-Type: text/markdown
+                     ****** [.github/images/intility.png]
+                                Metroid ******
+                           Subscribe, act, publish.
+[Python_version] [Django_version] [Celery_version] [ServiceBus_version] [Django
+                                 GUID_version]
+                 [Codecov] [Pre-commit] [Black] [mypy] [isort]
+# Metroid - Metro for Django This app is intended to streamline integration
+with Metro for all Django+Celery users by: * Asynchronous handling of
+subscriptions and messages with one command * Execute Celery tasks based on
+message topics, defined in `settings.py` * Retry failed tasks through your
+admin dashboard when using the `MetroidTask` base ## Overview * `python` >= 3.8
+* `django` >= 3.1.1 - For `asgiref`, settings * `django-guid` >= 3.2.0 -
+Storing correlation IDs for failed tasks in the database, making debugging easy
+* Choose one: * `celery` >= 5.0.0 - Execute tasks based on a subject * `rq` >=
+2.4.1 - Execute tasks based on a subject ### Implementation The `python
+manage.py metroid` app is fully asynchronous, and has no blocking code. It
+utilizes `Celery` to execute tasks. It works by: 1. Going through all your
+configured subscriptions and start a new async connection for each one of them
+2. Metro sends messages on the subscriptions 3. This app filters out messages
+matching subjects you have defined, and queues a celery task to execute the
+function as specified for that subject 3.1. If no task is found for that
+subject, the message is marked as complete 4. The message is marked as complete
+after the Celery task has successfully been queued 5. If the task is failed, an
+entry is automatically created in your database 6. All failed tasks can be
+retried manually through the admin dashboard ### Configure and install this
+package > **_Note_** > For a complete example, have a look in `demoproj/
+settings.py`. 1. Create a `METROID` key in `settings.py` with all your
+subscriptions and handlers. Example settings: ```python METROID =
+{ 'subscriptions': [ { 'topic_name': 'metro-demo', 'subscription_name': 'sub-
+metrodemo-metrodemoerfett', 'connection_string': config
+('CONNECTION_STRING_METRO_DEMO', None), 'handlers': [ { 'subject': 'MetroDemo/
+Type/GeekJokes', 'regex': False, 'handler_function':
+'demoproj.demoapp.services.my_func' } ], }, ], 'worker_type': 'celery', #
+default } ``` The `handler_function` is defined by providing the full dotted
+path as a string. For example,`from demoproj.demoapp.services import my_func`
+is provided as `'demoproj.demoapp.services.my_func'`. The handlers subject can
+be a regular expression or a string. If a regular expression is provided, the
+variable regex must be set to True. Example: ```python 'handlers': [{'subject':
+r'^MetroDemo/Type/.*$','regex':True,'handler_function': my_func}], ``` 2.
+Configure `Django-GUID` by adding the app to your installed apps, to your
+middlewares and configuring logging as described [here](https://github.com/
+snok/django-guid#configuration). Make sure you enable the [`CeleryIntegration`]
+(https://django-guid.readthedocs.io/en/latest/integrations.html#celery):
+```python from django_guid.integrations import CeleryIntegration DJANGO_GUID =
+{ 'INTEGRATIONS': [ CeleryIntegration( use_django_logging=True,
+log_parent=True, ) ], } ``` #### Creating your own handler functions Your
+functions will be called with keyword arguments for `message`, `topic_name`,
+`subscription_name` and `subject`. You function should in other words look
+something like this: ##### Celery ```python @app.task(base=MetroidTask) def
+my_func(*, message: dict, topic_name: str, subscription_name: str, subject:
+str) -> None: ``` ##### rq ```python def my_func(*, message: dict, topic_name:
+str, subscription_name: str, subject: str) -> None: ``` ### Running the project
+1. Ensure you have redis running: ```bash docker-compose up ``` 2. Run
+migrations ```bash python manage.py migrate ``` 3. Create an admin account
+```bash python manage.py createsuperuser ``` 4. Start a worker: ```python
+celery -A demoproj worker -l info ``` 5. Run the subscriber: ```python python
+manage.py metroid ``` 6. Send messages to Metro. Example code can be found in
+[`demoproj/demoapp/services.py`](demoproj/demoapp/services.py) 7. Run the
+webserver: ```python python manage.py runserver 8000 ``` 8. See failed messages
+under `http://localhost:8080/admin` To contribute, please see
+[`CONTRIBUTING.md`](CONTRIBUTING.md)
```

