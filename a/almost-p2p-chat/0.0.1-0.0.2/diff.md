# Comparing `tmp/almost_p2p_chat-0.0.1.tar.gz` & `tmp/almost_p2p_chat-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almost_p2p_chat-0.0.1.tar", last modified: Mon May 22 20:54:14 2023, max compression
+gzip compressed data, was "almost_p2p_chat-0.0.2.tar", last modified: Mon May 22 21:02:35 2023, max compression
```

## Comparing `almost_p2p_chat-0.0.1.tar` & `almost_p2p_chat-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 20:54:14.910260 almost_p2p_chat-0.0.1/
--rw-rw-rw-   0        0        0      300 2023-05-22 20:54:14.910260 almost_p2p_chat-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-22 20:54:14.903025 almost_p2p_chat-0.0.1/almost_p2p_chat/
--rw-rw-rw-   0        0        0        0 2023-05-21 20:08:34.000000 almost_p2p_chat-0.0.1/almost_p2p_chat/__init__.py
--rw-rw-rw-   0        0        0     3035 2023-05-21 20:08:34.000000 almost_p2p_chat-0.0.1/almost_p2p_chat/client.py
--rw-rw-rw-   0        0        0      388 2023-05-21 20:08:34.000000 almost_p2p_chat-0.0.1/almost_p2p_chat/message.py
--rw-rw-rw-   0        0        0     1533 2023-05-21 20:08:34.000000 almost_p2p_chat-0.0.1/almost_p2p_chat/my_socket.py
--rw-rw-rw-   0        0        0     1894 2023-05-21 20:08:34.000000 almost_p2p_chat-0.0.1/almost_p2p_chat/server.py
--rw-rw-rw-   0        0        0     1080 2023-05-21 20:08:34.000000 almost_p2p_chat-0.0.1/almost_p2p_chat/user.py
-drwxrwxrwx   0        0        0        0 2023-05-22 20:54:14.909259 almost_p2p_chat-0.0.1/almost_p2p_chat.egg-info/
--rw-rw-rw-   0        0        0      300 2023-05-22 20:54:14.000000 almost_p2p_chat-0.0.1/almost_p2p_chat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      324 2023-05-22 20:54:14.000000 almost_p2p_chat-0.0.1/almost_p2p_chat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 20:54:14.000000 almost_p2p_chat-0.0.1/almost_p2p_chat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-22 20:54:14.000000 almost_p2p_chat-0.0.1/almost_p2p_chat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 20:54:14.911260 almost_p2p_chat-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      456 2023-05-21 18:23:28.000000 almost_p2p_chat-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-22 21:02:35.298578 almost_p2p_chat-0.0.2/
+-rw-rw-rw-   0        0        0      300 2023-05-22 21:02:35.297579 almost_p2p_chat-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-22 21:02:35.289578 almost_p2p_chat-0.0.2/almost_p2p_chat/
+-rw-rw-rw-   0        0        0        0 2023-05-21 20:08:34.000000 almost_p2p_chat-0.0.2/almost_p2p_chat/__init__.py
+-rw-rw-rw-   0        0        0     3967 2023-05-22 21:02:30.000000 almost_p2p_chat-0.0.2/almost_p2p_chat/client.py
+-rw-rw-rw-   0        0        0      388 2023-05-21 20:08:34.000000 almost_p2p_chat-0.0.2/almost_p2p_chat/message.py
+-rw-rw-rw-   0        0        0     1533 2023-05-21 20:08:34.000000 almost_p2p_chat-0.0.2/almost_p2p_chat/my_socket.py
+-rw-rw-rw-   0        0        0     1894 2023-05-21 20:08:34.000000 almost_p2p_chat-0.0.2/almost_p2p_chat/server.py
+-rw-rw-rw-   0        0        0     1080 2023-05-21 20:08:34.000000 almost_p2p_chat-0.0.2/almost_p2p_chat/user.py
+drwxrwxrwx   0        0        0        0 2023-05-22 21:02:35.296586 almost_p2p_chat-0.0.2/almost_p2p_chat.egg-info/
+-rw-rw-rw-   0        0        0      300 2023-05-22 21:02:35.000000 almost_p2p_chat-0.0.2/almost_p2p_chat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-05-22 21:02:35.000000 almost_p2p_chat-0.0.2/almost_p2p_chat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-22 21:02:35.000000 almost_p2p_chat-0.0.2/almost_p2p_chat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-22 21:02:35.000000 almost_p2p_chat-0.0.2/almost_p2p_chat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-22 21:02:35.298578 almost_p2p_chat-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      456 2023-05-22 21:02:30.000000 almost_p2p_chat-0.0.2/setup.py
```

### Comparing `almost_p2p_chat-0.0.1/almost_p2p_chat/client.py` & `almost_p2p_chat-0.0.2/almost_p2p_chat/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import threading
 import time
 from my_socket import *
 import message
 import queue
