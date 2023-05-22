# Comparing `tmp/secret_message-0.1.tar.gz` & `tmp/secret_message-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secret_message-0.1.tar", last modified: Mon May 22 14:00:34 2023, max compression
+gzip compressed data, was "secret_message-0.2.tar", last modified: Mon May 22 14:05:18 2023, max compression
```

## Comparing `secret_message-0.1.tar` & `secret_message-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:00:34.415296 secret_message-0.1/
--rw-rw----   0 root         (0) everybody  (9997)     1065 2023-05-22 13:17:48.000000 secret_message-0.1/LICENSE.txt
--rw-rw----   0 root         (0) everybody  (9997)     2517 2023-05-22 14:00:34.415296 secret_message-0.1/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)     2140 2023-05-12 19:51:42.000000 secret_message-0.1/README.md
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:00:34.335296 secret_message-0.1/secret_message/
--rw-rw----   0 root         (0) everybody  (9997)     1762 2023-05-12 17:57:05.000000 secret_message-0.1/secret_message/__init__.py
-drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:00:34.405296 secret_message-0.1/secret_message.egg-info/
--rw-rw----   0 root         (0) everybody  (9997)     2517 2023-05-22 14:00:34.000000 secret_message-0.1/secret_message.egg-info/PKG-INFO
--rw-rw----   0 root         (0) everybody  (9997)      209 2023-05-22 14:00:34.000000 secret_message-0.1/secret_message.egg-info/SOURCES.txt
--rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-22 14:00:34.000000 secret_message-0.1/secret_message.egg-info/dependency_links.txt
--rw-rw----   0 root         (0) everybody  (9997)       15 2023-05-22 14:00:34.000000 secret_message-0.1/secret_message.egg-info/top_level.txt
--rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-22 14:00:34.415296 secret_message-0.1/setup.cfg
--rw-rw----   0 root         (0) everybody  (9997)     2685 2023-05-22 14:00:03.000000 secret_message-0.1/setup.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:05:18.055296 secret_message-0.2/
+-rw-rw----   0 root         (0) everybody  (9997)     1065 2023-05-22 13:17:48.000000 secret_message-0.2/LICENSE.txt
+-rw-rw----   0 root         (0) everybody  (9997)     2523 2023-05-22 14:05:18.045296 secret_message-0.2/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)     2140 2023-05-12 19:51:42.000000 secret_message-0.2/README.md
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:05:17.975296 secret_message-0.2/secret_message/
+-rw-rw----   0 root         (0) everybody  (9997)     1762 2023-05-12 17:57:05.000000 secret_message-0.2/secret_message/__init__.py
+drwxrwx---   0 root         (0) everybody  (9997)        0 2023-05-22 14:05:18.035296 secret_message-0.2/secret_message.egg-info/
+-rw-rw----   0 root         (0) everybody  (9997)     2523 2023-05-22 14:05:17.000000 secret_message-0.2/secret_message.egg-info/PKG-INFO
+-rw-rw----   0 root         (0) everybody  (9997)      209 2023-05-22 14:05:17.000000 secret_message-0.2/secret_message.egg-info/SOURCES.txt
+-rw-rw----   0 root         (0) everybody  (9997)        1 2023-05-22 14:05:17.000000 secret_message-0.2/secret_message.egg-info/dependency_links.txt
+-rw-rw----   0 root         (0) everybody  (9997)       15 2023-05-22 14:05:17.000000 secret_message-0.2/secret_message.egg-info/top_level.txt
+-rw-rw----   0 root         (0) everybody  (9997)       38 2023-05-22 14:05:18.055296 secret_message-0.2/setup.cfg
+-rw-rw----   0 root         (0) everybody  (9997)     2691 2023-05-22 14:04:38.000000 secret_message-0.2/setup.py
```

### Comparing `secret_message-0.1/LICENSE.txt` & `secret_message-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `secret_message-0.1/PKG-INFO` & `secret_message-0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,30 @@
-Metadata-Version: 2.1
-Name: secret_message
-Version: 0.1
-Summary: Create and share a Message Secretly.
-Author: E Lusifa Taehyung
-Author-email: purplebird7613@gmail.com
-Classifier: Programming Language :: Python
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
+import setuptools
 
+description = """
 # Secret-Message 
 Create and share Messages in a  **Secret** way.
 
 ## Install
 ```
