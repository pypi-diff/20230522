# Comparing `tmp/OpenAccess-0.3.tar.gz` & `tmp/OpenAccess-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenAccess-0.3.tar", last modified: Tue May  9 21:09:42 2023, max compression
+gzip compressed data, was "OpenAccess-0.4.tar", last modified: Mon May 22 15:29:12 2023, max compression
```

## Comparing `OpenAccess-0.3.tar` & `OpenAccess-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 21:09:42.436089 OpenAccess-0.3/
-drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 21:09:42.436089 OpenAccess-0.3/OpenAccess/
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)      103 2023-05-09 21:09:30.000000 OpenAccess-0.3/OpenAccess/__init__.py
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)    13803 2023-05-09 21:09:06.000000 OpenAccess-0.3/OpenAccess/openaccess.py
-drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-09 21:09:42.436089 OpenAccess-0.3/OpenAccess.egg-info/
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1579 2023-05-09 21:09:42.000000 OpenAccess-0.3/OpenAccess.egg-info/PKG-INFO
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)      235 2023-05-09 21:09:42.000000 OpenAccess-0.3/OpenAccess.egg-info/SOURCES.txt
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)        1 2023-05-09 21:09:42.000000 OpenAccess-0.3/OpenAccess.egg-info/dependency_links.txt
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)        9 2023-05-09 21:09:42.000000 OpenAccess-0.3/OpenAccess.egg-info/requires.txt
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)       11 2023-05-09 21:09:42.000000 OpenAccess-0.3/OpenAccess.egg-info/top_level.txt
--rw-rw-r--   0 jaiber    (1000) jaiber    (1000)     1579 2023-05-09 21:09:42.436089 OpenAccess-0.3/PKG-INFO
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1249 2023-04-24 21:19:05.000000 OpenAccess-0.3/README.md
--rw-rw-r--   0 jaiber    (1000) jaiber    (1000)       38 2023-05-09 21:09:42.436089 OpenAccess-0.3/setup.cfg
--rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1392 2023-04-03 16:58:33.000000 OpenAccess-0.3/setup.py
+drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-22 15:29:12.159237 OpenAccess-0.4/
+drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-22 15:29:12.159237 OpenAccess-0.4/OpenAccess/
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)      103 2023-05-22 15:25:27.000000 OpenAccess-0.4/OpenAccess/__init__.py
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)    16185 2023-05-22 15:24:25.000000 OpenAccess-0.4/OpenAccess/openaccess.py
+drwxrwxr-x   0 jaiber    (1000) jaiber    (1000)        0 2023-05-22 15:29:12.159237 OpenAccess-0.4/OpenAccess.egg-info/
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1579 2023-05-22 15:29:12.000000 OpenAccess-0.4/OpenAccess.egg-info/PKG-INFO
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)      235 2023-05-22 15:29:12.000000 OpenAccess-0.4/OpenAccess.egg-info/SOURCES.txt
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)        1 2023-05-22 15:29:12.000000 OpenAccess-0.4/OpenAccess.egg-info/dependency_links.txt
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)        9 2023-05-22 15:29:12.000000 OpenAccess-0.4/OpenAccess.egg-info/requires.txt
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)       11 2023-05-22 15:29:12.000000 OpenAccess-0.4/OpenAccess.egg-info/top_level.txt
+-rw-rw-r--   0 jaiber    (1000) jaiber    (1000)     1579 2023-05-22 15:29:12.159237 OpenAccess-0.4/PKG-INFO
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1249 2023-04-24 21:19:05.000000 OpenAccess-0.4/README.md
+-rw-rw-r--   0 jaiber    (1000) jaiber    (1000)       38 2023-05-22 15:29:12.159237 OpenAccess-0.4/setup.cfg
+-rw-r--r--   0 jaiber    (1000) jaiber    (1000)     1392 2023-04-03 16:58:33.000000 OpenAccess-0.4/setup.py
```

### Comparing `OpenAccess-0.3/OpenAccess/openaccess.py` & `OpenAccess-0.4/OpenAccess/openaccess.py`

 * *Files 8% similar despite different names*

```diff
@@ -215,14 +215,70 @@
             result = self.request_instances("Lnl_Reader", i, panelId)
 
             # Convert the response to Reader objects and add them to the list
             readers.extend(self.get_readers_from_result(result))
 
         return readers
     
