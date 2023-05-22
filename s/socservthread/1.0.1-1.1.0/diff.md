# Comparing `tmp/socservthread-1.0.1.tar.gz` & `tmp/socservthread-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socservthread-1.0.1.tar", last modified: Mon May 22 14:56:43 2023, max compression
+gzip compressed data, was "socservthread-1.1.0.tar", last modified: Mon May 22 15:54:56 2023, max compression
```

## Comparing `socservthread-1.0.1.tar` & `socservthread-1.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 14:56:43.099422 socservthread-1.0.1/
--rw-rw-rw-   0        0        0     1094 2021-02-10 19:27:17.000000 socservthread-1.0.1/LICENCE
--rw-rw-rw-   0        0        0      509 2023-05-22 14:56:43.099422 socservthread-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-05-22 14:50:28.000000 socservthread-1.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-22 14:56:43.099422 socservthread-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      733 2023-05-22 14:55:31.000000 socservthread-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:56:43.088348 socservthread-1.0.1/socservthread/
--rw-rw-rw-   0        0        0        2 2021-02-10 19:41:50.000000 socservthread-1.0.1/socservthread/__init__.py
--rw-rw-rw-   0        0        0     4822 2023-05-22 14:34:15.000000 socservthread-1.0.1/socservthread/main.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:56:43.098336 socservthread-1.0.1/socservthread.egg-info/
--rw-rw-rw-   0        0        0      509 2023-05-22 14:56:43.000000 socservthread-1.0.1/socservthread.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-22 14:56:43.000000 socservthread-1.0.1/socservthread.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 14:56:43.000000 socservthread-1.0.1/socservthread.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-22 14:56:43.000000 socservthread-1.0.1/socservthread.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-22 15:54:56.400466 socservthread-1.1.0/
+-rw-rw-rw-   0        0        0     1094 2021-02-10 19:27:17.000000 socservthread-1.1.0/LICENCE
+-rw-rw-rw-   0        0        0      509 2023-05-22 15:54:56.400466 socservthread-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-05-22 14:50:28.000000 socservthread-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-22 15:54:56.400466 socservthread-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      733 2023-05-22 15:54:14.000000 socservthread-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 15:54:56.387432 socservthread-1.1.0/socservthread/
+-rw-rw-rw-   0        0        0        2 2021-02-10 19:41:50.000000 socservthread-1.1.0/socservthread/__init__.py
+-rw-rw-rw-   0        0        0     5194 2023-05-22 15:53:00.000000 socservthread-1.1.0/socservthread/main.py
+drwxrwxrwx   0        0        0        0 2023-05-22 15:54:56.400466 socservthread-1.1.0/socservthread.egg-info/
+-rw-rw-rw-   0        0        0      509 2023-05-22 15:54:56.000000 socservthread-1.1.0/socservthread.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-22 15:54:56.000000 socservthread-1.1.0/socservthread.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 15:54:56.000000 socservthread-1.1.0/socservthread.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-22 15:54:56.000000 socservthread-1.1.0/socservthread.egg-info/top_level.txt
```

### Comparing `socservthread-1.0.1/LICENCE` & `socservthread-1.1.0/LICENCE`

 * *Files identical despite different names*

### Comparing `socservthread-1.0.1/setup.py` & `socservthread-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="socservthread", # Replace with your own username
-    version="1.0.1",
+    version="1.1.0",
     author="Didier Orlandi",
     author_email="didier.orlandi@wanadoo.fr",
     description="Serveur TCP socket",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #url="https://github.com/",
     packages=setuptools.find_packages(),
```

### Comparing `socservthread-1.0.1/socservthread/main.py` & `socservthread-1.1.0/socservthread/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,26 @@
 import socket
 import threading
 import struct
 from queue import Queue # queue pour partager les données entre 2 thread
 
-exit_event = threading.Event() # évenement pour arrêter le thread (serveur tcp qui reçoit les données de Blender)
-QSizeMax = 2000 # taille maximale de la queue FIFO
-
-tcpsock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-tcpsock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-#tcpsock.bind(("127.0.0.1",8080))
-# Initializing a queue
-q = Queue(maxsize = QSizeMax)# taille maximale de la queue FIFO 
-
 #-----------------------------------------------------
 class Tcp_Client(threading.Thread):
