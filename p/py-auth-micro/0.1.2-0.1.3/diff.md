# Comparing `tmp/py_auth_micro-0.1.2.tar.gz` & `tmp/py_auth_micro-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_auth_micro-0.1.2.tar", last modified: Fri May 19 10:10:50 2023, max compression
+gzip compressed data, was "py_auth_micro-0.1.3.tar", last modified: Mon May 22 13:00:57 2023, max compression
```

## Comparing `py_auth_micro-0.1.2.tar` & `py_auth_micro-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.530916 py_auth_micro-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-19 10:10:50.530916 py_auth_micro-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.522916 py_auth_micro-0.1.2/py_auth_micro/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.522916 py_auth_micro-0.1.2/py_auth_micro/Config/
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Config/_appconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Config/_dbconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Config/_ldapconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.526916 py_auth_micro-0.1.2/py_auth_micro/Core/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Core/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Core/_ldap_interactions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.526916 py_auth_micro-0.1.2/py_auth_micro/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.526916 py_auth_micro-0.1.2/py_auth_micro/LoginHandler/
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/LoginHandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/LoginHandler/_loginbaseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/LoginHandler/_loginkerberos.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/LoginHandler/_loginldap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/LoginHandler/_loginlocal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.526916 py_auth_micro-0.1.2/py_auth_micro/Models/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Models/_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Models/_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/Models/_user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.530916 py_auth_micro-0.1.2/py_auth_micro/WorkFlows/
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/WorkFlows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_groupworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_sessionworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_userworkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/py_auth_micro/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 10:10:50.522916 py_auth_micro-0.1.2/py_auth_micro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-19 10:10:50.000000 py_auth_micro-0.1.2/py_auth_micro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-19 10:10:50.000000 py_auth_micro-0.1.2/py_auth_micro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 10:10:50.000000 py_auth_micro-0.1.2/py_auth_micro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-19 10:10:50.000000 py_auth_micro-0.1.2/py_auth_micro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-19 10:10:50.000000 py_auth_micro-0.1.2/py_auth_micro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-19 10:10:50.530916 py_auth_micro-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-19 10:09:56.000000 py_auth_micro-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:00:57.475184 py_auth_micro-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-22 13:00:57.475184 py_auth_micro-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:00:57.471184 py_auth_micro-0.1.3/py_auth_micro/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:00:57.471184 py_auth_micro-0.1.3/py_auth_micro/Config/
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/Config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/Config/_appconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/Config/_dbconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/Config/_ldapconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:00:57.471184 py_auth_micro-0.1.3/py_auth_micro/Core/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/Core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/Core/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/Core/_ldap_interactions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:00:57.471184 py_auth_micro-0.1.3/py_auth_micro/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/Exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:00:57.471184 py_auth_micro-0.1.3/py_auth_micro/LoginHandler/
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/LoginHandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/LoginHandler/_loginbaseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/LoginHandler/_loginkerberos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/LoginHandler/_loginldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/LoginHandler/_loginlocal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:00:57.471184 py_auth_micro-0.1.3/py_auth_micro/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/Models/_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/Models/_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/Models/_user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:00:57.475184 py_auth_micro-0.1.3/py_auth_micro/WorkFlows/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/WorkFlows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7940 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/WorkFlows/_groupworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/WorkFlows/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/WorkFlows/_sessionworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/WorkFlows/_userworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/py_auth_micro/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 13:00:57.471184 py_auth_micro-0.1.3/py_auth_micro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-22 13:00:57.000000 py_auth_micro-0.1.3/py_auth_micro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-22 13:00:57.000000 py_auth_micro-0.1.3/py_auth_micro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 13:00:57.000000 py_auth_micro-0.1.3/py_auth_micro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-22 13:00:57.000000 py_auth_micro-0.1.3/py_auth_micro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-22 13:00:57.000000 py_auth_micro-0.1.3/py_auth_micro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-22 13:00:57.475184 py_auth_micro-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-22 12:59:53.000000 py_auth_micro-0.1.3/setup.py
```

### Comparing `py_auth_micro-0.1.2/LICENSE` & `py_auth_micro-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/PKG-INFO` & `py_auth_micro-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_auth_micro
-Version: 0.1.2
+Version: 0.1.3
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_micro
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: JWT
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_micro-0.1.2/README.rst` & `py_auth_micro-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro/Config/_appconfig.py` & `py_auth_micro-0.1.3/py_auth_micro/Config/_appconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro/Config/_dbconfig.py` & `py_auth_micro-0.1.3/py_auth_micro/Config/_dbconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro/Config/_ldapconfig.py` & `py_auth_micro-0.1.3/py_auth_micro/Config/_ldapconfig.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro/Core/_ldap_interactions.py` & `py_auth_micro-0.1.3/py_auth_micro/Core/_ldap_interactions.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro/LoginHandler/__init__.py` & `py_auth_micro-0.1.3/py_auth_micro/LoginHandler/__init__.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro/LoginHandler/_loginbaseclass.py` & `py_auth_micro-0.1.3/py_auth_micro/LoginHandler/_loginbaseclass.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro/LoginHandler/_loginldap.py` & `py_auth_micro-0.1.3/py_auth_micro/LoginHandler/_loginldap.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro/LoginHandler/_loginlocal.py` & `py_auth_micro-0.1.3/py_auth_micro/LoginHandler/_loginlocal.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro/Models/_token.py` & `py_auth_micro-0.1.3/py_auth_micro/Models/_token.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro/Models/_user.py` & `py_auth_micro-0.1.3/py_auth_micro/Models/_user.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro/WorkFlows/__init__.py` & `py_auth_micro-0.1.3/py_auth_micro/WorkFlows/__init__.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_groupworkflow.py` & `py_auth_micro-0.1.3/py_auth_micro/WorkFlows/_groupworkflow.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
         group = await self._perm_and_name_check(
             access_token=access_token, groupname=groupname
         )
         if group is None:
             raise ValueError("Group does not exist")
 
-        userlist = await group.users.values_list("username", True)
+        userlist = await group.users.all().values_list("username", True)
         return {"resp_code": 200, "resp_data": {"users": userlist}}
 
     async def create_group(
         self, *, access_token: str, groupname: str, **kwargs
     ) -> dict:
         """Creates a Group with the specified Name
```

### Comparing `py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_misc.py` & `py_auth_micro-0.1.3/py_auth_micro/WorkFlows/_misc.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_sessionworkflow.py` & `py_auth_micro-0.1.3/py_auth_micro/WorkFlows/_sessionworkflow.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro/WorkFlows/_userworkflow.py` & `py_auth_micro-0.1.3/py_auth_micro/WorkFlows/_userworkflow.py`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/py_auth_micro.egg-info/PKG-INFO` & `py_auth_micro-0.1.3/py_auth_micro.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-auth-micro
-Version: 0.1.2
+Version: 0.1.3
 Summary: A wrapper around pyjwt
 Home-page: https://github.com/bad-microservices/py_auth_micro
 Author: Ole Hannemann
 Author-email: cerberus885@gmail.com
 License: MIT
 Keywords: JWT
 Classifier: Programming Language :: Python :: 3.0
```

### Comparing `py_auth_micro-0.1.2/py_auth_micro.egg-info/SOURCES.txt` & `py_auth_micro-0.1.3/py_auth_micro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py_auth_micro-0.1.2/setup.cfg` & `py_auth_micro-0.1.3/setup.cfg`

 * *Files identical despite different names*

