# Comparing `tmp/secret_message-0.2.tar.gz` & `tmp/secret_message-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secret_message-0.2.tar", last modified: Mon May 22 14:05:18 2023, max compression
+gzip compressed data, was "secret_message-0.3.tar", last modified: Mon May 22 14:18:39 2023, max compression
```

## Comparing `secret_message-0.2.tar` & `secret_message-0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:05:18.055296 secret_message-0.2/
--rw-rw----   0 root         (0) everybody  (9997)     1065 2023-05-22 13:17:48.000000 secret_message-0.2/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)     2523 2023-05-22 14:05:18.045296 secret_message-0.2/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     2140 2023-05-12 19:51:42.000000 secret_message-0.2/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:05:17.975296 secret_message-0.2/secret_message/
--rw-rw----   0 root         (0) everybody  (9997)     1762 2023-05-12 17:57:05.000000 secret_message-0.2/secret_message/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:05:18.035296 secret_message-0.2/secret_message.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     2523 2023-05-22 14:05:17.000000 secret_message-0.2/secret_message.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      209 2023-05-22 14:05:17.000000 secret_message-0.2/secret_message.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-22 14:05:17.000000 secret_message-0.2/secret_message.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       15 2023-05-22 14:05:17.000000 secret_message-0.2/secret_message.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-22 14:05:18.055296 secret_message-0.2/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     2691 2023-05-22 14:04:38.000000 secret_message-0.2/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:18:39.395295 secret_message-0.3/
+-rw-rw----   0 root         (0) everybody  (9997)     1065 2023-05-22 13:17:48.000000 secret_message-0.3/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)     2523 2023-05-22 14:18:39.385295 secret_message-0.3/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     2140 2023-05-12 19:51:42.000000 secret_message-0.3/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:18:39.325296 secret_message-0.3/secret_message/
+-rw-rw----   0 root         (0) everybody  (9997)     1762 2023-05-12 17:57:05.000000 secret_message-0.3/secret_message/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:18:39.375295 secret_message-0.3/secret_message.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     2523 2023-05-22 14:18:39.000000 secret_message-0.3/secret_message.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      209 2023-05-22 14:18:39.000000 secret_message-0.3/secret_message.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-22 14:18:39.000000 secret_message-0.3/secret_message.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       15 2023-05-22 14:18:39.000000 secret_message-0.3/secret_message.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-22 14:18:39.395295 secret_message-0.3/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     2691 2023-05-22 14:16:00.000000 secret_message-0.3/setup.py
```

### Comparing `secret_message-0.2/LICENSE.txt` & `secret_message-0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `secret_message-0.2/PKG-INFO` & `secret_message-0.3/secret_message.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: secret_message
-Version: 0.2
+Name: secret-message
+Version: 0.3
 Summary: Create and share a Message Secretly.
 Author: E Lusifa Taehyung
 Author-email: purplebird7613@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -17,24 +17,24 @@
 ## Install
 ```
 pip install secret-message
 ```
 
 ## Import the package
 ```
-import secret-message
+import secret_message
 
 # ------OR------
 
-#from secret-message import create,show,history
+#from secret_message import create,show,history
 ```
 
 ## Create a Message:
 ```
-import secret-message as message 
+import secret_message as message 
 
 message.create("<USERNAME>","<YOUR_MESSAGE>","<PASSWORD_FOR_THE_MESSAGE>")
 ```
 For creating a message it takes only 3 parameters:
 
 	1. Username - Just add your name as username(No registration stuff is required.)
 	
@@ -54,15 +54,15 @@
 ```
 web_message_link - Using this link anyone will be able to access your message from web[Any web browser].
 
 api_msg_link - Using this link anyone will be able to access your message by api call 
 
 ## Show/Read Message
 ```
-import secret-message as message
+import secret_message as message
 
 message.show("<USERNAME>","<MESSAGE_LINK>","<PASSWORD_OF_THE_MESSAGE>")
 ```
 For showing or reading someone else's messages,it takes only 3 parameters:
 
 	1. Username - Just add your name as username(No registration stuff is required.)
 	
@@ -75,15 +75,15 @@
 {
   "text_message" : "<USER'S_MESSAGE>"
 }
 ```
 
 ## Message History 
 ```