+    
     def __init__(self, host, port, _structSize, Queue, clientsocket):      # arguments du de la classe
         threading.Thread.__init__(self)  # ne pas oublier cette ligne
         # (appel au constructeur de la classe mère)
         self.clientsocket = clientsocket
         self.host = host
         self.port = port
         self.structSize = _structSize # taille de la structure de données envoyées par le client (2 floats) '<ff'   8 octets
         #self.connected = False
         self.queue = Queue
         print("[+] Nouveau thread pour %s %s" % (self.host, self.port, ))
+        self.exit_event = threading.Event() # évenement pour arrêter le thread (serveur tcp qui reçoit les données de Blender)
     
     def run(self):
         print("Connexion de %s %s" % (self.host, self.port, ))
         while True:
             try:
                 # receive data stream. it won't accept data packet greater than 1024 bytes
                 data = self.clientsocket.recv(self.structSize[1])# Important taille du buffer de réception pour lire les données par 2 floats : 4*2
@@ -47,55 +40,64 @@
                             #print(qa)                    
                             #print("réception & entré 1er sorti :")
 
             except:
                 #pass
                 print("exception pour TCP server  ....")
             finally:
-                if exit_event.is_set():# si événement d'arrêt du thread est envoyé on arrête le thread
+                if self.exit_event.is_set():# si événement d'arrêt du thread est envoyé on arrête le thread
                     print("on a arrêté le thread tcp server  ! ")   
                     self.close()
                     break
 
     def close(self):
         self.clientsocket.shutdown(socket.SHUT_RDWR)
         self.clientsocket.close()
         print ("server TCP closed")
 
 #-----------------------------------------------------
 class Tcp_server(threading.Thread):
-    def __init__(self, hostServer, portServer, _SizeStruc=["<ff",8], Queue=q, clientsocket=tcpsock):      # arguments du de la classe
+    
+    def __init__(self, hostServer, portServer, _SizeStruc=["<ff",8]):      # arguments du de la classe
         threading.Thread.__init__(self)  # ne pas oublier cette ligne
         # (appel au constructeur de la classe mère)
-        self.clientsocket = clientsocket
+        tcpsock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        tcpsock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        #tcpsock.bind(("127.0.0.1",8080))
+        # Initializing a queue
+        self.QSizeMax = 2000 # taille maximale de la queue FIFO
+        self.queue = Queue(maxsize = self.QSizeMax)# taille maximale de la queue FIFO
+        self.exit_event = threading.Event() # évenement pour arrêter le thread (serveur tcp qui reçoit les données de Blender)
+        self.clientsocket = tcpsock
         self.hostS = hostServer
         self.portS = portServer
         self.SizeStruc = _SizeStruc # taille de la structure de données envoyées par le client (2 floats) '<ff'   8 octets
-        self.queue = Queue
         self.clientsocket.bind((self.hostS,self.portS))
         print("[+] Server TCP créé pour %s %s" % (self.hostS, self.portS, ))
     
     def run(self):
         newClient = None
         while True:
             try:
-                if exit_event.is_set():# si événement d'arrêt du thread est envoyé on arrête le thread
+                if self.exit_event.is_set():# si événement d'arrêt du thread est envoyé on arrête le thread
+                    Tcp_Client.exit_event.set()# on envoie l'événement d'arrêt au thread client
                     break
                 self.clientsocket.listen(10)
                 #don = Queue.get()
                 #print(Queue.get())
                 print( "En écoute...")
                 (clientsoc, (ip, port)) = self.clientsocket.accept()# bloque ici si pas de client
                 newClient = Tcp_Client(ip, port, self.SizeStruc, self.queue, clientsoc)# ip et port du client qui vient de se connecter
                 newClient.start()
             except:
                 #pass
                 print("exception pour TCP server ....")
             finally:
-                if exit_event.is_set():# si événement d'arrêt du thread est envoyé on arrête le thread
+                if self.exit_event.is_set():# si événement d'arrêt du thread est envoyé on arrête le thread
                     print("on a arrêté le thread TCP server ! ")
                     if newClient != None:
                         print("on ferme le socket")
+                        #newClient.exit_event.set()# on envoie l'événement d'arrêt au thread client
                         newClient.close()
                     break
 
 #-----------------------------------------------------
```

