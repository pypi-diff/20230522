# Comparing `tmp/civicrmapi-0.1.dev1.tar.gz` & `tmp/civicrmapi-0.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "civicrmapi-0.1.dev1.tar", last modified: Mon Mar 27 17:54:21 2023, max compression
+gzip compressed data, was "civicrmapi-0.1.dev2.tar", last modified: Mon May 22 10:18:22 2023, max compression
```

## Comparing `civicrmapi-0.1.dev1.tar` & `civicrmapi-0.1.dev2.tar`

### file list

```diff
@@ -1,25 +1,22 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-27 17:54:21.461356 civicrmapi-0.1.dev1/
--rw-r--r--   0 thomas    (1000) thomas    (1000)     1521 2023-03-07 12:30:48.000000 civicrmapi-0.1.dev1/LICENCE
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2036 2023-03-27 17:54:21.461356 civicrmapi-0.1.dev1/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1077 2023-03-17 17:38:00.000000 civicrmapi-0.1.dev1/README.rst
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-27 17:54:21.461356 civicrmapi-0.1.dev1/civicrmapi/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      283 2023-03-23 12:59:13.000000 civicrmapi-0.1.dev1/civicrmapi/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      666 2023-03-27 17:54:11.000000 civicrmapi-0.1.dev1/civicrmapi/__version__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3850 2023-03-20 14:36:04.000000 civicrmapi-0.1.dev1/civicrmapi/base.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2004 2023-03-20 15:31:37.000000 civicrmapi-0.1.dev1/civicrmapi/console.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1789 2023-03-20 15:26:04.000000 civicrmapi-0.1.dev1/civicrmapi/errors.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     4483 2023-03-20 15:26:20.000000 civicrmapi-0.1.dev1/civicrmapi/rest.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-27 17:54:21.461356 civicrmapi-0.1.dev1/civicrmapi/v3/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2592 2023-03-16 13:21:12.000000 civicrmapi-0.1.dev1/civicrmapi/v3/__init__.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-27 17:54:21.461356 civicrmapi-0.1.dev1/civicrmapi/v4/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2313 2023-03-16 13:21:20.000000 civicrmapi-0.1.dev1/civicrmapi/v4/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      151 2023-03-16 10:14:42.000000 civicrmapi-0.1.dev1/civicrmapi/v4/group.py
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-03-27 17:54:21.461356 civicrmapi-0.1.dev1/civicrmapi.egg-info/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2036 2023-03-27 17:54:21.000000 civicrmapi-0.1.dev1/civicrmapi.egg-info/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      430 2023-03-27 17:54:21.000000 civicrmapi-0.1.dev1/civicrmapi.egg-info/SOURCES.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-03-27 17:54:21.000000 civicrmapi-0.1.dev1/civicrmapi.egg-info/dependency_links.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       16 2023-03-27 17:54:21.000000 civicrmapi-0.1.dev1/civicrmapi.egg-info/requires.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       11 2023-03-27 17:54:21.000000 civicrmapi-0.1.dev1/civicrmapi.egg-info/top_level.txt
--rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-03-07 14:47:01.000000 civicrmapi-0.1.dev1/civicrmapi.egg-info/zip-safe
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-03-27 17:54:21.465356 civicrmapi-0.1.dev1/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1851 2023-03-17 17:38:16.000000 civicrmapi-0.1.dev1/setup.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-22 10:18:22.169340 civicrmapi-0.1.dev2/
+-rw-r--r--   0 thomas    (1000) thomas    (1000)     1521 2023-03-07 12:30:48.000000 civicrmapi-0.1.dev2/LICENCE
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2108 2023-05-22 10:18:22.169340 civicrmapi-0.1.dev2/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1149 2023-03-29 12:17:45.000000 civicrmapi-0.1.dev2/README.rst
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-22 10:18:22.165341 civicrmapi-0.1.dev2/civicrmapi/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      367 2023-03-30 12:45:03.000000 civicrmapi-0.1.dev2/civicrmapi/__init__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      666 2023-05-22 10:17:51.000000 civicrmapi-0.1.dev2/civicrmapi/__version__.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4671 2023-03-31 09:08:05.000000 civicrmapi-0.1.dev2/civicrmapi/base.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2702 2023-03-30 07:39:14.000000 civicrmapi-0.1.dev2/civicrmapi/console.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1903 2023-03-31 08:45:50.000000 civicrmapi-0.1.dev2/civicrmapi/errors.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     4123 2023-03-28 19:47:48.000000 civicrmapi-0.1.dev2/civicrmapi/rest.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2592 2023-03-31 09:23:38.000000 civicrmapi-0.1.dev2/civicrmapi/v3.py
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2288 2023-03-31 09:28:03.000000 civicrmapi-0.1.dev2/civicrmapi/v4.py
+drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2023-05-22 10:18:22.169340 civicrmapi-0.1.dev2/civicrmapi.egg-info/
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     2108 2023-05-22 10:18:22.000000 civicrmapi-0.1.dev2/civicrmapi.egg-info/PKG-INFO
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)      389 2023-05-22 10:18:22.000000 civicrmapi-0.1.dev2/civicrmapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-05-22 10:18:22.000000 civicrmapi-0.1.dev2/civicrmapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       16 2023-05-22 10:18:22.000000 civicrmapi-0.1.dev2/civicrmapi.egg-info/requires.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       11 2023-05-22 10:18:22.000000 civicrmapi-0.1.dev2/civicrmapi.egg-info/top_level.txt
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)        1 2023-03-07 14:47:01.000000 civicrmapi-0.1.dev2/civicrmapi.egg-info/zip-safe
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)       38 2023-05-22 10:18:22.169340 civicrmapi-0.1.dev2/setup.cfg
+-rw-rw-r--   0 thomas    (1000) thomas    (1000)     1851 2023-03-17 17:38:16.000000 civicrmapi-0.1.dev2/setup.py
```

### Comparing `civicrmapi-0.1.dev1/LICENCE` & `civicrmapi-0.1.dev2/LICENCE`

 * *Files identical despite different names*

### Comparing `civicrmapi-0.1.dev1/PKG-INFO` & `civicrmapi-0.1.dev2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civicrmapi
-Version: 0.1.dev1
+Version: 0.1.dev2
 Summary: Connect with the CiviCRM APIv4.
 Home-page: https://github.com/thomst/civicrmapi
 Author: Thomas Leichtfuß
 Author-email: thomas.leichtfuss@posteo.de
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
@@ -46,11 +46,22 @@
 tests are not yet available.
 
 Description
 ===========
 Clean and simple bindings to CiviCRM's API. Both APIv3 and APIv4 are supported.
 
 
