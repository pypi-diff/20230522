# Comparing `tmp/turbogpt-1.0.2.tar.gz` & `tmp/turbogpt-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbogpt-1.0.2.tar", last modified: Wed Mar 29 11:50:02 2023, max compression
+gzip compressed data, was "turbogpt-1.0.5.tar", last modified: Sun May 21 22:32:31 2023, max compression
```

## Comparing `turbogpt-1.0.2.tar` & `turbogpt-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-29 11:50:02.560805 turbogpt-1.0.2/
--rw-r--r--   0 root         (0) staff       (20)     1063 2023-03-24 13:32:31.000000 turbogpt-1.0.2/LICENSE.TXT
--rw-r--r--   0 root         (0) staff       (20)     2890 2023-03-29 11:50:02.560871 turbogpt-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2497 2023-03-29 11:48:43.000000 turbogpt-1.0.2/README.md
--rw-r--r--   0 root         (0) staff       (20)       84 2023-03-24 13:37:37.000000 turbogpt-1.0.2/pyproject.toml
--rw-r--r--   0 root         (0) staff       (20)      416 2023-03-29 11:50:02.561165 turbogpt-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)      690 2023-03-29 11:50:01.000000 turbogpt-1.0.2/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-29 11:50:02.560014 turbogpt-1.0.2/turbogpt/
--rw-r--r--   0 root         (0) staff       (20)       76 2023-03-24 15:07:56.000000 turbogpt-1.0.2/turbogpt/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3943 2023-03-29 11:48:43.000000 turbogpt-1.0.2/turbogpt/turbogpt.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-03-29 11:50:02.560681 turbogpt-1.0.2/turbogpt.egg-info/
--rw-r--r--   0 root         (0) staff       (20)     2890 2023-03-29 11:50:02.000000 turbogpt-1.0.2/turbogpt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      256 2023-03-29 11:50:02.000000 turbogpt-1.0.2/turbogpt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-03-29 11:50:02.000000 turbogpt-1.0.2/turbogpt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       39 2023-03-29 11:50:02.000000 turbogpt-1.0.2/turbogpt.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        9 2023-03-29 11:50:02.000000 turbogpt-1.0.2/turbogpt.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-21 22:32:31.081965 turbogpt-1.0.5/
+-rw-r--r--   0 root         (0) staff       (20)     1063 2023-03-24 13:32:31.000000 turbogpt-1.0.5/LICENSE.TXT
+-rw-r--r--   0 root         (0) staff       (20)     2940 2023-05-21 22:32:31.082044 turbogpt-1.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2547 2023-05-21 22:31:47.000000 turbogpt-1.0.5/README.md
+-rw-r--r--   0 root         (0) staff       (20)       84 2023-03-24 13:37:37.000000 turbogpt-1.0.5/pyproject.toml
+-rw-r--r--   0 root         (0) staff       (20)      416 2023-05-21 22:32:31.082336 turbogpt-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)      690 2023-05-21 22:32:21.000000 turbogpt-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-21 22:32:31.081211 turbogpt-1.0.5/turbogpt/
+-rw-r--r--   0 root         (0) staff       (20)       76 2023-03-24 15:07:56.000000 turbogpt-1.0.5/turbogpt/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4151 2023-05-21 22:24:23.000000 turbogpt-1.0.5/turbogpt/turbogpt.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-21 22:32:31.081847 turbogpt-1.0.5/turbogpt.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)     2940 2023-05-21 22:32:31.000000 turbogpt-1.0.5/turbogpt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      256 2023-05-21 22:32:31.000000 turbogpt-1.0.5/turbogpt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-21 22:32:31.000000 turbogpt-1.0.5/turbogpt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       39 2023-05-21 22:32:31.000000 turbogpt-1.0.5/turbogpt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        9 2023-05-21 22:32:31.000000 turbogpt-1.0.5/turbogpt.egg-info/top_level.txt
```

### Comparing `turbogpt-1.0.2/LICENSE.TXT` & `turbogpt-1.0.5/LICENSE.TXT`

 * *Files identical despite different names*

### Comparing `turbogpt-1.0.2/PKG-INFO` & `turbogpt-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 Metadata-Version: 2.1
 Name: turbogpt
-Version: 1.0.2
+Version: 1.0.5
 Summary: A python based wrapper for GPT-4 & GPT-3.5 PLUS.
 Author: daan-dj
 Author-email: daan@jumelet.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 
 # TurboGpt
 
 #### A python based wrapper for GPT-4 & GPT-3.5 PLUS. 
 
