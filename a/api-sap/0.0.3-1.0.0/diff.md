# Comparing `tmp/api_sap-0.0.3.tar.gz` & `tmp/api_sap-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "api_sap-0.0.3.tar", last modified: Sat May 20 14:29:13 2023, max compression
+gzip compressed data, was "api_sap-1.0.0.tar", last modified: Mon May 22 18:06:26 2023, max compression
```

## Comparing `api_sap-0.0.3.tar` & `api_sap-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 14:29:13.028168 api_sap-0.0.3/
--rw-rw-rw-   0        0        0     1075 2023-05-20 12:58:20.000000 api_sap-0.0.3/LICENCE
--rw-rw-rw-   0        0        0      434 2023-05-20 14:29:13.020828 api_sap-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      119 2023-05-20 14:26:04.000000 api_sap-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 14:29:12.984611 api_sap-0.0.3/api_sap.egg-info/
--rw-rw-rw-   0        0        0      434 2023-05-20 14:29:12.000000 api_sap-0.0.3/api_sap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-05-20 14:29:12.000000 api_sap-0.0.3/api_sap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 14:29:12.000000 api_sap-0.0.3/api_sap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-05-20 14:29:12.000000 api_sap-0.0.3/api_sap.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-20 14:29:12.000000 api_sap-0.0.3/api_sap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-20 14:29:13.007152 api_sap-0.0.3/py_sap/
--rw-rw-rw-   0        0        0       25 2023-05-19 23:13:01.000000 api_sap-0.0.3/py_sap/__init__.py
--rw-rw-rw-   0        0        0    29082 2023-05-08 18:17:20.000000 api_sap-0.0.3/py_sap/py_sap.py
--rw-rw-rw-   0        0        0       42 2023-05-20 14:29:13.028668 api_sap-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      784 2023-05-20 14:26:43.000000 api_sap-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 18:06:26.619069 api_sap-1.0.0/
+-rw-rw-rw-   0        0        0     1075 2023-05-20 12:58:20.000000 api_sap-1.0.0/LICENCE
+-rw-rw-rw-   0        0        0      434 2023-05-22 18:06:26.611225 api_sap-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      119 2023-05-20 14:26:04.000000 api_sap-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-22 18:06:26.566992 api_sap-1.0.0/api_sap.egg-info/
+-rw-rw-rw-   0        0        0      434 2023-05-22 18:06:26.000000 api_sap-1.0.0/api_sap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-05-22 18:06:26.000000 api_sap-1.0.0/api_sap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 18:06:26.000000 api_sap-1.0.0/api_sap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-05-22 18:06:26.000000 api_sap-1.0.0/api_sap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-22 18:06:26.000000 api_sap-1.0.0/api_sap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 18:06:26.597858 api_sap-1.0.0/py_sap/
+-rw-rw-rw-   0        0        0       25 2023-05-19 23:13:01.000000 api_sap-1.0.0/py_sap/__init__.py
+-rw-rw-rw-   0        0        0    29009 2023-05-22 18:03:48.000000 api_sap-1.0.0/py_sap/py_sap.py
+-rw-rw-rw-   0        0        0       42 2023-05-22 18:06:26.619069 api_sap-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      784 2023-05-22 18:06:02.000000 api_sap-1.0.0/setup.py
```

### Comparing `api_sap-0.0.3/LICENCE` & `api_sap-1.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `api_sap-0.0.3/py_sap/py_sap.py` & `api_sap-1.0.0/py_sap/py_sap.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,17 +98,15 @@
     @property
     def connections(self):
         """Método para retornar a conexao com o SAPGUI."""
         return self.__connection
 
     def __active_connection_sap_gui(self) -> None:
         """Método para ativar a conexão do objeto SAPGUI."""
-        self.__active_connection = self.__connection[
-            self.__connection.Count - 1
-        ]
+        self.__active_connection = self.__connection[0]
 
     @property
     def connection(self):
         """Método para retornar o objeto SAPGUI com a conexão ativa."""
         return self.__active_connection
 
     def __session_sap_gui(self) -> None:
@@ -118,15 +116,15 @@
     @property
     def sessions(self):
         """Método para retornar a sessão do objeto SAPGUI."""
         return self.__session
 
     def __active_session_sap_gui(self) -> None:
         """Método para ativar a sessão do objeto SAPGUI."""
-        self.__active_session = self.__session[self.__session.Count - 1]
+        self.__active_session = self.__session[0]
 
     @property
     def session(self):
         """Método para retornar o objeto SAPGUI com a sessão ativa."""
         return self.__active_session
 
     def __window_sap_gui(
```

### Comparing `api_sap-0.0.3/setup.py` & `api_sap-1.0.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """
     with open('README.md', 'r', encoding="utf-8") as arq:
         return arq.read()
 
 
 setup(
     name='api_sap',
-    version='0.0.3',
+    version='1.0.0',
     license='MIT License',
     author='Wilton Melo',
     long_description=readme(),
     requires_python='>=3.9.13',
     long_description_content_type='text/markdown',
     author_email='pmelo.wilton@gmail.com',
     keywords=['api sap', 'SAP', 'conectar ao SAP'],
```