+Installation
+============
+::
+
+   pip install civicrmapi
+
+Usage
+=====
+
+
+
 Links
 =====
 * `Repository <https://github.com/thomst/civicrmapi>`_
 * `Documentation <https://thomst.github.io/civicrmapi/>`_ (Not yet available!)
```

### Comparing `civicrmapi-0.1.dev1/README.rst` & `civicrmapi-0.1.dev2/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -21,11 +21,22 @@
 tests are not yet available.
 
 Description
 ===========
 Clean and simple bindings to CiviCRM's API. Both APIv3 and APIv4 are supported.
 
 
+Installation
+============
+::
+
+   pip install civicrmapi
+
+Usage
+=====
+
+
+
 Links
 =====
 * `Repository <https://github.com/thomst/civicrmapi>`_
 * `Documentation <https://thomst.github.io/civicrmapi/>`_ (Not yet available!)
```

### Comparing `civicrmapi-0.1.dev1/civicrmapi/__version__.py` & `civicrmapi-0.1.dev2/civicrmapi/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 internal code changes that do not affect the API. Development versions are
 incomplete states of a release .
 
 Version 0.x should be considered a development version with an unstable API,
 and backwards compatibility is not guaranteed for minor versions.
 """
 
-__version__ = "0.1.dev1"
+__version__ = "0.1.dev2"
```

### Comparing `civicrmapi-0.1.dev1/civicrmapi/base.py` & `civicrmapi-0.1.dev2/civicrmapi/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,75 +8,91 @@
 
 
 class BaseAction:
     ENTITY = None
     ACTION = None
 
     def __init__(self, api):
+        if not self.ENTITY or not self.ACTION:
+            raise NotImplemented('ENTITY and ACTION must be defined.')
         self._api = api
 
     def __call__(self, params=None):
         """
         :param dict params: api call parameters (optional)
         :return dict: api call result
         """
         return self._api(self.ENTITY, self.ACTION, params or dict())
 
 
 class BaseEntity:
     ENTITY = None
+    ACTIONS = list()
 
     def __init__(self, api):
+        if not self.ENTITY:
+            raise NotImplemented('ENTITY must be defined.')
         self._api = api
-        if api.VERSION:
-            self._add_actions(api.VERSION)
+        self._add_actions()
 
-    def _add_actions(self, version_mod):
-        for action in version_mod.ACTIONS:
-            if hasattr(self, action):
-                continue
-            else:
+    def _add_actions(self):
+        for action in self.ACTIONS + self._api.VERSION.ACTIONS:
+            if isinstance(action, str):
+                action_name = action
                 attrs = dict(ENTITY=self.ENTITY, ACTION=action)
                 action_class = type(action, (BaseAction,), attrs)
-                setattr(self, action, action_class(self._api))
+            elif isinstance(action, type) and issubclass(action, BaseAction):
+                action_name = action.__name__
+                action_class = action
+            else:
+                msg = 'ACTIONS item must be string or subclass of BaseAction.'
+                raise ValueError(msg)
+            if not hasattr(self, action_name):
+                setattr(self, action_name, action_class(self._api))
 
     def __call__(self, action, params=None):
         """
         :param str action: api call action
         :param dict params: api call parameters (optional)
         :return dict: api call result
         """
         return self._api(self.ENTITY, action, params or dict())
 
 
 class BaseApi:
     VERSION = None
+    ENTITIES = list()
 
     def __init__(self):
-        if self.VERSION:
-            self._add_entities(self.VERSION)
-
-    def _add_entities(self, version_mod):
-        for entity in version_mod.ENTITIES:
-            if hasattr(version_mod, entity):
-                setattr(self, entity, getattr(version_mod, entity)(self))
+        if not self.VERSION:
+            raise NotImplemented('VERSION must be defined.')
+        self._add_entities()
+
+    def _add_entities(self):
+        for entity in self.ENTITIES + self.VERSION.ENTITIES:
+            if isinstance(entity, str):
+                entity_name = entity
+                entity_class = type(entity, (BaseEntity,), dict(ENTITY=entity))
+            elif isinstance(entity, type) and issubclass(entity, BaseEntity):
+                entity_name = entity.__name__
+                entity_class = entity
             else:
-                attrs = dict(ENTITY=entity)
-                entity_class = type(entity, (BaseEntity,), attrs)
-                setattr(self, entity, entity_class(self))
+                msg = 'ENTITIES item must be string or subclass of BaseEntity.'
+                raise ValueError(msg)
+            if not hasattr(self, entity_name):
+                setattr(self, entity_name, entity_class(self))
 
     def __call__(self, entity, action, params=None):
         """
         :param str entity: CiviCRM-entitiy
         :param str action: api call action
         :param dict params: api call parameters (optional)