+<p align="center">
+Thank you for:
+<br>
+  <img src="https://static.pepy.tech/badge/turbogpt" alt="Sublime's custom image"/>
+<br>
+Downloads!
+<br>
+</p>
+
+
+![TurboGpt Tutorial](https://i.imgur.com/6tLLj7I.jpg)
 
-### Youtube demo / tutorial
-[![TurboGpt Tutorial](https://i.imgur.com/6tLLj7I.jpg)](https://www.youtube.com/watch?v=Ic69TsemE9g&ab_channel=blacksailslabs)
 
 ## Benefits and why.
 There is currently no way to use GPT-4 outside the online chat.openai.com interface. This wrapper allows you to use GPT-4 in your own projects. \
 the current API is extremely slow and even if you have premium it does not speed up the response time. TurboGpt does not use the API and instead uses the same interfaces as the chat.openai.com website.
 This means that you can use GPT-4 and GPT-3.5 PLUS in your own projects without having to wait 20+ seconds for a response.
 
 ## Install
```

### Comparing `turbogpt-1.0.2/README.md` & `turbogpt-1.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # TurboGpt
 
 #### A python based wrapper for GPT-4 & GPT-3.5 PLUS. 
 
+<p align="center">
+Thank you for:
+<br>
+  <img src="https://static.pepy.tech/badge/turbogpt" alt="Sublime's custom image"/>
+<br>
+Downloads!
+<br>
+</p>
+
+
+![TurboGpt Tutorial](https://i.imgur.com/6tLLj7I.jpg)
 
-### Youtube demo / tutorial
-[![TurboGpt Tutorial](https://i.imgur.com/6tLLj7I.jpg)](https://www.youtube.com/watch?v=Ic69TsemE9g&ab_channel=blacksailslabs)
 
 ## Benefits and why.
 There is currently no way to use GPT-4 outside the online chat.openai.com interface. This wrapper allows you to use GPT-4 in your own projects. \
 the current API is extremely slow and even if you have premium it does not speed up the response time. TurboGpt does not use the API and instead uses the same interfaces as the chat.openai.com website.
 This means that you can use GPT-4 and GPT-3.5 PLUS in your own projects without having to wait 20+ seconds for a response.
 
 ## Install
```

### Comparing `turbogpt-1.0.2/setup.py` & `turbogpt-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="turbogpt",
-    version="1.0.2",
+    version="1.0.5",
     author="daan-dj",
     author_email="daan@jumelet.net",
     description="A python based wrapper for GPT-4 & GPT-3.5 PLUS.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `turbogpt-1.0.2/turbogpt/turbogpt.py` & `turbogpt-1.0.5/turbogpt/turbogpt.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,14 +75,20 @@
     def resume_session(self, chat_id):
         res = self.session.get(
             "https://chat.openai.com/backend-api/conversation/" + chat_id,
         )
 
         parent_id = res.json()["current_node"]
         return {"conversation_id": chat_id, "message": {"id": parent_id}}
+        
+    def delete_session(self, chat_id):
+        res = self.session.patch(
+            "https://chat.openai.com/backend-api/conversation/" + chat_id,
+            json={"is_visible": "false"}
+        )
 
     def send_message(self, message, old_question):
         res = self.session.post(
             "https://chat.openai.com/backend-api/conversation",
             json={"id": str(uuid.uuid4()), "action": "next", "messages": [
                 {"author": {"role": "user"}, "role": "user",
                  "content": {"content_type": "text", "parts": [f"{message}\n"]}}],
```

### Comparing `turbogpt-1.0.2/turbogpt.egg-info/PKG-INFO` & `turbogpt-1.0.5/turbogpt.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,36 @@
 Metadata-Version: 2.1
 Name: turbogpt
-Version: 1.0.2
+Version: 1.0.5
 Summary: A python based wrapper for GPT-4 & GPT-3.5 PLUS.
 Author: daan-dj
 Author-email: daan@jumelet.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.TXT
 
 # TurboGpt
 
 #### A python based wrapper for GPT-4 & GPT-3.5 PLUS. 
 
+<p align="center">
+Thank you for:
+<br>
+  <img src="https://static.pepy.tech/badge/turbogpt" alt="Sublime's custom image"/>
+<br>
+Downloads!
+<br>
+</p>
+
+
+![TurboGpt Tutorial](https://i.imgur.com/6tLLj7I.jpg)
 
-### Youtube demo / tutorial
-[![TurboGpt Tutorial](https://i.imgur.com/6tLLj7I.jpg)](https://www.youtube.com/watch?v=Ic69TsemE9g&ab_channel=blacksailslabs)
 
 ## Benefits and why.
 There is currently no way to use GPT-4 outside the online chat.openai.com interface. This wrapper allows you to use GPT-4 in your own projects. \
 the current API is extremely slow and even if you have premium it does not speed up the response time. TurboGpt does not use the API and instead uses the same interfaces as the chat.openai.com website.
 This means that you can use GPT-4 and GPT-3.5 PLUS in your own projects without having to wait 20+ seconds for a response.
 
 ## Install
```