+import os
+import pickle
 
 
 class Client:
     UDP_MAX_SIZE = 65535
 
     def __init__(self, username: str, host: str = '127.0.0.1', port: int = 3000):
         self.host = host
@@ -17,31 +19,31 @@
         # self.own_port = self.my_socket.my_getsockname()[1]
         self.listen_thread = None
         self.sendto = None
         self.allowed_ports = [port]
         self.data_from_server = None
         self.window = None
         self.my_queue = queue.Queue()
+        self.client_connections = {}
 
     def listen(self):
         while True:
             msg, addr = self.my_socket.my_recvfrom(self.UDP_MAX_SIZE)
             self.data_from_server = msg
-            self.my_queue.put(str(msg))
-
             msg_port = addr[-1]
             allowed_ports = self.listen_thread.allowed_ports
             if msg_port not in allowed_ports:
                 continue
 
             if not msg:
                 continue
 
             else:
                 self.my_queue.put(str(msg))
+                self.client_connections[self.key_connection].append(msg)
                 print('\r\r' + str(msg) + '\n' + f'you: ', end='')
 
     def start_listen(self):
         self.listen_thread = threading.Thread(target=self.listen, daemon=True)
         self.listen_thread.allowed_ports = self.allowed_ports
         self.listen_thread.start()
 
@@ -54,41 +56,56 @@
         self.my_socket.my_sendto(('__members', self.username), self.sendto)
         time.sleep(0.01)
         return dict(self.data_from_server)
 
     def send_message(self, text):
         self.my_queue.put(f"you: {text}")
         msg = message.Message(self.username, text)
+        self.client_connections[self.key_connection].append(msg)
         self.my_socket.my_sendto(msg, self.sendto)
 
     def connect_by_name(self, username: str):
 
         self.get_members()
         time.sleep(0.001)
         if dict(self.data_from_server).get(username):
             addr = dict(self.data_from_server).get(username)
+            self.key_connection = f"{self.username}-{username}"
+            self.client_connections.setdefault(self.key_connection)
+            self.client_connections[self.key_connection] = list()
+
+            if os.path.isfile(self.key_connection):
+                with open(self.key_connection, 'rb') as file:
+                    print("Ok "*50)
+                    deserialized_message = pickle.load(file)
+                    print(deserialized_message)
+                    for i in deserialized_message:
+                        self.client_connections[self.key_connection].append(i)
+                        if i.sender == self.username:
+                            self.my_queue.put(f"you: {i.text}")
+                        else:
+                            self.my_queue.put(str(i))
+
+            with open(self.key_connection, 'wb') as file:
+                pass
+
             host = addr[0]
             port = addr[1]
             peer_port = port
             self.allowed_ports.append(peer_port)
             self.sendto = (host, peer_port)
             print(f'Connect to client: {username}')
         else:
             print(f'Failed to connect')
 
-
-
     def find_username_port(self, port: int):
         b = self.get_members()
         a = dict(self.data_from_server)
         for key, val in a.items():
             if val[1] == port:
                 return key
 
     def disconect_from_client(self):
 
-        # peer_port = self.sendto[-1]
-        # self.find_username_port(peer_port)
-        # self.allowed_ports.remove(peer_port)
         self.sendto = ("127.0.0.1", 3000)
-        # self.listen_thread.join()
-        # print(f'Disconnect from client:{self.find_username_port(peer_port)}')
+        with open(self.key_connection, 'wb') as file:
+            pickle.dump(self.client_connections.get(self.key_connection), file)
```

### Comparing `almost_p2p_chat-0.0.1/almost_p2p_chat/my_socket.py` & `almost_p2p_chat-0.0.2/almost_p2p_chat/my_socket.py`

 * *Files identical despite different names*

### Comparing `almost_p2p_chat-0.0.1/almost_p2p_chat/server.py` & `almost_p2p_chat-0.0.2/almost_p2p_chat/server.py`

 * *Files identical despite different names*

### Comparing `almost_p2p_chat-0.0.1/almost_p2p_chat/user.py` & `almost_p2p_chat-0.0.2/almost_p2p_chat/user.py`

 * *Files identical despite different names*