-        :return dict: api call result
+        :return dict: normalized api call result
         :raises RequestError: when the rest api could not be accessed
         :raises InvokeError: when the console api could not be accessed
-        :raises HttpError: when the rest api return an error code
         :raises ApiError: when the api call failed
         :raises InvalidJson: when the response is invalid json code
         """
         logger.info(f'Perform api call: {entity}.{action} with {params}')
         result = self._perform_api_call(entity, action, params or dict())
         return self._process_json_result(result)
```

### Comparing `civicrmapi-0.1.dev1/civicrmapi/errors.py` & `civicrmapi-0.1.dev2/civicrmapi/errors.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     A simple wrapper for a json.JSONDecodeError.
     """
     pass
 
 
 class ApiError(BaseException):
     """
-    Raised for all api related errors including all http error-codes.
+    Raised for all api related errors as well as return-code and http errors.
     """
     def __init__(self,value, msg=None):
         self.value = value
         self.msg = msg
 
     def _as_json(self, value):
         try:
@@ -48,17 +48,19 @@
 
     def __str__(self):
         if self.msg:
             msg = [f'ERROR: {self.msg}']
         else:
             msg = list()
         if isinstance(self.value, requests.Response):
+            msg.append(f'URL: {self.value.url}')
             msg.append(f'HTTP-CODE: {self.value.status_code}')
             msg.append('RESPONSE: {}'.format(self._as_json(self.value.text)))
         elif isinstance(self.value, invoke.runners.Result):