-import secret-message as message
+import secret_message as message
 
 message.history("<Username>")
 ```
 For getting history of your messages,it takes only 1 parameter:
 
 	1. Username - Just add your name as username(No registration stuff is required.)
```

### Comparing `secret_message-0.2/README.md` & `secret_message-0.3/README.md`

 * *Files identical despite different names*

### Comparing `secret_message-0.2/secret_message/__init__.py` & `secret_message-0.3/secret_message/__init__.py`

 * *Files identical despite different names*

### Comparing `secret_message-0.2/secret_message.egg-info/PKG-INFO` & `secret_message-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: secret-message
-Version: 0.2
+Name: secret_message
+Version: 0.3
 Summary: Create and share a Message Secretly.
 Author: E Lusifa Taehyung
 Author-email: purplebird7613@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -17,24 +17,24 @@
 ## Install
 ```
 pip install secret-message
 ```
 
 ## Import the package
 ```
-import secret-message
+import secret_message
 
 # ------OR------
 
-#from secret-message import create,show,history
+#from secret_message import create,show,history
 ```
 
 ## Create a Message:
 ```
-import secret-message as message 
+import secret_message as message 
 
 message.create("<USERNAME>","<YOUR_MESSAGE>","<PASSWORD_FOR_THE_MESSAGE>")
 ```
 For creating a message it takes only 3 parameters:
 
 	1. Username - Just add your name as username(No registration stuff is required.)
 	
@@ -54,15 +54,15 @@
 ```
 web_message_link - Using this link anyone will be able to access your message from web[Any web browser].
 
 api_msg_link - Using this link anyone will be able to access your message by api call 
 
 ## Show/Read Message
 ```
-import secret-message as message
+import secret_message as message
 
 message.show("<USERNAME>","<MESSAGE_LINK>","<PASSWORD_OF_THE_MESSAGE>")
 ```
 For showing or reading someone else's messages,it takes only 3 parameters:
 
 	1. Username - Just add your name as username(No registration stuff is required.)
 	
@@ -75,15 +75,15 @@
 {
   "text_message" : "<USER'S_MESSAGE>"
 }
 ```
 
 ## Message History 
 ```
-import secret-message as message
+import secret_message as message
 
 message.history("<Username>")
 ```
 For getting history of your messages,it takes only 1 parameter:
 
 	1. Username - Just add your name as username(No registration stuff is required.)
```

### Comparing `secret_message-0.2/setup.py` & `secret_message-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 ## Install
 ```
 pip install secret-message
 ```
 
 ## Import the package
 ```
-import secret-message
+import secret_message
 
 # ------OR------
 
-#from secret-message import create,show,history
+#from secret_message import create,show,history
 ```
 
 ## Create a Message:
 ```
-import secret-message as message 
+import secret_message as message 
 
 message.create("<USERNAME>","<YOUR_MESSAGE>","<PASSWORD_FOR_THE_MESSAGE>")
 ```
 For creating a message it takes only 3 parameters:
 
 	1. Username - Just add your name as username(No registration stuff is required.)
 	
@@ -44,15 +44,15 @@
 ```
 web_message_link - Using this link anyone will be able to access your message from web[Any web browser].
 
 api_msg_link - Using this link anyone will be able to access your message by api call 
 
 ## Show/Read Message
 ```
-import secret-message as message
+import secret_message as message
 
 message.show("<USERNAME>","<MESSAGE_LINK>","<PASSWORD_OF_THE_MESSAGE>")
 ```
 For showing or reading someone else's messages,it takes only 3 parameters:
 
 	1. Username - Just add your name as username(No registration stuff is required.)
 	
@@ -65,15 +65,15 @@
 {
   "text_message" : "<USER'S_MESSAGE>"
 }
 ```
 
 ## Message History 
 ```
-import secret-message as message
+import secret_message as message
 
 message.history("<Username>")
 ```
 For getting history of your messages,it takes only 1 parameter:
 
 	1. Username - Just add your name as username(No registration stuff is required.)
 
@@ -95,15 +95,15 @@
 
 """          
 
 setuptools.setup(
 
 	name = 'secret_message', 
 
-	version = '0.2',
+	version = '0.3',
 
 	author = "E Lusifa Taehyung",
 
 	author_email = "purplebird7613@gmail.com",
 
 	description = "Create and share a Message Secretly.",
```

