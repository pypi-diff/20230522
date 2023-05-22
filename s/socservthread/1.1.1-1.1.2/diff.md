# Comparing `tmp/socservthread-1.1.1.tar.gz` & `tmp/socservthread-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socservthread-1.1.1.tar", last modified: Mon May 22 16:04:13 2023, max compression
+gzip compressed data, was "socservthread-1.1.2.tar", last modified: Mon May 22 16:14:47 2023, max compression
```

## Comparing `socservthread-1.1.1.tar` & `socservthread-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 16:04:13.812859 socservthread-1.1.1/
--rw-rw-rw-   0        0        0     1094 2021-02-10 19:27:17.000000 socservthread-1.1.1/LICENCE
--rw-rw-rw-   0        0        0      509 2023-05-22 16:04:13.812859 socservthread-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-05-22 14:50:28.000000 socservthread-1.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 16:04:13.812859 socservthread-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-05-22 16:03:32.000000 socservthread-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:04:13.805341 socservthread-1.1.1/socservthread/
--rw-rw-rw-   0        0        0        2 2021-02-10 19:41:50.000000 socservthread-1.1.1/socservthread/__init__.py
--rw-rw-rw-   0        0        0     5194 2023-05-22 15:53:00.000000 socservthread-1.1.1/socservthread/socservthread.py
-drwxrwxrwx   0        0        0        0 2023-05-22 16:04:13.812859 socservthread-1.1.1/socservthread.egg-info/
--rw-rw-rw-   0        0        0      509 2023-05-22 16:04:13.000000 socservthread-1.1.1/socservthread.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-22 16:04:13.000000 socservthread-1.1.1/socservthread.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 16:04:13.000000 socservthread-1.1.1/socservthread.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-22 16:04:13.000000 socservthread-1.1.1/socservthread.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 16:14:47.408563 socservthread-1.1.2/
+-rw-rw-rw-   0        0        0     1094 2021-02-10 19:27:17.000000 socservthread-1.1.2/LICENCE
+-rw-rw-rw-   0        0        0      509 2023-05-22 16:14:47.408563 socservthread-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-05-22 14:50:28.000000 socservthread-1.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 16:14:47.408563 socservthread-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-05-22 16:14:17.000000 socservthread-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:14:47.395550 socservthread-1.1.2/socservthread/
+-rw-rw-rw-   0        0        0        2 2021-02-10 19:41:50.000000 socservthread-1.1.2/socservthread/__init__.py
+-rw-rw-rw-   0        0        0     5197 2023-05-22 16:11:12.000000 socservthread-1.1.2/socservthread/socservthread.py
+drwxrwxrwx   0        0        0        0 2023-05-22 16:14:47.408563 socservthread-1.1.2/socservthread.egg-info/
+-rw-rw-rw-   0        0        0      509 2023-05-22 16:14:47.000000 socservthread-1.1.2/socservthread.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-22 16:14:47.000000 socservthread-1.1.2/socservthread.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 16:14:47.000000 socservthread-1.1.2/socservthread.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 16:14:47.000000 socservthread-1.1.2/socservthread.egg-info/top_level.txt
```

### Comparing `socservthread-1.1.1/LICENCE` & `socservthread-1.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `socservthread-1.1.1/setup.py` & `socservthread-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="socservthread", # Replace with your own username
-    version="1.1.1",
+    version="1.1.2",
     author="Didier Orlandi",
     author_email="didier.orlandi@wanadoo.fr",
     description="Serveur TCP socket",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #url="https://github.com/",
     packages=setuptools.find_packages(),
```

### Comparing `socservthread-1.1.1/socservthread/socservthread.py` & `socservthread-1.1.2/socservthread/socservthread.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
     def close(self):
         self.clientsocket.shutdown(socket.SHUT_RDWR)
         self.clientsocket.close()
         print ("server TCP closed")
 
 #-----------------------------------------------------
-class Tcp_server(threading.Thread):
+class socservthread(threading.Thread):
     
     def __init__(self, hostServer, portServer, _SizeStruc=["<ff",8]):      # arguments du de la classe
         threading.Thread.__init__(self)  # ne pas oublier cette ligne
         # (appel au constructeur de la classe mère)
         tcpsock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         tcpsock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         #tcpsock.bind(("127.0.0.1",8080))
```