+            msg.append(f'COMMAND: {self.value.command}')
             msg.append(f'RETURN-CODE: {self.value.return_code}')
             msg.append('STDOUT: {}'.format(self._as_json(self.value.stdout)))
             msg.append('STDERR: {}'.format(self._as_json(self.value.stderr)))
         elif isinstance(self.value, dict) or isinstance(self.value, list):
             msg.append(json.dumps(self.value, sort_keys=True, indent=4))
         else:
             msg.append(self.value)
```

### Comparing `civicrmapi-0.1.dev1/civicrmapi/rest.py` & `civicrmapi-0.1.dev2/civicrmapi/rest.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,21 +9,14 @@
 
 
 logger = logging.getLogger('civicrmapi')
 
 
 class BaseRestApi(BaseApi):
     def __init__(self, url, htaccess=None, verify_ssl=True, timeout=None, headers=None):
-        """
-        :param str url: rest api endoint
-        :param dict htaccess: htaccess credentials with 'user' and 'pass' keys. (optional)
-        :param bool verify_ssl: Verify SSL-certificate or not. Default is True. (optional)
-        :param int timeout: Timeout in seconds. (optional)
-        :param dict headers: HTTP headers. (optional)
-        """
         super().__init__()
         self.url = url
         self.verify_ssl = verify_ssl
         self.timeout = timeout
         self.headers = headers
 
         # Setup basic-auth
```

### Comparing `civicrmapi-0.1.dev1/civicrmapi/v3/__init__.py` & `civicrmapi-0.1.dev2/civicrmapi/v3.py`

 * *Files identical despite different names*

### Comparing `civicrmapi-0.1.dev1/civicrmapi/v4/__init__.py` & `civicrmapi-0.1.dev2/civicrmapi/v4.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,9 +118,8 @@
     'getFields',
     'get',
     'create',
     'update',
     'save',
     'delete',
     'replace',
-]
-from .group import Group
+]
```

### Comparing `civicrmapi-0.1.dev1/civicrmapi.egg-info/PKG-INFO` & `civicrmapi-0.1.dev2/civicrmapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: civicrmapi
-Version: 0.1.dev1
+Version: 0.1.dev2
 Summary: Connect with the CiviCRM APIv4.
 Home-page: https://github.com/thomst/civicrmapi
 Author: Thomas Leichtfuß
 Author-email: thomas.leichtfuss@posteo.de
 License: BSD License
 Platform: OS Independent
 Classifier: Development Status :: 3 - Alpha
@@ -46,11 +46,22 @@
 tests are not yet available.
 
 Description
 ===========
 Clean and simple bindings to CiviCRM's API. Both APIv3 and APIv4 are supported.
 
 
+Installation
+============
+::
+
+   pip install civicrmapi
+
+Usage
+=====
+
+
+
 Links
 =====
 * `Repository <https://github.com/thomst/civicrmapi>`_
 * `Documentation <https://thomst.github.io/civicrmapi/>`_ (Not yet available!)
```

### Comparing `civicrmapi-0.1.dev1/setup.py` & `civicrmapi-0.1.dev2/setup.py`

 * *Files identical despite different names*