+    def get_panels_filtered(self, panel_filter:str):
+        """
+        Get panel information using a filter panel_filter(str)
+        i.e. get_panel_filtered(panel_filter="ID=8")
+
+        GET /api/access/onguard/openaccess/instances
+
+        Get a supported data class against a specific instance of a particular type (Lnl_Panel against a panelID in this case)
+        """
+
+        # Data object to be serialized by PostAsJsonAsync
+        em = {
+            "type_name":"Lnl_Panel", 
+            "filter":panel_filter
+        }
+
+        
+        self.client.headers.update({"Session-Token": self.session_token})
+        response = self.client.get(self.build_uri_with_version("instances","1.0"), json=em, verify=self.client.verify)
+
+        # If a response is recieved, parse it into a dict so its properties can be retrieved easily
+        if response.status_code == 200:
+            return self.parse_response(response)
+
+        # If an error occurred on the server side, return its information
+        else:
+            return f"A server error occurred during your request. If the status code is available, it is shown below\n{response.status_code}: {response.text}"
+    
+    def get_readers_filtered(self, reader_filter:str):
+        """
+        Get reader information using a reader panel_filter(str)
+        i.e. get_reader_filtered(reader_filter="ReaderID=8 AND PanelID=9")
+
+        GET /api/access/onguard/openaccess/instances
+
+        Get a supported data class against a specific instance of a particular type (Lnl_Reader against a panelID in this case)
+        """
+
+        # Data object to be serialized by PostAsJsonAsync
+        em = {
+            "type_name":"Lnl_Reader", 
+            "filter":reader_filter
+        }
+
+        
+        self.client.headers.update({"Session-Token": self.session_token})
+        response = self.client.get(self.build_uri_with_version("instances","1.0"), json=em, verify=self.client.verify)
+
+        # If a response is recieved, parse it into a dict so its properties can be retrieved easily
+        if response.status_code == 200:
+            return self.parse_response(response)
+
+        # If an error occurred on the server side, return its information
+        else:
+            return f"A server error occurred during your request. If the status code is available, it is shown below\n{response.status_code}: {response.text}"
+    
     def OpenDoor(self, reader):
         """
         OpenAccess "execute_method" request
 
         POST /api/access/onguard/openaccess/execute_method
 
         Executes a supported method against a specific instance of a particular type (OpenDoor() against a reader in this case)
```

### Comparing `OpenAccess-0.3/OpenAccess.egg-info/PKG-INFO` & `OpenAccess-0.4/OpenAccess.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenAccess
-Version: 0.3
+Version: 0.4
 Summary: Librería no oficial para leer comunicarse con un servidor de LENEL OpenAccess 
 Home-page: https://github.com/alejomejia1
 Author: Alejandro Mejia Ayala, Jaiber Camacho
 Author-email: alejandromejia@qaingenieros.com
 License: GNU
 Description-Content-Type: text/markdown
```

### Comparing `OpenAccess-0.3/PKG-INFO` & `OpenAccess-0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpenAccess
-Version: 0.3
+Version: 0.4
 Summary: Librería no oficial para leer comunicarse con un servidor de LENEL OpenAccess 
 Home-page: https://github.com/alejomejia1
 Author: Alejandro Mejia Ayala, Jaiber Camacho
 Author-email: alejandromejia@qaingenieros.com
 License: GNU
 Description-Content-Type: text/markdown
```

### Comparing `OpenAccess-0.3/README.md` & `OpenAccess-0.4/README.md`

 * *Files identical despite different names*

### Comparing `OpenAccess-0.3/setup.py` & `OpenAccess-0.4/setup.py`

 * *Files identical despite different names*