-pip install secretmessage
+pip install secret-message
 ```
 
 ## Import the package
 ```
-import secretmessage
+import secret-message
 
 # ------OR------
 
-#from secretmessage import create,show,history
+#from secret-message import create,show,history
 ```
 
 ## Create a Message:
 ```
-import secretmessage as message 
+import secret-message as message 
 
 message.create("<USERNAME>","<YOUR_MESSAGE>","<PASSWORD_FOR_THE_MESSAGE>")
 ```
 For creating a message it takes only 3 parameters:
 
 	1. Username - Just add your name as username(No registration stuff is required.)
 	
@@ -54,15 +44,15 @@
 ```
 web_message_link - Using this link anyone will be able to access your message from web[Any web browser].
 
 api_msg_link - Using this link anyone will be able to access your message by api call 
 
 ## Show/Read Message
 ```
-import secretmessage as message
+import secret-message as message
 
 message.show("<USERNAME>","<MESSAGE_LINK>","<PASSWORD_OF_THE_MESSAGE>")
 ```
 For showing or reading someone else's messages,it takes only 3 parameters:
 
 	1. Username - Just add your name as username(No registration stuff is required.)
 	
@@ -75,15 +65,15 @@
 {
   "text_message" : "<USER'S_MESSAGE>"
 }
 ```
 
 ## Message History 
 ```
-import secretmessage as message
+import secret-message as message
 
 message.history("<Username>")
 ```
 For getting history of your messages,it takes only 1 parameter:
 
 	1. Username - Just add your name as username(No registration stuff is required.)
 
@@ -99,7 +89,39 @@
   	   "api_msg_link": "<YOUR_MESSAGE_LINK_FOR_API_CALL>" 
   	},
   	........
   ]
 }
 ```
 
+"""          
+
+setuptools.setup(
+
+	name = 'secret_message', 
+
+	version = '0.2',
+
+	author = "E Lusifa Taehyung",
+
+	author_email = "purplebird7613@gmail.com",
+
+	description = "Create and share a Message Secretly.",
+	
+	long_description = description,
+	
+    long_description_content_type = 'text/markdown',
+  
+	
+	packages = setuptools.find_packages(),
+ 
+	classifiers = [
+
+    "Programming Language :: Python",
+
+    "License :: OSI Approved :: MIT License",
+
+    "Operating System :: OS Independent",
+
+    ],
+
+)
```

### Comparing `secret_message-0.1/README.md` & `secret_message-0.2/README.md`

 * *Files identical despite different names*

### Comparing `secret_message-0.1/secret_message/__init__.py` & `secret_message-0.2/secret_message/__init__.py`

 * *Files identical despite different names*

### Comparing `secret_message-0.1/secret_message.egg-info/PKG-INFO` & `secret_message-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: secret-message
-Version: 0.1
+Name: secret_message
+Version: 0.2
 Summary: Create and share a Message Secretly.
 Author: E Lusifa Taehyung
 Author-email: purplebird7613@gmail.com
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -12,29 +12,29 @@
 
 
 # Secret-Message 
 Create and share Messages in a  **Secret** way.
 
 ## Install
 ```
-pip install secretmessage
+pip install secret-message
 ```
 
 ## Import the package
 ```
-import secretmessage
+import secret-message
 
 # ------OR------
 
-#from secretmessage import create,show,history
+#from secret-message import create,show,history
 ```
 
 ## Create a Message:
 ```
-import secretmessage as message 
+import secret-message as message 
 
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
-import secretmessage as message
+import secret-message as message
 
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
-import secretmessage as message
+import secret-message as message
 
 message.history("<Username>")
 ```
 For getting history of your messages,it takes only 1 parameter:
 
 	1. Username - Just add your name as username(No registration stuff is required.)
```

